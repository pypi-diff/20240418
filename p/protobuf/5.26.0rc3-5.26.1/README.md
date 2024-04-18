# Comparing `tmp/protobuf-5.26.0rc3.tar.gz` & `tmp/protobuf-5.26.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/protobuf-5.26.0rc3.tar", last modified: Tue Feb 27 22:12:27 2024, max compression
+gzip compressed data, was "dist/protobuf-5.26.1.tar", last modified: Wed Mar 27 18:00:33 2024, max compression
```

## Comparing `protobuf-5.26.0rc3.tar` & `protobuf-5.26.1.tar`

### file list

```diff
@@ -1,286 +1,286 @@
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1732 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/LICENSE
--rw-r--r--   0 bazel     (1000) bazel     (1003)       39 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/MANIFEST.in
--rw-r--r--   0 bazel     (1000) bazel     (1003)      821 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/PKG-INFO
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4624 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/README.md
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/google/
--rw-r--r--   0 bazel     (1000) bazel     (1003)      150 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/__init__.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/google/protobuf/
--rw-r--r--   0 bazel     (1000) bazel     (1003)      349 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1483 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/any_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2903 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/api_pb2.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/google/protobuf/compiler/
--rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/compiler/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3543 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/compiler/plugin_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    52063 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/descriptor.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)        1 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/descriptor.upb.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)   430985 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/descriptor.upb.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    67645 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/descriptor.upb_minitable.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4556 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/descriptor.upb_minitable.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    65671 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/descriptor.upbdefs.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     9059 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/descriptor.upbdefs.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5444 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/descriptor_database.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)   330700 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/descriptor_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    48373 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/descriptor_pool.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1558 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/duration_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1425 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/empty_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1516 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/field_mask_pb2.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/google/protobuf/internal/
--rw-r--r--   0 bazel     (1000) bazel     (1003)      272 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/internal/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    14073 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/internal/_parameterized.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4787 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/internal/api_implementation.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4082 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/internal/builder.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    21722 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/internal/containers.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    37437 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/internal/decoder.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    27297 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/internal/encoder.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3462 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/internal/enum_type_wrapper.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7225 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/internal/extension_dict.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    10416 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/internal/field_mask.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2008 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/internal/message_listener.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)      425 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/internal/python_edition_defaults.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    56576 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/internal/python_message.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4080 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/internal/testing_refleaks.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    15450 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/internal/type_checkers.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    20380 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/internal/well_known_types.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7087 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/internal/wire_format.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    35233 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/json_format.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    12844 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/message.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     8271 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/message_factory.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4203 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/proto_builder.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/google/protobuf/pyext/
--rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/pyext/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1704 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/pyext/cpp_message.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2413 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/reflection.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7787 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/service.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    10058 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/service_reflection.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1538 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/source_context_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2816 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/struct_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6709 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/symbol_database.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/google/protobuf/testdata/
--rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/testdata/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3621 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/text_encoding.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    62691 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/text_format.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1567 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/timestamp_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5195 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/type_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3127 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/unknown_fields.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/google/protobuf/util/
--rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/util/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2790 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/google/protobuf/wrappers_pb2.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/protobuf.egg-info/
--rw-r--r--   0 bazel     (1000) bazel     (1003)      821 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/protobuf.egg-info/PKG-INFO
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7232 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/protobuf.egg-info/SOURCES.txt
--rw-r--r--   0 bazel     (1000) bazel     (1003)        1 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/protobuf.egg-info/dependency_links.txt
--rw-r--r--   0 bazel     (1000) bazel     (1003)        7 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/protobuf.egg-info/namespace_packages.txt
--rw-r--r--   0 bazel     (1000) bazel     (1003)        7 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/protobuf.egg-info/top_level.txt
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/python/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    14972 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/python/convert.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1909 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/python/convert.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    76030 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/python/descriptor.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2572 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/python/descriptor.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    27874 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/python/descriptor_containers.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4157 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/python/descriptor_containers.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    23336 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/python/descriptor_pool.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      936 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/python/descriptor_pool.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     8703 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/python/extension_dict.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      530 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/python/extension_dict.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    19273 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/python/map.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1610 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/python/map.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    71894 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/python/message.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3875 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/python/message.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    12674 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/python/protobuf.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     8085 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/python/protobuf.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1642 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/python/python_api.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    29250 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/python/repeated.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2087 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/python/repeated.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    10792 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/python/unknown_fields.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      531 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/python/unknown_fields.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)       38 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/setup.cfg
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2462 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/setup.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/upb/
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/upb/base/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3581 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/base/descriptor_constants.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/upb/base/internal/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1130 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/base/internal/endian.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      873 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/base/internal/log2.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1747 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/base/status.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1359 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/base/status.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1597 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/base/string_view.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      820 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/base/upcast.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1189 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/generated_code_support.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/upb/hash/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    23982 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/hash/common.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5511 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/hash/common.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2868 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/hash/int_table.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4857 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/hash/str_table.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/upb/lex/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1140 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/lex/atoi.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      991 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/lex/atoi.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1525 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/lex/round_trip.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1042 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/lex/round_trip.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2775 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/lex/strtod.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      586 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/lex/strtod.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      909 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/lex/unicode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1737 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/lex/unicode.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/upb/mem/
--rw-r--r--   0 bazel     (1000) bazel     (1003)      699 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mem/alloc.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2278 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mem/alloc.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    17946 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mem/arena.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2693 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mem/arena.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/upb/mem/internal/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3444 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mem/internal/arena.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/upb/message/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1824 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/accessors.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)    19056 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/accessors.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2609 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/accessors_split64.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4229 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/array.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3013 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/array.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2397 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/array_split64.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1401 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/compare.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      871 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/compare.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1151 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/compat.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1213 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/compat.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    12165 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/copy.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1884 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/copy.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/upb/message/internal/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    13453 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/internal/accessors.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4866 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/internal/array.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2030 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/internal/extension.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2148 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/internal/extension.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4892 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/internal/map.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1405 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/internal/map_entry.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2829 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/internal/map_sorter.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1828 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/internal/message.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3053 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/internal/message.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1625 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/internal/tagged_ptr.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      541 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/internal/types.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3731 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/map.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4316 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/map.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1687 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/map_gencode_util.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5108 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/map_sorter.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2426 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/message.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1364 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/message.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    14898 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/promote.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6063 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/promote.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1647 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/tagged_ptr.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1261 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/message/value.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/upb/mini_descriptor/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4811 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_descriptor/build_enum.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1484 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_descriptor/build_enum.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    33903 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_descriptor/decode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4982 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_descriptor/decode.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/upb/mini_descriptor/internal/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1291 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_descriptor/internal/base92.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1723 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_descriptor/internal/base92.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1686 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_descriptor/internal/decoder.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    12665 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_descriptor/internal/encode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3631 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_descriptor/internal/encode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1034 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_descriptor/internal/modifiers.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2169 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_descriptor/internal/wire_constants.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4545 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_descriptor/link.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3566 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_descriptor/link.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/upb/mini_table/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4176 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_table/compat.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1376 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_table/compat.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      920 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_table/enum.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1421 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_table/extension.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2733 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_table/extension_registry.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3577 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_table/extension_registry.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2392 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_table/field.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1669 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_table/file.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/upb/mini_table/internal/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1715 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_table/internal/enum.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1732 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_table/internal/extension.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7109 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_table/internal/field.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1920 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_table/internal/file.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      882 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_table/internal/message.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5789 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_table/internal/message.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2622 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_table/internal/size_log2.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1424 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_table/internal/sub.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2146 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_table/message.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3184 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_table/message.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1331 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/mini_table/sub.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/upb/port/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3197 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/port/atomic.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    10253 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/port/def.inc
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1400 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/port/undef.inc
--rw-r--r--   0 bazel     (1000) bazel     (1003)      972 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/port/vsnprintf_compat.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/upb/reflection/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1620 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/common.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      826 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    17888 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/def_pool.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3593 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/def_pool.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      958 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/def_type.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1711 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/def_type.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      926 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/desc_state.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)    10834 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/enum_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2356 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/enum_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2027 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/enum_reserved_range.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      815 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/enum_reserved_range.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5271 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/enum_value_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1245 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/enum_value_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2778 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/extension_range.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1057 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/extension_range.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    32976 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/field_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3447 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/field_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    14538 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/file_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2159 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/file_def.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/upb/reflection/internal/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    13068 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/internal/def_builder.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6985 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/internal/def_builder.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2068 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/internal/def_pool.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1108 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/internal/desc_state.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1204 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/internal/enum_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1059 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/internal/enum_reserved_range.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1184 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/internal/enum_value_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1021 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/internal/extension_range.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2238 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/internal/field_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1120 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/internal/file_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1813 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/internal/message_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1038 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/internal/message_reserved_range.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1087 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/internal/method_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1286 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/internal/oneof_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1078 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/internal/service_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      849 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/internal/strdup2.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      796 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/internal/strdup2.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      960 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/internal/upb_edition_defaults.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7801 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/message.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3386 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/message.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    27264 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/message_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6403 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/message_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1995 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/message_reserved_range.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      836 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/message_reserved_range.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3812 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/method_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1372 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/method_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7367 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/oneof_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1836 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/oneof_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4039 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/service_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1408 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/reflection/service_def.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/upb/text/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    15311 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/text/encode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1454 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/text/encode.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/upb/util/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     9750 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/util/compare.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1580 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/util/compare.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    23869 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/util/def_to_proto.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1737 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/util/def_to_proto.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     9941 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/util/required_fields.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2842 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/util/required_fields.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/upb/wire/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    52609 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/wire/decode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5658 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/wire/decode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    21988 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/wire/encode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2272 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/wire/encode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      724 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/wire/eps_copy_input_stream.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)    17122 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/wire/eps_copy_input_stream.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/upb/wire/internal/
--rw-r--r--   0 bazel     (1000) bazel     (1003)      716 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/wire/internal/constants.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    50837 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/wire/internal/decode_fast.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3998 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/wire/internal/decode_fast.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4286 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/wire/internal/decoder.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1662 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/wire/internal/reader.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1451 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/wire/reader.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6697 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/wire/reader.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      620 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/upb/wire/types.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-02-27 22:12:27.000000 protobuf-5.26.0rc3/utf8_range/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    17939 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/utf8_range/utf8_range.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      540 2000-01-01 00:00:00.000000 protobuf-5.26.0rc3/utf8_range/utf8_range.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1732 2000-01-01 00:00:00.000000 protobuf-5.26.1/LICENSE
+-rw-r--r--   0 bazel     (1000) bazel     (1003)       39 2000-01-01 00:00:00.000000 protobuf-5.26.1/MANIFEST.in
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      818 2024-03-27 18:00:33.000000 protobuf-5.26.1/PKG-INFO
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4624 2000-01-01 00:00:00.000000 protobuf-5.26.1/README.md
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/google/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      150 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/__init__.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/google/protobuf/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      346 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1479 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/any_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2899 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/api_pb2.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/google/protobuf/compiler/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/compiler/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3539 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/compiler/plugin_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    52063 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/descriptor.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        1 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/descriptor.upb.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)   430985 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/descriptor.upb.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    67645 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/descriptor.upb_minitable.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4556 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/descriptor.upb_minitable.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    65671 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/descriptor.upbdefs.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     9059 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/descriptor.upbdefs.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5444 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/descriptor_database.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)   330696 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/descriptor_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    48373 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/descriptor_pool.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1554 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/duration_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1421 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/empty_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1512 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/field_mask_pb2.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/google/protobuf/internal/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      272 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    14073 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/_parameterized.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4787 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/api_implementation.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4082 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/builder.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    21722 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/containers.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    37437 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/decoder.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    27297 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/encoder.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3462 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/enum_type_wrapper.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     7225 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/extension_dict.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    10416 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/field_mask.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2008 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/message_listener.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      425 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/python_edition_defaults.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    56576 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/python_message.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4080 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/testing_refleaks.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    15450 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/type_checkers.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    20380 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/well_known_types.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     7087 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/wire_format.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    35233 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/json_format.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    12844 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/message.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8271 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/message_factory.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4203 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/proto_builder.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/google/protobuf/pyext/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/pyext/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1704 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/pyext/cpp_message.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2413 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/reflection.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     7787 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/service.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    10058 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/service_reflection.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1534 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/source_context_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2812 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/struct_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6709 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/symbol_database.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/google/protobuf/testdata/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/testdata/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3621 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/text_encoding.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    62691 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/text_format.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1563 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/timestamp_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5191 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/type_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3127 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/unknown_fields.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/google/protobuf/util/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/util/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2786 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/wrappers_pb2.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/protobuf.egg-info/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      818 2024-03-27 18:00:33.000000 protobuf-5.26.1/protobuf.egg-info/PKG-INFO
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     7232 2024-03-27 18:00:33.000000 protobuf-5.26.1/protobuf.egg-info/SOURCES.txt
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        1 2024-03-27 18:00:33.000000 protobuf-5.26.1/protobuf.egg-info/dependency_links.txt
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        7 2024-03-27 18:00:33.000000 protobuf-5.26.1/protobuf.egg-info/namespace_packages.txt
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        7 2024-03-27 18:00:33.000000 protobuf-5.26.1/protobuf.egg-info/top_level.txt
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/python/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    14972 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/convert.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1909 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/convert.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    76030 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/descriptor.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2572 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/descriptor.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    27874 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/descriptor_containers.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4157 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/descriptor_containers.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    23336 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/descriptor_pool.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      936 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/descriptor_pool.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8703 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/extension_dict.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      530 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/extension_dict.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    19273 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/map.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1610 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/map.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    71894 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/message.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3875 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/message.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    12674 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/protobuf.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8085 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/protobuf.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1642 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/python_api.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    29250 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/repeated.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2087 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/repeated.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    10792 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/unknown_fields.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      531 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/unknown_fields.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)       38 2024-03-27 18:00:33.000000 protobuf-5.26.1/setup.cfg
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2462 2000-01-01 00:00:00.000000 protobuf-5.26.1/setup.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/base/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3581 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/base/descriptor_constants.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/base/internal/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1130 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/base/internal/endian.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      873 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/base/internal/log2.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1747 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/base/status.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1359 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/base/status.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1597 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/base/string_view.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      820 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/base/upcast.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1189 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/generated_code_support.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/hash/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    23982 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/hash/common.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5511 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/hash/common.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2868 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/hash/int_table.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4857 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/hash/str_table.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/lex/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1140 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/lex/atoi.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      991 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/lex/atoi.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1525 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/lex/round_trip.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1042 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/lex/round_trip.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2775 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/lex/strtod.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      586 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/lex/strtod.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      909 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/lex/unicode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1737 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/lex/unicode.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/mem/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      699 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mem/alloc.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2278 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mem/alloc.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    17946 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mem/arena.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2693 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mem/arena.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/mem/internal/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3444 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mem/internal/arena.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/message/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1824 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/accessors.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    19056 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/accessors.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2609 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/accessors_split64.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4229 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/array.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3013 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/array.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2397 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/array_split64.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1401 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/compare.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      871 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/compare.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1151 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/compat.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1213 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/compat.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    12165 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/copy.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1884 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/copy.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/message/internal/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    13453 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/internal/accessors.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4866 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/internal/array.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2030 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/internal/extension.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2148 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/internal/extension.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4892 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/internal/map.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1405 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/internal/map_entry.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2829 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/internal/map_sorter.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1828 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/internal/message.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3053 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/internal/message.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1625 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/internal/tagged_ptr.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      541 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/internal/types.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3731 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/map.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4316 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/map.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1687 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/map_gencode_util.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5108 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/map_sorter.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2426 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/message.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1364 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/message.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    14898 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/promote.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6063 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/promote.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1647 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/tagged_ptr.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1261 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/value.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/mini_descriptor/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4811 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_descriptor/build_enum.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1484 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_descriptor/build_enum.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    33903 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_descriptor/decode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4982 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_descriptor/decode.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/mini_descriptor/internal/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1291 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_descriptor/internal/base92.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1723 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_descriptor/internal/base92.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1686 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_descriptor/internal/decoder.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    12665 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_descriptor/internal/encode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3631 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_descriptor/internal/encode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1034 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_descriptor/internal/modifiers.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2169 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_descriptor/internal/wire_constants.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4545 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_descriptor/link.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3566 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_descriptor/link.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/mini_table/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4176 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/compat.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1376 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/compat.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      920 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/enum.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1421 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/extension.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2733 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/extension_registry.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3577 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/extension_registry.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2392 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/field.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1669 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/file.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/mini_table/internal/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1715 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/internal/enum.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1732 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/internal/extension.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     7109 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/internal/field.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1920 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/internal/file.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      882 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/internal/message.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5789 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/internal/message.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2622 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/internal/size_log2.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1424 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/internal/sub.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2146 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/message.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3184 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/message.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1331 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/sub.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/port/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3197 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/port/atomic.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    10253 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/port/def.inc
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1400 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/port/undef.inc
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      972 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/port/vsnprintf_compat.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/reflection/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1620 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/common.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      826 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    17888 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/def_pool.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3593 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/def_pool.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      958 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/def_type.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1711 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/def_type.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      926 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/desc_state.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    10834 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/enum_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2356 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/enum_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2027 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/enum_reserved_range.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      815 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/enum_reserved_range.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5271 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/enum_value_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1245 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/enum_value_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2778 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/extension_range.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1057 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/extension_range.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    32976 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/field_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3447 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/field_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    14538 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/file_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2159 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/file_def.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/reflection/internal/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    13068 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/def_builder.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6985 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/def_builder.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2068 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/def_pool.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1108 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/desc_state.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1204 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/enum_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1059 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/enum_reserved_range.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1184 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/enum_value_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1021 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/extension_range.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2238 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/field_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1120 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/file_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1813 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/message_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1038 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/message_reserved_range.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1087 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/method_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1286 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/oneof_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1078 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/service_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      849 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/strdup2.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      796 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/strdup2.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      960 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/upb_edition_defaults.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     7801 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/message.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3386 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/message.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    27264 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/message_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6403 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/message_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1995 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/message_reserved_range.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      836 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/message_reserved_range.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3812 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/method_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1372 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/method_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     7367 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/oneof_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1836 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/oneof_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4039 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/service_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1408 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/service_def.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/text/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    15311 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/text/encode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1454 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/text/encode.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/util/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     9750 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/util/compare.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1580 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/util/compare.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    23869 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/util/def_to_proto.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1737 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/util/def_to_proto.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     9941 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/util/required_fields.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2842 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/util/required_fields.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/wire/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    52609 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/decode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5658 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/decode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    21988 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/encode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2272 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/encode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      724 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/eps_copy_input_stream.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    17122 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/eps_copy_input_stream.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/wire/internal/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      716 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/internal/constants.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    50837 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/internal/decode_fast.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3998 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/internal/decode_fast.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4286 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/internal/decoder.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1662 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/internal/reader.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1451 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/reader.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6697 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/reader.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      620 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/types.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/utf8_range/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    17939 2000-01-01 00:00:00.000000 protobuf-5.26.1/utf8_range/utf8_range.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      540 2000-01-01 00:00:00.000000 protobuf-5.26.1/utf8_range/utf8_range.h
```

### Comparing `protobuf-5.26.0rc3/LICENSE` & `protobuf-5.26.1/LICENSE`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/PKG-INFO` & `protobuf-5.26.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protobuf
-Version: 5.26.0rc3
+Version: 5.26.1
 Summary: Protocol Buffers
 Home-page: https://developers.google.com/protocol-buffers/
 Download-URL: https://github.com/protocolbuffers/protobuf/releases
 Maintainer: protobuf@googlegroups.com
 Maintainer-email: protobuf@googlegroups.com
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/protocolbuffers/protobuf
```

### Comparing `protobuf-5.26.0rc3/README.md` & `protobuf-5.26.1/README.md`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/any_pb2.py` & `protobuf-5.26.1/google/protobuf/any_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/protobuf/any.proto
-# Protobuf Python Version: 5.26.0-rc3
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `protobuf-5.26.0rc3/google/protobuf/api_pb2.py` & `protobuf-5.26.1/google/protobuf/api_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/protobuf/api.proto
-# Protobuf Python Version: 5.26.0-rc3
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `protobuf-5.26.0rc3/google/protobuf/compiler/plugin_pb2.py` & `protobuf-5.26.1/google/protobuf/compiler/plugin_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/protobuf/compiler/plugin.proto
-# Protobuf Python Version: 5.26.0-rc3
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `protobuf-5.26.0rc3/google/protobuf/descriptor.py` & `protobuf-5.26.1/google/protobuf/descriptor.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/descriptor.upb.h` & `protobuf-5.26.1/google/protobuf/descriptor.upb.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/descriptor.upb_minitable.c` & `protobuf-5.26.1/google/protobuf/descriptor.upb_minitable.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/descriptor.upb_minitable.h` & `protobuf-5.26.1/google/protobuf/descriptor.upb_minitable.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/descriptor.upbdefs.c` & `protobuf-5.26.1/google/protobuf/descriptor.upbdefs.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/descriptor.upbdefs.h` & `protobuf-5.26.1/google/protobuf/descriptor.upbdefs.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/descriptor_database.py` & `protobuf-5.26.1/google/protobuf/descriptor_database.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/descriptor_pb2.py` & `protobuf-5.26.1/google/protobuf/descriptor_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/protobuf/descriptor.proto
-# Protobuf Python Version: 5.26.0-rc3
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `protobuf-5.26.0rc3/google/protobuf/descriptor_pool.py` & `protobuf-5.26.1/google/protobuf/descriptor_pool.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/duration_pb2.py` & `protobuf-5.26.1/google/protobuf/duration_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/protobuf/duration.proto
-# Protobuf Python Version: 5.26.0-rc3
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `protobuf-5.26.0rc3/google/protobuf/empty_pb2.py` & `protobuf-5.26.1/google/protobuf/empty_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/protobuf/empty.proto
-# Protobuf Python Version: 5.26.0-rc3
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `protobuf-5.26.0rc3/google/protobuf/field_mask_pb2.py` & `protobuf-5.26.1/google/protobuf/field_mask_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/protobuf/field_mask.proto
-# Protobuf Python Version: 5.26.0-rc3
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `protobuf-5.26.0rc3/google/protobuf/internal/_parameterized.py` & `protobuf-5.26.1/google/protobuf/internal/_parameterized.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/internal/api_implementation.py` & `protobuf-5.26.1/google/protobuf/internal/api_implementation.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/internal/builder.py` & `protobuf-5.26.1/google/protobuf/internal/builder.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/internal/containers.py` & `protobuf-5.26.1/google/protobuf/internal/containers.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/internal/decoder.py` & `protobuf-5.26.1/google/protobuf/internal/decoder.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/internal/encoder.py` & `protobuf-5.26.1/google/protobuf/internal/encoder.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/internal/enum_type_wrapper.py` & `protobuf-5.26.1/google/protobuf/internal/enum_type_wrapper.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/internal/extension_dict.py` & `protobuf-5.26.1/google/protobuf/internal/extension_dict.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/internal/field_mask.py` & `protobuf-5.26.1/google/protobuf/internal/field_mask.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/internal/message_listener.py` & `protobuf-5.26.1/google/protobuf/internal/message_listener.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/internal/python_message.py` & `protobuf-5.26.1/google/protobuf/internal/python_message.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/internal/testing_refleaks.py` & `protobuf-5.26.1/google/protobuf/internal/testing_refleaks.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/internal/type_checkers.py` & `protobuf-5.26.1/google/protobuf/internal/type_checkers.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/internal/well_known_types.py` & `protobuf-5.26.1/google/protobuf/internal/well_known_types.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/internal/wire_format.py` & `protobuf-5.26.1/google/protobuf/internal/wire_format.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/json_format.py` & `protobuf-5.26.1/google/protobuf/json_format.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/message.py` & `protobuf-5.26.1/google/protobuf/message.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/message_factory.py` & `protobuf-5.26.1/google/protobuf/message_factory.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/proto_builder.py` & `protobuf-5.26.1/google/protobuf/proto_builder.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/pyext/cpp_message.py` & `protobuf-5.26.1/google/protobuf/pyext/cpp_message.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/reflection.py` & `protobuf-5.26.1/google/protobuf/reflection.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/service.py` & `protobuf-5.26.1/google/protobuf/service.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/service_reflection.py` & `protobuf-5.26.1/google/protobuf/service_reflection.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/source_context_pb2.py` & `protobuf-5.26.1/google/protobuf/source_context_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/protobuf/source_context.proto
-# Protobuf Python Version: 5.26.0-rc3
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `protobuf-5.26.0rc3/google/protobuf/struct_pb2.py` & `protobuf-5.26.1/google/protobuf/struct_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/protobuf/struct.proto
-# Protobuf Python Version: 5.26.0-rc3
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `protobuf-5.26.0rc3/google/protobuf/symbol_database.py` & `protobuf-5.26.1/google/protobuf/symbol_database.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/text_encoding.py` & `protobuf-5.26.1/google/protobuf/text_encoding.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/text_format.py` & `protobuf-5.26.1/google/protobuf/text_format.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/timestamp_pb2.py` & `protobuf-5.26.1/google/protobuf/timestamp_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/protobuf/timestamp.proto
-# Protobuf Python Version: 5.26.0-rc3
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `protobuf-5.26.0rc3/google/protobuf/type_pb2.py` & `protobuf-5.26.1/google/protobuf/type_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/protobuf/type.proto
-# Protobuf Python Version: 5.26.0-rc3
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `protobuf-5.26.0rc3/google/protobuf/unknown_fields.py` & `protobuf-5.26.1/google/protobuf/unknown_fields.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/google/protobuf/wrappers_pb2.py` & `protobuf-5.26.1/google/protobuf/wrappers_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/protobuf/wrappers.proto
-# Protobuf Python Version: 5.26.0-rc3
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `protobuf-5.26.0rc3/protobuf.egg-info/PKG-INFO` & `protobuf-5.26.1/protobuf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protobuf
-Version: 5.26.0rc3
+Version: 5.26.1
 Summary: Protocol Buffers
 Home-page: https://developers.google.com/protocol-buffers/
 Download-URL: https://github.com/protocolbuffers/protobuf/releases
 Maintainer: protobuf@googlegroups.com
 Maintainer-email: protobuf@googlegroups.com
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/protocolbuffers/protobuf
```

### Comparing `protobuf-5.26.0rc3/protobuf.egg-info/SOURCES.txt` & `protobuf-5.26.1/protobuf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/python/convert.c` & `protobuf-5.26.1/python/convert.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/python/convert.h` & `protobuf-5.26.1/python/convert.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/python/descriptor.c` & `protobuf-5.26.1/python/descriptor.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/python/descriptor.h` & `protobuf-5.26.1/python/descriptor.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/python/descriptor_containers.c` & `protobuf-5.26.1/python/descriptor_containers.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/python/descriptor_containers.h` & `protobuf-5.26.1/python/descriptor_containers.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/python/descriptor_pool.c` & `protobuf-5.26.1/python/descriptor_pool.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/python/descriptor_pool.h` & `protobuf-5.26.1/python/descriptor_pool.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/python/extension_dict.c` & `protobuf-5.26.1/python/extension_dict.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/python/extension_dict.h` & `protobuf-5.26.1/python/extension_dict.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/python/map.c` & `protobuf-5.26.1/python/map.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/python/map.h` & `protobuf-5.26.1/python/map.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/python/message.c` & `protobuf-5.26.1/python/message.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/python/message.h` & `protobuf-5.26.1/python/message.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/python/protobuf.c` & `protobuf-5.26.1/python/protobuf.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/python/protobuf.h` & `protobuf-5.26.1/python/protobuf.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/python/python_api.h` & `protobuf-5.26.1/python/python_api.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/python/repeated.c` & `protobuf-5.26.1/python/repeated.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/python/repeated.h` & `protobuf-5.26.1/python/repeated.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/python/unknown_fields.c` & `protobuf-5.26.1/python/unknown_fields.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/python/unknown_fields.h` & `protobuf-5.26.1/python/unknown_fields.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/setup.py` & `protobuf-5.26.1/setup.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/base/descriptor_constants.h` & `protobuf-5.26.1/upb/base/descriptor_constants.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/base/internal/endian.h` & `protobuf-5.26.1/upb/base/internal/endian.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/base/internal/log2.h` & `protobuf-5.26.1/upb/base/internal/log2.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/base/status.c` & `protobuf-5.26.1/upb/base/status.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/base/status.h` & `protobuf-5.26.1/upb/base/status.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/base/string_view.h` & `protobuf-5.26.1/upb/base/string_view.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/base/upcast.h` & `protobuf-5.26.1/upb/base/upcast.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/generated_code_support.h` & `protobuf-5.26.1/upb/generated_code_support.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/hash/common.c` & `protobuf-5.26.1/upb/hash/common.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/hash/common.h` & `protobuf-5.26.1/upb/hash/common.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/hash/int_table.h` & `protobuf-5.26.1/upb/hash/int_table.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/hash/str_table.h` & `protobuf-5.26.1/upb/hash/str_table.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/lex/atoi.c` & `protobuf-5.26.1/upb/lex/atoi.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/lex/atoi.h` & `protobuf-5.26.1/upb/lex/atoi.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/lex/round_trip.c` & `protobuf-5.26.1/upb/lex/round_trip.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/lex/round_trip.h` & `protobuf-5.26.1/upb/lex/round_trip.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/lex/strtod.c` & `protobuf-5.26.1/upb/lex/strtod.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/lex/strtod.h` & `protobuf-5.26.1/upb/lex/strtod.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/lex/unicode.c` & `protobuf-5.26.1/upb/lex/unicode.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/lex/unicode.h` & `protobuf-5.26.1/upb/lex/unicode.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mem/alloc.c` & `protobuf-5.26.1/upb/mem/alloc.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mem/alloc.h` & `protobuf-5.26.1/upb/mem/alloc.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mem/arena.c` & `protobuf-5.26.1/upb/mem/arena.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mem/arena.h` & `protobuf-5.26.1/upb/mem/arena.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mem/internal/arena.h` & `protobuf-5.26.1/upb/mem/internal/arena.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/accessors.c` & `protobuf-5.26.1/upb/message/accessors.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/accessors.h` & `protobuf-5.26.1/upb/message/accessors.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/accessors_split64.h` & `protobuf-5.26.1/upb/message/accessors_split64.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/array.c` & `protobuf-5.26.1/upb/message/array.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/array.h` & `protobuf-5.26.1/upb/message/array.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/array_split64.h` & `protobuf-5.26.1/upb/message/array_split64.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/compare.c` & `protobuf-5.26.1/upb/message/compare.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/compare.h` & `protobuf-5.26.1/upb/message/compare.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/compat.c` & `protobuf-5.26.1/upb/message/compat.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/compat.h` & `protobuf-5.26.1/upb/message/compat.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/copy.c` & `protobuf-5.26.1/upb/message/copy.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/copy.h` & `protobuf-5.26.1/upb/message/copy.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/internal/accessors.h` & `protobuf-5.26.1/upb/message/internal/accessors.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/internal/array.h` & `protobuf-5.26.1/upb/message/internal/array.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/internal/extension.c` & `protobuf-5.26.1/upb/message/internal/extension.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/internal/extension.h` & `protobuf-5.26.1/upb/message/internal/extension.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/internal/map.h` & `protobuf-5.26.1/upb/message/internal/map.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/internal/map_entry.h` & `protobuf-5.26.1/upb/message/internal/map_entry.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/internal/map_sorter.h` & `protobuf-5.26.1/upb/message/internal/map_sorter.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/internal/message.c` & `protobuf-5.26.1/upb/message/internal/message.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/internal/message.h` & `protobuf-5.26.1/upb/message/internal/message.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/internal/tagged_ptr.h` & `protobuf-5.26.1/upb/message/internal/tagged_ptr.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/internal/types.h` & `protobuf-5.26.1/upb/message/internal/types.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/map.c` & `protobuf-5.26.1/upb/message/map.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/map.h` & `protobuf-5.26.1/upb/message/map.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/map_gencode_util.h` & `protobuf-5.26.1/upb/message/map_gencode_util.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/map_sorter.c` & `protobuf-5.26.1/upb/message/map_sorter.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/message.c` & `protobuf-5.26.1/upb/message/message.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/message.h` & `protobuf-5.26.1/upb/message/message.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/promote.c` & `protobuf-5.26.1/upb/message/promote.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/promote.h` & `protobuf-5.26.1/upb/message/promote.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/tagged_ptr.h` & `protobuf-5.26.1/upb/message/tagged_ptr.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/message/value.h` & `protobuf-5.26.1/upb/message/value.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_descriptor/build_enum.c` & `protobuf-5.26.1/upb/mini_descriptor/build_enum.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_descriptor/build_enum.h` & `protobuf-5.26.1/upb/mini_descriptor/build_enum.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_descriptor/decode.c` & `protobuf-5.26.1/upb/mini_descriptor/decode.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_descriptor/decode.h` & `protobuf-5.26.1/upb/mini_descriptor/decode.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_descriptor/internal/base92.c` & `protobuf-5.26.1/upb/mini_descriptor/internal/base92.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_descriptor/internal/base92.h` & `protobuf-5.26.1/upb/mini_descriptor/internal/base92.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_descriptor/internal/decoder.h` & `protobuf-5.26.1/upb/mini_descriptor/internal/decoder.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_descriptor/internal/encode.c` & `protobuf-5.26.1/upb/mini_descriptor/internal/encode.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_descriptor/internal/encode.h` & `protobuf-5.26.1/upb/mini_descriptor/internal/encode.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_descriptor/internal/modifiers.h` & `protobuf-5.26.1/upb/mini_descriptor/internal/modifiers.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_descriptor/internal/wire_constants.h` & `protobuf-5.26.1/upb/mini_descriptor/internal/wire_constants.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_descriptor/link.c` & `protobuf-5.26.1/upb/mini_descriptor/link.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_descriptor/link.h` & `protobuf-5.26.1/upb/mini_descriptor/link.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_table/compat.c` & `protobuf-5.26.1/upb/mini_table/compat.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_table/compat.h` & `protobuf-5.26.1/upb/mini_table/compat.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_table/enum.h` & `protobuf-5.26.1/upb/mini_table/enum.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_table/extension.h` & `protobuf-5.26.1/upb/mini_table/extension.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_table/extension_registry.c` & `protobuf-5.26.1/upb/mini_table/extension_registry.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_table/extension_registry.h` & `protobuf-5.26.1/upb/mini_table/extension_registry.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_table/field.h` & `protobuf-5.26.1/upb/mini_table/field.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_table/file.h` & `protobuf-5.26.1/upb/mini_table/file.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_table/internal/enum.h` & `protobuf-5.26.1/upb/mini_table/internal/enum.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_table/internal/extension.h` & `protobuf-5.26.1/upb/mini_table/internal/extension.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_table/internal/field.h` & `protobuf-5.26.1/upb/mini_table/internal/field.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_table/internal/file.h` & `protobuf-5.26.1/upb/mini_table/internal/file.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_table/internal/message.c` & `protobuf-5.26.1/upb/mini_table/internal/message.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_table/internal/message.h` & `protobuf-5.26.1/upb/mini_table/internal/message.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_table/internal/size_log2.h` & `protobuf-5.26.1/upb/mini_table/internal/size_log2.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_table/internal/sub.h` & `protobuf-5.26.1/upb/mini_table/internal/sub.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_table/message.c` & `protobuf-5.26.1/upb/mini_table/message.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_table/message.h` & `protobuf-5.26.1/upb/mini_table/message.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/mini_table/sub.h` & `protobuf-5.26.1/upb/mini_table/sub.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/port/atomic.h` & `protobuf-5.26.1/upb/port/atomic.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/port/def.inc` & `protobuf-5.26.1/upb/port/def.inc`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/port/undef.inc` & `protobuf-5.26.1/upb/port/undef.inc`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/port/vsnprintf_compat.h` & `protobuf-5.26.1/upb/port/vsnprintf_compat.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/common.h` & `protobuf-5.26.1/upb/reflection/common.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/def.h` & `protobuf-5.26.1/upb/reflection/def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/def_pool.c` & `protobuf-5.26.1/upb/reflection/def_pool.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/def_pool.h` & `protobuf-5.26.1/upb/reflection/def_pool.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/def_type.c` & `protobuf-5.26.1/upb/reflection/def_type.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/def_type.h` & `protobuf-5.26.1/upb/reflection/def_type.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/desc_state.c` & `protobuf-5.26.1/upb/reflection/desc_state.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/enum_def.c` & `protobuf-5.26.1/upb/reflection/enum_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/enum_def.h` & `protobuf-5.26.1/upb/reflection/enum_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/enum_reserved_range.c` & `protobuf-5.26.1/upb/reflection/enum_reserved_range.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/enum_reserved_range.h` & `protobuf-5.26.1/upb/reflection/enum_reserved_range.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/enum_value_def.c` & `protobuf-5.26.1/upb/reflection/enum_value_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/enum_value_def.h` & `protobuf-5.26.1/upb/reflection/enum_value_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/extension_range.c` & `protobuf-5.26.1/upb/reflection/extension_range.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/extension_range.h` & `protobuf-5.26.1/upb/reflection/extension_range.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/field_def.c` & `protobuf-5.26.1/upb/reflection/field_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/field_def.h` & `protobuf-5.26.1/upb/reflection/field_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/file_def.c` & `protobuf-5.26.1/upb/reflection/file_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/file_def.h` & `protobuf-5.26.1/upb/reflection/file_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/internal/def_builder.c` & `protobuf-5.26.1/upb/reflection/internal/def_builder.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/internal/def_builder.h` & `protobuf-5.26.1/upb/reflection/internal/def_builder.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/internal/def_pool.h` & `protobuf-5.26.1/upb/reflection/internal/def_pool.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/internal/desc_state.h` & `protobuf-5.26.1/upb/reflection/internal/desc_state.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/internal/enum_def.h` & `protobuf-5.26.1/upb/reflection/internal/enum_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/internal/enum_reserved_range.h` & `protobuf-5.26.1/upb/reflection/internal/enum_reserved_range.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/internal/enum_value_def.h` & `protobuf-5.26.1/upb/reflection/internal/enum_value_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/internal/extension_range.h` & `protobuf-5.26.1/upb/reflection/internal/extension_range.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/internal/field_def.h` & `protobuf-5.26.1/upb/reflection/internal/field_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/internal/file_def.h` & `protobuf-5.26.1/upb/reflection/internal/file_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/internal/message_def.h` & `protobuf-5.26.1/upb/reflection/internal/message_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/internal/message_reserved_range.h` & `protobuf-5.26.1/upb/reflection/internal/message_reserved_range.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/internal/method_def.h` & `protobuf-5.26.1/upb/reflection/internal/method_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/internal/oneof_def.h` & `protobuf-5.26.1/upb/reflection/internal/oneof_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/internal/service_def.h` & `protobuf-5.26.1/upb/reflection/internal/service_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/internal/strdup2.c` & `protobuf-5.26.1/upb/reflection/internal/strdup2.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/internal/strdup2.h` & `protobuf-5.26.1/upb/reflection/internal/strdup2.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/internal/upb_edition_defaults.h` & `protobuf-5.26.1/upb/reflection/internal/upb_edition_defaults.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/message.c` & `protobuf-5.26.1/upb/reflection/message.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/message.h` & `protobuf-5.26.1/upb/reflection/message.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/message_def.c` & `protobuf-5.26.1/upb/reflection/message_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/message_def.h` & `protobuf-5.26.1/upb/reflection/message_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/message_reserved_range.c` & `protobuf-5.26.1/upb/reflection/message_reserved_range.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/message_reserved_range.h` & `protobuf-5.26.1/upb/reflection/message_reserved_range.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/method_def.c` & `protobuf-5.26.1/upb/reflection/method_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/method_def.h` & `protobuf-5.26.1/upb/reflection/method_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/oneof_def.c` & `protobuf-5.26.1/upb/reflection/oneof_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/oneof_def.h` & `protobuf-5.26.1/upb/reflection/oneof_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/service_def.c` & `protobuf-5.26.1/upb/reflection/service_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/reflection/service_def.h` & `protobuf-5.26.1/upb/reflection/service_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/text/encode.c` & `protobuf-5.26.1/upb/text/encode.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/text/encode.h` & `protobuf-5.26.1/upb/text/encode.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/util/compare.c` & `protobuf-5.26.1/upb/util/compare.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/util/compare.h` & `protobuf-5.26.1/upb/util/compare.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/util/def_to_proto.c` & `protobuf-5.26.1/upb/util/def_to_proto.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/util/def_to_proto.h` & `protobuf-5.26.1/upb/util/def_to_proto.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/util/required_fields.c` & `protobuf-5.26.1/upb/util/required_fields.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/util/required_fields.h` & `protobuf-5.26.1/upb/util/required_fields.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/wire/decode.c` & `protobuf-5.26.1/upb/wire/decode.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/wire/decode.h` & `protobuf-5.26.1/upb/wire/decode.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/wire/encode.c` & `protobuf-5.26.1/upb/wire/encode.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/wire/encode.h` & `protobuf-5.26.1/upb/wire/encode.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/wire/eps_copy_input_stream.c` & `protobuf-5.26.1/upb/wire/eps_copy_input_stream.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/wire/eps_copy_input_stream.h` & `protobuf-5.26.1/upb/wire/eps_copy_input_stream.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/wire/internal/constants.h` & `protobuf-5.26.1/upb/wire/internal/constants.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/wire/internal/decode_fast.c` & `protobuf-5.26.1/upb/wire/internal/decode_fast.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/wire/internal/decode_fast.h` & `protobuf-5.26.1/upb/wire/internal/decode_fast.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/wire/internal/decoder.h` & `protobuf-5.26.1/upb/wire/internal/decoder.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/wire/internal/reader.h` & `protobuf-5.26.1/upb/wire/internal/reader.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/wire/reader.c` & `protobuf-5.26.1/upb/wire/reader.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/wire/reader.h` & `protobuf-5.26.1/upb/wire/reader.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/upb/wire/types.h` & `protobuf-5.26.1/upb/wire/types.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/utf8_range/utf8_range.c` & `protobuf-5.26.1/utf8_range/utf8_range.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.0rc3/utf8_range/utf8_range.h` & `protobuf-5.26.1/utf8_range/utf8_range.h`

 * *Files identical despite different names*

