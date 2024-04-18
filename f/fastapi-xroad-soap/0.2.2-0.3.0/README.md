# Comparing `tmp/fastapi_xroad_soap-0.2.2.tar.gz` & `tmp/fastapi_xroad_soap-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_xroad_soap-0.2.2.tar", max compression
+gzip compressed data, was "fastapi_xroad_soap-0.3.0.tar", max compression
```

## Comparing `fastapi_xroad_soap-0.2.2.tar` & `fastapi_xroad_soap-0.3.0.tar`

### file list

```diff
@@ -1,57 +1,62 @@
--rw-r--r--   0        0        0    13749 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/LICENSE
--rw-r--r--   0        0        0     2819 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/README.md
--rw-r--r--   0        0        0      524 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/__init__.py
--rw-r--r--   0        0        0      567 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/elements.py
--rw-r--r--   0        0        0      471 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/faults.py
--rw-r--r--   0        0        0      340 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/__init__.py
--rw-r--r--   0        0        0      579 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/base/__init__.py
--rw-r--r--   0        0        0     4150 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/base/body.py
--rw-r--r--   0        0        0     1181 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/base/meta.py
--rw-r--r--   0        0        0     3299 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/base/spec.py
--rw-r--r--   0        0        0      955 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/cid_gen.py
--rw-r--r--   0        0        0     1119 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/constants.py
--rw-r--r--   0        0        0     1031 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/elements/__init__.py
--rw-r--r--   0        0        0     1120 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/elements/boolean.py
--rw-r--r--   0        0        0     2205 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/elements/common.py
--rw-r--r--   0        0        0     1146 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/elements/date.py
--rw-r--r--   0        0        0     1194 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/elements/datetime.py
--rw-r--r--   0        0        0     1131 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/elements/float.py
--rw-r--r--   0        0        0     1278 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/elements/integer.py
--rw-r--r--   0        0        0     1201 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/elements/netres.py
--rw-r--r--   0        0        0     1235 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/elements/string.py
--rw-r--r--   0        0        0     5104 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/elements/swaref.py
--rw-r--r--   0        0        0     1146 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/elements/time.py
--rw-r--r--   0        0        0     3157 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/elements/validators.py
--rw-r--r--   0        0        0      679 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/envelope/__init__.py
--rw-r--r--   0        0        0     2783 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/envelope/factory.py
--rw-r--r--   0        0        0     1401 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/envelope/generics.py
--rw-r--r--   0        0        0     1910 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/envelope/header.py
--rw-r--r--   0        0        0     1910 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/file_size.py
--rw-r--r--   0        0        0      732 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/multipart/__init__.py
--rw-r--r--   0        0        0     2801 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/multipart/bodypart.py
--rw-r--r--   0        0        0     2124 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/multipart/decoder.py
--rw-r--r--   0        0        0     2502 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/multipart/encoder.py
--rw-r--r--   0        0        0     1024 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/multipart/errors.py
--rw-r--r--   0        0        0      901 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/soap/__init__.py
--rw-r--r--   0        0        0     4699 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/soap/action.py
--rw-r--r--   0        0        0     4023 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/soap/faults.py
--rw-r--r--   0        0        0     2742 2024-04-14 17:30:49.118490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/soap/response.py
--rw-r--r--   0        0        0     4822 2024-04-14 17:30:49.122490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/soap/service.py
--rw-r--r--   0        0        0     1938 2024-04-14 17:30:49.122490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/soap/service.pyi
--rw-r--r--   0        0        0     5033 2024-04-14 17:30:49.122490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/storage.py
--rw-r--r--   0        0        0      874 2024-04-14 17:30:49.122490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/utils/__init__.py
--rw-r--r--   0        0        0     1750 2024-04-14 17:30:49.122490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/utils/content_utils.py
--rw-r--r--   0        0        0     2673 2024-04-14 17:30:49.122490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/utils/path_utils.py
--rw-r--r--   0        0        0     2575 2024-04-14 17:30:49.122490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/utils/route_utils.py
--rw-r--r--   0        0        0     2487 2024-04-14 17:30:49.122490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/wsdl/__init__.py
--rw-r--r--   0        0        0     2840 2024-04-14 17:30:49.122490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/wsdl/binding.py
--rw-r--r--   0        0        0     1558 2024-04-14 17:30:49.122490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/wsdl/conditions.py
--rw-r--r--   0        0        0     1334 2024-04-14 17:30:49.122490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/wsdl/definitions.py
--rw-r--r--   0        0        0      640 2024-04-14 17:30:49.122490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/wsdl/generator.py
--rw-r--r--   0        0        0     1534 2024-04-14 17:30:49.122490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/wsdl/port_type.py
--rw-r--r--   0        0        0     4947 2024-04-14 17:30:49.122490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/wsdl/restrictions.py
--rw-r--r--   0        0        0     2264 2024-04-14 17:30:49.122490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/wsdl/schema.py
--rw-r--r--   0        0        0     1335 2024-04-14 17:30:49.122490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/wsdl/service.py
--rw-r--r--   0        0        0      506 2024-04-14 17:30:49.122490 fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/utils.py
--rw-r--r--   0        0        0     2579 2024-04-14 17:30:49.122490 fastapi_xroad_soap-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4540 1970-01-01 00:00:00.000000 fastapi_xroad_soap-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    13831 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2939 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/README.md
+-rw-r--r--   0        0        0      524 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/__init__.py
+-rw-r--r--   0        0        0      574 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/elements.py
+-rw-r--r--   0        0        0      471 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/faults.py
+-rw-r--r--   0        0        0      340 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/__init__.py
+-rw-r--r--   0        0        0      610 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/base/__init__.py
+-rw-r--r--   0        0        0     4737 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/base/body.py
+-rw-r--r--   0        0        0     1181 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/base/meta.py
+-rw-r--r--   0        0        0     4348 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/base/spec.py
+-rw-r--r--   0        0        0     1062 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/constants.py
+-rw-r--r--   0        0        0      486 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/__init__.py
+-rw-r--r--   0        0        0     1257 2024-04-18 11:28:45.422820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/boolean.py
+-rw-r--r--   0        0        0     1195 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/date.py
+-rw-r--r--   0        0        0     1243 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/datetime.py
+-rw-r--r--   0        0        0     1180 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/float.py
+-rw-r--r--   0        0        0     1223 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/integer.py
+-rw-r--r--   0        0        0     1247 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/netres.py
+-rw-r--r--   0        0        0     1284 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/string.py
+-rw-r--r--   0        0        0     7247 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/swaref.py
+-rw-r--r--   0        0        0     1195 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/time.py
+-rw-r--r--   0        0        0     2007 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/numeric_type_spec.py
+-rw-r--r--   0        0        0     2158 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/string_type_spec.py
+-rw-r--r--   0        0        0     3157 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/validators.py
+-rw-r--r--   0        0        0      679 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/envelope/__init__.py
+-rw-r--r--   0        0        0     2783 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/envelope/factory.py
+-rw-r--r--   0        0        0     1401 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/envelope/generics.py
+-rw-r--r--   0        0        0     1912 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/envelope/header.py
+-rw-r--r--   0        0        0     1910 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/file_size.py
+-rw-r--r--   0        0        0      732 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/multipart/__init__.py
+-rw-r--r--   0        0        0     2801 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/multipart/bodypart.py
+-rw-r--r--   0        0        0     2124 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/multipart/decoder.py
+-rw-r--r--   0        0        0     2493 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/multipart/encoder.py
+-rw-r--r--   0        0        0     1024 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/multipart/errors.py
+-rw-r--r--   0        0        0      901 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/soap/__init__.py
+-rw-r--r--   0        0        0     5286 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/soap/action.py
+-rw-r--r--   0        0        0     4155 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/soap/faults.py
+-rw-r--r--   0        0        0     1613 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/soap/response.py
+-rw-r--r--   0        0        0     5117 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/soap/service.py
+-rw-r--r--   0        0        0     2071 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/soap/service.pyi
+-rw-r--r--   0        0        0     2122 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/soap/validators.py
+-rw-r--r--   0        0        0     5005 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/storage.py
+-rw-r--r--   0        0        0     1695 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/uid_gen.py
+-rw-r--r--   0        0        0      900 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/utils/__init__.py
+-rw-r--r--   0        0        0     1907 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/utils/content_utils.py
+-rw-r--r--   0        0        0     2673 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/utils/path_utils.py
+-rw-r--r--   0        0        0      851 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/utils/route_utils.py
+-rw-r--r--   0        0        0      397 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/__init__.py
+-rw-r--r--   0        0        0     4747 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/generator.py
+-rw-r--r--   0        0        0     3706 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/helpers.py
+-rw-r--r--   0        0        0     2024 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/__init__.py
+-rw-r--r--   0        0        0     2864 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/binding.py
+-rw-r--r--   0        0        0     1270 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/conditions.py
+-rw-r--r--   0        0        0     1360 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/definitions.py
+-rw-r--r--   0        0        0     1698 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/port_type.py
+-rw-r--r--   0        0        0     1315 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/restrictions.py
+-rw-r--r--   0        0        0     1947 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/schema.py
+-rw-r--r--   0        0        0     1361 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/service.py
+-rw-r--r--   0        0        0      561 2024-04-18 11:28:45.426820 fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/utils.py
+-rw-r--r--   0        0        0     2579 2024-04-18 11:28:45.518821 fastapi_xroad_soap-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4660 1970-01-01 00:00:00.000000 fastapi_xroad_soap-0.3.0/PKG-INFO
```

### Comparing `fastapi_xroad_soap-0.2.2/LICENSE` & `fastapi_xroad_soap-0.3.0/LICENSE`

 * *Files 5% similar despite different names*

```diff
@@ -1,860 +1,865 @@
 00000000: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00000010: 2020 2020 2020 2020 4555 524f 5045 414e          EUROPEAN
 00000020: 2055 4e49 4f4e 2050 5542 4c49 4320 4c49   UNION PUBLIC LI
 00000030: 4345 4e43 4520 762e 2031 2e32 0a20 2020  CENCE v. 1.2.   
 00000040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000050: 2020 2045 5550 4c20 a920 7468 6520 4575     EUPL . the Eu
-00000060: 726f 7065 616e 2055 6e69 6f6e 2032 3030  ropean Union 200
-00000070: 372c 2032 3031 360a 0a54 6869 7320 4575  7, 2016..This Eu
-00000080: 726f 7065 616e 2055 6e69 6f6e 2050 7562  ropean Union Pub
-00000090: 6c69 6320 4c69 6365 6e63 6520 2874 6865  lic Licence (the
-000000a0: 2091 4555 504c 9229 2061 7070 6c69 6573   .EUPL.) applies
-000000b0: 2074 6f20 7468 6520 576f 726b 2028 6173   to the Work (as
-000000c0: 0a64 6566 696e 6564 2062 656c 6f77 2920  .defined below) 
-000000d0: 7768 6963 6820 6973 2070 726f 7669 6465  which is provide
-000000e0: 6420 756e 6465 7220 7468 6520 7465 726d  d under the term
-000000f0: 7320 6f66 2074 6869 7320 4c69 6365 6e63  s of this Licenc
-00000100: 652e 2041 6e79 2075 7365 206f 660a 7468  e. Any use of.th
-00000110: 6520 576f 726b 2c20 6f74 6865 7220 7468  e Work, other th
-00000120: 616e 2061 7320 6175 7468 6f72 6973 6564  an as authorised
-00000130: 2075 6e64 6572 2074 6869 7320 4c69 6365   under this Lice
-00000140: 6e63 6520 6973 2070 726f 6869 6269 7465  nce is prohibite
-00000150: 6420 2874 6f20 7468 650a 6578 7465 6e74  d (to the.extent
-00000160: 2073 7563 6820 7573 6520 6973 2063 6f76   such use is cov
-00000170: 6572 6564 2062 7920 6120 7269 6768 7420  ered by a right 
-00000180: 6f66 2074 6865 2063 6f70 7972 6967 6874  of the copyright
-00000190: 2068 6f6c 6465 7220 6f66 2074 6865 2057   holder of the W
-000001a0: 6f72 6b29 2e0a 0a54 6865 2057 6f72 6b20  ork)...The Work 
-000001b0: 6973 2070 726f 7669 6465 6420 756e 6465  is provided unde
-000001c0: 7220 7468 6520 7465 726d 7320 6f66 2074  r the terms of t
-000001d0: 6869 7320 4c69 6365 6e63 6520 7768 656e  his Licence when
-000001e0: 2074 6865 204c 6963 656e 736f 7220 2861   the Licensor (a
-000001f0: 730a 6465 6669 6e65 6420 6265 6c6f 7729  s.defined below)
-00000200: 2068 6173 2070 6c61 6365 6420 7468 6520   has placed the 
-00000210: 666f 6c6c 6f77 696e 6720 6e6f 7469 6365  following notice
-00000220: 2069 6d6d 6564 6961 7465 6c79 2066 6f6c   immediately fol
-00000230: 6c6f 7769 6e67 2074 6865 0a63 6f70 7972  lowing the.copyr
-00000240: 6967 6874 206e 6f74 6963 6520 666f 7220  ight notice for 
-00000250: 7468 6520 576f 726b 3a0a 0a20 2020 2020  the Work:..     
-00000260: 2020 204c 6963 656e 7365 6420 756e 6465     Licensed unde
-00000270: 7220 7468 6520 4555 504c 0a0a 6f72 2068  r the EUPL..or h
-00000280: 6173 2065 7870 7265 7373 6564 2062 7920  as expressed by 
-00000290: 616e 7920 6f74 6865 7220 6d65 616e 7320  any other means 
-000002a0: 6869 7320 7769 6c6c 696e 676e 6573 7320  his willingness 
-000002b0: 746f 206c 6963 656e 7365 2075 6e64 6572  to license under
-000002c0: 2074 6865 2045 5550 4c2e 0a0a 312e 2044   the EUPL...1. D
-000002d0: 6566 696e 6974 696f 6e73 0a0a 496e 2074  efinitions..In t
-000002e0: 6869 7320 4c69 6365 6e63 652c 2074 6865  his Licence, the
-000002f0: 2066 6f6c 6c6f 7769 6e67 2074 6572 6d73   following terms
-00000300: 2068 6176 6520 7468 6520 666f 6c6c 6f77   have the follow
-00000310: 696e 6720 6d65 616e 696e 673a 0a0a 2d20  ing meaning:..- 
-00000320: 9154 6865 204c 6963 656e 6365 923a 2074  .The Licence.: t
-00000330: 6869 7320 4c69 6365 6e63 652e 0a0a 2d20  his Licence...- 
-00000340: 9154 6865 204f 7269 6769 6e61 6c20 576f  .The Original Wo
-00000350: 726b 923a 2074 6865 2077 6f72 6b20 6f72  rk.: the work or
-00000360: 2073 6f66 7477 6172 6520 6469 7374 7269   software distri
-00000370: 6275 7465 6420 6f72 2063 6f6d 6d75 6e69  buted or communi
-00000380: 6361 7465 6420 6279 2074 6865 0a20 204c  cated by the.  L
-00000390: 6963 656e 736f 7220 756e 6465 7220 7468  icensor under th
-000003a0: 6973 204c 6963 656e 6365 2c20 6176 6169  is Licence, avai
-000003b0: 6c61 626c 6520 6173 2053 6f75 7263 6520  lable as Source 
-000003c0: 436f 6465 2061 6e64 2061 6c73 6f20 6173  Code and also as
-000003d0: 2045 7865 6375 7461 626c 650a 2020 436f   Executable.  Co
-000003e0: 6465 2061 7320 7468 6520 6361 7365 206d  de as the case m
-000003f0: 6179 2062 652e 0a0a 2d20 9144 6572 6976  ay be...- .Deriv
-00000400: 6174 6976 6520 576f 726b 7392 3a20 7468  ative Works.: th
-00000410: 6520 776f 726b 7320 6f72 2073 6f66 7477  e works or softw
-00000420: 6172 6520 7468 6174 2063 6f75 6c64 2062  are that could b
-00000430: 6520 6372 6561 7465 6420 6279 2074 6865  e created by the
-00000440: 0a20 204c 6963 656e 7365 652c 2062 6173  .  Licensee, bas
-00000450: 6564 2075 706f 6e20 7468 6520 4f72 6967  ed upon the Orig
-00000460: 696e 616c 2057 6f72 6b20 6f72 206d 6f64  inal Work or mod
-00000470: 6966 6963 6174 696f 6e73 2074 6865 7265  ifications there
-00000480: 6f66 2e20 5468 6973 0a20 204c 6963 656e  of. This.  Licen
-00000490: 6365 2064 6f65 7320 6e6f 7420 6465 6669  ce does not defi
-000004a0: 6e65 2074 6865 2065 7874 656e 7420 6f66  ne the extent of
-000004b0: 206d 6f64 6966 6963 6174 696f 6e20 6f72   modification or
-000004c0: 2064 6570 656e 6465 6e63 6520 6f6e 2074   dependence on t
-000004d0: 6865 0a20 204f 7269 6769 6e61 6c20 576f  he.  Original Wo
-000004e0: 726b 2072 6571 7569 7265 6420 696e 206f  rk required in o
-000004f0: 7264 6572 2074 6f20 636c 6173 7369 6679  rder to classify
-00000500: 2061 2077 6f72 6b20 6173 2061 2044 6572   a work as a Der
-00000510: 6976 6174 6976 6520 576f 726b 3b0a 2020  ivative Work;.  
-00000520: 7468 6973 2065 7874 656e 7420 6973 2064  this extent is d
-00000530: 6574 6572 6d69 6e65 6420 6279 2063 6f70  etermined by cop
-00000540: 7972 6967 6874 206c 6177 2061 7070 6c69  yright law appli
-00000550: 6361 626c 6520 696e 2074 6865 2063 6f75  cable in the cou
-00000560: 6e74 7279 0a20 206d 656e 7469 6f6e 6564  ntry.  mentioned
-00000570: 2069 6e20 4172 7469 636c 6520 3135 2e0a   in Article 15..
-00000580: 0a2d 2091 5468 6520 576f 726b 923a 2074  .- .The Work.: t
-00000590: 6865 204f 7269 6769 6e61 6c20 576f 726b  he Original Work
-000005a0: 206f 7220 6974 7320 4465 7269 7661 7469   or its Derivati
-000005b0: 7665 2057 6f72 6b73 2e0a 0a2d 2091 5468  ve Works...- .Th
-000005c0: 6520 536f 7572 6365 2043 6f64 6592 3a20  e Source Code.: 
-000005d0: 7468 6520 6875 6d61 6e2d 7265 6164 6162  the human-readab
-000005e0: 6c65 2066 6f72 6d20 6f66 2074 6865 2057  le form of the W
-000005f0: 6f72 6b20 7768 6963 6820 6973 2074 6865  ork which is the
-00000600: 206d 6f73 740a 2020 636f 6e76 656e 6965   most.  convenie
-00000610: 6e74 2066 6f72 2070 656f 706c 6520 746f  nt for people to
-00000620: 2073 7475 6479 2061 6e64 206d 6f64 6966   study and modif
-00000630: 792e 0a0a 2d20 9154 6865 2045 7865 6375  y...- .The Execu
-00000640: 7461 626c 6520 436f 6465 923a 2061 6e79  table Code.: any
-00000650: 2063 6f64 6520 7768 6963 6820 6861 7320   code which has 
-00000660: 6765 6e65 7261 6c6c 7920 6265 656e 2063  generally been c
-00000670: 6f6d 7069 6c65 6420 616e 6420 7768 6963  ompiled and whic
-00000680: 680a 2020 6973 206d 6561 6e74 2074 6f20  h.  is meant to 
-00000690: 6265 2069 6e74 6572 7072 6574 6564 2062  be interpreted b
-000006a0: 7920 6120 636f 6d70 7574 6572 2061 7320  y a computer as 
-000006b0: 6120 7072 6f67 7261 6d2e 0a0a 2d20 9154  a program...- .T
-000006c0: 6865 204c 6963 656e 736f 7292 3a20 7468  he Licensor.: th
-000006d0: 6520 6e61 7475 7261 6c20 6f72 206c 6567  e natural or leg
-000006e0: 616c 2070 6572 736f 6e20 7468 6174 2064  al person that d
-000006f0: 6973 7472 6962 7574 6573 206f 7220 636f  istributes or co
-00000700: 6d6d 756e 6963 6174 6573 0a20 2074 6865  mmunicates.  the
-00000710: 2057 6f72 6b20 756e 6465 7220 7468 6520   Work under the 
-00000720: 4c69 6365 6e63 652e 0a0a 2d20 9143 6f6e  Licence...- .Con
-00000730: 7472 6962 7574 6f72 2873 2992 3a20 616e  tributor(s).: an
-00000740: 7920 6e61 7475 7261 6c20 6f72 206c 6567  y natural or leg
-00000750: 616c 2070 6572 736f 6e20 7768 6f20 6d6f  al person who mo
-00000760: 6469 6669 6573 2074 6865 2057 6f72 6b20  difies the Work 
-00000770: 756e 6465 720a 2020 7468 6520 4c69 6365  under.  the Lice
-00000780: 6e63 652c 206f 7220 6f74 6865 7277 6973  nce, or otherwis
-00000790: 6520 636f 6e74 7269 6275 7465 7320 746f  e contributes to
-000007a0: 2074 6865 2063 7265 6174 696f 6e20 6f66   the creation of
-000007b0: 2061 2044 6572 6976 6174 6976 6520 576f   a Derivative Wo
-000007c0: 726b 2e0a 0a2d 2091 5468 6520 4c69 6365  rk...- .The Lice
-000007d0: 6e73 6565 9220 6f72 2091 596f 7592 3a20  nsee. or .You.: 
-000007e0: 616e 7920 6e61 7475 7261 6c20 6f72 206c  any natural or l
-000007f0: 6567 616c 2070 6572 736f 6e20 7768 6f20  egal person who 
-00000800: 6d61 6b65 7320 616e 7920 7573 6167 6520  makes any usage 
-00000810: 6f66 0a20 2074 6865 2057 6f72 6b20 756e  of.  the Work un
-00000820: 6465 7220 7468 6520 7465 726d 7320 6f66  der the terms of
-00000830: 2074 6865 204c 6963 656e 6365 2e0a 0a2d   the Licence...-
-00000840: 2091 4469 7374 7269 6275 7469 6f6e 9220   .Distribution. 
-00000850: 6f72 2091 436f 6d6d 756e 6963 6174 696f  or .Communicatio
-00000860: 6e92 3a20 616e 7920 6163 7420 6f66 2073  n.: any act of s
-00000870: 656c 6c69 6e67 2c20 6769 7669 6e67 2c20  elling, giving, 
-00000880: 6c65 6e64 696e 672c 0a20 2072 656e 7469  lending,.  renti
-00000890: 6e67 2c20 6469 7374 7269 6275 7469 6e67  ng, distributing
-000008a0: 2c20 636f 6d6d 756e 6963 6174 696e 672c  , communicating,
-000008b0: 2074 7261 6e73 6d69 7474 696e 672c 206f   transmitting, o
-000008c0: 7220 6f74 6865 7277 6973 6520 6d61 6b69  r otherwise maki
-000008d0: 6e67 0a20 2061 7661 696c 6162 6c65 2c20  ng.  available, 
-000008e0: 6f6e 6c69 6e65 206f 7220 6f66 666c 696e  online or offlin
-000008f0: 652c 2063 6f70 6965 7320 6f66 2074 6865  e, copies of the
-00000900: 2057 6f72 6b20 6f72 2070 726f 7669 6469   Work or providi
-00000910: 6e67 2061 6363 6573 7320 746f 2069 7473  ng access to its
-00000920: 0a20 2065 7373 656e 7469 616c 2066 756e  .  essential fun
-00000930: 6374 696f 6e61 6c69 7469 6573 2061 7420  ctionalities at 
-00000940: 7468 6520 6469 7370 6f73 616c 206f 6620  the disposal of 
-00000950: 616e 7920 6f74 6865 7220 6e61 7475 7261  any other natura
-00000960: 6c20 6f72 206c 6567 616c 0a20 2070 6572  l or legal.  per
-00000970: 736f 6e2e 0a0a 322e 2053 636f 7065 206f  son...2. Scope o
-00000980: 6620 7468 6520 7269 6768 7473 2067 7261  f the rights gra
-00000990: 6e74 6564 2062 7920 7468 6520 4c69 6365  nted by the Lice
-000009a0: 6e63 650a 0a54 6865 204c 6963 656e 736f  nce..The Licenso
-000009b0: 7220 6865 7265 6279 2067 7261 6e74 7320  r hereby grants 
-000009c0: 596f 7520 6120 776f 726c 6477 6964 652c  You a worldwide,
-000009d0: 2072 6f79 616c 7479 2d66 7265 652c 206e   royalty-free, n
-000009e0: 6f6e 2d65 7863 6c75 7369 7665 2c0a 7375  on-exclusive,.su
-000009f0: 626c 6963 656e 7361 626c 6520 6c69 6365  blicensable lice
-00000a00: 6e63 6520 746f 2064 6f20 7468 6520 666f  nce to do the fo
-00000a10: 6c6c 6f77 696e 672c 2066 6f72 2074 6865  llowing, for the
-00000a20: 2064 7572 6174 696f 6e20 6f66 2063 6f70   duration of cop
-00000a30: 7972 6967 6874 0a76 6573 7465 6420 696e  yright.vested in
-00000a40: 2074 6865 204f 7269 6769 6e61 6c20 576f   the Original Wo
-00000a50: 726b 3a0a 0a2d 2075 7365 2074 6865 2057  rk:..- use the W
-00000a60: 6f72 6b20 696e 2061 6e79 2063 6972 6375  ork in any circu
-00000a70: 6d73 7461 6e63 6520 616e 6420 666f 7220  mstance and for 
-00000a80: 616c 6c20 7573 6167 652c 0a2d 2072 6570  all usage,.- rep
-00000a90: 726f 6475 6365 2074 6865 2057 6f72 6b2c  roduce the Work,
-00000aa0: 0a2d 206d 6f64 6966 7920 7468 6520 576f  .- modify the Wo
-00000ab0: 726b 2c20 616e 6420 6d61 6b65 2044 6572  rk, and make Der
-00000ac0: 6976 6174 6976 6520 576f 726b 7320 6261  ivative Works ba
-00000ad0: 7365 6420 7570 6f6e 2074 6865 2057 6f72  sed upon the Wor
-00000ae0: 6b2c 0a2d 2063 6f6d 6d75 6e69 6361 7465  k,.- communicate
-00000af0: 2074 6f20 7468 6520 7075 626c 6963 2c20   to the public, 
-00000b00: 696e 636c 7564 696e 6720 7468 6520 7269  including the ri
-00000b10: 6768 7420 746f 206d 616b 6520 6176 6169  ght to make avai
-00000b20: 6c61 626c 6520 6f72 2064 6973 706c 6179  lable or display
-00000b30: 0a20 2074 6865 2057 6f72 6b20 6f72 2063  .  the Work or c
-00000b40: 6f70 6965 7320 7468 6572 656f 6620 746f  opies thereof to
-00000b50: 2074 6865 2070 7562 6c69 6320 616e 6420   the public and 
-00000b60: 7065 7266 6f72 6d20 7075 626c 6963 6c79  perform publicly
-00000b70: 2c20 6173 2074 6865 2063 6173 650a 2020  , as the case.  
-00000b80: 6d61 7920 6265 2c20 7468 6520 576f 726b  may be, the Work
-00000b90: 2c0a 2d20 6469 7374 7269 6275 7465 2074  ,.- distribute t
-00000ba0: 6865 2057 6f72 6b20 6f72 2063 6f70 6965  he Work or copie
-00000bb0: 7320 7468 6572 656f 662c 0a2d 206c 656e  s thereof,.- len
-00000bc0: 6420 616e 6420 7265 6e74 2074 6865 2057  d and rent the W
-00000bd0: 6f72 6b20 6f72 2063 6f70 6965 7320 7468  ork or copies th
-00000be0: 6572 656f 662c 0a2d 2073 7562 6c69 6365  ereof,.- sublice
-00000bf0: 6e73 6520 7269 6768 7473 2069 6e20 7468  nse rights in th
-00000c00: 6520 576f 726b 206f 7220 636f 7069 6573  e Work or copies
-00000c10: 2074 6865 7265 6f66 2e0a 0a54 686f 7365   thereof...Those
-00000c20: 2072 6967 6874 7320 6361 6e20 6265 2065   rights can be e
-00000c30: 7865 7263 6973 6564 206f 6e20 616e 7920  xercised on any 
-00000c40: 6d65 6469 612c 2073 7570 706f 7274 7320  media, supports 
-00000c50: 616e 6420 666f 726d 6174 732c 2077 6865  and formats, whe
-00000c60: 7468 6572 206e 6f77 0a6b 6e6f 776e 206f  ther now.known o
-00000c70: 7220 6c61 7465 7220 696e 7665 6e74 6564  r later invented
-00000c80: 2c20 6173 2066 6172 2061 7320 7468 6520  , as far as the 
-00000c90: 6170 706c 6963 6162 6c65 206c 6177 2070  applicable law p
-00000ca0: 6572 6d69 7473 2073 6f2e 0a0a 496e 2074  ermits so...In t
-00000cb0: 6865 2063 6f75 6e74 7269 6573 2077 6865  he countries whe
-00000cc0: 7265 206d 6f72 616c 2072 6967 6874 7320  re moral rights 
-00000cd0: 6170 706c 792c 2074 6865 204c 6963 656e  apply, the Licen
-00000ce0: 736f 7220 7761 6976 6573 2068 6973 2072  sor waives his r
-00000cf0: 6967 6874 2074 6f0a 6578 6572 6369 7365  ight to.exercise
-00000d00: 2068 6973 206d 6f72 616c 2072 6967 6874   his moral right
-00000d10: 2074 6f20 7468 6520 6578 7465 6e74 2061   to the extent a
-00000d20: 6c6c 6f77 6564 2062 7920 6c61 7720 696e  llowed by law in
-00000d30: 206f 7264 6572 2074 6f20 6d61 6b65 0a65   order to make.e
-00000d40: 6666 6563 7469 7665 2074 6865 206c 6963  ffective the lic
-00000d50: 656e 6365 206f 6620 7468 6520 6563 6f6e  ence of the econ
-00000d60: 6f6d 6963 2072 6967 6874 7320 6865 7265  omic rights here
-00000d70: 2061 626f 7665 206c 6973 7465 642e 0a0a   above listed...
-00000d80: 5468 6520 4c69 6365 6e73 6f72 2067 7261  The Licensor gra
-00000d90: 6e74 7320 746f 2074 6865 204c 6963 656e  nts to the Licen
-00000da0: 7365 6520 726f 7961 6c74 792d 6672 6565  see royalty-free
-00000db0: 2c20 6e6f 6e2d 6578 636c 7573 6976 6520  , non-exclusive 
-00000dc0: 7573 6167 6520 7269 6768 7473 0a74 6f20  usage rights.to 
-00000dd0: 616e 7920 7061 7465 6e74 7320 6865 6c64  any patents held
-00000de0: 2062 7920 7468 6520 4c69 6365 6e73 6f72   by the Licensor
-00000df0: 2c20 746f 2074 6865 2065 7874 656e 7420  , to the extent 
-00000e00: 6e65 6365 7373 6172 7920 746f 206d 616b  necessary to mak
-00000e10: 6520 7573 6520 6f66 0a74 6865 2072 6967  e use of.the rig
-00000e20: 6874 7320 6772 616e 7465 6420 6f6e 2074  hts granted on t
-00000e30: 6865 2057 6f72 6b20 756e 6465 7220 7468  he Work under th
-00000e40: 6973 204c 6963 656e 6365 2e0a 0a33 2e20  is Licence...3. 
-00000e50: 436f 6d6d 756e 6963 6174 696f 6e20 6f66  Communication of
-00000e60: 2074 6865 2053 6f75 7263 6520 436f 6465   the Source Code
-00000e70: 0a0a 5468 6520 4c69 6365 6e73 6f72 206d  ..The Licensor m
-00000e80: 6179 2070 726f 7669 6465 2074 6865 2057  ay provide the W
-00000e90: 6f72 6b20 6569 7468 6572 2069 6e20 6974  ork either in it
-00000ea0: 7320 536f 7572 6365 2043 6f64 6520 666f  s Source Code fo
-00000eb0: 726d 2c20 6f72 2061 730a 4578 6563 7574  rm, or as.Execut
-00000ec0: 6162 6c65 2043 6f64 652e 2049 6620 7468  able Code. If th
-00000ed0: 6520 576f 726b 2069 7320 7072 6f76 6964  e Work is provid
-00000ee0: 6564 2061 7320 4578 6563 7574 6162 6c65  ed as Executable
-00000ef0: 2043 6f64 652c 2074 6865 204c 6963 656e   Code, the Licen
-00000f00: 736f 720a 7072 6f76 6964 6573 2069 6e20  sor.provides in 
-00000f10: 6164 6469 7469 6f6e 2061 206d 6163 6869  addition a machi
-00000f20: 6e65 2d72 6561 6461 626c 6520 636f 7079  ne-readable copy
-00000f30: 206f 6620 7468 6520 536f 7572 6365 2043   of the Source C
-00000f40: 6f64 6520 6f66 2074 6865 2057 6f72 6b0a  ode of the Work.
-00000f50: 616c 6f6e 6720 7769 7468 2065 6163 6820  along with each 
-00000f60: 636f 7079 206f 6620 7468 6520 576f 726b  copy of the Work
-00000f70: 2074 6861 7420 7468 6520 4c69 6365 6e73   that the Licens
-00000f80: 6f72 2064 6973 7472 6962 7574 6573 206f  or distributes o
-00000f90: 7220 696e 6469 6361 7465 732c 0a69 6e20  r indicates,.in 
-00000fa0: 6120 6e6f 7469 6365 2066 6f6c 6c6f 7769  a notice followi
-00000fb0: 6e67 2074 6865 2063 6f70 7972 6967 6874  ng the copyright
-00000fc0: 206e 6f74 6963 6520 6174 7461 6368 6564   notice attached
-00000fd0: 2074 6f20 7468 6520 576f 726b 2c20 6120   to the Work, a 
-00000fe0: 7265 706f 7369 746f 7279 0a77 6865 7265  repository.where
-00000ff0: 2074 6865 2053 6f75 7263 6520 436f 6465   the Source Code
-00001000: 2069 7320 6561 7369 6c79 2061 6e64 2066   is easily and f
-00001010: 7265 656c 7920 6163 6365 7373 6962 6c65  reely accessible
-00001020: 2066 6f72 2061 7320 6c6f 6e67 2061 7320   for as long as 
-00001030: 7468 650a 4c69 6365 6e73 6f72 2063 6f6e  the.Licensor con
-00001040: 7469 6e75 6573 2074 6f20 6469 7374 7269  tinues to distri
-00001050: 6275 7465 206f 7220 636f 6d6d 756e 6963  bute or communic
-00001060: 6174 6520 7468 6520 576f 726b 2e0a 0a34  ate the Work...4
-00001070: 2e20 4c69 6d69 7461 7469 6f6e 7320 6f6e  . Limitations on
-00001080: 2063 6f70 7972 6967 6874 0a0a 4e6f 7468   copyright..Noth
-00001090: 696e 6720 696e 2074 6869 7320 4c69 6365  ing in this Lice
-000010a0: 6e63 6520 6973 2069 6e74 656e 6465 6420  nce is intended 
-000010b0: 746f 2064 6570 7269 7665 2074 6865 204c  to deprive the L
-000010c0: 6963 656e 7365 6520 6f66 2074 6865 2062  icensee of the b
-000010d0: 656e 6566 6974 730a 6672 6f6d 2061 6e79  enefits.from any
-000010e0: 2065 7863 6570 7469 6f6e 206f 7220 6c69   exception or li
-000010f0: 6d69 7461 7469 6f6e 2074 6f20 7468 6520  mitation to the 
-00001100: 6578 636c 7573 6976 6520 7269 6768 7473  exclusive rights
-00001110: 206f 6620 7468 6520 7269 6768 7473 206f   of the rights o
-00001120: 776e 6572 730a 696e 2074 6865 2057 6f72  wners.in the Wor
-00001130: 6b2c 206f 6620 7468 6520 6578 6861 7573  k, of the exhaus
-00001140: 7469 6f6e 206f 6620 7468 6f73 6520 7269  tion of those ri
-00001150: 6768 7473 206f 7220 6f66 206f 7468 6572  ghts or of other
-00001160: 2061 7070 6c69 6361 626c 650a 6c69 6d69   applicable.limi
-00001170: 7461 7469 6f6e 7320 7468 6572 6574 6f2e  tations thereto.
-00001180: 0a0a 352e 204f 626c 6967 6174 696f 6e73  ..5. Obligations
-00001190: 206f 6620 7468 6520 4c69 6365 6e73 6565   of the Licensee
-000011a0: 0a0a 5468 6520 6772 616e 7420 6f66 2074  ..The grant of t
-000011b0: 6865 2072 6967 6874 7320 6d65 6e74 696f  he rights mentio
-000011c0: 6e65 6420 6162 6f76 6520 6973 2073 7562  ned above is sub
-000011d0: 6a65 6374 2074 6f20 736f 6d65 2072 6573  ject to some res
-000011e0: 7472 6963 7469 6f6e 7320 616e 640a 6f62  trictions and.ob
-000011f0: 6c69 6761 7469 6f6e 7320 696d 706f 7365  ligations impose
-00001200: 6420 6f6e 2074 6865 204c 6963 656e 7365  d on the License
-00001210: 652e 2054 686f 7365 206f 626c 6967 6174  e. Those obligat
-00001220: 696f 6e73 2061 7265 2074 6865 2066 6f6c  ions are the fol
-00001230: 6c6f 7769 6e67 3a0a 0a41 7474 7269 6275  lowing:..Attribu
-00001240: 7469 6f6e 2072 6967 6874 3a20 5468 6520  tion right: The 
-00001250: 4c69 6365 6e73 6565 2073 6861 6c6c 206b  Licensee shall k
-00001260: 6565 7020 696e 7461 6374 2061 6c6c 2063  eep intact all c
-00001270: 6f70 7972 6967 6874 2c20 7061 7465 6e74  opyright, patent
-00001280: 206f 720a 7472 6164 656d 6172 6b73 206e   or.trademarks n
-00001290: 6f74 6963 6573 2061 6e64 2061 6c6c 206e  otices and all n
-000012a0: 6f74 6963 6573 2074 6861 7420 7265 6665  otices that refe
-000012b0: 7220 746f 2074 6865 204c 6963 656e 6365  r to the Licence
-000012c0: 2061 6e64 2074 6f20 7468 650a 6469 7363   and to the.disc
-000012d0: 6c61 696d 6572 206f 6620 7761 7272 616e  laimer of warran
-000012e0: 7469 6573 2e20 5468 6520 4c69 6365 6e73  ties. The Licens
-000012f0: 6565 206d 7573 7420 696e 636c 7564 6520  ee must include 
-00001300: 6120 636f 7079 206f 6620 7375 6368 206e  a copy of such n
-00001310: 6f74 6963 6573 2061 6e64 0a61 2063 6f70  otices and.a cop
-00001320: 7920 6f66 2074 6865 204c 6963 656e 6365  y of the Licence
-00001330: 2077 6974 6820 6576 6572 7920 636f 7079   with every copy
-00001340: 206f 6620 7468 6520 576f 726b 2068 652f   of the Work he/
-00001350: 7368 6520 6469 7374 7269 6275 7465 7320  she distributes 
-00001360: 6f72 0a63 6f6d 6d75 6e69 6361 7465 732e  or.communicates.
-00001370: 2054 6865 204c 6963 656e 7365 6520 6d75   The Licensee mu
-00001380: 7374 2063 6175 7365 2061 6e79 2044 6572  st cause any Der
-00001390: 6976 6174 6976 6520 576f 726b 2074 6f20  ivative Work to 
-000013a0: 6361 7272 7920 7072 6f6d 696e 656e 740a  carry prominent.
-000013b0: 6e6f 7469 6365 7320 7374 6174 696e 6720  notices stating 
-000013c0: 7468 6174 2074 6865 2057 6f72 6b20 6861  that the Work ha
-000013d0: 7320 6265 656e 206d 6f64 6966 6965 6420  s been modified 
-000013e0: 616e 6420 7468 6520 6461 7465 206f 6620  and the date of 
-000013f0: 6d6f 6469 6669 6361 7469 6f6e 2e0a 0a43  modification...C
-00001400: 6f70 796c 6566 7420 636c 6175 7365 3a20  opyleft clause: 
-00001410: 4966 2074 6865 204c 6963 656e 7365 6520  If the Licensee 
-00001420: 6469 7374 7269 6275 7465 7320 6f72 2063  distributes or c
-00001430: 6f6d 6d75 6e69 6361 7465 7320 636f 7069  ommunicates copi
-00001440: 6573 206f 6620 7468 650a 4f72 6967 696e  es of the.Origin
-00001450: 616c 2057 6f72 6b73 206f 7220 4465 7269  al Works or Deri
-00001460: 7661 7469 7665 2057 6f72 6b73 2c20 7468  vative Works, th
-00001470: 6973 2044 6973 7472 6962 7574 696f 6e20  is Distribution 
-00001480: 6f72 2043 6f6d 6d75 6e69 6361 7469 6f6e  or Communication
-00001490: 2077 696c 6c20 6265 0a64 6f6e 6520 756e   will be.done un
-000014a0: 6465 7220 7468 6520 7465 726d 7320 6f66  der the terms of
-000014b0: 2074 6869 7320 4c69 6365 6e63 6520 6f72   this Licence or
-000014c0: 206f 6620 6120 6c61 7465 7220 7665 7273   of a later vers
-000014d0: 696f 6e20 6f66 2074 6869 7320 4c69 6365  ion of this Lice
-000014e0: 6e63 650a 756e 6c65 7373 2074 6865 204f  nce.unless the O
-000014f0: 7269 6769 6e61 6c20 576f 726b 2069 7320  riginal Work is 
-00001500: 6578 7072 6573 736c 7920 6469 7374 7269  expressly distri
-00001510: 6275 7465 6420 6f6e 6c79 2075 6e64 6572  buted only under
-00001520: 2074 6869 7320 7665 7273 696f 6e20 6f66   this version of
-00001530: 0a74 6865 204c 6963 656e 6365 2097 2066  .the Licence . f
-00001540: 6f72 2065 7861 6d70 6c65 2062 7920 636f  or example by co
-00001550: 6d6d 756e 6963 6174 696e 6720 9145 5550  mmunicating .EUP
-00001560: 4c20 762e 2031 2e32 206f 6e6c 7992 2e20  L v. 1.2 only.. 
-00001570: 5468 6520 4c69 6365 6e73 6565 0a28 6265  The Licensee.(be
-00001580: 636f 6d69 6e67 204c 6963 656e 736f 7229  coming Licensor)
-00001590: 2063 616e 6e6f 7420 6f66 6665 7220 6f72   cannot offer or
-000015a0: 2069 6d70 6f73 6520 616e 7920 6164 6469   impose any addi
-000015b0: 7469 6f6e 616c 2074 6572 6d73 206f 7220  tional terms or 
-000015c0: 636f 6e64 6974 696f 6e73 0a6f 6e20 7468  conditions.on th
-000015d0: 6520 576f 726b 206f 7220 4465 7269 7661  e Work or Deriva
-000015e0: 7469 7665 2057 6f72 6b20 7468 6174 2061  tive Work that a
-000015f0: 6c74 6572 206f 7220 7265 7374 7269 6374  lter or restrict
-00001600: 2074 6865 2074 6572 6d73 206f 6620 7468   the terms of th
-00001610: 650a 4c69 6365 6e63 652e 0a0a 436f 6d70  e.Licence...Comp
-00001620: 6174 6962 696c 6974 7920 636c 6175 7365  atibility clause
-00001630: 3a20 4966 2074 6865 204c 6963 656e 7365  : If the License
-00001640: 6520 4469 7374 7269 6275 7465 7320 6f72  e Distributes or
-00001650: 2043 6f6d 6d75 6e69 6361 7465 7320 4465   Communicates De
-00001660: 7269 7661 7469 7665 0a57 6f72 6b73 206f  rivative.Works o
-00001670: 7220 636f 7069 6573 2074 6865 7265 6f66  r copies thereof
-00001680: 2062 6173 6564 2075 706f 6e20 626f 7468   based upon both
-00001690: 2074 6865 2057 6f72 6b20 616e 6420 616e   the Work and an
-000016a0: 6f74 6865 7220 776f 726b 206c 6963 656e  other work licen
-000016b0: 7365 640a 756e 6465 7220 6120 436f 6d70  sed.under a Comp
-000016c0: 6174 6962 6c65 204c 6963 656e 6365 2c20  atible Licence, 
-000016d0: 7468 6973 2044 6973 7472 6962 7574 696f  this Distributio
-000016e0: 6e20 6f72 2043 6f6d 6d75 6e69 6361 7469  n or Communicati
-000016f0: 6f6e 2063 616e 2062 6520 646f 6e65 0a75  on can be done.u
-00001700: 6e64 6572 2074 6865 2074 6572 6d73 206f  nder the terms o
-00001710: 6620 7468 6973 2043 6f6d 7061 7469 626c  f this Compatibl
-00001720: 6520 4c69 6365 6e63 652e 2046 6f72 2074  e Licence. For t
-00001730: 6865 2073 616b 6520 6f66 2074 6869 7320  he sake of this 
-00001740: 636c 6175 7365 2c0a 9143 6f6d 7061 7469  clause,..Compati
-00001750: 626c 6520 4c69 6365 6e63 6592 2072 6566  ble Licence. ref
-00001760: 6572 7320 746f 2074 6865 206c 6963 656e  ers to the licen
-00001770: 6365 7320 6c69 7374 6564 2069 6e20 7468  ces listed in th
-00001780: 6520 6170 7065 6e64 6978 2061 7474 6163  e appendix attac
-00001790: 6865 6420 746f 0a74 6869 7320 4c69 6365  hed to.this Lice
-000017a0: 6e63 652e 2053 686f 756c 6420 7468 6520  nce. Should the 
-000017b0: 4c69 6365 6e73 6565 2773 206f 626c 6967  Licensee's oblig
-000017c0: 6174 696f 6e73 2075 6e64 6572 2074 6865  ations under the
-000017d0: 2043 6f6d 7061 7469 626c 6520 4c69 6365   Compatible Lice
-000017e0: 6e63 650a 636f 6e66 6c69 6374 2077 6974  nce.conflict wit
-000017f0: 6820 6869 732f 6865 7220 6f62 6c69 6761  h his/her obliga
-00001800: 7469 6f6e 7320 756e 6465 7220 7468 6973  tions under this
-00001810: 204c 6963 656e 6365 2c20 7468 6520 6f62   Licence, the ob
-00001820: 6c69 6761 7469 6f6e 7320 6f66 2074 6865  ligations of the
-00001830: 0a43 6f6d 7061 7469 626c 6520 4c69 6365  .Compatible Lice
-00001840: 6e63 6520 7368 616c 6c20 7072 6576 6169  nce shall prevai
-00001850: 6c2e 0a0a 5072 6f76 6973 696f 6e20 6f66  l...Provision of
-00001860: 2053 6f75 7263 6520 436f 6465 3a20 5768   Source Code: Wh
-00001870: 656e 2064 6973 7472 6962 7574 696e 6720  en distributing 
-00001880: 6f72 2063 6f6d 6d75 6e69 6361 7469 6e67  or communicating
-00001890: 2063 6f70 6965 7320 6f66 2074 6865 0a57   copies of the.W
-000018a0: 6f72 6b2c 2074 6865 204c 6963 656e 7365  ork, the License
-000018b0: 6520 7769 6c6c 2070 726f 7669 6465 2061  e will provide a
-000018c0: 206d 6163 6869 6e65 2d72 6561 6461 626c   machine-readabl
-000018d0: 6520 636f 7079 206f 6620 7468 6520 536f  e copy of the So
-000018e0: 7572 6365 2043 6f64 6520 6f72 0a69 6e64  urce Code or.ind
-000018f0: 6963 6174 6520 6120 7265 706f 7369 746f  icate a reposito
-00001900: 7279 2077 6865 7265 2074 6869 7320 536f  ry where this So
-00001910: 7572 6365 2077 696c 6c20 6265 2065 6173  urce will be eas
-00001920: 696c 7920 616e 6420 6672 6565 6c79 2061  ily and freely a
-00001930: 7661 696c 6162 6c65 0a66 6f72 2061 7320  vailable.for as 
-00001940: 6c6f 6e67 2061 7320 7468 6520 4c69 6365  long as the Lice
-00001950: 6e73 6565 2063 6f6e 7469 6e75 6573 2074  nsee continues t
-00001960: 6f20 6469 7374 7269 6275 7465 206f 7220  o distribute or 
-00001970: 636f 6d6d 756e 6963 6174 6520 7468 6520  communicate the 
-00001980: 576f 726b 2e0a 0a4c 6567 616c 2050 726f  Work...Legal Pro
-00001990: 7465 6374 696f 6e3a 2054 6869 7320 4c69  tection: This Li
-000019a0: 6365 6e63 6520 646f 6573 206e 6f74 2067  cence does not g
-000019b0: 7261 6e74 2070 6572 6d69 7373 696f 6e20  rant permission 
-000019c0: 746f 2075 7365 2074 6865 2074 7261 6465  to use the trade
-000019d0: 0a6e 616d 6573 2c20 7472 6164 656d 6172  .names, trademar
-000019e0: 6b73 2c20 7365 7276 6963 6520 6d61 726b  ks, service mark
-000019f0: 732c 206f 7220 6e61 6d65 7320 6f66 2074  s, or names of t
-00001a00: 6865 204c 6963 656e 736f 722c 2065 7863  he Licensor, exc
-00001a10: 6570 7420 6173 2072 6571 7569 7265 640a  ept as required.
-00001a20: 666f 7220 7265 6173 6f6e 6162 6c65 2061  for reasonable a
-00001a30: 6e64 2063 7573 746f 6d61 7279 2075 7365  nd customary use
-00001a40: 2069 6e20 6465 7363 7269 6269 6e67 2074   in describing t
-00001a50: 6865 206f 7269 6769 6e20 6f66 2074 6865  he origin of the
-00001a60: 2057 6f72 6b20 616e 640a 7265 7072 6f64   Work and.reprod
-00001a70: 7563 696e 6720 7468 6520 636f 6e74 656e  ucing the conten
-00001a80: 7420 6f66 2074 6865 2063 6f70 7972 6967  t of the copyrig
-00001a90: 6874 206e 6f74 6963 652e 0a0a 362e 2043  ht notice...6. C
-00001aa0: 6861 696e 206f 6620 4175 7468 6f72 7368  hain of Authorsh
-00001ab0: 6970 0a0a 5468 6520 6f72 6967 696e 616c  ip..The original
-00001ac0: 204c 6963 656e 736f 7220 7761 7272 616e   Licensor warran
-00001ad0: 7473 2074 6861 7420 7468 6520 636f 7079  ts that the copy
-00001ae0: 7269 6768 7420 696e 2074 6865 204f 7269  right in the Ori
-00001af0: 6769 6e61 6c20 576f 726b 2067 7261 6e74  ginal Work grant
-00001b00: 6564 0a68 6572 6575 6e64 6572 2069 7320  ed.hereunder is 
-00001b10: 6f77 6e65 6420 6279 2068 696d 2f68 6572  owned by him/her
-00001b20: 206f 7220 6c69 6365 6e73 6564 2074 6f20   or licensed to 
-00001b30: 6869 6d2f 6865 7220 616e 6420 7468 6174  him/her and that
-00001b40: 2068 652f 7368 6520 6861 7320 7468 650a   he/she has the.
-00001b50: 706f 7765 7220 616e 6420 6175 7468 6f72  power and author
-00001b60: 6974 7920 746f 2067 7261 6e74 2074 6865  ity to grant the
-00001b70: 204c 6963 656e 6365 2e0a 0a45 6163 6820   Licence...Each 
-00001b80: 436f 6e74 7269 6275 746f 7220 7761 7272  Contributor warr
-00001b90: 616e 7473 2074 6861 7420 7468 6520 636f  ants that the co
-00001ba0: 7079 7269 6768 7420 696e 2074 6865 206d  pyright in the m
-00001bb0: 6f64 6966 6963 6174 696f 6e73 2068 652f  odifications he/
-00001bc0: 7368 650a 6272 696e 6773 2074 6f20 7468  she.brings to th
-00001bd0: 6520 576f 726b 2061 7265 206f 776e 6564  e Work are owned
-00001be0: 2062 7920 6869 6d2f 6865 7220 6f72 206c   by him/her or l
-00001bf0: 6963 656e 7365 6420 746f 2068 696d 2f68  icensed to him/h
-00001c00: 6572 2061 6e64 2074 6861 7420 6865 2f73  er and that he/s
-00001c10: 6865 0a68 6173 2074 6865 2070 6f77 6572  he.has the power
-00001c20: 2061 6e64 2061 7574 686f 7269 7479 2074   and authority t
-00001c30: 6f20 6772 616e 7420 7468 6520 4c69 6365  o grant the Lice
-00001c40: 6e63 652e 0a0a 4561 6368 2074 696d 6520  nce...Each time 
-00001c50: 596f 7520 6163 6365 7074 2074 6865 204c  You accept the L
-00001c60: 6963 656e 6365 2c20 7468 6520 6f72 6967  icence, the orig
-00001c70: 696e 616c 204c 6963 656e 736f 7220 616e  inal Licensor an
-00001c80: 6420 7375 6273 6571 7565 6e74 0a43 6f6e  d subsequent.Con
-00001c90: 7472 6962 7574 6f72 7320 6772 616e 7420  tributors grant 
-00001ca0: 596f 7520 6120 6c69 6365 6e63 6520 746f  You a licence to
-00001cb0: 2074 6865 6972 2063 6f6e 7472 6962 7574   their contribut
-00001cc0: 696f 6e73 2074 6f20 7468 6520 576f 726b  ions to the Work
-00001cd0: 2c20 756e 6465 7220 7468 650a 7465 726d  , under the.term
-00001ce0: 7320 6f66 2074 6869 7320 4c69 6365 6e63  s of this Licenc
-00001cf0: 652e 0a0a 372e 2044 6973 636c 6169 6d65  e...7. Disclaime
-00001d00: 7220 6f66 2057 6172 7261 6e74 790a 0a54  r of Warranty..T
-00001d10: 6865 2057 6f72 6b20 6973 2061 2077 6f72  he Work is a wor
-00001d20: 6b20 696e 2070 726f 6772 6573 732c 2077  k in progress, w
-00001d30: 6869 6368 2069 7320 636f 6e74 696e 756f  hich is continuo
-00001d40: 7573 6c79 2069 6d70 726f 7665 6420 6279  usly improved by
-00001d50: 206e 756d 6572 6f75 730a 436f 6e74 7269   numerous.Contri
-00001d60: 6275 746f 7273 2e20 4974 2069 7320 6e6f  butors. It is no
-00001d70: 7420 6120 6669 6e69 7368 6564 2077 6f72  t a finished wor
-00001d80: 6b20 616e 6420 6d61 7920 7468 6572 6566  k and may theref
-00001d90: 6f72 6520 636f 6e74 6169 6e20 6465 6665  ore contain defe
-00001da0: 6374 7320 6f72 0a91 6275 6773 9220 696e  cts or..bugs. in
-00001db0: 6865 7265 6e74 2074 6f20 7468 6973 2074  herent to this t
-00001dc0: 7970 6520 6f66 2064 6576 656c 6f70 6d65  ype of developme
-00001dd0: 6e74 2e0a 0a46 6f72 2074 6865 2061 626f  nt...For the abo
-00001de0: 7665 2072 6561 736f 6e2c 2074 6865 2057  ve reason, the W
-00001df0: 6f72 6b20 6973 2070 726f 7669 6465 6420  ork is provided 
-00001e00: 756e 6465 7220 7468 6520 4c69 6365 6e63  under the Licenc
-00001e10: 6520 6f6e 2061 6e20 9161 7320 6973 920a  e on an .as is..
-00001e20: 6261 7369 7320 616e 6420 7769 7468 6f75  basis and withou
-00001e30: 7420 7761 7272 616e 7469 6573 206f 6620  t warranties of 
-00001e40: 616e 7920 6b69 6e64 2063 6f6e 6365 726e  any kind concern
-00001e50: 696e 6720 7468 6520 576f 726b 2c20 696e  ing the Work, in
-00001e60: 636c 7564 696e 670a 7769 7468 6f75 7420  cluding.without 
-00001e70: 6c69 6d69 7461 7469 6f6e 206d 6572 6368  limitation merch
-00001e80: 616e 7461 6269 6c69 7479 2c20 6669 746e  antability, fitn
-00001e90: 6573 7320 666f 7220 6120 7061 7274 6963  ess for a partic
-00001ea0: 756c 6172 2070 7572 706f 7365 2c20 6162  ular purpose, ab
-00001eb0: 7365 6e63 650a 6f66 2064 6566 6563 7473  sence.of defects
-00001ec0: 206f 7220 6572 726f 7273 2c20 6163 6375   or errors, accu
-00001ed0: 7261 6379 2c20 6e6f 6e2d 696e 6672 696e  racy, non-infrin
-00001ee0: 6765 6d65 6e74 206f 6620 696e 7465 6c6c  gement of intell
-00001ef0: 6563 7475 616c 2070 726f 7065 7274 790a  ectual property.
-00001f00: 7269 6768 7473 206f 7468 6572 2074 6861  rights other tha
-00001f10: 6e20 636f 7079 7269 6768 7420 6173 2073  n copyright as s
-00001f20: 7461 7465 6420 696e 2041 7274 6963 6c65  tated in Article
-00001f30: 2036 206f 6620 7468 6973 204c 6963 656e   6 of this Licen
-00001f40: 6365 2e0a 0a54 6869 7320 6469 7363 6c61  ce...This discla
-00001f50: 696d 6572 206f 6620 7761 7272 616e 7479  imer of warranty
-00001f60: 2069 7320 616e 2065 7373 656e 7469 616c   is an essential
-00001f70: 2070 6172 7420 6f66 2074 6865 204c 6963   part of the Lic
-00001f80: 656e 6365 2061 6e64 2061 0a63 6f6e 6469  ence and a.condi
-00001f90: 7469 6f6e 2066 6f72 2074 6865 2067 7261  tion for the gra
-00001fa0: 6e74 206f 6620 616e 7920 7269 6768 7473  nt of any rights
-00001fb0: 2074 6f20 7468 6520 576f 726b 2e0a 0a38   to the Work...8
-00001fc0: 2e20 4469 7363 6c61 696d 6572 206f 6620  . Disclaimer of 
-00001fd0: 4c69 6162 696c 6974 790a 0a45 7863 6570  Liability..Excep
-00001fe0: 7420 696e 2074 6865 2063 6173 6573 206f  t in the cases o
-00001ff0: 6620 7769 6c66 756c 206d 6973 636f 6e64  f wilful miscond
-00002000: 7563 7420 6f72 2064 616d 6167 6573 2064  uct or damages d
-00002010: 6972 6563 746c 7920 6361 7573 6564 2074  irectly caused t
-00002020: 6f20 6e61 7475 7261 6c0a 7065 7273 6f6e  o natural.person
-00002030: 732c 2074 6865 204c 6963 656e 736f 7220  s, the Licensor 
-00002040: 7769 6c6c 2069 6e20 6e6f 2065 7665 6e74  will in no event
-00002050: 2062 6520 6c69 6162 6c65 2066 6f72 2061   be liable for a
-00002060: 6e79 2064 6972 6563 7420 6f72 2069 6e64  ny direct or ind
-00002070: 6972 6563 742c 0a6d 6174 6572 6961 6c20  irect,.material 
-00002080: 6f72 206d 6f72 616c 2c20 6461 6d61 6765  or moral, damage
-00002090: 7320 6f66 2061 6e79 206b 696e 642c 2061  s of any kind, a
-000020a0: 7269 7369 6e67 206f 7574 206f 6620 7468  rising out of th
-000020b0: 6520 4c69 6365 6e63 6520 6f72 206f 6620  e Licence or of 
-000020c0: 7468 650a 7573 6520 6f66 2074 6865 2057  the.use of the W
-000020d0: 6f72 6b2c 2069 6e63 6c75 6469 6e67 2077  ork, including w
-000020e0: 6974 686f 7574 206c 696d 6974 6174 696f  ithout limitatio
-000020f0: 6e2c 2064 616d 6167 6573 2066 6f72 206c  n, damages for l
-00002100: 6f73 7320 6f66 2067 6f6f 6477 696c 6c2c  oss of goodwill,
-00002110: 0a77 6f72 6b20 7374 6f70 7061 6765 2c20  .work stoppage, 
-00002120: 636f 6d70 7574 6572 2066 6169 6c75 7265  computer failure
-00002130: 206f 7220 6d61 6c66 756e 6374 696f 6e2c   or malfunction,
-00002140: 206c 6f73 7320 6f66 2064 6174 6120 6f72   loss of data or
-00002150: 2061 6e79 2063 6f6d 6d65 7263 6961 6c0a   any commercial.
-00002160: 6461 6d61 6765 2c20 6576 656e 2069 6620  damage, even if 
-00002170: 7468 6520 4c69 6365 6e73 6f72 2068 6173  the Licensor has
-00002180: 2062 6565 6e20 6164 7669 7365 6420 6f66   been advised of
-00002190: 2074 6865 2070 6f73 7369 6269 6c69 7479   the possibility
-000021a0: 206f 6620 7375 6368 0a64 616d 6167 652e   of such.damage.
-000021b0: 2048 6f77 6576 6572 2c20 7468 6520 4c69   However, the Li
-000021c0: 6365 6e73 6f72 2077 696c 6c20 6265 206c  censor will be l
-000021d0: 6961 626c 6520 756e 6465 7220 7374 6174  iable under stat
-000021e0: 7574 6f72 7920 7072 6f64 7563 7420 6c69  utory product li
-000021f0: 6162 696c 6974 790a 6c61 7773 2061 7320  ability.laws as 
-00002200: 6661 7220 7375 6368 206c 6177 7320 6170  far such laws ap
-00002210: 706c 7920 746f 2074 6865 2057 6f72 6b2e  ply to the Work.
-00002220: 0a0a 392e 2041 6464 6974 696f 6e61 6c20  ..9. Additional 
-00002230: 6167 7265 656d 656e 7473 0a0a 5768 696c  agreements..Whil
-00002240: 6520 6469 7374 7269 6275 7469 6e67 2074  e distributing t
-00002250: 6865 2057 6f72 6b2c 2059 6f75 206d 6179  he Work, You may
-00002260: 2063 686f 6f73 6520 746f 2063 6f6e 636c   choose to concl
-00002270: 7564 6520 616e 2061 6464 6974 696f 6e61  ude an additiona
-00002280: 6c0a 6167 7265 656d 656e 742c 2064 6566  l.agreement, def
-00002290: 696e 696e 6720 6f62 6c69 6761 7469 6f6e  ining obligation
-000022a0: 7320 6f72 2073 6572 7669 6365 7320 636f  s or services co
-000022b0: 6e73 6973 7465 6e74 2077 6974 6820 7468  nsistent with th
-000022c0: 6973 204c 6963 656e 6365 2e0a 486f 7765  is Licence..Howe
-000022d0: 7665 722c 2069 6620 6163 6365 7074 696e  ver, if acceptin
-000022e0: 6720 6f62 6c69 6761 7469 6f6e 732c 2059  g obligations, Y
-000022f0: 6f75 206d 6179 2061 6374 206f 6e6c 7920  ou may act only 
-00002300: 6f6e 2079 6f75 7220 6f77 6e20 6265 6861  on your own beha
-00002310: 6c66 2061 6e64 206f 6e0a 796f 7572 2073  lf and on.your s
-00002320: 6f6c 6520 7265 7370 6f6e 7369 6269 6c69  ole responsibili
-00002330: 7479 2c20 6e6f 7420 6f6e 2062 6568 616c  ty, not on behal
-00002340: 6620 6f66 2074 6865 206f 7269 6769 6e61  f of the origina
-00002350: 6c20 4c69 6365 6e73 6f72 206f 7220 616e  l Licensor or an
-00002360: 7920 6f74 6865 720a 436f 6e74 7269 6275  y other.Contribu
-00002370: 746f 722c 2061 6e64 206f 6e6c 7920 6966  tor, and only if
-00002380: 2059 6f75 2061 6772 6565 2074 6f20 696e   You agree to in
-00002390: 6465 6d6e 6966 792c 2064 6566 656e 642c  demnify, defend,
-000023a0: 2061 6e64 2068 6f6c 6420 6561 6368 0a43   and hold each.C
-000023b0: 6f6e 7472 6962 7574 6f72 2068 6172 6d6c  ontributor harml
-000023c0: 6573 7320 666f 7220 616e 7920 6c69 6162  ess for any liab
-000023d0: 696c 6974 7920 696e 6375 7272 6564 2062  ility incurred b
-000023e0: 792c 206f 7220 636c 6169 6d73 2061 7373  y, or claims ass
-000023f0: 6572 7465 6420 6167 6169 6e73 740a 7375  erted against.su
-00002400: 6368 2043 6f6e 7472 6962 7574 6f72 2062  ch Contributor b
-00002410: 7920 7468 6520 6661 6374 2059 6f75 2068  y the fact You h
-00002420: 6176 6520 6163 6365 7074 6564 2061 6e79  ave accepted any
-00002430: 2077 6172 7261 6e74 7920 6f72 2061 6464   warranty or add
-00002440: 6974 696f 6e61 6c0a 6c69 6162 696c 6974  itional.liabilit
-00002450: 792e 0a0a 3130 2e20 4163 6365 7074 616e  y...10. Acceptan
-00002460: 6365 206f 6620 7468 6520 4c69 6365 6e63  ce of the Licenc
-00002470: 650a 0a54 6865 2070 726f 7669 7369 6f6e  e..The provision
-00002480: 7320 6f66 2074 6869 7320 4c69 6365 6e63  s of this Licenc
-00002490: 6520 6361 6e20 6265 2061 6363 6570 7465  e can be accepte
-000024a0: 6420 6279 2063 6c69 636b 696e 6720 6f6e  d by clicking on
-000024b0: 2061 6e20 6963 6f6e 2091 490a 6167 7265   an icon .I.agre
-000024c0: 6592 2070 6c61 6365 6420 756e 6465 7220  e. placed under 
-000024d0: 7468 6520 626f 7474 6f6d 206f 6620 6120  the bottom of a 
-000024e0: 7769 6e64 6f77 2064 6973 706c 6179 696e  window displayin
-000024f0: 6720 7468 6520 7465 7874 206f 6620 7468  g the text of th
-00002500: 6973 204c 6963 656e 6365 0a6f 7220 6279  is Licence.or by
-00002510: 2061 6666 6972 6d69 6e67 2063 6f6e 7365   affirming conse
-00002520: 6e74 2069 6e20 616e 7920 6f74 6865 7220  nt in any other 
-00002530: 7369 6d69 6c61 7220 7761 792c 2069 6e20  similar way, in 
-00002540: 6163 636f 7264 616e 6365 2077 6974 6820  accordance with 
-00002550: 7468 6520 7275 6c65 730a 6f66 2061 7070  the rules.of app
-00002560: 6c69 6361 626c 6520 6c61 772e 2043 6c69  licable law. Cli
-00002570: 636b 696e 6720 6f6e 2074 6861 7420 6963  cking on that ic
-00002580: 6f6e 2069 6e64 6963 6174 6573 2079 6f75  on indicates you
-00002590: 7220 636c 6561 7220 616e 6420 6972 7265  r clear and irre
-000025a0: 766f 6361 626c 650a 6163 6365 7074 616e  vocable.acceptan
-000025b0: 6365 206f 6620 7468 6973 204c 6963 656e  ce of this Licen
-000025c0: 6365 2061 6e64 2061 6c6c 206f 6620 6974  ce and all of it
-000025d0: 7320 7465 726d 7320 616e 6420 636f 6e64  s terms and cond
-000025e0: 6974 696f 6e73 2e0a 0a53 696d 696c 6172  itions...Similar
-000025f0: 6c79 2c20 796f 7520 6972 7265 766f 6361  ly, you irrevoca
-00002600: 626c 7920 6163 6365 7074 2074 6869 7320  bly accept this 
-00002610: 4c69 6365 6e63 6520 616e 6420 616c 6c20  Licence and all 
-00002620: 6f66 2069 7473 2074 6572 6d73 2061 6e64  of its terms and
-00002630: 0a63 6f6e 6469 7469 6f6e 7320 6279 2065  .conditions by e
-00002640: 7865 7263 6973 696e 6720 616e 7920 7269  xercising any ri
-00002650: 6768 7473 2067 7261 6e74 6564 2074 6f20  ghts granted to 
-00002660: 596f 7520 6279 2041 7274 6963 6c65 2032  You by Article 2
-00002670: 206f 6620 7468 6973 0a4c 6963 656e 6365   of this.Licence
-00002680: 2c20 7375 6368 2061 7320 7468 6520 7573  , such as the us
-00002690: 6520 6f66 2074 6865 2057 6f72 6b2c 2074  e of the Work, t
-000026a0: 6865 2063 7265 6174 696f 6e20 6279 2059  he creation by Y
-000026b0: 6f75 206f 6620 6120 4465 7269 7661 7469  ou of a Derivati
-000026c0: 7665 2057 6f72 6b0a 6f72 2074 6865 2044  ve Work.or the D
-000026d0: 6973 7472 6962 7574 696f 6e20 6f72 2043  istribution or C
-000026e0: 6f6d 6d75 6e69 6361 7469 6f6e 2062 7920  ommunication by 
-000026f0: 596f 7520 6f66 2074 6865 2057 6f72 6b20  You of the Work 
-00002700: 6f72 2063 6f70 6965 7320 7468 6572 656f  or copies thereo
-00002710: 662e 0a0a 3131 2e20 496e 666f 726d 6174  f...11. Informat
-00002720: 696f 6e20 746f 2074 6865 2070 7562 6c69  ion to the publi
-00002730: 630a 0a49 6e20 6361 7365 206f 6620 616e  c..In case of an
-00002740: 7920 4469 7374 7269 6275 7469 6f6e 206f  y Distribution o
-00002750: 7220 436f 6d6d 756e 6963 6174 696f 6e20  r Communication 
-00002760: 6f66 2074 6865 2057 6f72 6b20 6279 206d  of the Work by m
-00002770: 6561 6e73 206f 660a 656c 6563 7472 6f6e  eans of.electron
-00002780: 6963 2063 6f6d 6d75 6e69 6361 7469 6f6e  ic communication
-00002790: 2062 7920 596f 7520 2866 6f72 2065 7861   by You (for exa
-000027a0: 6d70 6c65 2c20 6279 206f 6666 6572 696e  mple, by offerin
-000027b0: 6720 746f 2064 6f77 6e6c 6f61 6420 7468  g to download th
-000027c0: 6520 576f 726b 0a66 726f 6d20 6120 7265  e Work.from a re
-000027d0: 6d6f 7465 206c 6f63 6174 696f 6e29 2074  mote location) t
-000027e0: 6865 2064 6973 7472 6962 7574 696f 6e20  he distribution 
-000027f0: 6368 616e 6e65 6c20 6f72 206d 6564 6961  channel or media
-00002800: 2028 666f 7220 6578 616d 706c 652c 2061   (for example, a
-00002810: 0a77 6562 7369 7465 2920 6d75 7374 2061  .website) must a
-00002820: 7420 6c65 6173 7420 7072 6f76 6964 6520  t least provide 
-00002830: 746f 2074 6865 2070 7562 6c69 6320 7468  to the public th
-00002840: 6520 696e 666f 726d 6174 696f 6e20 7265  e information re
-00002850: 7175 6573 7465 6420 6279 2074 6865 0a61  quested by the.a
-00002860: 7070 6c69 6361 626c 6520 6c61 7720 7265  pplicable law re
-00002870: 6761 7264 696e 6720 7468 6520 4c69 6365  garding the Lice
-00002880: 6e73 6f72 2c20 7468 6520 4c69 6365 6e63  nsor, the Licenc
-00002890: 6520 616e 6420 7468 6520 7761 7920 6974  e and the way it
-000028a0: 206d 6179 2062 650a 6163 6365 7373 6962   may be.accessib
-000028b0: 6c65 2c20 636f 6e63 6c75 6465 642c 2073  le, concluded, s
-000028c0: 746f 7265 6420 616e 6420 7265 7072 6f64  tored and reprod
-000028d0: 7563 6564 2062 7920 7468 6520 4c69 6365  uced by the Lice
-000028e0: 6e73 6565 2e0a 0a31 322e 2054 6572 6d69  nsee...12. Termi
-000028f0: 6e61 7469 6f6e 206f 6620 7468 6520 4c69  nation of the Li
-00002900: 6365 6e63 650a 0a54 6865 204c 6963 656e  cence..The Licen
-00002910: 6365 2061 6e64 2074 6865 2072 6967 6874  ce and the right
-00002920: 7320 6772 616e 7465 6420 6865 7265 756e  s granted hereun
-00002930: 6465 7220 7769 6c6c 2074 6572 6d69 6e61  der will termina
-00002940: 7465 2061 7574 6f6d 6174 6963 616c 6c79  te automatically
-00002950: 2075 706f 6e0a 616e 7920 6272 6561 6368   upon.any breach
-00002960: 2062 7920 7468 6520 4c69 6365 6e73 6565   by the Licensee
-00002970: 206f 6620 7468 6520 7465 726d 7320 6f66   of the terms of
-00002980: 2074 6865 204c 6963 656e 6365 2e0a 0a53   the Licence...S
-00002990: 7563 6820 6120 7465 726d 696e 6174 696f  uch a terminatio
-000029a0: 6e20 7769 6c6c 206e 6f74 2074 6572 6d69  n will not termi
-000029b0: 6e61 7465 2074 6865 206c 6963 656e 6365  nate the licence
-000029c0: 7320 6f66 2061 6e79 2070 6572 736f 6e20  s of any person 
-000029d0: 7768 6f20 6861 730a 7265 6365 6976 6564  who has.received
-000029e0: 2074 6865 2057 6f72 6b20 6672 6f6d 2074   the Work from t
-000029f0: 6865 204c 6963 656e 7365 6520 756e 6465  he Licensee unde
-00002a00: 7220 7468 6520 4c69 6365 6e63 652c 2070  r the Licence, p
-00002a10: 726f 7669 6465 6420 7375 6368 2070 6572  rovided such per
-00002a20: 736f 6e73 0a72 656d 6169 6e20 696e 2066  sons.remain in f
-00002a30: 756c 6c20 636f 6d70 6c69 616e 6365 2077  ull compliance w
-00002a40: 6974 6820 7468 6520 4c69 6365 6e63 652e  ith the Licence.
-00002a50: 0a0a 3133 2e20 4d69 7363 656c 6c61 6e65  ..13. Miscellane
-00002a60: 6f75 730a 0a57 6974 686f 7574 2070 7265  ous..Without pre
-00002a70: 6a75 6469 6365 206f 6620 4172 7469 636c  judice of Articl
-00002a80: 6520 3920 6162 6f76 652c 2074 6865 204c  e 9 above, the L
-00002a90: 6963 656e 6365 2072 6570 7265 7365 6e74  icence represent
-00002aa0: 7320 7468 6520 636f 6d70 6c65 7465 0a61  s the complete.a
-00002ab0: 6772 6565 6d65 6e74 2062 6574 7765 656e  greement between
-00002ac0: 2074 6865 2050 6172 7469 6573 2061 7320   the Parties as 
-00002ad0: 746f 2074 6865 2057 6f72 6b2e 0a0a 4966  to the Work...If
-00002ae0: 2061 6e79 2070 726f 7669 7369 6f6e 206f   any provision o
-00002af0: 6620 7468 6520 4c69 6365 6e63 6520 6973  f the Licence is
-00002b00: 2069 6e76 616c 6964 206f 7220 756e 656e   invalid or unen
-00002b10: 666f 7263 6561 626c 6520 756e 6465 7220  forceable under 
-00002b20: 6170 706c 6963 6162 6c65 0a6c 6177 2c20  applicable.law, 
-00002b30: 7468 6973 2077 696c 6c20 6e6f 7420 6166  this will not af
-00002b40: 6665 6374 2074 6865 2076 616c 6964 6974  fect the validit
-00002b50: 7920 6f72 2065 6e66 6f72 6365 6162 696c  y or enforceabil
-00002b60: 6974 7920 6f66 2074 6865 204c 6963 656e  ity of the Licen
-00002b70: 6365 2061 7320 610a 7768 6f6c 652e 2053  ce as a.whole. S
-00002b80: 7563 6820 7072 6f76 6973 696f 6e20 7769  uch provision wi
-00002b90: 6c6c 2062 6520 636f 6e73 7472 7565 6420  ll be construed 
-00002ba0: 6f72 2072 6566 6f72 6d65 6420 736f 2061  or reformed so a
-00002bb0: 7320 6e65 6365 7373 6172 7920 746f 206d  s necessary to m
-00002bc0: 616b 6520 6974 0a76 616c 6964 2061 6e64  ake it.valid and
-00002bd0: 2065 6e66 6f72 6365 6162 6c65 2e0a 0a54   enforceable...T
-00002be0: 6865 2045 7572 6f70 6561 6e20 436f 6d6d  he European Comm
-00002bf0: 6973 7369 6f6e 206d 6179 2070 7562 6c69  ission may publi
-00002c00: 7368 206f 7468 6572 206c 696e 6775 6973  sh other linguis
-00002c10: 7469 6320 7665 7273 696f 6e73 206f 7220  tic versions or 
-00002c20: 6e65 7720 7665 7273 696f 6e73 0a6f 6620  new versions.of 
-00002c30: 7468 6973 204c 6963 656e 6365 206f 7220  this Licence or 
-00002c40: 7570 6461 7465 6420 7665 7273 696f 6e73  updated versions
-00002c50: 206f 6620 7468 6520 4170 7065 6e64 6978   of the Appendix
-00002c60: 2c20 736f 2066 6172 2074 6869 7320 6973  , so far this is
-00002c70: 2072 6571 7569 7265 640a 616e 6420 7265   required.and re
-00002c80: 6173 6f6e 6162 6c65 2c20 7769 7468 6f75  asonable, withou
-00002c90: 7420 7265 6475 6369 6e67 2074 6865 2073  t reducing the s
-00002ca0: 636f 7065 206f 6620 7468 6520 7269 6768  cope of the righ
-00002cb0: 7473 2067 7261 6e74 6564 2062 7920 7468  ts granted by th
-00002cc0: 650a 4c69 6365 6e63 652e 204e 6577 2076  e.Licence. New v
-00002cd0: 6572 7369 6f6e 7320 6f66 2074 6865 204c  ersions of the L
-00002ce0: 6963 656e 6365 2077 696c 6c20 6265 2070  icence will be p
-00002cf0: 7562 6c69 7368 6564 2077 6974 6820 6120  ublished with a 
-00002d00: 756e 6971 7565 2076 6572 7369 6f6e 0a6e  unique version.n
-00002d10: 756d 6265 722e 0a0a 416c 6c20 6c69 6e67  umber...All ling
-00002d20: 7569 7374 6963 2076 6572 7369 6f6e 7320  uistic versions 
-00002d30: 6f66 2074 6869 7320 4c69 6365 6e63 652c  of this Licence,
-00002d40: 2061 7070 726f 7665 6420 6279 2074 6865   approved by the
-00002d50: 2045 7572 6f70 6561 6e20 436f 6d6d 6973   European Commis
-00002d60: 7369 6f6e 2c0a 6861 7665 2069 6465 6e74  sion,.have ident
-00002d70: 6963 616c 2076 616c 7565 2e20 5061 7274  ical value. Part
-00002d80: 6965 7320 6361 6e20 7461 6b65 2061 6476  ies can take adv
-00002d90: 616e 7461 6765 206f 6620 7468 6520 6c69  antage of the li
-00002da0: 6e67 7569 7374 6963 2076 6572 7369 6f6e  nguistic version
-00002db0: 206f 660a 7468 6569 7220 6368 6f69 6365   of.their choice
-00002dc0: 2e0a 0a31 342e 204a 7572 6973 6469 6374  ...14. Jurisdict
-00002dd0: 696f 6e0a 0a57 6974 686f 7574 2070 7265  ion..Without pre
-00002de0: 6a75 6469 6365 2074 6f20 7370 6563 6966  judice to specif
-00002df0: 6963 2061 6772 6565 6d65 6e74 2062 6574  ic agreement bet
-00002e00: 7765 656e 2070 6172 7469 6573 2c0a 0a2d  ween parties,..-
-00002e10: 2061 6e79 206c 6974 6967 6174 696f 6e20   any litigation 
-00002e20: 7265 7375 6c74 696e 6720 6672 6f6d 2074  resulting from t
-00002e30: 6865 2069 6e74 6572 7072 6574 6174 696f  he interpretatio
-00002e40: 6e20 6f66 2074 6869 7320 4c69 6365 6e73  n of this Licens
-00002e50: 652c 2061 7269 7369 6e67 0a20 2062 6574  e, arising.  bet
-00002e60: 7765 656e 2074 6865 2045 7572 6f70 6561  ween the Europea
-00002e70: 6e20 556e 696f 6e20 696e 7374 6974 7574  n Union institut
-00002e80: 696f 6e73 2c20 626f 6469 6573 2c20 6f66  ions, bodies, of
-00002e90: 6669 6365 7320 6f72 2061 6765 6e63 6965  fices or agencie
-00002ea0: 732c 2061 7320 610a 2020 4c69 6365 6e73  s, as a.  Licens
-00002eb0: 6f72 2c20 616e 6420 616e 7920 4c69 6365  or, and any Lice
-00002ec0: 6e73 6565 2c20 7769 6c6c 2062 6520 7375  nsee, will be su
-00002ed0: 626a 6563 7420 746f 2074 6865 206a 7572  bject to the jur
-00002ee0: 6973 6469 6374 696f 6e20 6f66 2074 6865  isdiction of the
-00002ef0: 2043 6f75 7274 0a20 206f 6620 4a75 7374   Court.  of Just
-00002f00: 6963 6520 6f66 2074 6865 2045 7572 6f70  ice of the Europ
-00002f10: 6561 6e20 556e 696f 6e2c 2061 7320 6c61  ean Union, as la
-00002f20: 6964 2064 6f77 6e20 696e 2061 7274 6963  id down in artic
-00002f30: 6c65 2032 3732 206f 6620 7468 6520 5472  le 272 of the Tr
-00002f40: 6561 7479 0a20 206f 6e20 7468 6520 4675  eaty.  on the Fu
-00002f50: 6e63 7469 6f6e 696e 6720 6f66 2074 6865  nctioning of the
-00002f60: 2045 7572 6f70 6561 6e20 556e 696f 6e2c   European Union,
-00002f70: 0a0a 2d20 616e 7920 6c69 7469 6761 7469  ..- any litigati
-00002f80: 6f6e 2061 7269 7369 6e67 2062 6574 7765  on arising betwe
-00002f90: 656e 206f 7468 6572 2070 6172 7469 6573  en other parties
-00002fa0: 2061 6e64 2072 6573 756c 7469 6e67 2066   and resulting f
-00002fb0: 726f 6d20 7468 650a 2020 696e 7465 7270  rom the.  interp
-00002fc0: 7265 7461 7469 6f6e 206f 6620 7468 6973  retation of this
-00002fd0: 204c 6963 656e 7365 2c20 7769 6c6c 2062   License, will b
-00002fe0: 6520 7375 626a 6563 7420 746f 2074 6865  e subject to the
-00002ff0: 2065 7863 6c75 7369 7665 0a20 206a 7572   exclusive.  jur
-00003000: 6973 6469 6374 696f 6e20 6f66 2074 6865  isdiction of the
-00003010: 2063 6f6d 7065 7465 6e74 2063 6f75 7274   competent court
-00003020: 2077 6865 7265 2074 6865 204c 6963 656e   where the Licen
-00003030: 736f 7220 7265 7369 6465 7320 6f72 2063  sor resides or c
-00003040: 6f6e 6475 6374 730a 2020 6974 7320 7072  onducts.  its pr
-00003050: 696d 6172 7920 6275 7369 6e65 7373 2e0a  imary business..
-00003060: 0a31 352e 2041 7070 6c69 6361 626c 6520  .15. Applicable 
-00003070: 4c61 770a 0a57 6974 686f 7574 2070 7265  Law..Without pre
-00003080: 6a75 6469 6365 2074 6f20 7370 6563 6966  judice to specif
-00003090: 6963 2061 6772 6565 6d65 6e74 2062 6574  ic agreement bet
-000030a0: 7765 656e 2070 6172 7469 6573 2c0a 0a2d  ween parties,..-
-000030b0: 2074 6869 7320 4c69 6365 6e63 6520 7368   this Licence sh
-000030c0: 616c 6c20 6265 2067 6f76 6572 6e65 6420  all be governed 
-000030d0: 6279 2074 6865 206c 6177 206f 6620 7468  by the law of th
-000030e0: 6520 4575 726f 7065 616e 2055 6e69 6f6e  e European Union
-000030f0: 204d 656d 6265 7220 5374 6174 650a 2020   Member State.  
-00003100: 7768 6572 6520 7468 6520 4c69 6365 6e73  where the Licens
-00003110: 6f72 2068 6173 2068 6973 2073 6561 742c  or has his seat,
-00003120: 2072 6573 6964 6573 206f 7220 6861 7320   resides or has 
-00003130: 6869 7320 7265 6769 7374 6572 6564 206f  his registered o
-00003140: 6666 6963 652c 0a0a 2d20 7468 6973 206c  ffice,..- this l
-00003150: 6963 656e 6365 2073 6861 6c6c 2062 6520  icence shall be 
-00003160: 676f 7665 726e 6564 2062 7920 4265 6c67  governed by Belg
-00003170: 6961 6e20 6c61 7720 6966 2074 6865 204c  ian law if the L
-00003180: 6963 656e 736f 7220 6861 7320 6e6f 2073  icensor has no s
-00003190: 6561 742c 0a20 2072 6573 6964 656e 6365  eat,.  residence
-000031a0: 206f 7220 7265 6769 7374 6572 6564 206f   or registered o
-000031b0: 6666 6963 6520 696e 7369 6465 2061 2045  ffice inside a E
-000031c0: 7572 6f70 6561 6e20 556e 696f 6e20 4d65  uropean Union Me
-000031d0: 6d62 6572 2053 7461 7465 2e0a 0a41 7070  mber State...App
-000031e0: 656e 6469 780a 0a91 436f 6d70 6174 6962  endix...Compatib
-000031f0: 6c65 204c 6963 656e 6365 7392 2061 6363  le Licences. acc
-00003200: 6f72 6469 6e67 2074 6f20 4172 7469 636c  ording to Articl
-00003210: 6520 3520 4555 504c 2061 7265 3a0a 0a2d  e 5 EUPL are:..-
-00003220: 2047 4e55 2047 656e 6572 616c 2050 7562   GNU General Pub
-00003230: 6c69 6320 4c69 6365 6e73 6520 2847 504c  lic License (GPL
-00003240: 2920 762e 2032 2c20 762e 2033 0a2d 2047  ) v. 2, v. 3.- G
-00003250: 4e55 2041 6666 6572 6f20 4765 6e65 7261  NU Affero Genera
-00003260: 6c20 5075 626c 6963 204c 6963 656e 7365  l Public License
-00003270: 2028 4147 504c 2920 762e 2033 0a2d 204f   (AGPL) v. 3.- O
-00003280: 7065 6e20 536f 6674 7761 7265 204c 6963  pen Software Lic
-00003290: 656e 7365 2028 4f53 4c29 2076 2e20 322e  ense (OSL) v. 2.
-000032a0: 312c 2076 2e20 332e 300a 2d20 4563 6c69  1, v. 3.0.- Ecli
-000032b0: 7073 6520 5075 626c 6963 204c 6963 656e  pse Public Licen
-000032c0: 7365 2028 4550 4c29 2076 2e20 312e 300a  se (EPL) v. 1.0.
-000032d0: 2d20 4365 4349 4c4c 2076 2e20 322e 302c  - CeCILL v. 2.0,
-000032e0: 2076 2e20 322e 310a 2d20 4d6f 7a69 6c6c   v. 2.1.- Mozill
-000032f0: 6120 5075 626c 6963 204c 6963 656e 6365  a Public Licence
-00003300: 2028 4d50 4c29 2076 2e20 320a 2d20 474e   (MPL) v. 2.- GN
-00003310: 5520 4c65 7373 6572 2047 656e 6572 616c  U Lesser General
-00003320: 2050 7562 6c69 6320 4c69 6365 6e63 6520   Public Licence 
-00003330: 284c 4750 4c29 2076 2e20 322e 312c 2076  (LGPL) v. 2.1, v
-00003340: 2e20 330a 2d20 4372 6561 7469 7665 2043  . 3.- Creative C
-00003350: 6f6d 6d6f 6e73 2041 7474 7269 6275 7469  ommons Attributi
-00003360: 6f6e 2d53 6861 7265 416c 696b 6520 762e  on-ShareAlike v.
-00003370: 2033 2e30 2055 6e70 6f72 7465 6420 2843   3.0 Unported (C
-00003380: 4320 4259 2d53 4120 332e 3029 2066 6f72  C BY-SA 3.0) for
-00003390: 0a20 2077 6f72 6b73 206f 7468 6572 2074  .  works other t
-000033a0: 6861 6e20 736f 6674 7761 7265 0a2d 2045  han software.- E
-000033b0: 7572 6f70 6561 6e20 556e 696f 6e20 5075  uropean Union Pu
-000033c0: 626c 6963 204c 6963 656e 6365 2028 4555  blic Licence (EU
-000033d0: 504c 2920 762e 2031 2e31 2c20 762e 2031  PL) v. 1.1, v. 1
-000033e0: 2e32 0a2d 2051 75e9 6265 6320 4672 6565  .2.- Qu.bec Free
-000033f0: 2061 6e64 204f 7065 6e2d 536f 7572 6365   and Open-Source
-00003400: 204c 6963 656e 6365 2097 2052 6563 6970   Licence . Recip
-00003410: 726f 6369 7479 2028 4c69 4c69 512d 5229  rocity (LiLiQ-R)
-00003420: 206f 7220 5374 726f 6e67 0a20 2052 6563   or Strong.  Rec
-00003430: 6970 726f 6369 7479 2028 4c69 4c69 512d  iprocity (LiLiQ-
-00003440: 522b 292e 0a0a 5468 6520 4575 726f 7065  R+)...The Europe
-00003450: 616e 2043 6f6d 6d69 7373 696f 6e20 6d61  an Commission ma
-00003460: 7920 7570 6461 7465 2074 6869 7320 4170  y update this Ap
-00003470: 7065 6e64 6978 2074 6f20 6c61 7465 7220  pendix to later 
-00003480: 7665 7273 696f 6e73 206f 6620 7468 650a  versions of the.
-00003490: 6162 6f76 6520 6c69 6365 6e63 6573 2077  above licences w
-000034a0: 6974 686f 7574 2070 726f 6475 6369 6e67  ithout producing
-000034b0: 2061 206e 6577 2076 6572 7369 6f6e 206f   a new version o
-000034c0: 6620 7468 6520 4555 504c 2c20 6173 206c  f the EUPL, as l
-000034d0: 6f6e 6720 6173 2074 6865 790a 7072 6f76  ong as they.prov
-000034e0: 6964 6520 7468 6520 7269 6768 7473 2067  ide the rights g
-000034f0: 7261 6e74 6564 2069 6e20 4172 7469 636c  ranted in Articl
-00003500: 6520 3220 6f66 2074 6869 7320 4c69 6365  e 2 of this Lice
-00003510: 6e63 6520 616e 6420 7072 6f74 6563 7420  nce and protect 
-00003520: 7468 650a 636f 7665 7265 6420 536f 7572  the.covered Sour
-00003530: 6365 2043 6f64 6520 6672 6f6d 2065 7863  ce Code from exc
-00003540: 6c75 7369 7665 2061 7070 726f 7072 6961  lusive appropria
-00003550: 7469 6f6e 2e0a 0a41 6c6c 206f 7468 6572  tion...All other
-00003560: 2063 6861 6e67 6573 206f 7220 6164 6469   changes or addi
-00003570: 7469 6f6e 7320 746f 2074 6869 7320 4170  tions to this Ap
-00003580: 7065 6e64 6978 2072 6571 7569 7265 2074  pendix require t
-00003590: 6865 2070 726f 6475 6374 696f 6e20 6f66  he production of
-000035a0: 2061 0a6e 6577 2045 5550 4c20 7665 7273   a.new EUPL vers
-000035b0: 696f 6e2e 0a                             ion..
+00000050: 2020 2045 5550 4c20 c2a9 2074 6865 2045     EUPL .. the E
+00000060: 7572 6f70 6561 6e20 556e 696f 6e20 3230  uropean Union 20
+00000070: 3037 2c20 3230 3136 0a0a 5468 6973 2045  07, 2016..This E
+00000080: 7572 6f70 6561 6e20 556e 696f 6e20 5075  uropean Union Pu
+00000090: 626c 6963 204c 6963 656e 6365 2028 7468  blic Licence (th
+000000a0: 6520 e280 9845 5550 4ce2 8099 2920 6170  e ...EUPL...) ap
+000000b0: 706c 6965 7320 746f 2074 6865 2057 6f72  plies to the Wor
+000000c0: 6b20 2861 730a 6465 6669 6e65 6420 6265  k (as.defined be
+000000d0: 6c6f 7729 2077 6869 6368 2069 7320 7072  low) which is pr
+000000e0: 6f76 6964 6564 2075 6e64 6572 2074 6865  ovided under the
+000000f0: 2074 6572 6d73 206f 6620 7468 6973 204c   terms of this L
+00000100: 6963 656e 6365 2e20 416e 7920 7573 6520  icence. Any use 
+00000110: 6f66 0a74 6865 2057 6f72 6b2c 206f 7468  of.the Work, oth
+00000120: 6572 2074 6861 6e20 6173 2061 7574 686f  er than as autho
+00000130: 7269 7365 6420 756e 6465 7220 7468 6973  rised under this
+00000140: 204c 6963 656e 6365 2069 7320 7072 6f68   Licence is proh
+00000150: 6962 6974 6564 2028 746f 2074 6865 0a65  ibited (to the.e
+00000160: 7874 656e 7420 7375 6368 2075 7365 2069  xtent such use i
+00000170: 7320 636f 7665 7265 6420 6279 2061 2072  s covered by a r
+00000180: 6967 6874 206f 6620 7468 6520 636f 7079  ight of the copy
+00000190: 7269 6768 7420 686f 6c64 6572 206f 6620  right holder of 
+000001a0: 7468 6520 576f 726b 292e 0a0a 5468 6520  the Work)...The 
+000001b0: 576f 726b 2069 7320 7072 6f76 6964 6564  Work is provided
+000001c0: 2075 6e64 6572 2074 6865 2074 6572 6d73   under the terms
+000001d0: 206f 6620 7468 6973 204c 6963 656e 6365   of this Licence
+000001e0: 2077 6865 6e20 7468 6520 4c69 6365 6e73   when the Licens
+000001f0: 6f72 2028 6173 0a64 6566 696e 6564 2062  or (as.defined b
+00000200: 656c 6f77 2920 6861 7320 706c 6163 6564  elow) has placed
+00000210: 2074 6865 2066 6f6c 6c6f 7769 6e67 206e   the following n
+00000220: 6f74 6963 6520 696d 6d65 6469 6174 656c  otice immediatel
+00000230: 7920 666f 6c6c 6f77 696e 6720 7468 650a  y following the.
+00000240: 636f 7079 7269 6768 7420 6e6f 7469 6365  copyright notice
+00000250: 2066 6f72 2074 6865 2057 6f72 6b3a 0a0a   for the Work:..
+00000260: 2020 2020 2020 2020 4c69 6365 6e73 6564          Licensed
+00000270: 2075 6e64 6572 2074 6865 2045 5550 4c0a   under the EUPL.
+00000280: 0a6f 7220 6861 7320 6578 7072 6573 7365  .or has expresse
+00000290: 6420 6279 2061 6e79 206f 7468 6572 206d  d by any other m
+000002a0: 6561 6e73 2068 6973 2077 696c 6c69 6e67  eans his willing
+000002b0: 6e65 7373 2074 6f20 6c69 6365 6e73 6520  ness to license 
+000002c0: 756e 6465 7220 7468 6520 4555 504c 2e0a  under the EUPL..
+000002d0: 0a31 2e20 4465 6669 6e69 7469 6f6e 730a  .1. Definitions.
+000002e0: 0a49 6e20 7468 6973 204c 6963 656e 6365  .In this Licence
+000002f0: 2c20 7468 6520 666f 6c6c 6f77 696e 6720  , the following 
+00000300: 7465 726d 7320 6861 7665 2074 6865 2066  terms have the f
+00000310: 6f6c 6c6f 7769 6e67 206d 6561 6e69 6e67  ollowing meaning
+00000320: 3a0a 0a2d 20e2 8098 5468 6520 4c69 6365  :..- ...The Lice
+00000330: 6e63 65e2 8099 3a20 7468 6973 204c 6963  nce...: this Lic
+00000340: 656e 6365 2e0a 0a2d 20e2 8098 5468 6520  ence...- ...The 
+00000350: 4f72 6967 696e 616c 2057 6f72 6be2 8099  Original Work...
+00000360: 3a20 7468 6520 776f 726b 206f 7220 736f  : the work or so
+00000370: 6674 7761 7265 2064 6973 7472 6962 7574  ftware distribut
+00000380: 6564 206f 7220 636f 6d6d 756e 6963 6174  ed or communicat
+00000390: 6564 2062 7920 7468 650a 2020 4c69 6365  ed by the.  Lice
+000003a0: 6e73 6f72 2075 6e64 6572 2074 6869 7320  nsor under this 
+000003b0: 4c69 6365 6e63 652c 2061 7661 696c 6162  Licence, availab
+000003c0: 6c65 2061 7320 536f 7572 6365 2043 6f64  le as Source Cod
+000003d0: 6520 616e 6420 616c 736f 2061 7320 4578  e and also as Ex
+000003e0: 6563 7574 6162 6c65 0a20 2043 6f64 6520  ecutable.  Code 
+000003f0: 6173 2074 6865 2063 6173 6520 6d61 7920  as the case may 
+00000400: 6265 2e0a 0a2d 20e2 8098 4465 7269 7661  be...- ...Deriva
+00000410: 7469 7665 2057 6f72 6b73 e280 993a 2074  tive Works...: t
+00000420: 6865 2077 6f72 6b73 206f 7220 736f 6674  he works or soft
+00000430: 7761 7265 2074 6861 7420 636f 756c 6420  ware that could 
+00000440: 6265 2063 7265 6174 6564 2062 7920 7468  be created by th
+00000450: 650a 2020 4c69 6365 6e73 6565 2c20 6261  e.  Licensee, ba
+00000460: 7365 6420 7570 6f6e 2074 6865 204f 7269  sed upon the Ori
+00000470: 6769 6e61 6c20 576f 726b 206f 7220 6d6f  ginal Work or mo
+00000480: 6469 6669 6361 7469 6f6e 7320 7468 6572  difications ther
+00000490: 656f 662e 2054 6869 730a 2020 4c69 6365  eof. This.  Lice
+000004a0: 6e63 6520 646f 6573 206e 6f74 2064 6566  nce does not def
+000004b0: 696e 6520 7468 6520 6578 7465 6e74 206f  ine the extent o
+000004c0: 6620 6d6f 6469 6669 6361 7469 6f6e 206f  f modification o
+000004d0: 7220 6465 7065 6e64 656e 6365 206f 6e20  r dependence on 
+000004e0: 7468 650a 2020 4f72 6967 696e 616c 2057  the.  Original W
+000004f0: 6f72 6b20 7265 7175 6972 6564 2069 6e20  ork required in 
+00000500: 6f72 6465 7220 746f 2063 6c61 7373 6966  order to classif
+00000510: 7920 6120 776f 726b 2061 7320 6120 4465  y a work as a De
+00000520: 7269 7661 7469 7665 2057 6f72 6b3b 0a20  rivative Work;. 
+00000530: 2074 6869 7320 6578 7465 6e74 2069 7320   this extent is 
+00000540: 6465 7465 726d 696e 6564 2062 7920 636f  determined by co
+00000550: 7079 7269 6768 7420 6c61 7720 6170 706c  pyright law appl
+00000560: 6963 6162 6c65 2069 6e20 7468 6520 636f  icable in the co
+00000570: 756e 7472 790a 2020 6d65 6e74 696f 6e65  untry.  mentione
+00000580: 6420 696e 2041 7274 6963 6c65 2031 352e  d in Article 15.
+00000590: 0a0a 2d20 e280 9854 6865 2057 6f72 6be2  ..- ...The Work.
+000005a0: 8099 3a20 7468 6520 4f72 6967 696e 616c  ..: the Original
+000005b0: 2057 6f72 6b20 6f72 2069 7473 2044 6572   Work or its Der
+000005c0: 6976 6174 6976 6520 576f 726b 732e 0a0a  ivative Works...
+000005d0: 2d20 e280 9854 6865 2053 6f75 7263 6520  - ...The Source 
+000005e0: 436f 6465 e280 993a 2074 6865 2068 756d  Code...: the hum
+000005f0: 616e 2d72 6561 6461 626c 6520 666f 726d  an-readable form
+00000600: 206f 6620 7468 6520 576f 726b 2077 6869   of the Work whi
+00000610: 6368 2069 7320 7468 6520 6d6f 7374 0a20  ch is the most. 
+00000620: 2063 6f6e 7665 6e69 656e 7420 666f 7220   convenient for 
+00000630: 7065 6f70 6c65 2074 6f20 7374 7564 7920  people to study 
+00000640: 616e 6420 6d6f 6469 6679 2e0a 0a2d 20e2  and modify...- .
+00000650: 8098 5468 6520 4578 6563 7574 6162 6c65  ..The Executable
+00000660: 2043 6f64 65e2 8099 3a20 616e 7920 636f   Code...: any co
+00000670: 6465 2077 6869 6368 2068 6173 2067 656e  de which has gen
+00000680: 6572 616c 6c79 2062 6565 6e20 636f 6d70  erally been comp
+00000690: 696c 6564 2061 6e64 2077 6869 6368 0a20  iled and which. 
+000006a0: 2069 7320 6d65 616e 7420 746f 2062 6520   is meant to be 
+000006b0: 696e 7465 7270 7265 7465 6420 6279 2061  interpreted by a
+000006c0: 2063 6f6d 7075 7465 7220 6173 2061 2070   computer as a p
+000006d0: 726f 6772 616d 2e0a 0a2d 20e2 8098 5468  rogram...- ...Th
+000006e0: 6520 4c69 6365 6e73 6f72 e280 993a 2074  e Licensor...: t
+000006f0: 6865 206e 6174 7572 616c 206f 7220 6c65  he natural or le
+00000700: 6761 6c20 7065 7273 6f6e 2074 6861 7420  gal person that 
+00000710: 6469 7374 7269 6275 7465 7320 6f72 2063  distributes or c
+00000720: 6f6d 6d75 6e69 6361 7465 730a 2020 7468  ommunicates.  th
+00000730: 6520 576f 726b 2075 6e64 6572 2074 6865  e Work under the
+00000740: 204c 6963 656e 6365 2e0a 0a2d 20e2 8098   Licence...- ...
+00000750: 436f 6e74 7269 6275 746f 7228 7329 e280  Contributor(s)..
+00000760: 993a 2061 6e79 206e 6174 7572 616c 206f  .: any natural o
+00000770: 7220 6c65 6761 6c20 7065 7273 6f6e 2077  r legal person w
+00000780: 686f 206d 6f64 6966 6965 7320 7468 6520  ho modifies the 
+00000790: 576f 726b 2075 6e64 6572 0a20 2074 6865  Work under.  the
+000007a0: 204c 6963 656e 6365 2c20 6f72 206f 7468   Licence, or oth
+000007b0: 6572 7769 7365 2063 6f6e 7472 6962 7574  erwise contribut
+000007c0: 6573 2074 6f20 7468 6520 6372 6561 7469  es to the creati
+000007d0: 6f6e 206f 6620 6120 4465 7269 7661 7469  on of a Derivati
+000007e0: 7665 2057 6f72 6b2e 0a0a 2d20 e280 9854  ve Work...- ...T
+000007f0: 6865 204c 6963 656e 7365 65e2 8099 206f  he Licensee... o
+00000800: 7220 e280 9859 6f75 e280 993a 2061 6e79  r ...You...: any
+00000810: 206e 6174 7572 616c 206f 7220 6c65 6761   natural or lega
+00000820: 6c20 7065 7273 6f6e 2077 686f 206d 616b  l person who mak
+00000830: 6573 2061 6e79 2075 7361 6765 206f 660a  es any usage of.
+00000840: 2020 7468 6520 576f 726b 2075 6e64 6572    the Work under
+00000850: 2074 6865 2074 6572 6d73 206f 6620 7468   the terms of th
+00000860: 6520 4c69 6365 6e63 652e 0a0a 2d20 e280  e Licence...- ..
+00000870: 9844 6973 7472 6962 7574 696f 6ee2 8099  .Distribution...
+00000880: 206f 7220 e280 9843 6f6d 6d75 6e69 6361   or ...Communica
+00000890: 7469 6f6e e280 993a 2061 6e79 2061 6374  tion...: any act
+000008a0: 206f 6620 7365 6c6c 696e 672c 2067 6976   of selling, giv
+000008b0: 696e 672c 206c 656e 6469 6e67 2c0a 2020  ing, lending,.  
+000008c0: 7265 6e74 696e 672c 2064 6973 7472 6962  renting, distrib
+000008d0: 7574 696e 672c 2063 6f6d 6d75 6e69 6361  uting, communica
+000008e0: 7469 6e67 2c20 7472 616e 736d 6974 7469  ting, transmitti
+000008f0: 6e67 2c20 6f72 206f 7468 6572 7769 7365  ng, or otherwise
+00000900: 206d 616b 696e 670a 2020 6176 6169 6c61   making.  availa
+00000910: 626c 652c 206f 6e6c 696e 6520 6f72 206f  ble, online or o
+00000920: 6666 6c69 6e65 2c20 636f 7069 6573 206f  ffline, copies o
+00000930: 6620 7468 6520 576f 726b 206f 7220 7072  f the Work or pr
+00000940: 6f76 6964 696e 6720 6163 6365 7373 2074  oviding access t
+00000950: 6f20 6974 730a 2020 6573 7365 6e74 6961  o its.  essentia
+00000960: 6c20 6675 6e63 7469 6f6e 616c 6974 6965  l functionalitie
+00000970: 7320 6174 2074 6865 2064 6973 706f 7361  s at the disposa
+00000980: 6c20 6f66 2061 6e79 206f 7468 6572 206e  l of any other n
+00000990: 6174 7572 616c 206f 7220 6c65 6761 6c0a  atural or legal.
+000009a0: 2020 7065 7273 6f6e 2e0a 0a32 2e20 5363    person...2. Sc
+000009b0: 6f70 6520 6f66 2074 6865 2072 6967 6874  ope of the right
+000009c0: 7320 6772 616e 7465 6420 6279 2074 6865  s granted by the
+000009d0: 204c 6963 656e 6365 0a0a 5468 6520 4c69   Licence..The Li
+000009e0: 6365 6e73 6f72 2068 6572 6562 7920 6772  censor hereby gr
+000009f0: 616e 7473 2059 6f75 2061 2077 6f72 6c64  ants You a world
+00000a00: 7769 6465 2c20 726f 7961 6c74 792d 6672  wide, royalty-fr
+00000a10: 6565 2c20 6e6f 6e2d 6578 636c 7573 6976  ee, non-exclusiv
+00000a20: 652c 0a73 7562 6c69 6365 6e73 6162 6c65  e,.sublicensable
+00000a30: 206c 6963 656e 6365 2074 6f20 646f 2074   licence to do t
+00000a40: 6865 2066 6f6c 6c6f 7769 6e67 2c20 666f  he following, fo
+00000a50: 7220 7468 6520 6475 7261 7469 6f6e 206f  r the duration o
+00000a60: 6620 636f 7079 7269 6768 740a 7665 7374  f copyright.vest
+00000a70: 6564 2069 6e20 7468 6520 4f72 6967 696e  ed in the Origin
+00000a80: 616c 2057 6f72 6b3a 0a0a 2d20 7573 6520  al Work:..- use 
+00000a90: 7468 6520 576f 726b 2069 6e20 616e 7920  the Work in any 
+00000aa0: 6369 7263 756d 7374 616e 6365 2061 6e64  circumstance and
+00000ab0: 2066 6f72 2061 6c6c 2075 7361 6765 2c0a   for all usage,.
+00000ac0: 2d20 7265 7072 6f64 7563 6520 7468 6520  - reproduce the 
+00000ad0: 576f 726b 2c0a 2d20 6d6f 6469 6679 2074  Work,.- modify t
+00000ae0: 6865 2057 6f72 6b2c 2061 6e64 206d 616b  he Work, and mak
+00000af0: 6520 4465 7269 7661 7469 7665 2057 6f72  e Derivative Wor
+00000b00: 6b73 2062 6173 6564 2075 706f 6e20 7468  ks based upon th
+00000b10: 6520 576f 726b 2c0a 2d20 636f 6d6d 756e  e Work,.- commun
+00000b20: 6963 6174 6520 746f 2074 6865 2070 7562  icate to the pub
+00000b30: 6c69 632c 2069 6e63 6c75 6469 6e67 2074  lic, including t
+00000b40: 6865 2072 6967 6874 2074 6f20 6d61 6b65  he right to make
+00000b50: 2061 7661 696c 6162 6c65 206f 7220 6469   available or di
+00000b60: 7370 6c61 790a 2020 7468 6520 576f 726b  splay.  the Work
+00000b70: 206f 7220 636f 7069 6573 2074 6865 7265   or copies there
+00000b80: 6f66 2074 6f20 7468 6520 7075 626c 6963  of to the public
+00000b90: 2061 6e64 2070 6572 666f 726d 2070 7562   and perform pub
+00000ba0: 6c69 636c 792c 2061 7320 7468 6520 6361  licly, as the ca
+00000bb0: 7365 0a20 206d 6179 2062 652c 2074 6865  se.  may be, the
+00000bc0: 2057 6f72 6b2c 0a2d 2064 6973 7472 6962   Work,.- distrib
+00000bd0: 7574 6520 7468 6520 576f 726b 206f 7220  ute the Work or 
+00000be0: 636f 7069 6573 2074 6865 7265 6f66 2c0a  copies thereof,.
+00000bf0: 2d20 6c65 6e64 2061 6e64 2072 656e 7420  - lend and rent 
+00000c00: 7468 6520 576f 726b 206f 7220 636f 7069  the Work or copi
+00000c10: 6573 2074 6865 7265 6f66 2c0a 2d20 7375  es thereof,.- su
+00000c20: 626c 6963 656e 7365 2072 6967 6874 7320  blicense rights 
+00000c30: 696e 2074 6865 2057 6f72 6b20 6f72 2063  in the Work or c
+00000c40: 6f70 6965 7320 7468 6572 656f 662e 0a0a  opies thereof...
+00000c50: 5468 6f73 6520 7269 6768 7473 2063 616e  Those rights can
+00000c60: 2062 6520 6578 6572 6369 7365 6420 6f6e   be exercised on
+00000c70: 2061 6e79 206d 6564 6961 2c20 7375 7070   any media, supp
+00000c80: 6f72 7473 2061 6e64 2066 6f72 6d61 7473  orts and formats
+00000c90: 2c20 7768 6574 6865 7220 6e6f 770a 6b6e  , whether now.kn
+00000ca0: 6f77 6e20 6f72 206c 6174 6572 2069 6e76  own or later inv
+00000cb0: 656e 7465 642c 2061 7320 6661 7220 6173  ented, as far as
+00000cc0: 2074 6865 2061 7070 6c69 6361 626c 6520   the applicable 
+00000cd0: 6c61 7720 7065 726d 6974 7320 736f 2e0a  law permits so..
+00000ce0: 0a49 6e20 7468 6520 636f 756e 7472 6965  .In the countrie
+00000cf0: 7320 7768 6572 6520 6d6f 7261 6c20 7269  s where moral ri
+00000d00: 6768 7473 2061 7070 6c79 2c20 7468 6520  ghts apply, the 
+00000d10: 4c69 6365 6e73 6f72 2077 6169 7665 7320  Licensor waives 
+00000d20: 6869 7320 7269 6768 7420 746f 0a65 7865  his right to.exe
+00000d30: 7263 6973 6520 6869 7320 6d6f 7261 6c20  rcise his moral 
+00000d40: 7269 6768 7420 746f 2074 6865 2065 7874  right to the ext
+00000d50: 656e 7420 616c 6c6f 7765 6420 6279 206c  ent allowed by l
+00000d60: 6177 2069 6e20 6f72 6465 7220 746f 206d  aw in order to m
+00000d70: 616b 650a 6566 6665 6374 6976 6520 7468  ake.effective th
+00000d80: 6520 6c69 6365 6e63 6520 6f66 2074 6865  e licence of the
+00000d90: 2065 636f 6e6f 6d69 6320 7269 6768 7473   economic rights
+00000da0: 2068 6572 6520 6162 6f76 6520 6c69 7374   here above list
+00000db0: 6564 2e0a 0a54 6865 204c 6963 656e 736f  ed...The Licenso
+00000dc0: 7220 6772 616e 7473 2074 6f20 7468 6520  r grants to the 
+00000dd0: 4c69 6365 6e73 6565 2072 6f79 616c 7479  Licensee royalty
+00000de0: 2d66 7265 652c 206e 6f6e 2d65 7863 6c75  -free, non-exclu
+00000df0: 7369 7665 2075 7361 6765 2072 6967 6874  sive usage right
+00000e00: 730a 746f 2061 6e79 2070 6174 656e 7473  s.to any patents
+00000e10: 2068 656c 6420 6279 2074 6865 204c 6963   held by the Lic
+00000e20: 656e 736f 722c 2074 6f20 7468 6520 6578  ensor, to the ex
+00000e30: 7465 6e74 206e 6563 6573 7361 7279 2074  tent necessary t
+00000e40: 6f20 6d61 6b65 2075 7365 206f 660a 7468  o make use of.th
+00000e50: 6520 7269 6768 7473 2067 7261 6e74 6564  e rights granted
+00000e60: 206f 6e20 7468 6520 576f 726b 2075 6e64   on the Work und
+00000e70: 6572 2074 6869 7320 4c69 6365 6e63 652e  er this Licence.
+00000e80: 0a0a 332e 2043 6f6d 6d75 6e69 6361 7469  ..3. Communicati
+00000e90: 6f6e 206f 6620 7468 6520 536f 7572 6365  on of the Source
+00000ea0: 2043 6f64 650a 0a54 6865 204c 6963 656e   Code..The Licen
+00000eb0: 736f 7220 6d61 7920 7072 6f76 6964 6520  sor may provide 
+00000ec0: 7468 6520 576f 726b 2065 6974 6865 7220  the Work either 
+00000ed0: 696e 2069 7473 2053 6f75 7263 6520 436f  in its Source Co
+00000ee0: 6465 2066 6f72 6d2c 206f 7220 6173 0a45  de form, or as.E
+00000ef0: 7865 6375 7461 626c 6520 436f 6465 2e20  xecutable Code. 
+00000f00: 4966 2074 6865 2057 6f72 6b20 6973 2070  If the Work is p
+00000f10: 726f 7669 6465 6420 6173 2045 7865 6375  rovided as Execu
+00000f20: 7461 626c 6520 436f 6465 2c20 7468 6520  table Code, the 
+00000f30: 4c69 6365 6e73 6f72 0a70 726f 7669 6465  Licensor.provide
+00000f40: 7320 696e 2061 6464 6974 696f 6e20 6120  s in addition a 
+00000f50: 6d61 6368 696e 652d 7265 6164 6162 6c65  machine-readable
+00000f60: 2063 6f70 7920 6f66 2074 6865 2053 6f75   copy of the Sou
+00000f70: 7263 6520 436f 6465 206f 6620 7468 6520  rce Code of the 
+00000f80: 576f 726b 0a61 6c6f 6e67 2077 6974 6820  Work.along with 
+00000f90: 6561 6368 2063 6f70 7920 6f66 2074 6865  each copy of the
+00000fa0: 2057 6f72 6b20 7468 6174 2074 6865 204c   Work that the L
+00000fb0: 6963 656e 736f 7220 6469 7374 7269 6275  icensor distribu
+00000fc0: 7465 7320 6f72 2069 6e64 6963 6174 6573  tes or indicates
+00000fd0: 2c0a 696e 2061 206e 6f74 6963 6520 666f  ,.in a notice fo
+00000fe0: 6c6c 6f77 696e 6720 7468 6520 636f 7079  llowing the copy
+00000ff0: 7269 6768 7420 6e6f 7469 6365 2061 7474  right notice att
+00001000: 6163 6865 6420 746f 2074 6865 2057 6f72  ached to the Wor
+00001010: 6b2c 2061 2072 6570 6f73 6974 6f72 790a  k, a repository.
+00001020: 7768 6572 6520 7468 6520 536f 7572 6365  where the Source
+00001030: 2043 6f64 6520 6973 2065 6173 696c 7920   Code is easily 
+00001040: 616e 6420 6672 6565 6c79 2061 6363 6573  and freely acces
+00001050: 7369 626c 6520 666f 7220 6173 206c 6f6e  sible for as lon
+00001060: 6720 6173 2074 6865 0a4c 6963 656e 736f  g as the.Licenso
+00001070: 7220 636f 6e74 696e 7565 7320 746f 2064  r continues to d
+00001080: 6973 7472 6962 7574 6520 6f72 2063 6f6d  istribute or com
+00001090: 6d75 6e69 6361 7465 2074 6865 2057 6f72  municate the Wor
+000010a0: 6b2e 0a0a 342e 204c 696d 6974 6174 696f  k...4. Limitatio
+000010b0: 6e73 206f 6e20 636f 7079 7269 6768 740a  ns on copyright.
+000010c0: 0a4e 6f74 6869 6e67 2069 6e20 7468 6973  .Nothing in this
+000010d0: 204c 6963 656e 6365 2069 7320 696e 7465   Licence is inte
+000010e0: 6e64 6564 2074 6f20 6465 7072 6976 6520  nded to deprive 
+000010f0: 7468 6520 4c69 6365 6e73 6565 206f 6620  the Licensee of 
+00001100: 7468 6520 6265 6e65 6669 7473 0a66 726f  the benefits.fro
+00001110: 6d20 616e 7920 6578 6365 7074 696f 6e20  m any exception 
+00001120: 6f72 206c 696d 6974 6174 696f 6e20 746f  or limitation to
+00001130: 2074 6865 2065 7863 6c75 7369 7665 2072   the exclusive r
+00001140: 6967 6874 7320 6f66 2074 6865 2072 6967  ights of the rig
+00001150: 6874 7320 6f77 6e65 7273 0a69 6e20 7468  hts owners.in th
+00001160: 6520 576f 726b 2c20 6f66 2074 6865 2065  e Work, of the e
+00001170: 7868 6175 7374 696f 6e20 6f66 2074 686f  xhaustion of tho
+00001180: 7365 2072 6967 6874 7320 6f72 206f 6620  se rights or of 
+00001190: 6f74 6865 7220 6170 706c 6963 6162 6c65  other applicable
+000011a0: 0a6c 696d 6974 6174 696f 6e73 2074 6865  .limitations the
+000011b0: 7265 746f 2e0a 0a35 2e20 4f62 6c69 6761  reto...5. Obliga
+000011c0: 7469 6f6e 7320 6f66 2074 6865 204c 6963  tions of the Lic
+000011d0: 656e 7365 650a 0a54 6865 2067 7261 6e74  ensee..The grant
+000011e0: 206f 6620 7468 6520 7269 6768 7473 206d   of the rights m
+000011f0: 656e 7469 6f6e 6564 2061 626f 7665 2069  entioned above i
+00001200: 7320 7375 626a 6563 7420 746f 2073 6f6d  s subject to som
+00001210: 6520 7265 7374 7269 6374 696f 6e73 2061  e restrictions a
+00001220: 6e64 0a6f 626c 6967 6174 696f 6e73 2069  nd.obligations i
+00001230: 6d70 6f73 6564 206f 6e20 7468 6520 4c69  mposed on the Li
+00001240: 6365 6e73 6565 2e20 5468 6f73 6520 6f62  censee. Those ob
+00001250: 6c69 6761 7469 6f6e 7320 6172 6520 7468  ligations are th
+00001260: 6520 666f 6c6c 6f77 696e 673a 0a0a 4174  e following:..At
+00001270: 7472 6962 7574 696f 6e20 7269 6768 743a  tribution right:
+00001280: 2054 6865 204c 6963 656e 7365 6520 7368   The Licensee sh
+00001290: 616c 6c20 6b65 6570 2069 6e74 6163 7420  all keep intact 
+000012a0: 616c 6c20 636f 7079 7269 6768 742c 2070  all copyright, p
+000012b0: 6174 656e 7420 6f72 0a74 7261 6465 6d61  atent or.tradema
+000012c0: 726b 7320 6e6f 7469 6365 7320 616e 6420  rks notices and 
+000012d0: 616c 6c20 6e6f 7469 6365 7320 7468 6174  all notices that
+000012e0: 2072 6566 6572 2074 6f20 7468 6520 4c69   refer to the Li
+000012f0: 6365 6e63 6520 616e 6420 746f 2074 6865  cence and to the
+00001300: 0a64 6973 636c 6169 6d65 7220 6f66 2077  .disclaimer of w
+00001310: 6172 7261 6e74 6965 732e 2054 6865 204c  arranties. The L
+00001320: 6963 656e 7365 6520 6d75 7374 2069 6e63  icensee must inc
+00001330: 6c75 6465 2061 2063 6f70 7920 6f66 2073  lude a copy of s
+00001340: 7563 6820 6e6f 7469 6365 7320 616e 640a  uch notices and.
+00001350: 6120 636f 7079 206f 6620 7468 6520 4c69  a copy of the Li
+00001360: 6365 6e63 6520 7769 7468 2065 7665 7279  cence with every
+00001370: 2063 6f70 7920 6f66 2074 6865 2057 6f72   copy of the Wor
+00001380: 6b20 6865 2f73 6865 2064 6973 7472 6962  k he/she distrib
+00001390: 7574 6573 206f 720a 636f 6d6d 756e 6963  utes or.communic
+000013a0: 6174 6573 2e20 5468 6520 4c69 6365 6e73  ates. The Licens
+000013b0: 6565 206d 7573 7420 6361 7573 6520 616e  ee must cause an
+000013c0: 7920 4465 7269 7661 7469 7665 2057 6f72  y Derivative Wor
+000013d0: 6b20 746f 2063 6172 7279 2070 726f 6d69  k to carry promi
+000013e0: 6e65 6e74 0a6e 6f74 6963 6573 2073 7461  nent.notices sta
+000013f0: 7469 6e67 2074 6861 7420 7468 6520 576f  ting that the Wo
+00001400: 726b 2068 6173 2062 6565 6e20 6d6f 6469  rk has been modi
+00001410: 6669 6564 2061 6e64 2074 6865 2064 6174  fied and the dat
+00001420: 6520 6f66 206d 6f64 6966 6963 6174 696f  e of modificatio
+00001430: 6e2e 0a0a 436f 7079 6c65 6674 2063 6c61  n...Copyleft cla
+00001440: 7573 653a 2049 6620 7468 6520 4c69 6365  use: If the Lice
+00001450: 6e73 6565 2064 6973 7472 6962 7574 6573  nsee distributes
+00001460: 206f 7220 636f 6d6d 756e 6963 6174 6573   or communicates
+00001470: 2063 6f70 6965 7320 6f66 2074 6865 0a4f   copies of the.O
+00001480: 7269 6769 6e61 6c20 576f 726b 7320 6f72  riginal Works or
+00001490: 2044 6572 6976 6174 6976 6520 576f 726b   Derivative Work
+000014a0: 732c 2074 6869 7320 4469 7374 7269 6275  s, this Distribu
+000014b0: 7469 6f6e 206f 7220 436f 6d6d 756e 6963  tion or Communic
+000014c0: 6174 696f 6e20 7769 6c6c 2062 650a 646f  ation will be.do
+000014d0: 6e65 2075 6e64 6572 2074 6865 2074 6572  ne under the ter
+000014e0: 6d73 206f 6620 7468 6973 204c 6963 656e  ms of this Licen
+000014f0: 6365 206f 7220 6f66 2061 206c 6174 6572  ce or of a later
+00001500: 2076 6572 7369 6f6e 206f 6620 7468 6973   version of this
+00001510: 204c 6963 656e 6365 0a75 6e6c 6573 7320   Licence.unless 
+00001520: 7468 6520 4f72 6967 696e 616c 2057 6f72  the Original Wor
+00001530: 6b20 6973 2065 7870 7265 7373 6c79 2064  k is expressly d
+00001540: 6973 7472 6962 7574 6564 206f 6e6c 7920  istributed only 
+00001550: 756e 6465 7220 7468 6973 2076 6572 7369  under this versi
+00001560: 6f6e 206f 660a 7468 6520 4c69 6365 6e63  on of.the Licenc
+00001570: 6520 e280 9420 666f 7220 6578 616d 706c  e ... for exampl
+00001580: 6520 6279 2063 6f6d 6d75 6e69 6361 7469  e by communicati
+00001590: 6e67 20e2 8098 4555 504c 2076 2e20 312e  ng ...EUPL v. 1.
+000015a0: 3220 6f6e 6c79 e280 992e 2054 6865 204c  2 only.... The L
+000015b0: 6963 656e 7365 650a 2862 6563 6f6d 696e  icensee.(becomin
+000015c0: 6720 4c69 6365 6e73 6f72 2920 6361 6e6e  g Licensor) cann
+000015d0: 6f74 206f 6666 6572 206f 7220 696d 706f  ot offer or impo
+000015e0: 7365 2061 6e79 2061 6464 6974 696f 6e61  se any additiona
+000015f0: 6c20 7465 726d 7320 6f72 2063 6f6e 6469  l terms or condi
+00001600: 7469 6f6e 730a 6f6e 2074 6865 2057 6f72  tions.on the Wor
+00001610: 6b20 6f72 2044 6572 6976 6174 6976 6520  k or Derivative 
+00001620: 576f 726b 2074 6861 7420 616c 7465 7220  Work that alter 
+00001630: 6f72 2072 6573 7472 6963 7420 7468 6520  or restrict the 
+00001640: 7465 726d 7320 6f66 2074 6865 0a4c 6963  terms of the.Lic
+00001650: 656e 6365 2e0a 0a43 6f6d 7061 7469 6269  ence...Compatibi
+00001660: 6c69 7479 2063 6c61 7573 653a 2049 6620  lity clause: If 
+00001670: 7468 6520 4c69 6365 6e73 6565 2044 6973  the Licensee Dis
+00001680: 7472 6962 7574 6573 206f 7220 436f 6d6d  tributes or Comm
+00001690: 756e 6963 6174 6573 2044 6572 6976 6174  unicates Derivat
+000016a0: 6976 650a 576f 726b 7320 6f72 2063 6f70  ive.Works or cop
+000016b0: 6965 7320 7468 6572 656f 6620 6261 7365  ies thereof base
+000016c0: 6420 7570 6f6e 2062 6f74 6820 7468 6520  d upon both the 
+000016d0: 576f 726b 2061 6e64 2061 6e6f 7468 6572  Work and another
+000016e0: 2077 6f72 6b20 6c69 6365 6e73 6564 0a75   work licensed.u
+000016f0: 6e64 6572 2061 2043 6f6d 7061 7469 626c  nder a Compatibl
+00001700: 6520 4c69 6365 6e63 652c 2074 6869 7320  e Licence, this 
+00001710: 4469 7374 7269 6275 7469 6f6e 206f 7220  Distribution or 
+00001720: 436f 6d6d 756e 6963 6174 696f 6e20 6361  Communication ca
+00001730: 6e20 6265 2064 6f6e 650a 756e 6465 7220  n be done.under 
+00001740: 7468 6520 7465 726d 7320 6f66 2074 6869  the terms of thi
+00001750: 7320 436f 6d70 6174 6962 6c65 204c 6963  s Compatible Lic
+00001760: 656e 6365 2e20 466f 7220 7468 6520 7361  ence. For the sa
+00001770: 6b65 206f 6620 7468 6973 2063 6c61 7573  ke of this claus
+00001780: 652c 0ae2 8098 436f 6d70 6174 6962 6c65  e,....Compatible
+00001790: 204c 6963 656e 6365 e280 9920 7265 6665   Licence... refe
+000017a0: 7273 2074 6f20 7468 6520 6c69 6365 6e63  rs to the licenc
+000017b0: 6573 206c 6973 7465 6420 696e 2074 6865  es listed in the
+000017c0: 2061 7070 656e 6469 7820 6174 7461 6368   appendix attach
+000017d0: 6564 2074 6f0a 7468 6973 204c 6963 656e  ed to.this Licen
+000017e0: 6365 2e20 5368 6f75 6c64 2074 6865 204c  ce. Should the L
+000017f0: 6963 656e 7365 6527 7320 6f62 6c69 6761  icensee's obliga
+00001800: 7469 6f6e 7320 756e 6465 7220 7468 6520  tions under the 
+00001810: 436f 6d70 6174 6962 6c65 204c 6963 656e  Compatible Licen
+00001820: 6365 0a63 6f6e 666c 6963 7420 7769 7468  ce.conflict with
+00001830: 2068 6973 2f68 6572 206f 626c 6967 6174   his/her obligat
+00001840: 696f 6e73 2075 6e64 6572 2074 6869 7320  ions under this 
+00001850: 4c69 6365 6e63 652c 2074 6865 206f 626c  Licence, the obl
+00001860: 6967 6174 696f 6e73 206f 6620 7468 650a  igations of the.
+00001870: 436f 6d70 6174 6962 6c65 204c 6963 656e  Compatible Licen
+00001880: 6365 2073 6861 6c6c 2070 7265 7661 696c  ce shall prevail
+00001890: 2e0a 0a50 726f 7669 7369 6f6e 206f 6620  ...Provision of 
+000018a0: 536f 7572 6365 2043 6f64 653a 2057 6865  Source Code: Whe
+000018b0: 6e20 6469 7374 7269 6275 7469 6e67 206f  n distributing o
+000018c0: 7220 636f 6d6d 756e 6963 6174 696e 6720  r communicating 
+000018d0: 636f 7069 6573 206f 6620 7468 650a 576f  copies of the.Wo
+000018e0: 726b 2c20 7468 6520 4c69 6365 6e73 6565  rk, the Licensee
+000018f0: 2077 696c 6c20 7072 6f76 6964 6520 6120   will provide a 
+00001900: 6d61 6368 696e 652d 7265 6164 6162 6c65  machine-readable
+00001910: 2063 6f70 7920 6f66 2074 6865 2053 6f75   copy of the Sou
+00001920: 7263 6520 436f 6465 206f 720a 696e 6469  rce Code or.indi
+00001930: 6361 7465 2061 2072 6570 6f73 6974 6f72  cate a repositor
+00001940: 7920 7768 6572 6520 7468 6973 2053 6f75  y where this Sou
+00001950: 7263 6520 7769 6c6c 2062 6520 6561 7369  rce will be easi
+00001960: 6c79 2061 6e64 2066 7265 656c 7920 6176  ly and freely av
+00001970: 6169 6c61 626c 650a 666f 7220 6173 206c  ailable.for as l
+00001980: 6f6e 6720 6173 2074 6865 204c 6963 656e  ong as the Licen
+00001990: 7365 6520 636f 6e74 696e 7565 7320 746f  see continues to
+000019a0: 2064 6973 7472 6962 7574 6520 6f72 2063   distribute or c
+000019b0: 6f6d 6d75 6e69 6361 7465 2074 6865 2057  ommunicate the W
+000019c0: 6f72 6b2e 0a0a 4c65 6761 6c20 5072 6f74  ork...Legal Prot
+000019d0: 6563 7469 6f6e 3a20 5468 6973 204c 6963  ection: This Lic
+000019e0: 656e 6365 2064 6f65 7320 6e6f 7420 6772  ence does not gr
+000019f0: 616e 7420 7065 726d 6973 7369 6f6e 2074  ant permission t
+00001a00: 6f20 7573 6520 7468 6520 7472 6164 650a  o use the trade.
+00001a10: 6e61 6d65 732c 2074 7261 6465 6d61 726b  names, trademark
+00001a20: 732c 2073 6572 7669 6365 206d 6172 6b73  s, service marks
+00001a30: 2c20 6f72 206e 616d 6573 206f 6620 7468  , or names of th
+00001a40: 6520 4c69 6365 6e73 6f72 2c20 6578 6365  e Licensor, exce
+00001a50: 7074 2061 7320 7265 7175 6972 6564 0a66  pt as required.f
+00001a60: 6f72 2072 6561 736f 6e61 626c 6520 616e  or reasonable an
+00001a70: 6420 6375 7374 6f6d 6172 7920 7573 6520  d customary use 
+00001a80: 696e 2064 6573 6372 6962 696e 6720 7468  in describing th
+00001a90: 6520 6f72 6967 696e 206f 6620 7468 6520  e origin of the 
+00001aa0: 576f 726b 2061 6e64 0a72 6570 726f 6475  Work and.reprodu
+00001ab0: 6369 6e67 2074 6865 2063 6f6e 7465 6e74  cing the content
+00001ac0: 206f 6620 7468 6520 636f 7079 7269 6768   of the copyrigh
+00001ad0: 7420 6e6f 7469 6365 2e0a 0a36 2e20 4368  t notice...6. Ch
+00001ae0: 6169 6e20 6f66 2041 7574 686f 7273 6869  ain of Authorshi
+00001af0: 700a 0a54 6865 206f 7269 6769 6e61 6c20  p..The original 
+00001b00: 4c69 6365 6e73 6f72 2077 6172 7261 6e74  Licensor warrant
+00001b10: 7320 7468 6174 2074 6865 2063 6f70 7972  s that the copyr
+00001b20: 6967 6874 2069 6e20 7468 6520 4f72 6967  ight in the Orig
+00001b30: 696e 616c 2057 6f72 6b20 6772 616e 7465  inal Work grante
+00001b40: 640a 6865 7265 756e 6465 7220 6973 206f  d.hereunder is o
+00001b50: 776e 6564 2062 7920 6869 6d2f 6865 7220  wned by him/her 
+00001b60: 6f72 206c 6963 656e 7365 6420 746f 2068  or licensed to h
+00001b70: 696d 2f68 6572 2061 6e64 2074 6861 7420  im/her and that 
+00001b80: 6865 2f73 6865 2068 6173 2074 6865 0a70  he/she has the.p
+00001b90: 6f77 6572 2061 6e64 2061 7574 686f 7269  ower and authori
+00001ba0: 7479 2074 6f20 6772 616e 7420 7468 6520  ty to grant the 
+00001bb0: 4c69 6365 6e63 652e 0a0a 4561 6368 2043  Licence...Each C
+00001bc0: 6f6e 7472 6962 7574 6f72 2077 6172 7261  ontributor warra
+00001bd0: 6e74 7320 7468 6174 2074 6865 2063 6f70  nts that the cop
+00001be0: 7972 6967 6874 2069 6e20 7468 6520 6d6f  yright in the mo
+00001bf0: 6469 6669 6361 7469 6f6e 7320 6865 2f73  difications he/s
+00001c00: 6865 0a62 7269 6e67 7320 746f 2074 6865  he.brings to the
+00001c10: 2057 6f72 6b20 6172 6520 6f77 6e65 6420   Work are owned 
+00001c20: 6279 2068 696d 2f68 6572 206f 7220 6c69  by him/her or li
+00001c30: 6365 6e73 6564 2074 6f20 6869 6d2f 6865  censed to him/he
+00001c40: 7220 616e 6420 7468 6174 2068 652f 7368  r and that he/sh
+00001c50: 650a 6861 7320 7468 6520 706f 7765 7220  e.has the power 
+00001c60: 616e 6420 6175 7468 6f72 6974 7920 746f  and authority to
+00001c70: 2067 7261 6e74 2074 6865 204c 6963 656e   grant the Licen
+00001c80: 6365 2e0a 0a45 6163 6820 7469 6d65 2059  ce...Each time Y
+00001c90: 6f75 2061 6363 6570 7420 7468 6520 4c69  ou accept the Li
+00001ca0: 6365 6e63 652c 2074 6865 206f 7269 6769  cence, the origi
+00001cb0: 6e61 6c20 4c69 6365 6e73 6f72 2061 6e64  nal Licensor and
+00001cc0: 2073 7562 7365 7175 656e 740a 436f 6e74   subsequent.Cont
+00001cd0: 7269 6275 746f 7273 2067 7261 6e74 2059  ributors grant Y
+00001ce0: 6f75 2061 206c 6963 656e 6365 2074 6f20  ou a licence to 
+00001cf0: 7468 6569 7220 636f 6e74 7269 6275 7469  their contributi
+00001d00: 6f6e 7320 746f 2074 6865 2057 6f72 6b2c  ons to the Work,
+00001d10: 2075 6e64 6572 2074 6865 0a74 6572 6d73   under the.terms
+00001d20: 206f 6620 7468 6973 204c 6963 656e 6365   of this Licence
+00001d30: 2e0a 0a37 2e20 4469 7363 6c61 696d 6572  ...7. Disclaimer
+00001d40: 206f 6620 5761 7272 616e 7479 0a0a 5468   of Warranty..Th
+00001d50: 6520 576f 726b 2069 7320 6120 776f 726b  e Work is a work
+00001d60: 2069 6e20 7072 6f67 7265 7373 2c20 7768   in progress, wh
+00001d70: 6963 6820 6973 2063 6f6e 7469 6e75 6f75  ich is continuou
+00001d80: 736c 7920 696d 7072 6f76 6564 2062 7920  sly improved by 
+00001d90: 6e75 6d65 726f 7573 0a43 6f6e 7472 6962  numerous.Contrib
+00001da0: 7574 6f72 732e 2049 7420 6973 206e 6f74  utors. It is not
+00001db0: 2061 2066 696e 6973 6865 6420 776f 726b   a finished work
+00001dc0: 2061 6e64 206d 6179 2074 6865 7265 666f   and may therefo
+00001dd0: 7265 2063 6f6e 7461 696e 2064 6566 6563  re contain defec
+00001de0: 7473 206f 720a e280 9862 7567 73e2 8099  ts or....bugs...
+00001df0: 2069 6e68 6572 656e 7420 746f 2074 6869   inherent to thi
+00001e00: 7320 7479 7065 206f 6620 6465 7665 6c6f  s type of develo
+00001e10: 706d 656e 742e 0a0a 466f 7220 7468 6520  pment...For the 
+00001e20: 6162 6f76 6520 7265 6173 6f6e 2c20 7468  above reason, th
+00001e30: 6520 576f 726b 2069 7320 7072 6f76 6964  e Work is provid
+00001e40: 6564 2075 6e64 6572 2074 6865 204c 6963  ed under the Lic
+00001e50: 656e 6365 206f 6e20 616e 20e2 8098 6173  ence on an ...as
+00001e60: 2069 73e2 8099 0a62 6173 6973 2061 6e64   is....basis and
+00001e70: 2077 6974 686f 7574 2077 6172 7261 6e74   without warrant
+00001e80: 6965 7320 6f66 2061 6e79 206b 696e 6420  ies of any kind 
+00001e90: 636f 6e63 6572 6e69 6e67 2074 6865 2057  concerning the W
+00001ea0: 6f72 6b2c 2069 6e63 6c75 6469 6e67 0a77  ork, including.w
+00001eb0: 6974 686f 7574 206c 696d 6974 6174 696f  ithout limitatio
+00001ec0: 6e20 6d65 7263 6861 6e74 6162 696c 6974  n merchantabilit
+00001ed0: 792c 2066 6974 6e65 7373 2066 6f72 2061  y, fitness for a
+00001ee0: 2070 6172 7469 6375 6c61 7220 7075 7270   particular purp
+00001ef0: 6f73 652c 2061 6273 656e 6365 0a6f 6620  ose, absence.of 
+00001f00: 6465 6665 6374 7320 6f72 2065 7272 6f72  defects or error
+00001f10: 732c 2061 6363 7572 6163 792c 206e 6f6e  s, accuracy, non
+00001f20: 2d69 6e66 7269 6e67 656d 656e 7420 6f66  -infringement of
+00001f30: 2069 6e74 656c 6c65 6374 7561 6c20 7072   intellectual pr
+00001f40: 6f70 6572 7479 0a72 6967 6874 7320 6f74  operty.rights ot
+00001f50: 6865 7220 7468 616e 2063 6f70 7972 6967  her than copyrig
+00001f60: 6874 2061 7320 7374 6174 6564 2069 6e20  ht as stated in 
+00001f70: 4172 7469 636c 6520 3620 6f66 2074 6869  Article 6 of thi
+00001f80: 7320 4c69 6365 6e63 652e 0a0a 5468 6973  s Licence...This
+00001f90: 2064 6973 636c 6169 6d65 7220 6f66 2077   disclaimer of w
+00001fa0: 6172 7261 6e74 7920 6973 2061 6e20 6573  arranty is an es
+00001fb0: 7365 6e74 6961 6c20 7061 7274 206f 6620  sential part of 
+00001fc0: 7468 6520 4c69 6365 6e63 6520 616e 6420  the Licence and 
+00001fd0: 610a 636f 6e64 6974 696f 6e20 666f 7220  a.condition for 
+00001fe0: 7468 6520 6772 616e 7420 6f66 2061 6e79  the grant of any
+00001ff0: 2072 6967 6874 7320 746f 2074 6865 2057   rights to the W
+00002000: 6f72 6b2e 0a0a 382e 2044 6973 636c 6169  ork...8. Disclai
+00002010: 6d65 7220 6f66 204c 6961 6269 6c69 7479  mer of Liability
+00002020: 0a0a 4578 6365 7074 2069 6e20 7468 6520  ..Except in the 
+00002030: 6361 7365 7320 6f66 2077 696c 6675 6c20  cases of wilful 
+00002040: 6d69 7363 6f6e 6475 6374 206f 7220 6461  misconduct or da
+00002050: 6d61 6765 7320 6469 7265 6374 6c79 2063  mages directly c
+00002060: 6175 7365 6420 746f 206e 6174 7572 616c  aused to natural
+00002070: 0a70 6572 736f 6e73 2c20 7468 6520 4c69  .persons, the Li
+00002080: 6365 6e73 6f72 2077 696c 6c20 696e 206e  censor will in n
+00002090: 6f20 6576 656e 7420 6265 206c 6961 626c  o event be liabl
+000020a0: 6520 666f 7220 616e 7920 6469 7265 6374  e for any direct
+000020b0: 206f 7220 696e 6469 7265 6374 2c0a 6d61   or indirect,.ma
+000020c0: 7465 7269 616c 206f 7220 6d6f 7261 6c2c  terial or moral,
+000020d0: 2064 616d 6167 6573 206f 6620 616e 7920   damages of any 
+000020e0: 6b69 6e64 2c20 6172 6973 696e 6720 6f75  kind, arising ou
+000020f0: 7420 6f66 2074 6865 204c 6963 656e 6365  t of the Licence
+00002100: 206f 7220 6f66 2074 6865 0a75 7365 206f   or of the.use o
+00002110: 6620 7468 6520 576f 726b 2c20 696e 636c  f the Work, incl
+00002120: 7564 696e 6720 7769 7468 6f75 7420 6c69  uding without li
+00002130: 6d69 7461 7469 6f6e 2c20 6461 6d61 6765  mitation, damage
+00002140: 7320 666f 7220 6c6f 7373 206f 6620 676f  s for loss of go
+00002150: 6f64 7769 6c6c 2c0a 776f 726b 2073 746f  odwill,.work sto
+00002160: 7070 6167 652c 2063 6f6d 7075 7465 7220  ppage, computer 
+00002170: 6661 696c 7572 6520 6f72 206d 616c 6675  failure or malfu
+00002180: 6e63 7469 6f6e 2c20 6c6f 7373 206f 6620  nction, loss of 
+00002190: 6461 7461 206f 7220 616e 7920 636f 6d6d  data or any comm
+000021a0: 6572 6369 616c 0a64 616d 6167 652c 2065  ercial.damage, e
+000021b0: 7665 6e20 6966 2074 6865 204c 6963 656e  ven if the Licen
+000021c0: 736f 7220 6861 7320 6265 656e 2061 6476  sor has been adv
+000021d0: 6973 6564 206f 6620 7468 6520 706f 7373  ised of the poss
+000021e0: 6962 696c 6974 7920 6f66 2073 7563 680a  ibility of such.
+000021f0: 6461 6d61 6765 2e20 486f 7765 7665 722c  damage. However,
+00002200: 2074 6865 204c 6963 656e 736f 7220 7769   the Licensor wi
+00002210: 6c6c 2062 6520 6c69 6162 6c65 2075 6e64  ll be liable und
+00002220: 6572 2073 7461 7475 746f 7279 2070 726f  er statutory pro
+00002230: 6475 6374 206c 6961 6269 6c69 7479 0a6c  duct liability.l
+00002240: 6177 7320 6173 2066 6172 2073 7563 6820  aws as far such 
+00002250: 6c61 7773 2061 7070 6c79 2074 6f20 7468  laws apply to th
+00002260: 6520 576f 726b 2e0a 0a39 2e20 4164 6469  e Work...9. Addi
+00002270: 7469 6f6e 616c 2061 6772 6565 6d65 6e74  tional agreement
+00002280: 730a 0a57 6869 6c65 2064 6973 7472 6962  s..While distrib
+00002290: 7574 696e 6720 7468 6520 576f 726b 2c20  uting the Work, 
+000022a0: 596f 7520 6d61 7920 6368 6f6f 7365 2074  You may choose t
+000022b0: 6f20 636f 6e63 6c75 6465 2061 6e20 6164  o conclude an ad
+000022c0: 6469 7469 6f6e 616c 0a61 6772 6565 6d65  ditional.agreeme
+000022d0: 6e74 2c20 6465 6669 6e69 6e67 206f 626c  nt, defining obl
+000022e0: 6967 6174 696f 6e73 206f 7220 7365 7276  igations or serv
+000022f0: 6963 6573 2063 6f6e 7369 7374 656e 7420  ices consistent 
+00002300: 7769 7468 2074 6869 7320 4c69 6365 6e63  with this Licenc
+00002310: 652e 0a48 6f77 6576 6572 2c20 6966 2061  e..However, if a
+00002320: 6363 6570 7469 6e67 206f 626c 6967 6174  ccepting obligat
+00002330: 696f 6e73 2c20 596f 7520 6d61 7920 6163  ions, You may ac
+00002340: 7420 6f6e 6c79 206f 6e20 796f 7572 206f  t only on your o
+00002350: 776e 2062 6568 616c 6620 616e 6420 6f6e  wn behalf and on
+00002360: 0a79 6f75 7220 736f 6c65 2072 6573 706f  .your sole respo
+00002370: 6e73 6962 696c 6974 792c 206e 6f74 206f  nsibility, not o
+00002380: 6e20 6265 6861 6c66 206f 6620 7468 6520  n behalf of the 
+00002390: 6f72 6967 696e 616c 204c 6963 656e 736f  original Licenso
+000023a0: 7220 6f72 2061 6e79 206f 7468 6572 0a43  r or any other.C
+000023b0: 6f6e 7472 6962 7574 6f72 2c20 616e 6420  ontributor, and 
+000023c0: 6f6e 6c79 2069 6620 596f 7520 6167 7265  only if You agre
+000023d0: 6520 746f 2069 6e64 656d 6e69 6679 2c20  e to indemnify, 
+000023e0: 6465 6665 6e64 2c20 616e 6420 686f 6c64  defend, and hold
+000023f0: 2065 6163 680a 436f 6e74 7269 6275 746f   each.Contributo
+00002400: 7220 6861 726d 6c65 7373 2066 6f72 2061  r harmless for a
+00002410: 6e79 206c 6961 6269 6c69 7479 2069 6e63  ny liability inc
+00002420: 7572 7265 6420 6279 2c20 6f72 2063 6c61  urred by, or cla
+00002430: 696d 7320 6173 7365 7274 6564 2061 6761  ims asserted aga
+00002440: 696e 7374 0a73 7563 6820 436f 6e74 7269  inst.such Contri
+00002450: 6275 746f 7220 6279 2074 6865 2066 6163  butor by the fac
+00002460: 7420 596f 7520 6861 7665 2061 6363 6570  t You have accep
+00002470: 7465 6420 616e 7920 7761 7272 616e 7479  ted any warranty
+00002480: 206f 7220 6164 6469 7469 6f6e 616c 0a6c   or additional.l
+00002490: 6961 6269 6c69 7479 2e0a 0a31 302e 2041  iability...10. A
+000024a0: 6363 6570 7461 6e63 6520 6f66 2074 6865  cceptance of the
+000024b0: 204c 6963 656e 6365 0a0a 5468 6520 7072   Licence..The pr
+000024c0: 6f76 6973 696f 6e73 206f 6620 7468 6973  ovisions of this
+000024d0: 204c 6963 656e 6365 2063 616e 2062 6520   Licence can be 
+000024e0: 6163 6365 7074 6564 2062 7920 636c 6963  accepted by clic
+000024f0: 6b69 6e67 206f 6e20 616e 2069 636f 6e20  king on an icon 
+00002500: e280 9849 0a61 6772 6565 e280 9920 706c  ...I.agree... pl
+00002510: 6163 6564 2075 6e64 6572 2074 6865 2062  aced under the b
+00002520: 6f74 746f 6d20 6f66 2061 2077 696e 646f  ottom of a windo
+00002530: 7720 6469 7370 6c61 7969 6e67 2074 6865  w displaying the
+00002540: 2074 6578 7420 6f66 2074 6869 7320 4c69   text of this Li
+00002550: 6365 6e63 650a 6f72 2062 7920 6166 6669  cence.or by affi
+00002560: 726d 696e 6720 636f 6e73 656e 7420 696e  rming consent in
+00002570: 2061 6e79 206f 7468 6572 2073 696d 696c   any other simil
+00002580: 6172 2077 6179 2c20 696e 2061 6363 6f72  ar way, in accor
+00002590: 6461 6e63 6520 7769 7468 2074 6865 2072  dance with the r
+000025a0: 756c 6573 0a6f 6620 6170 706c 6963 6162  ules.of applicab
+000025b0: 6c65 206c 6177 2e20 436c 6963 6b69 6e67  le law. Clicking
+000025c0: 206f 6e20 7468 6174 2069 636f 6e20 696e   on that icon in
+000025d0: 6469 6361 7465 7320 796f 7572 2063 6c65  dicates your cle
+000025e0: 6172 2061 6e64 2069 7272 6576 6f63 6162  ar and irrevocab
+000025f0: 6c65 0a61 6363 6570 7461 6e63 6520 6f66  le.acceptance of
+00002600: 2074 6869 7320 4c69 6365 6e63 6520 616e   this Licence an
+00002610: 6420 616c 6c20 6f66 2069 7473 2074 6572  d all of its ter
+00002620: 6d73 2061 6e64 2063 6f6e 6469 7469 6f6e  ms and condition
+00002630: 732e 0a0a 5369 6d69 6c61 726c 792c 2079  s...Similarly, y
+00002640: 6f75 2069 7272 6576 6f63 6162 6c79 2061  ou irrevocably a
+00002650: 6363 6570 7420 7468 6973 204c 6963 656e  ccept this Licen
+00002660: 6365 2061 6e64 2061 6c6c 206f 6620 6974  ce and all of it
+00002670: 7320 7465 726d 7320 616e 640a 636f 6e64  s terms and.cond
+00002680: 6974 696f 6e73 2062 7920 6578 6572 6369  itions by exerci
+00002690: 7369 6e67 2061 6e79 2072 6967 6874 7320  sing any rights 
+000026a0: 6772 616e 7465 6420 746f 2059 6f75 2062  granted to You b
+000026b0: 7920 4172 7469 636c 6520 3220 6f66 2074  y Article 2 of t
+000026c0: 6869 730a 4c69 6365 6e63 652c 2073 7563  his.Licence, suc
+000026d0: 6820 6173 2074 6865 2075 7365 206f 6620  h as the use of 
+000026e0: 7468 6520 576f 726b 2c20 7468 6520 6372  the Work, the cr
+000026f0: 6561 7469 6f6e 2062 7920 596f 7520 6f66  eation by You of
+00002700: 2061 2044 6572 6976 6174 6976 6520 576f   a Derivative Wo
+00002710: 726b 0a6f 7220 7468 6520 4469 7374 7269  rk.or the Distri
+00002720: 6275 7469 6f6e 206f 7220 436f 6d6d 756e  bution or Commun
+00002730: 6963 6174 696f 6e20 6279 2059 6f75 206f  ication by You o
+00002740: 6620 7468 6520 576f 726b 206f 7220 636f  f the Work or co
+00002750: 7069 6573 2074 6865 7265 6f66 2e0a 0a31  pies thereof...1
+00002760: 312e 2049 6e66 6f72 6d61 7469 6f6e 2074  1. Information t
+00002770: 6f20 7468 6520 7075 626c 6963 0a0a 496e  o the public..In
+00002780: 2063 6173 6520 6f66 2061 6e79 2044 6973   case of any Dis
+00002790: 7472 6962 7574 696f 6e20 6f72 2043 6f6d  tribution or Com
+000027a0: 6d75 6e69 6361 7469 6f6e 206f 6620 7468  munication of th
+000027b0: 6520 576f 726b 2062 7920 6d65 616e 7320  e Work by means 
+000027c0: 6f66 0a65 6c65 6374 726f 6e69 6320 636f  of.electronic co
+000027d0: 6d6d 756e 6963 6174 696f 6e20 6279 2059  mmunication by Y
+000027e0: 6f75 2028 666f 7220 6578 616d 706c 652c  ou (for example,
+000027f0: 2062 7920 6f66 6665 7269 6e67 2074 6f20   by offering to 
+00002800: 646f 776e 6c6f 6164 2074 6865 2057 6f72  download the Wor
+00002810: 6b0a 6672 6f6d 2061 2072 656d 6f74 6520  k.from a remote 
+00002820: 6c6f 6361 7469 6f6e 2920 7468 6520 6469  location) the di
+00002830: 7374 7269 6275 7469 6f6e 2063 6861 6e6e  stribution chann
+00002840: 656c 206f 7220 6d65 6469 6120 2866 6f72  el or media (for
+00002850: 2065 7861 6d70 6c65 2c20 610a 7765 6273   example, a.webs
+00002860: 6974 6529 206d 7573 7420 6174 206c 6561  ite) must at lea
+00002870: 7374 2070 726f 7669 6465 2074 6f20 7468  st provide to th
+00002880: 6520 7075 626c 6963 2074 6865 2069 6e66  e public the inf
+00002890: 6f72 6d61 7469 6f6e 2072 6571 7565 7374  ormation request
+000028a0: 6564 2062 7920 7468 650a 6170 706c 6963  ed by the.applic
+000028b0: 6162 6c65 206c 6177 2072 6567 6172 6469  able law regardi
+000028c0: 6e67 2074 6865 204c 6963 656e 736f 722c  ng the Licensor,
+000028d0: 2074 6865 204c 6963 656e 6365 2061 6e64   the Licence and
+000028e0: 2074 6865 2077 6179 2069 7420 6d61 7920   the way it may 
+000028f0: 6265 0a61 6363 6573 7369 626c 652c 2063  be.accessible, c
+00002900: 6f6e 636c 7564 6564 2c20 7374 6f72 6564  oncluded, stored
+00002910: 2061 6e64 2072 6570 726f 6475 6365 6420   and reproduced 
+00002920: 6279 2074 6865 204c 6963 656e 7365 652e  by the Licensee.
+00002930: 0a0a 3132 2e20 5465 726d 696e 6174 696f  ..12. Terminatio
+00002940: 6e20 6f66 2074 6865 204c 6963 656e 6365  n of the Licence
+00002950: 0a0a 5468 6520 4c69 6365 6e63 6520 616e  ..The Licence an
+00002960: 6420 7468 6520 7269 6768 7473 2067 7261  d the rights gra
+00002970: 6e74 6564 2068 6572 6575 6e64 6572 2077  nted hereunder w
+00002980: 696c 6c20 7465 726d 696e 6174 6520 6175  ill terminate au
+00002990: 746f 6d61 7469 6361 6c6c 7920 7570 6f6e  tomatically upon
+000029a0: 0a61 6e79 2062 7265 6163 6820 6279 2074  .any breach by t
+000029b0: 6865 204c 6963 656e 7365 6520 6f66 2074  he Licensee of t
+000029c0: 6865 2074 6572 6d73 206f 6620 7468 6520  he terms of the 
+000029d0: 4c69 6365 6e63 652e 0a0a 5375 6368 2061  Licence...Such a
+000029e0: 2074 6572 6d69 6e61 7469 6f6e 2077 696c   termination wil
+000029f0: 6c20 6e6f 7420 7465 726d 696e 6174 6520  l not terminate 
+00002a00: 7468 6520 6c69 6365 6e63 6573 206f 6620  the licences of 
+00002a10: 616e 7920 7065 7273 6f6e 2077 686f 2068  any person who h
+00002a20: 6173 0a72 6563 6569 7665 6420 7468 6520  as.received the 
+00002a30: 576f 726b 2066 726f 6d20 7468 6520 4c69  Work from the Li
+00002a40: 6365 6e73 6565 2075 6e64 6572 2074 6865  censee under the
+00002a50: 204c 6963 656e 6365 2c20 7072 6f76 6964   Licence, provid
+00002a60: 6564 2073 7563 6820 7065 7273 6f6e 730a  ed such persons.
+00002a70: 7265 6d61 696e 2069 6e20 6675 6c6c 2063  remain in full c
+00002a80: 6f6d 706c 6961 6e63 6520 7769 7468 2074  ompliance with t
+00002a90: 6865 204c 6963 656e 6365 2e0a 0a31 332e  he Licence...13.
+00002aa0: 204d 6973 6365 6c6c 616e 656f 7573 0a0a   Miscellaneous..
+00002ab0: 5769 7468 6f75 7420 7072 656a 7564 6963  Without prejudic
+00002ac0: 6520 6f66 2041 7274 6963 6c65 2039 2061  e of Article 9 a
+00002ad0: 626f 7665 2c20 7468 6520 4c69 6365 6e63  bove, the Licenc
+00002ae0: 6520 7265 7072 6573 656e 7473 2074 6865  e represents the
+00002af0: 2063 6f6d 706c 6574 650a 6167 7265 656d   complete.agreem
+00002b00: 656e 7420 6265 7477 6565 6e20 7468 6520  ent between the 
+00002b10: 5061 7274 6965 7320 6173 2074 6f20 7468  Parties as to th
+00002b20: 6520 576f 726b 2e0a 0a49 6620 616e 7920  e Work...If any 
+00002b30: 7072 6f76 6973 696f 6e20 6f66 2074 6865  provision of the
+00002b40: 204c 6963 656e 6365 2069 7320 696e 7661   Licence is inva
+00002b50: 6c69 6420 6f72 2075 6e65 6e66 6f72 6365  lid or unenforce
+00002b60: 6162 6c65 2075 6e64 6572 2061 7070 6c69  able under appli
+00002b70: 6361 626c 650a 6c61 772c 2074 6869 7320  cable.law, this 
+00002b80: 7769 6c6c 206e 6f74 2061 6666 6563 7420  will not affect 
+00002b90: 7468 6520 7661 6c69 6469 7479 206f 7220  the validity or 
+00002ba0: 656e 666f 7263 6561 6269 6c69 7479 206f  enforceability o
+00002bb0: 6620 7468 6520 4c69 6365 6e63 6520 6173  f the Licence as
+00002bc0: 2061 0a77 686f 6c65 2e20 5375 6368 2070   a.whole. Such p
+00002bd0: 726f 7669 7369 6f6e 2077 696c 6c20 6265  rovision will be
+00002be0: 2063 6f6e 7374 7275 6564 206f 7220 7265   construed or re
+00002bf0: 666f 726d 6564 2073 6f20 6173 206e 6563  formed so as nec
+00002c00: 6573 7361 7279 2074 6f20 6d61 6b65 2069  essary to make i
+00002c10: 740a 7661 6c69 6420 616e 6420 656e 666f  t.valid and enfo
+00002c20: 7263 6561 626c 652e 0a0a 5468 6520 4575  rceable...The Eu
+00002c30: 726f 7065 616e 2043 6f6d 6d69 7373 696f  ropean Commissio
+00002c40: 6e20 6d61 7920 7075 626c 6973 6820 6f74  n may publish ot
+00002c50: 6865 7220 6c69 6e67 7569 7374 6963 2076  her linguistic v
+00002c60: 6572 7369 6f6e 7320 6f72 206e 6577 2076  ersions or new v
+00002c70: 6572 7369 6f6e 730a 6f66 2074 6869 7320  ersions.of this 
+00002c80: 4c69 6365 6e63 6520 6f72 2075 7064 6174  Licence or updat
+00002c90: 6564 2076 6572 7369 6f6e 7320 6f66 2074  ed versions of t
+00002ca0: 6865 2041 7070 656e 6469 782c 2073 6f20  he Appendix, so 
+00002cb0: 6661 7220 7468 6973 2069 7320 7265 7175  far this is requ
+00002cc0: 6972 6564 0a61 6e64 2072 6561 736f 6e61  ired.and reasona
+00002cd0: 626c 652c 2077 6974 686f 7574 2072 6564  ble, without red
+00002ce0: 7563 696e 6720 7468 6520 7363 6f70 6520  ucing the scope 
+00002cf0: 6f66 2074 6865 2072 6967 6874 7320 6772  of the rights gr
+00002d00: 616e 7465 6420 6279 2074 6865 0a4c 6963  anted by the.Lic
+00002d10: 656e 6365 2e20 4e65 7720 7665 7273 696f  ence. New versio
+00002d20: 6e73 206f 6620 7468 6520 4c69 6365 6e63  ns of the Licenc
+00002d30: 6520 7769 6c6c 2062 6520 7075 626c 6973  e will be publis
+00002d40: 6865 6420 7769 7468 2061 2075 6e69 7175  hed with a uniqu
+00002d50: 6520 7665 7273 696f 6e0a 6e75 6d62 6572  e version.number
+00002d60: 2e0a 0a41 6c6c 206c 696e 6775 6973 7469  ...All linguisti
+00002d70: 6320 7665 7273 696f 6e73 206f 6620 7468  c versions of th
+00002d80: 6973 204c 6963 656e 6365 2c20 6170 7072  is Licence, appr
+00002d90: 6f76 6564 2062 7920 7468 6520 4575 726f  oved by the Euro
+00002da0: 7065 616e 2043 6f6d 6d69 7373 696f 6e2c  pean Commission,
+00002db0: 0a68 6176 6520 6964 656e 7469 6361 6c20  .have identical 
+00002dc0: 7661 6c75 652e 2050 6172 7469 6573 2063  value. Parties c
+00002dd0: 616e 2074 616b 6520 6164 7661 6e74 6167  an take advantag
+00002de0: 6520 6f66 2074 6865 206c 696e 6775 6973  e of the linguis
+00002df0: 7469 6320 7665 7273 696f 6e20 6f66 0a74  tic version of.t
+00002e00: 6865 6972 2063 686f 6963 652e 0a0a 3134  heir choice...14
+00002e10: 2e20 4a75 7269 7364 6963 7469 6f6e 0a0a  . Jurisdiction..
+00002e20: 5769 7468 6f75 7420 7072 656a 7564 6963  Without prejudic
+00002e30: 6520 746f 2073 7065 6369 6669 6320 6167  e to specific ag
+00002e40: 7265 656d 656e 7420 6265 7477 6565 6e20  reement between 
+00002e50: 7061 7274 6965 732c 0a0a 2d20 616e 7920  parties,..- any 
+00002e60: 6c69 7469 6761 7469 6f6e 2072 6573 756c  litigation resul
+00002e70: 7469 6e67 2066 726f 6d20 7468 6520 696e  ting from the in
+00002e80: 7465 7270 7265 7461 7469 6f6e 206f 6620  terpretation of 
+00002e90: 7468 6973 204c 6963 656e 7365 2c20 6172  this License, ar
+00002ea0: 6973 696e 670a 2020 6265 7477 6565 6e20  ising.  between 
+00002eb0: 7468 6520 4575 726f 7065 616e 2055 6e69  the European Uni
+00002ec0: 6f6e 2069 6e73 7469 7475 7469 6f6e 732c  on institutions,
+00002ed0: 2062 6f64 6965 732c 206f 6666 6963 6573   bodies, offices
+00002ee0: 206f 7220 6167 656e 6369 6573 2c20 6173   or agencies, as
+00002ef0: 2061 0a20 204c 6963 656e 736f 722c 2061   a.  Licensor, a
+00002f00: 6e64 2061 6e79 204c 6963 656e 7365 652c  nd any Licensee,
+00002f10: 2077 696c 6c20 6265 2073 7562 6a65 6374   will be subject
+00002f20: 2074 6f20 7468 6520 6a75 7269 7364 6963   to the jurisdic
+00002f30: 7469 6f6e 206f 6620 7468 6520 436f 7572  tion of the Cour
+00002f40: 740a 2020 6f66 204a 7573 7469 6365 206f  t.  of Justice o
+00002f50: 6620 7468 6520 4575 726f 7065 616e 2055  f the European U
+00002f60: 6e69 6f6e 2c20 6173 206c 6169 6420 646f  nion, as laid do
+00002f70: 776e 2069 6e20 6172 7469 636c 6520 3237  wn in article 27
+00002f80: 3220 6f66 2074 6865 2054 7265 6174 790a  2 of the Treaty.
+00002f90: 2020 6f6e 2074 6865 2046 756e 6374 696f    on the Functio
+00002fa0: 6e69 6e67 206f 6620 7468 6520 4575 726f  ning of the Euro
+00002fb0: 7065 616e 2055 6e69 6f6e 2c0a 0a2d 2061  pean Union,..- a
+00002fc0: 6e79 206c 6974 6967 6174 696f 6e20 6172  ny litigation ar
+00002fd0: 6973 696e 6720 6265 7477 6565 6e20 6f74  ising between ot
+00002fe0: 6865 7220 7061 7274 6965 7320 616e 6420  her parties and 
+00002ff0: 7265 7375 6c74 696e 6720 6672 6f6d 2074  resulting from t
+00003000: 6865 0a20 2069 6e74 6572 7072 6574 6174  he.  interpretat
+00003010: 696f 6e20 6f66 2074 6869 7320 4c69 6365  ion of this Lice
+00003020: 6e73 652c 2077 696c 6c20 6265 2073 7562  nse, will be sub
+00003030: 6a65 6374 2074 6f20 7468 6520 6578 636c  ject to the excl
+00003040: 7573 6976 650a 2020 6a75 7269 7364 6963  usive.  jurisdic
+00003050: 7469 6f6e 206f 6620 7468 6520 636f 6d70  tion of the comp
+00003060: 6574 656e 7420 636f 7572 7420 7768 6572  etent court wher
+00003070: 6520 7468 6520 4c69 6365 6e73 6f72 2072  e the Licensor r
+00003080: 6573 6964 6573 206f 7220 636f 6e64 7563  esides or conduc
+00003090: 7473 0a20 2069 7473 2070 7269 6d61 7279  ts.  its primary
+000030a0: 2062 7573 696e 6573 732e 0a0a 3135 2e20   business...15. 
+000030b0: 4170 706c 6963 6162 6c65 204c 6177 0a0a  Applicable Law..
+000030c0: 5769 7468 6f75 7420 7072 656a 7564 6963  Without prejudic
+000030d0: 6520 746f 2073 7065 6369 6669 6320 6167  e to specific ag
+000030e0: 7265 656d 656e 7420 6265 7477 6565 6e20  reement between 
+000030f0: 7061 7274 6965 732c 0a0a 2d20 7468 6973  parties,..- this
+00003100: 204c 6963 656e 6365 2073 6861 6c6c 2062   Licence shall b
+00003110: 6520 676f 7665 726e 6564 2062 7920 7468  e governed by th
+00003120: 6520 6c61 7720 6f66 2074 6865 2045 7572  e law of the Eur
+00003130: 6f70 6561 6e20 556e 696f 6e20 4d65 6d62  opean Union Memb
+00003140: 6572 2053 7461 7465 0a20 2077 6865 7265  er State.  where
+00003150: 2074 6865 204c 6963 656e 736f 7220 6861   the Licensor ha
+00003160: 7320 6869 7320 7365 6174 2c20 7265 7369  s his seat, resi
+00003170: 6465 7320 6f72 2068 6173 2068 6973 2072  des or has his r
+00003180: 6567 6973 7465 7265 6420 6f66 6669 6365  egistered office
+00003190: 2c0a 0a2d 2074 6869 7320 6c69 6365 6e63  ,..- this licenc
+000031a0: 6520 7368 616c 6c20 6265 2067 6f76 6572  e shall be gover
+000031b0: 6e65 6420 6279 2042 656c 6769 616e 206c  ned by Belgian l
+000031c0: 6177 2069 6620 7468 6520 4c69 6365 6e73  aw if the Licens
+000031d0: 6f72 2068 6173 206e 6f20 7365 6174 2c0a  or has no seat,.
+000031e0: 2020 7265 7369 6465 6e63 6520 6f72 2072    residence or r
+000031f0: 6567 6973 7465 7265 6420 6f66 6669 6365  egistered office
+00003200: 2069 6e73 6964 6520 6120 4575 726f 7065   inside a Europe
+00003210: 616e 2055 6e69 6f6e 204d 656d 6265 7220  an Union Member 
+00003220: 5374 6174 652e 0a0a 4170 7065 6e64 6978  State...Appendix
+00003230: 0a0a e280 9843 6f6d 7061 7469 626c 6520  .....Compatible 
+00003240: 4c69 6365 6e63 6573 e280 9920 6163 636f  Licences... acco
+00003250: 7264 696e 6720 746f 2041 7274 6963 6c65  rding to Article
+00003260: 2035 2045 5550 4c20 6172 653a 0a0a 2d20   5 EUPL are:..- 
+00003270: 474e 5520 4765 6e65 7261 6c20 5075 626c  GNU General Publ
+00003280: 6963 204c 6963 656e 7365 2028 4750 4c29  ic License (GPL)
+00003290: 2076 2e20 322c 2076 2e20 330a 2d20 474e   v. 2, v. 3.- GN
+000032a0: 5520 4166 6665 726f 2047 656e 6572 616c  U Affero General
+000032b0: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
+000032c0: 2841 4750 4c29 2076 2e20 330a 2d20 4f70  (AGPL) v. 3.- Op
+000032d0: 656e 2053 6f66 7477 6172 6520 4c69 6365  en Software Lice
+000032e0: 6e73 6520 284f 534c 2920 762e 2032 2e31  nse (OSL) v. 2.1
+000032f0: 2c20 762e 2033 2e30 0a2d 2045 636c 6970  , v. 3.0.- Eclip
+00003300: 7365 2050 7562 6c69 6320 4c69 6365 6e73  se Public Licens
+00003310: 6520 2845 504c 2920 762e 2031 2e30 0a2d  e (EPL) v. 1.0.-
+00003320: 2043 6543 494c 4c20 762e 2032 2e30 2c20   CeCILL v. 2.0, 
+00003330: 762e 2032 2e31 0a2d 204d 6f7a 696c 6c61  v. 2.1.- Mozilla
+00003340: 2050 7562 6c69 6320 4c69 6365 6e63 6520   Public Licence 
+00003350: 284d 504c 2920 762e 2032 0a2d 2047 4e55  (MPL) v. 2.- GNU
+00003360: 204c 6573 7365 7220 4765 6e65 7261 6c20   Lesser General 
+00003370: 5075 626c 6963 204c 6963 656e 6365 2028  Public Licence (
+00003380: 4c47 504c 2920 762e 2032 2e31 2c20 762e  LGPL) v. 2.1, v.
+00003390: 2033 0a2d 2043 7265 6174 6976 6520 436f   3.- Creative Co
+000033a0: 6d6d 6f6e 7320 4174 7472 6962 7574 696f  mmons Attributio
+000033b0: 6e2d 5368 6172 6541 6c69 6b65 2076 2e20  n-ShareAlike v. 
+000033c0: 332e 3020 556e 706f 7274 6564 2028 4343  3.0 Unported (CC
+000033d0: 2042 592d 5341 2033 2e30 2920 666f 720a   BY-SA 3.0) for.
+000033e0: 2020 776f 726b 7320 6f74 6865 7220 7468    works other th
+000033f0: 616e 2073 6f66 7477 6172 650a 2d20 4575  an software.- Eu
+00003400: 726f 7065 616e 2055 6e69 6f6e 2050 7562  ropean Union Pub
+00003410: 6c69 6320 4c69 6365 6e63 6520 2845 5550  lic Licence (EUP
+00003420: 4c29 2076 2e20 312e 312c 2076 2e20 312e  L) v. 1.1, v. 1.
+00003430: 320a 2d20 5175 c3a9 6265 6320 4672 6565  2.- Qu..bec Free
+00003440: 2061 6e64 204f 7065 6e2d 536f 7572 6365   and Open-Source
+00003450: 204c 6963 656e 6365 20e2 8094 2052 6563   Licence ... Rec
+00003460: 6970 726f 6369 7479 2028 4c69 4c69 512d  iprocity (LiLiQ-
+00003470: 5229 206f 7220 5374 726f 6e67 0a20 2052  R) or Strong.  R
+00003480: 6563 6970 726f 6369 7479 2028 4c69 4c69  eciprocity (LiLi
+00003490: 512d 522b 292e 0a0a 5468 6520 4575 726f  Q-R+)...The Euro
+000034a0: 7065 616e 2043 6f6d 6d69 7373 696f 6e20  pean Commission 
+000034b0: 6d61 7920 7570 6461 7465 2074 6869 7320  may update this 
+000034c0: 4170 7065 6e64 6978 2074 6f20 6c61 7465  Appendix to late
+000034d0: 7220 7665 7273 696f 6e73 206f 6620 7468  r versions of th
+000034e0: 650a 6162 6f76 6520 6c69 6365 6e63 6573  e.above licences
+000034f0: 2077 6974 686f 7574 2070 726f 6475 6369   without produci
+00003500: 6e67 2061 206e 6577 2076 6572 7369 6f6e  ng a new version
+00003510: 206f 6620 7468 6520 4555 504c 2c20 6173   of the EUPL, as
+00003520: 206c 6f6e 6720 6173 2074 6865 790a 7072   long as they.pr
+00003530: 6f76 6964 6520 7468 6520 7269 6768 7473  ovide the rights
+00003540: 2067 7261 6e74 6564 2069 6e20 4172 7469   granted in Arti
+00003550: 636c 6520 3220 6f66 2074 6869 7320 4c69  cle 2 of this Li
+00003560: 6365 6e63 6520 616e 6420 7072 6f74 6563  cence and protec
+00003570: 7420 7468 650a 636f 7665 7265 6420 536f  t the.covered So
+00003580: 7572 6365 2043 6f64 6520 6672 6f6d 2065  urce Code from e
+00003590: 7863 6c75 7369 7665 2061 7070 726f 7072  xclusive appropr
+000035a0: 6961 7469 6f6e 2e0a 0a41 6c6c 206f 7468  iation...All oth
+000035b0: 6572 2063 6861 6e67 6573 206f 7220 6164  er changes or ad
+000035c0: 6469 7469 6f6e 7320 746f 2074 6869 7320  ditions to this 
+000035d0: 4170 7065 6e64 6978 2072 6571 7569 7265  Appendix require
+000035e0: 2074 6865 2070 726f 6475 6374 696f 6e20   the production 
+000035f0: 6f66 2061 0a6e 6577 2045 5550 4c20 7665  of a.new EUPL ve
+00003600: 7273 696f 6e2e 0a                        rsion..
```

### Comparing `fastapi_xroad_soap-0.2.2/README.md` & `fastapi_xroad_soap-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # FastAPI X-Road SOAP
 
+<img src="https://raw.githubusercontent.com/rik-ee/fastapi-xroad-soap/main/media/fxs_logo.jpg" alt="Logo" width="500">
+
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fastapi-xroad-soap)](https://pypi.org/project/fastapi-xroad-soap/)
 [![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/rik-ee/fastapi-xroad-soap/build-publish.yaml)](https://github.com/rik-ee/fastapi-xroad-soap/actions/workflows/build-publish.yaml)
 [![codecov](https://codecov.io/gh/rik-ee/fastapi-xroad-soap/graph/badge.svg?token=KB58NGDC1N)](https://codecov.io/gh/rik-ee/fastapi-xroad-soap)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/fastapi-xroad-soap)](https://pypistats.org/packages/fastapi-xroad-soap)
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/__init__.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/elements.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/elements.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 #   Copyright (c) 2024, Centre of Registers and Information Systems
 #
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
-from .internal.elements import (
+from .internal.elements.models import (
 	Boolean,
 	Date,
-	Time,
 	DateTime,
 	Float,
 	Integer,
-	String,
 	NetRes,
-	SwaRef
+	String,
+	SwaRef,
+	Time
 )
 
 
 __all__ = [
 	"Boolean",
 	"Date",
-	"Time",
 	"DateTime",
 	"Float",
 	"Integer",
-	"String",
 	"NetRes",
-	"SwaRef"
+	"String",
+	"SwaRef",
+	"Time"
 ]
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/base/__init__.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/base/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 #   Copyright (c) 2024, Centre of Registers and Information Systems
 #
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
-from .body import MessageBody, MessageBodyType
+from .body import NestedModels, MessageBody, MessageBodyType
 from .meta import ElementSpecMeta, CompositeMeta
 from .spec import BaseElementSpec
 
 
 __all__ = [
+	"NestedModels",
 	"MessageBody",
 	"MessageBodyType",
 	"BaseElementSpec",
 	"ElementSpecMeta",
 	"CompositeMeta"
 ]
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/base/body.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/base/body.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,34 +7,58 @@
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 from __future__ import annotations
 import typing as t
 from pydantic_xml import model
+from pydantic.fields import ModelPrivateAttr
 from pydantic import (
 	PrivateAttr,
 	ValidationInfo,
 	model_validator
 )
 from ..constants import A8nType
 from .meta import CompositeMeta
 
 try:
 	from .spec import BaseElementSpec
 except ImportError:  # pragma: no cover
 	BaseElementSpec: t.TypeAlias = t.Any
 
 
-__all__ = ["MessageBody", "MessageBodyType"]
+__all__ = ["NestedModels", "MessageBody", "MessageBodyType"]
+
+
+NestedModels = t.List[t.Tuple[
+	t.Type["MessageBody"],
+	t.List[t.Type["MessageBody"]]
+]]
 
 
 class MessageBody(model.BaseXmlModel, metaclass=CompositeMeta, search_mode='unordered', skip_empty=True):
 	_element_specs: t.Dict[str, BaseElementSpec] = PrivateAttr(default_factory=dict)
 
+	@classmethod
+	def model_specs(cls) -> t.Dict[str, BaseElementSpec]:
+		privates = getattr(cls, "__private_attributes__", {})
+		attr: t.Union[ModelPrivateAttr, None] = privates.get("_element_specs")
+		return attr.get_default() if attr is not None else dict()
+
+	@classmethod
+	def nested_models(cls) -> NestedModels:
+		models, children = [], []
+		a8ns = getattr(cls, '__annotations__', {})
+		for key, value in a8ns.items():
+			if type(value) is CompositeMeta:
+				models.extend(value.get_nested_models())
+				children.append(value)
+		models.append((cls, children))
+		return models
+
 	@staticmethod
 	def _validate_list(attr: str, data: t.List[MessageBody], spec: BaseElementSpec):
 		if not isinstance(data, list):
 			raise ValueError(
 				f"expected attribute '{attr}' value to be a list, "
 				f"but received '{type(data).__name__}' instead."
 			)
@@ -62,36 +86,30 @@
 	@classmethod
 	def _validate_before(cls, data: t.Dict[str, t.Any], info: ValidationInfo) -> t.Any:
 		# Used for validating model instantiation in user code
 		is_incoming_request = (info.context or {}).get("deserializing", False)
 		if is_incoming_request or not isinstance(data, dict):
 			return data
 
-		private_attrs = getattr(cls, "__private_attributes__")
-		class_specs = private_attrs.get("_element_specs").get_default()
-
-		for attr, spec in class_specs.items():
+		for attr, spec in cls.model_specs().items():
 			expected = spec.internal_type or spec.element_type
 			value = data.get(attr)
 
 			if spec.a8n_type == A8nType.LIST:
 				cls._validate_list(attr, value, spec)
 				spec.init_instantiated_data(value)
 				continue
 			elif spec.a8n_type == A8nType.OPT and value is None:
 				data[attr] = []
 				continue
 			elif spec.a8n_type == A8nType.MAND and attr not in data:
 				raise ValueError(f"argument '{attr}' is missing")
 			elif not isinstance(value, expected):
 				arg_type = type(value).__name__
-				raise ValueError(
-					f"unexpected type '{arg_type}' "
-					f"for argument '{attr}'"
-				)
+				raise ValueError(f"unexpected type '{arg_type}' for argument '{attr}'")
 			data[attr] = [value]
 			spec.init_instantiated_data(data[attr])
 		return data
 
 	@model_validator(mode="after")
 	def _validate_after(self, info: ValidationInfo) -> MessageBody:
 		# Used for validating deserialized incoming requests
@@ -108,15 +126,15 @@
 			if spec is None:
 				continue
 			elif not isinstance(value, list):
 				value = [value]
 			count = len(value)
 
 			if count > 1 and spec.a8n_type in [A8nType.MAND, A8nType.OPT]:
-				raise ValueError(f"only one {spec.tag} element is allowed $$Count: {count}$$")
+				raise ValueError(f"only one {spec.tag} element is allowed, got {count}")
 			elif count == 0 and spec.a8n_type == A8nType.MAND:
 				raise ValueError(f"must provide at least one {spec.tag} element")
 			elif spec.a8n_type == A8nType.LIST:
 				self._validate_list(attr, value, spec)
 				spec.init_deserialized_data(value)
 				continue
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/base/meta.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/base/meta.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/constants.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,16 +24,15 @@
 ENV_NSMAP = {"soapenv": "http://schemas.xmlsoap.org/soap/envelope/"}
 XRO_NSMAP = {"xro": "http://x-road.eu/xsd/xroad.xsd"}
 IDEN_NSMAP = {"iden": "http://x-road.eu/xsd/identifiers"}
 HEADER_NSMAP = {**ENV_NSMAP, **XRO_NSMAP, **IDEN_NSMAP}
 WSDL_NSMAP = {
     "wsdl": "http://schemas.xmlsoap.org/wsdl/",
     "soap": "http://schemas.xmlsoap.org/wsdl/soap/",
-    "enc": "http://schemas.xmlsoap.org/soap/encoding/",
-    "wsi": "http://ws-i.org/profiles/basic/1.1/xsd/",
+    "wsi": "http://ws-i.org/profiles/basic/1.1/xsd",
     "xsd": "http://www.w3.org/2001/XMLSchema",
     **XRO_NSMAP
 }
 
 
 class A8nType(Enum):
     LIST = "list"
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/elements/__init__.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 from .string import StringSpec, String
 from .netres import NetResSpec, NetRes
 from .swaref import (
 	SwaRefFile,
 	SwaRefInternal,
 	SwaRefSpec,
 	SwaRefElement,
-	SwaRef
+	SwaRef,
+	SwaRefUtils
 )
 
 
 __all__ = [
 	"BooleanSpec", "Boolean",
 	"DateSpec", "Date",
 	"DateTimeSpec", "DateTime",
@@ -34,9 +35,10 @@
 	"IntegerSpec", "Integer",
 	"StringSpec", "String",
 	"NetResSpec", "NetRes",
 	"SwaRefFile",
 	"SwaRefInternal",
 	"SwaRefSpec",
 	"SwaRefElement",
-	"SwaRef"
+	"SwaRef",
+	"SwaRefUtils"
 ]
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/elements/date.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/time.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,38 +6,39 @@
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 import typing as t
 from enum import Enum
-from datetime import date
-from .common import CommonSpecTypeA
+from datetime import time
+from ..numeric_type_spec import NumericTypeSpec
 
 
-__all__ = ["DateSpec", "Date"]
+__all__ = ["TimeSpec", "Time"]
 
 
-class DateSpec(CommonSpecTypeA):
+class TimeSpec(NumericTypeSpec):
 	def __init__(self, **kwargs) -> None:
-		super().__init__(
-			element_type=date,
-			**kwargs
-		)
+		super().__init__(element_type=time, **kwargs)
 
+	@property
+	def default_wsdl_type_name(self) -> str:
+		return "time"
 
-class Date:
+
+class Time:
 	def __new__(
 			cls,
 			*,
 			tag: t.Optional[str] = None,
 			ns: t.Optional[str] = None,
 			nsmap: t.Optional[t.Dict[str, str]] = None,
 			min_occurs: int = None,
 			max_occurs: t.Union[int, t.Literal["unbounded"]] = None,
-			min_value: t.Optional[date] = None,
-			max_value: t.Optional[date] = None,
+			min_value: t.Optional[time] = None,
+			max_value: t.Optional[time] = None,
 			enumerations: t.Optional[t.Type[Enum]] = None,
 			pattern: t.Optional[str] = None
-	) -> t.Union[date, t.List[date]]:
+	) -> time:
 		kwargs = {k: v for k, v in locals().items() if v != cls}
-		return t.cast(date, DateSpec(**kwargs))
+		return t.cast(time, TimeSpec(**kwargs))
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/elements/datetime.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/datetime.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 import typing as t
 from enum import Enum
 from datetime import datetime
-from .common import CommonSpecTypeA
+from ..numeric_type_spec import NumericTypeSpec
 
 
 __all__ = ["DateTimeSpec", "DateTime"]
 
 
-class DateTimeSpec(CommonSpecTypeA):
+class DateTimeSpec(NumericTypeSpec):
 	def __init__(self, **kwargs) -> None:
-		super().__init__(
-			element_type=datetime,
-			**kwargs
-		)
+		super().__init__(element_type=datetime, **kwargs)
+
+	@property
+	def default_wsdl_type_name(self) -> str:
+		return "dateTime"
 
 
 class DateTime:
 	def __new__(
 			cls,
 			*,
 			tag: t.Optional[str] = None,
@@ -34,10 +35,10 @@
 			nsmap: t.Optional[t.Dict[str, str]] = None,
 			min_occurs: int = None,
 			max_occurs: t.Union[int, t.Literal["unbounded"]] = None,
 			min_value: t.Optional[datetime] = None,
 			max_value: t.Optional[datetime] = None,
 			enumerations: t.Optional[t.Type[Enum]] = None,
 			pattern: t.Optional[str] = None
-	) -> t.Union[datetime, t.List[datetime]]:
+	) -> datetime:
 		kwargs = {k: v for k, v in locals().items() if v != cls}
 		return t.cast(datetime, DateTimeSpec(**kwargs))
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/elements/float.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/float.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,26 +6,27 @@
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 import typing as t
 from enum import Enum
-from .common import CommonSpecTypeA
+from ..numeric_type_spec import NumericTypeSpec
 
 
 __all__ = ["FloatSpec", "Float"]
 
 
-class FloatSpec(CommonSpecTypeA):
+class FloatSpec(NumericTypeSpec):
 	def __init__(self, **kwargs) -> None:
-		super().__init__(
-			element_type=float,
-			**kwargs
-		)
+		super().__init__(element_type=float, **kwargs)
+
+	@property
+	def default_wsdl_type_name(self) -> str:
+		return "float"
 
 
 class Float:
 	def __new__(
 			cls,
 			*,
 			tag: t.Optional[str] = None,
@@ -33,10 +34,10 @@
 			nsmap: t.Optional[t.Dict[str, str]] = None,
 			min_occurs: int = None,
 			max_occurs: t.Union[int, t.Literal["unbounded"]] = None,
 			min_value: t.Optional[float] = None,
 			max_value: t.Optional[float] = None,
 			enumerations: t.Optional[t.Type[Enum]] = None,
 			pattern: t.Optional[str] = None
-	) -> t.Union[float, t.List[float]]:
+	) -> float:
 		kwargs = {k: v for k, v in locals().items() if v != cls}
 		return t.cast(float, FloatSpec(**kwargs))
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/elements/integer.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/integer.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,28 +6,27 @@
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 import typing as t
 from enum import Enum
-from .common import CommonSpecTypeA
-from .validators import NumberValidators
+from ..numeric_type_spec import NumericTypeSpec
 
 
 __all__ = ["IntegerSpec", "Integer"]
 
 
-class IntegerSpec(CommonSpecTypeA, NumberValidators):
+class IntegerSpec(NumericTypeSpec):
 	def __init__(self, **kwargs) -> None:
-		self.total_digits = kwargs.pop("total_digits")
-		super().__init__(
-			element_type=int,
-			**kwargs
-		)
+		super().__init__(element_type=int, **kwargs)
+
+	@property
+	def default_wsdl_type_name(self) -> str:
+		return "integer"
 
 
 class Integer:
 	def __new__(
 			cls,
 			*,
 			tag: t.Optional[str] = None,
@@ -36,10 +35,10 @@
 			min_occurs: int = None,
 			max_occurs: t.Union[int, t.Literal["unbounded"]] = None,
 			min_value: t.Optional[int] = None,
 			max_value: t.Optional[int] = None,
 			total_digits: t.Optional[int] = None,
 			enumerations: t.Optional[t.Type[Enum]] = None,
 			pattern: t.Optional[str] = None
-	) -> t.Union[int, t.List[int]]:
+	) -> int:
 		kwargs = {k: v for k, v in locals().items() if v != cls}
 		return t.cast(int, IntegerSpec(**kwargs))
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/elements/netres.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/netres.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 import typing as t
 from enum import Enum
 from pydantic import AnyUrl
-from .common import CommonSpecTypeB
+from ..string_type_spec import StringTypeSpec
 
 
 __all__ = ["NetResSpec", "NetRes"]
 
 
-class NetResSpec(CommonSpecTypeB):
+class NetResSpec(StringTypeSpec):
 	def __init__(self, **kwargs) -> None:
-		super().__init__(
-			element_type=AnyUrl,
-			**kwargs
-		)
+		super().__init__(element_type=AnyUrl, **kwargs)
+
+	@property
+	def default_wsdl_type_name(self) -> str:
+		return "anyURI"
 
 
 class NetRes:
 	def __new__(
 			cls,
 			*,
 			tag: t.Optional[str] = None,
@@ -35,10 +36,10 @@
 			min_occurs: int = None,
 			max_occurs: t.Union[int, t.Literal["unbounded"]] = None,
 			length: t.Optional[int] = None,
 			min_length: t.Optional[int] = None,
 			max_length: t.Optional[int] = None,
 			enumerations: t.Optional[t.Type[Enum]] = None,
 			pattern: t.Optional[str] = None
-	) -> t.Union[AnyUrl, t.List[AnyUrl]]:
+	) -> AnyUrl:
 		kwargs = {k: v for k, v in locals().items() if v != cls}
 		return t.cast(AnyUrl, NetResSpec(**kwargs))
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/elements/string.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/string.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,26 +6,27 @@
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 import typing as t
 from enum import Enum
-from .common import CommonSpecTypeB
+from ..string_type_spec import StringTypeSpec
 
 
 __all__ = ["StringSpec", "String"]
 
 
-class StringSpec(CommonSpecTypeB):
+class StringSpec(StringTypeSpec):
 	def __init__(self, **kwargs) -> None:
-		super().__init__(
-			element_type=str,
-			**kwargs
-		)
+		super().__init__(element_type=str, **kwargs)
+
+	@property
+	def default_wsdl_type_name(self) -> str:
+		return "string"
 
 
 class String:
 	def __new__(
 			cls,
 			*,
 			tag: t.Optional[str] = None,
@@ -35,10 +36,10 @@
 			max_occurs: t.Union[int, t.Literal["unbounded"]] = None,
 			length: t.Optional[int] = None,
 			min_length: t.Optional[int] = None,
 			max_length: t.Optional[int] = None,
 			enumerations: t.Optional[t.Type[Enum]] = None,
 			pattern: t.Optional[str] = None,
 			whitespace: t.Literal["preserve", "replace", "collapse"] = "preserve"
-	) -> t.Union[str, t.List[str]]:
+	) -> str:
 		kwargs = {k: v for k, v in locals().items() if v != cls}
 		return t.cast(str, StringSpec(**kwargs))
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/elements/swaref.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/swaref.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,36 +8,42 @@
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 from __future__ import annotations
 import base64
 import hashlib
 import typing as t
-from pydantic import Field
-from ..base import BaseElementSpec, MessageBody
-from ..storage import GlobalWeakStorage
-from ..multipart import DecodedBodyPart
-from ..file_size import FileSize
-from .. import utils
+from pydantic.fields import Field
+from fastapi_xroad_soap.internal import utils
+from fastapi_xroad_soap.internal.storage import GlobalWeakStorage
+from fastapi_xroad_soap.internal.multipart import DecodedBodyPart
+from fastapi_xroad_soap.internal.file_size import FileSize
+from fastapi_xroad_soap.internal.base import (
+	BaseElementSpec,
+	CompositeMeta,
+	MessageBody
+)
 
 
 __all__ = [
 	"SwaRefFile",
 	"SwaRefInternal",
 	"SwaRefSpec",
 	"SwaRefElement",
-	"SwaRef"
+	"SwaRef",
+	"SwaRefUtils"
 ]
 
 
 _NSMap = t.Optional[t.Dict[str, str]]
 _FileType = t.Union[DecodedBodyPart, None]
 _FileSizeType = t.Union[FileSize, None]
 _Filetypes = t.Union[t.List[str], t.Literal["all"]]
 _HashFuncType = t.Literal["sha256", "sha512", "sha3_256", "sha3_384", "sha3_512"]
+_SwaRefTypes = t.Tuple[t.List["SwaRefSpec"], t.List["SwaRefFile"]]
 
 
 class SwaRefFile(MessageBody):
 	name: str = Field(exclude=True, default='')
 	size: int = Field(exclude=True, default=0)
 	digest: str = Field(exclude=True, default='')
 	mimetype: str = Field(exclude=True, default='')
@@ -81,37 +87,46 @@
 		self.hash_func = kwargs.pop("hash_func")
 		super().__init__(
 			element_type=SwaRefFile,
 			internal_type=SwaRefInternal,
 			**kwargs
 		)
 
+	@property
+	def has_constraints(self) -> bool:
+		return False
+
+	def wsdl_type_name(self, *, with_tns: bool = False) -> str:
+		return "wsi:swaRef"
+
 	def digest(self, content: bytes) -> str:
 		hash_func = getattr(hashlib, self.hash_func)
 		digest = hash_func(content).digest()
 		name = self.hash_func.replace('_', '-')
 		b64_hash = base64.b64encode(digest).decode()
 		return f"{name}={b64_hash}"
 
 	def validate_file(self, name: str, size: int, content_id: str = None) -> None:
-		extract = '' if content_id is None else f"$${content_id}$$"
+		extract = '' if content_id is None else f"$$Content-ID: {content_id}$$"
 		if '.' not in name:
-			raise ValueError(f"invalid file name: {name}")
-		if self.allowed_filetypes != "all":
+			raise ValueError(f"invalid file name $${name}$$")
+		aft = self.allowed_filetypes
+		if aft != "all" and isinstance(aft, list):
 			file_ext = '.' + name.split('.')[-1]
 			if file_ext not in self.allowed_filetypes:
 				raise ValueError(
-					f"file type not allowed: {file_ext} "
-					f"(allowed: {self.allowed_filetypes}){extract}"
+					f"file type '{file_ext}' not in allowed "
+					f"filetypes {self.allowed_filetypes}{extract}"
 				)
-		if self.max_filesize and size > self.max_filesize.value:
-			size_str = FileSize.bytes_to_iec_str(size)
+		mfs = self.max_filesize
+		if isinstance(mfs, FileSize) and size > mfs.value:
+			input_size = FileSize.bytes_to_iec_str(size)
 			raise ValueError(
-				f"file size too large: {size_str} "
-				f"(max: {self.max_filesize}){extract}"
+				f"file size {input_size} larger than "
+				f"allowed max size {mfs}{extract}"
 			)
 
 	def init_instantiated_data(self, data: t.List[SwaRefInternal]) -> t.List[SwaRefInternal]:
 		for obj in data:
 			obj.size = len(obj.content)
 			self.validate_file(obj.name, obj.size)
 
@@ -153,21 +168,81 @@
 			ns: t.Optional[str] = None,
 			nsmap: _NSMap = None,
 			min_occurs: int = None,
 			max_occurs: t.Union[int, t.Literal["unbounded"]] = None,
 			allowed_filetypes: _Filetypes = "all",
 			max_filesize: _FileSizeType = None,
 			hash_func: _HashFuncType = "sha3_512"
-	) -> t.Union[SwaRefFile, t.List[SwaRefFile]]:
+	) -> SwaRefFile:
 		kwargs = {k: v for k, v in locals().items() if v != cls}
 		return t.cast(SwaRefFile, SwaRefSpec(**kwargs))
 
 
 class SwaRef:
 	File: t.Type[SwaRefFile] = SwaRefFile
 	Element: t.Type[SwaRefElement] = SwaRefElement
 
 	def __init__(self):
 		raise NotImplementedError(
 			"Cannot directly instantiate SwaRef, you must "
 			"instantiate one of its attribute classes."
 		)
+
+
+class SwaRefUtils:
+	@classmethod
+	def contains_swa_ref_specs(cls, content_cls: t.Type[MessageBody]) -> bool:
+		# print(type(content_cls))
+		has_swa_ref = False
+
+		# Define recursion behavior
+		fields = getattr(content_cls, "model_fields", {})
+		for sub_content_cls in fields.values():
+			res = cls.contains_swa_ref_specs(sub_content_cls)
+			has_swa_ref |= res
+
+		# Check private attributes for SwaRef specs
+		if type(content_cls) is not CompositeMeta:
+			return has_swa_ref
+		specs = content_cls.model_specs()
+		for spec in specs.values():
+			if type(spec).__name__ == "SwaRefSpec":
+				has_swa_ref |= True
+		return has_swa_ref
+
+	@classmethod
+	def gather_specs_and_files(cls, content: MessageBody) -> _SwaRefTypes:
+		specs, files = [], []
+		if not isinstance(content, MessageBody):
+			return specs, files
+
+		# Define recursion behavior
+		for sub_content in vars(content).values():
+			if isinstance(sub_content, MessageBody):
+				_specs, _files = cls.gather_specs_and_files(sub_content)
+				for a, b in [(specs, _specs), (files, _files)]:
+					a.extend(b)
+
+		# Gather specs and files from content
+		cls._add_specs_and_files(specs, files, content)
+		return specs, files
+
+	@staticmethod
+	def _add_specs_and_files(
+			specs: t.List[SwaRefSpec],
+			files: t.List[SwaRefFile],
+			content: MessageBody
+	) -> None:
+		_specs = getattr(content, "_element_specs", None)
+		if _specs is None:
+			return
+		for attr, spec in _specs.items():
+			if not isinstance(spec, SwaRefSpec):
+				continue
+			specs.append(spec)
+			obj = getattr(content, attr)
+			if isinstance(obj, SwaRefFile):
+				files.append(obj)
+			elif isinstance(obj, list):
+				for item in obj:
+					if isinstance(item, SwaRefFile):
+						files.append(item)
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/elements/time.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/models/boolean.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,39 +5,43 @@
 #
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 import typing as t
-from enum import Enum
-from datetime import time
-from .common import CommonSpecTypeA
+from fastapi_xroad_soap.internal.base import BaseElementSpec
 
 
-__all__ = ["TimeSpec", "Time"]
+__all__ = ["BooleanSpec", "Boolean"]
 
 
-class TimeSpec(CommonSpecTypeA):
+class BooleanSpec(BaseElementSpec):
 	def __init__(self, **kwargs) -> None:
-		super().__init__(
-			element_type=time,
-			**kwargs
-		)
+		super().__init__(element_type=bool, **kwargs)
 
+	def init_instantiated_data(self, data: t.List[bool]) -> t.List[bool]:
+		return data
 
-class Time:
+	def init_deserialized_data(self, data: t.List[bool]) -> t.List[bool]:
+		return data
+
+	@property
+	def has_constraints(self) -> bool:
+		return False
+
+	def wsdl_type_name(self, *, with_tns: bool = False) -> str:
+		return "boolean"
+
+
+class Boolean:
 	def __new__(
 			cls,
 			*,
 			tag: t.Optional[str] = None,
 			ns: t.Optional[str] = None,
 			nsmap: t.Optional[t.Dict[str, str]] = None,
 			min_occurs: int = None,
-			max_occurs: t.Union[int, t.Literal["unbounded"]] = None,
-			min_value: t.Optional[time] = None,
-			max_value: t.Optional[time] = None,
-			enumerations: t.Optional[t.Type[Enum]] = None,
-			pattern: t.Optional[str] = None
-	) -> t.Union[time, t.List[time]]:
+			max_occurs: t.Union[int, t.Literal["unbounded"]] = None
+	) -> bool:
 		kwargs = {k: v for k, v in locals().items() if v != cls}
-		return t.cast(time, TimeSpec(**kwargs))
+		return t.cast(bool, BooleanSpec(**kwargs))
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/elements/validators.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/elements/validators.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/envelope/__init__.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/envelope/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/envelope/factory.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/envelope/factory.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/envelope/generics.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/envelope/generics.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/envelope/header.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/envelope/header.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 from ..constants import HEADER_NSMAP
 
 
 __all__ = ["XroadService", "XroadClient", "XroadHeader"]
 
 
 class XroadService(BaseXmlModel, tag="service", ns="xro", nsmap=HEADER_NSMAP, search_mode='unordered'):
-	object_type: str = attr(tag="objectType", ns="iden", default="SERVICE")
+	object_type: str = attr(name="objectType", ns="iden", default="SERVICE")
 	xroad_instance: str = element(tag="xRoadInstance", ns="iden")
 	member_class: str = element(tag="memberClass", ns="iden")
 	member_code: str = element(tag="memberCode", ns="iden")
 	subsystem_code: t.Union[str, None] = element(tag="subsystemCode", ns="iden", default=None)
 	service_code: str = element(tag="serviceCode", ns="iden")
 	service_version: t.Union[str, None] = element(tag="serviceVersion", ns="iden", default=None)
 
 
 class XroadClient(BaseXmlModel, tag="client", ns="xro", nsmap=HEADER_NSMAP, search_mode='unordered'):
-	object_type: str = attr(tag="objectType", ns="iden", default="SUBSYSTEM")
+	object_type: str = attr(name="objectType", ns="iden", default="SUBSYSTEM")
 	xroad_instance: str = element(tag="xRoadInstance", ns="iden")
 	member_class: str = element(tag="memberClass", ns="iden")
 	member_code: str = element(tag="memberCode", ns="iden")
 	subsystem_code: t.Union[str, None] = element(tag="subsystemCode", ns="iden", default=None)
 
 
 class XroadHeader(BaseXmlModel, tag="Header", ns="soapenv", nsmap=HEADER_NSMAP, search_mode='unordered'):
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/file_size.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/file_size.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/multipart/__init__.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/multipart/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/multipart/bodypart.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/multipart/bodypart.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/multipart/decoder.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/multipart/decoder.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/multipart/encoder.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/multipart/encoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 #
 import typing as t
 from email import policy
 from email import encoders
 from email.mime.text import MIMEText
 from email.mime.base import MIMEBase
 from email.mime.multipart import MIMEMultipart
-from ..elements import SwaRefInternal
+from ..elements.models import SwaRefFile
 
 
 __all__ = ["MultipartEncoder"]
 
 
 class MultipartEncoder:
-	def __init__(self, content: bytes, files: t.List[SwaRefInternal]) -> None:
+	def __init__(self, content: bytes, files: t.List[SwaRefFile]) -> None:
 		multipart = self.compute_multipart(content, files)
 		headers, message = multipart.split(b"\r\n\r\n", 1)
 		self.headers = self.raw_headers_to_dict(headers)
 		self.message = b'\r\n' + message  # type: bytes
 		self.headers["Content-Length"] = str(len(self.message))
 
 	@classmethod
-	def compute_multipart(cls, xml_str: bytes, files: t.List[SwaRefInternal]) -> bytes:
+	def compute_multipart(cls, xml_str: bytes, files: t.List[SwaRefFile]) -> bytes:
 		root = MIMEMultipart("related", type="text/xml", start="<rootpart>")
 		cls.attach_soap_envelope(xml_str, root)
 		if len(files) > 1:
 			mixed = MIMEMultipart("mixed")
 			mixed.add_header("Content-Transfer-Encoding", "binary")
 			for file in files:
 				cls.attach_file(file, mixed)
@@ -47,15 +47,15 @@
 		part = MIMEText(xml_str.decode('utf-8'))
 		part.replace_header("Content-Transfer-Encoding", "8bit")
 		part.replace_header("Content-Type", "text/xml; charset=UTF-8")
 		part.add_header("Content-ID", "<rootpart>")
 		parent.attach(part)
 
 	@staticmethod
-	def attach_file(file: SwaRefInternal, parent: MIMEMultipart):
+	def attach_file(file: SwaRefFile, parent: MIMEMultipart):
 		part = MIMEBase(*file.mimetype.split('/'))
 		part.add_header("Content-ID", file.mime_cid)
 		part.add_header("Content-Digest", file.digest)
 		part.add_header("Content-Length", str(file.size))
 		part.add_header('Content-Disposition', '; '.join([
 			"attachment", f'name="{file.name}"', f'filename="{file.name}"'
 		]))
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/multipart/errors.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/multipart/errors.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/soap/__init__.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/soap/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/soap/action.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/soap/action.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,17 +6,20 @@
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 import re
 import typing as t
-from dataclasses import dataclass
-from pydantic import ValidationError
-from fastapi import Response
+from fastapi import Request, Response
+from pydantic import (
+	BaseModel,
+	ValidationError,
+	field_validator
+)
 from ..base import MessageBody
 from ..storage import GlobalWeakStorage
 from ..constants import HEADER_NSMAP
 from ..multipart import (
 	MultipartDecoder,
 	DecodedBodyPart
 )
@@ -28,76 +31,88 @@
 from .response import SoapResponse
 from . import faults as f
 
 
 __all__ = ["SoapAction"]
 
 
-@dataclass(frozen=True)
-class SoapAction:
+_ArgsFrom = t.List[t.Union[MessageBody, XroadHeader]]
+_RespFrom = t.Union[Response, SoapResponse]
+
+
+class SoapAction(BaseModel, arbitrary_types_allowed=True):
 	name: str
 	handler: t.Callable[..., t.Optional[MessageBody]]
-	body_type: t.Type[MessageBody]
+	description: t.Optional[str]
+	body_type: t.Optional[t.Type[MessageBody]]
 	body_index: t.Optional[int]
-	header_type: t.Type[XroadHeader]
+	header_type: t.Optional[t.Type[XroadHeader]]
 	header_index: t.Optional[int]
 	return_type: t.Optional[t.Type[MessageBody]]
 	storage: GlobalWeakStorage
 
-	def arguments_from(
-			self,
-			envelope: GenericEnvelope,
-			action_name: str
-	) -> t.List[t.Union[MessageBody, XroadHeader]]:
+	# noinspection PyNestedDecorators
+	@field_validator("name")
+	@classmethod
+	def validate_name(cls, value: t.Any) -> str:
+		vl = len(value)
+		if vl < 5 or vl > 30:
+			raise ValueError(
+				f"Invalid SOAP action name length {vl} chars for "
+				f"name '{value}'. Length must be >= 5 and <= 30."
+			)
+		return value
+
+	def arguments_from(self, envelope: GenericEnvelope) -> _ArgsFrom:
 		args = list()
 		if self.body_type is not None:
 			if envelope.body is None:
-				raise f.MissingBodyFault(action_name)
+				raise f.MissingBodyFault(self.name)
 			args.insert(self.body_index, envelope.body.content)
 		if self.header_type is not None:
 			if envelope.header is None:
-				raise f.MissingHeaderFault(action_name)
+				raise f.MissingHeaderFault(self.name)
 			args.insert(self.header_index, envelope.header)
 		return args
 
-	def response_from(
-			self,
-			ret_obj: t.Optional[MessageBody],
-			header: XroadHeader
-	) -> t.Union[Response, SoapResponse]:
+	def response_from(self, ret_obj: t.Optional[MessageBody], header: XroadHeader) -> _RespFrom:
 		has_return = self.return_type is not None
 		if not has_return and ret_obj is None:
 			return Response()
 		elif has_return and isinstance(ret_obj, self.return_type):
 			return SoapResponse(content=ret_obj, header=header)
 		raise TypeError(
 			f"Expected return type {self.return_type}, "
 			f"but received {ret_obj}"
 		)
 
-	def parse(self, http_body: bytes, content_type: t.Optional[str]) -> GenericEnvelope:
-		body_ct = content_type.split(';')[0]
-		if body_ct == "multipart/related":
+	async def parse(self, http_request: Request) -> GenericEnvelope:
+		content_type = http_request.headers.get("content-type")
+		body_type = content_type.split(';')[0]
+		http_body = await http_request.body()
+
+		if body_type in ["text/xml", "application/xml", "application/soap+xml"]:
+			return self.deserialize(http_body)
+		elif body_type in ["multipart/related", "multipart/mixed"]:
 			files: t.List[DecodedBodyPart] = list()
-			decoder1 = MultipartDecoder(http_body, content_type)
+			decoder = MultipartDecoder(http_body, content_type)
 			envelope = None
-			for index, part1 in enumerate(decoder1.parts):
+			for index, part in enumerate(decoder.parts):
 				if index == 0:
-					envelope = part1
-				elif part1.is_mixed_multipart:
-					content_type = part1.headers.get('content-type')
-					decoder2 = MultipartDecoder(part1.content, content_type)
-					for part2 in decoder2.parts:
-						files.append(part2)
+					envelope = part
+				elif part.is_mixed_multipart:
+					content_type = part.headers.get('content-type')
+					nested_decoder = MultipartDecoder(part.content, content_type)
+					for nested_part in nested_decoder.parts:
+						files.append(nested_part)
 				else:
-					files.append(part1)
+					files.append(part)
 			http_body = self.process_files(envelope.content, files)
-		elif body_ct not in ["text/xml", "application/xml"]:
-			raise f.ClientFault(f"Invalid content type: {body_ct}")
-		return self.deserialize(http_body)
+			return self.deserialize(http_body)
+		raise f.ClientFault(f"Invalid content type: {body_type}")
 
 	def process_files(self, xml_str: bytes, files: t.List[DecodedBodyPart]) -> bytes:
 		ids = [file.content_id for file in files]
 		for cid in ids:
 			if ids.count(cid) > 1:
 				raise f.DuplicateCIDFault(cid)
 		for file in files:
@@ -110,42 +125,44 @@
 			uid = self.storage.insert_object(file).encode()
 			xml_str = xml_str.replace(cid, uid)
 		return xml_str
 
 	def deserialize(self, http_body: bytes) -> GenericEnvelope:
 		if self.body_type is None:
 			return EnvelopeFactory().deserialize(http_body)
-		try:
-			factory = EnvelopeFactory[self.body_type]
-			return factory().deserialize(http_body)
-		except ValidationError as ex:
-			extra_nsmap = self.extract_extra_nsmap(http_body)
-			name = self.body_type.__name__
-			last_err = ex
-			for ns in extra_nsmap.keys():
-				new = t.cast(t.Type[MessageBody], type(
-					name, (self.body_type,), {},
-					ns=ns, nsmap=extra_nsmap
-				))
-				attrs = self.body_type.__private_attributes__
-				new.__private_attributes__ = attrs
-				try:
-					factory = EnvelopeFactory[new]
-					return factory().deserialize(http_body)
-				except ValidationError as ex:
-					last_err = ex
-			raise last_err
+
+		extra_nsmap = self.extract_extra_nsmap(http_body)
+		attrs = self.body_type.__private_attributes__
+		name = self.body_type.__name__
+		last_err = None
+
+		def inner(**kwargs) -> GenericEnvelope:
+			strict_type = t.cast(t.Type[MessageBody], type(
+				name, (self.body_type,), {}, extra="forbid", **kwargs
+			))
+			strict_type.__private_attributes__ = attrs
+			envelope = EnvelopeFactory[strict_type]()
+			return envelope.deserialize(http_body)
+
+		if not extra_nsmap:
+			return inner()
+		for ns in extra_nsmap.keys():
+			try:
+				return inner(ns=ns, nsmap=extra_nsmap)
+			except ValidationError as ex:
+				last_err = ex
+		raise last_err
 
 	@staticmethod
 	def extract_extra_nsmap(http_body: bytes) -> t.Dict[str, str]:
 		parts = re.split(r'>\s*<', http_body.decode(), maxsplit=1)
 		match = re.search(r'envelope', parts[0], re.IGNORECASE)
 		if len(parts) == 1 or match is None:
 			raise f.ClientFault("Unexpected envelope structure")
-		parts = re.split(r'[ :]', parts[0])
+		parts = re.split(r' |xmlns:', parts[0])
 		nsmap = dict()
 		for part in parts:
 			if '=' not in part:
 				continue
 			key, value = part.split('=')  # type: str, str
 			if key not in HEADER_NSMAP:
 				nsmap[key] = value.strip('"')
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/soap/faults.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/soap/faults.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,26 +6,28 @@
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 import re
 import typing as t
+import inflection
 from pydantic_xml import element
 from ..base import MessageBody
 from ..envelope import GenericFault
 from .response import SoapResponse
 
 
 __all__ = [
 	"SoapFault",
 	"ClientFault",
 	"ServerFault",
 	"InvalidMethodFault",
 	"InvalidActionFault",
+	"MissingActionFault",
 	"MissingBodyFault",
 	"MissingHeaderFault",
 	"MissingCIDFault",
 	"DuplicateCIDFault",
 	"ValidationFault"
 ]
 
@@ -81,14 +83,20 @@
 
 class InvalidActionFault(SoapFault):
 	def __init__(self, action: str) -> None:
 		msg = f"Service does not support SOAP action: {action}"
 		super().__init__(string=msg)
 
 
+class MissingActionFault(SoapFault):
+	def __init__(self):
+		msg = "SOAP action HTTP header is missing."
+		super().__init__(string=msg)
+
+
 class MissingBodyFault(SoapFault):
 	def __init__(self, action_name: str) -> None:
 		msg = f"Body element missing from envelope for {action_name} SOAP action"
 		super().__init__(string=msg)
 
 
 class MissingHeaderFault(SoapFault):
@@ -123,28 +131,26 @@
 		)
 
 	@staticmethod
 	def extract_details(parts: t.List[str]) -> MessageBody:
 		class Detail(MessageBody):
 			location: str = element()
 			reason: str = element()
-			input_value: str = element()
+			input_value: str = element(tag="inputValue")
 
 		class ErrorDetails(MessageBody):
 			details: t.List[Detail] = element(tag="validationError")
 
 		details = list()
 		for part in parts:
 			loc, msg = part.split('\n')
 			iv_match = re.search(r"\$\$(.*?)\$\$", msg)
 			if iv_match:
 				msg = msg.replace(f"$${iv_match.group(1)}$$", '')
-			else:
-				iv_match = re.search(r"input_value=(.+?),", msg)
 			ln_match = re.search(r"(\[line -?\d+]: )", msg)
 			re_match = re.search(r"\[line -?\d+]: (.+?) \[type=", msg)
 			details.append(Detail(
-				location=(ln_match.group(1) + loc) if ln_match else "unknown",
-				input_value=iv_match.group(1) if iv_match else "unknown",
-				reason=re_match.group(1) if re_match else "unknown"
+				location=inflection.camelize(loc) if ln_match else "Unknown",
+				reason=re_match.group(1) if re_match else "Unknown",
+				input_value=iv_match.group(1) if iv_match else "Unknown",
 			))
 		return ErrorDetails(details=details)
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/soap/service.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/soap/service.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,23 +16,25 @@
 from fastapi import FastAPI, Request, Response
 from fastapi.types import DecoratedCallable
 from starlette.types import Lifespan
 from starlette.middleware.base import BaseHTTPMiddleware
 from ..multipart import MultipartError
 from ..storage import GlobalWeakStorage
 from .. import utils, wsdl
+from .validators import validate_annotations
 from .action import SoapAction
 from . import faults as f
 
 
 __all__ = ["SoapService"]
 
 
 SoapMiddleware: t.TypeAlias = BaseHTTPMiddleware
 FuncOrCoro = t.Union[t.Callable[..., t.Any], t.Awaitable[t.Any]]
+ActionType = t.Callable[[DecoratedCallable], DecoratedCallable]
 
 
 class SoapService(FastAPI):
 	def __init__(
 			self,
 			*,
 			name: str = "SoapService",
@@ -61,41 +63,32 @@
 		super().__init__(
 			root_path=path,
 			lifespan=lifespan,
 			openapi_url=None,
 			redoc_url=None,
 			docs_url=None,
 		)
-		self._as_fastapi().add_middleware(
+		app = t.cast(FastAPI, self)
+		app.add_middleware(
 			middleware_class=SoapMiddleware,
 			dispatch=self._soap_middleware
 		)
 
-	def _as_fastapi(self) -> FastAPI:
-		return t.cast(FastAPI, self)
-
 	async def _soap_middleware(self, http_request: Request, _: t.Callable) -> t.Optional[Response]:
 		try:
 			if "wsdl" in http_request.query_params:
 				if self._wsdl_response is None:
 					self.regenerate_wsdl()
 				return self._wsdl_response
 			elif http_request.method != "POST":
 				raise f.InvalidMethodFault(http_request.method)
 
-			action_name = http_request.headers.get("soapaction", '').strip('"')
-			if not action_name or action_name not in self._actions.keys():
-				raise f.InvalidActionFault(action_name)
-
-			http_body = await http_request.body()
-			content_type = http_request.headers.get("content-type")
-
-			action = self._actions[action_name]
-			envelope = action.parse(http_body, content_type)
-			args = action.arguments_from(envelope, action_name)
+			action = self._determine_action(http_request)
+			envelope = await action.parse(http_request)
+			args = action.arguments_from(envelope)
 			ret = await self._await_or_call(action.handler, *args)
 			return action.response_from(ret, envelope.header)
 
 		except f.SoapFault as ex:
 			err, resp = ex, ex.response
 		except ValidationError as ex:
 			err, resp = ex, f.ValidationFault(ex).response
@@ -109,39 +102,54 @@
 		if self._fault_callback is not None:
 			await self._await_or_call(
 				self._fault_callback,
 				http_request, err
 			)
 		return resp
 
+	def _determine_action(self, http_request: Request) -> SoapAction:
+		name = http_request.headers.get("soapaction", '').strip('"')
+		valid_names = self._actions.keys()
+		if not name:
+			raise f.MissingActionFault()
+		elif name in valid_names:
+			return self._actions[name]
+		sep = '#' if '#' in name else '/'
+		fragment: str = name.split(sep)[-1]
+		for vn in valid_names:
+			if vn == fragment:
+				return self._actions[name]
+		raise f.InvalidActionFault(name)
+
 	@staticmethod
 	async def _await_or_call(func: FuncOrCoro, *args, **kwargs) -> t.Any:
 		if inspect.iscoroutinefunction(func):
 			return await func(*args, **kwargs)
 		return func(*args, **kwargs)
 
-	def add_action(self, name: str, handler: t.Callable[..., t.Any]) -> None:
+	def add_action(self, name: str, handler: t.Callable[..., t.Any], description: t.Optional[str] = None) -> None:
 		if name in self._actions.keys():
 			raise ValueError(f"Cannot add duplicate {name} SOAP action.")
-		anno = utils.validate_annotations(name, handler)
+		anno = validate_annotations(name, handler)
 		pos = utils.extract_parameter_positions(anno)
 		self._actions[name] = SoapAction(
 			name=name,
 			handler=handler,
+			description=description,
 			body_type=anno.get("body"),
 			body_index=pos.get("body"),
 			header_type=anno.get("header"),
 			header_index=pos.get("header"),
 			return_type=anno.get("return"),
 			storage=self._storage
 		)
 
-	def action(self, name: str) -> t.Callable[[DecoratedCallable], DecoratedCallable]:
+	def action(self, name: str, description: t.Optional[str] = None) -> ActionType:
 		def closure(func: DecoratedCallable) -> DecoratedCallable:
-			self.add_action(name, func)
+			self.add_action(name, func, description)
 			return func
 		return closure
 
 	def regenerate_wsdl(self, *, force: bool = False) -> None:
 		if self._wsdl_override is not None and not force:
 			raise RuntimeError(
 				"WSDL regeneration must be explicitly forced when "
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/storage.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import secrets
 import typing as t
 from weakref import WeakValueDictionary
 
 
 __all__ = [
 	"GlobalWeakStorage",
-	"ExportableGlobalWeakStorage"
+	"ExportableGWS"
 ]
 
 
 class GlobalWeakStorage:
 	_instances = WeakValueDictionary()
 	_inst_counter = 0
 	_uid = ''
@@ -134,8 +134,8 @@
 		self.validate_fingerprint(fingerprint)
 		obj_id = fingerprint.split('-$$-')[1]
 		if raise_on_miss:
 			return self._objects[obj_id]
 		return self._objects.get(obj_id, None)
 
 
-ExportableGlobalWeakStorage = type('GlobalWeakStorage', (GlobalWeakStorage,), {})
+ExportableGWS = type('GlobalWeakStorage', (GlobalWeakStorage,), {})
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/utils/__init__.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,34 +8,35 @@
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 from .content_utils import (
 	split_on_find,
 	guess_mime_type,
 	detect_decode,
-	convert_to_utf8
+	convert_to_utf8,
+	remove_memory_addresses
 )
 from .path_utils import (
 	search_upwards,
 	resolve_relpath,
 	read_cached_file,
 	read_cached_xml_file
 )
 from .route_utils import (
 	get_annotations,
-	validate_annotations,
 	extract_parameter_positions
 )
 
 
 __all__ = [
 	"split_on_find",
 	"guess_mime_type",
 	"detect_decode",
+	"convert_to_utf8",
+	"remove_memory_addresses",
 	"search_upwards",
 	"resolve_relpath",
 	"read_cached_file",
 	"read_cached_xml_file",
 	"get_annotations",
-	"validate_annotations",
 	"extract_parameter_positions"
 ]
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/utils/content_utils.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/utils/content_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 #   Copyright (c) 2024, Centre of Registers and Information Systems
 #
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
+import re
 import chardet
 import mimetypes
 import typing as t
 import charset_normalizer as charset
-from ..base import MessageBody, BaseElementSpec
 
 
 __all__ = [
 	"split_on_find",
 	"guess_mime_type",
 	"detect_decode",
-	"convert_to_utf8"
+	"convert_to_utf8",
+	"remove_memory_addresses"
 ]
 
 
 _USB = t.Union[str, bytes]
 _USN = t.Union[str, None]
 
 
@@ -56,7 +57,13 @@
 
 
 def convert_to_utf8(string: bytes) -> bytes:
 	decoded, encoding = detect_decode(string)
 	if encoding not in [None, 'utf-8']:
 		string = decoded.encode('utf-8')
 	return string
+
+
+def remove_memory_addresses(string: bytes) -> bytes:
+	pattern = r"0x[0-9A-Fa-f]+"
+	cleaned_text = re.sub(pattern, '', string.decode())
+	return cleaned_text.encode()
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/utils/path_utils.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/utils/route_utils.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/soap/validators.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,33 +8,22 @@
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 import typing as t
 from fastapi.types import DecoratedCallable
 from ..envelope import XroadHeader
 from ..base import MessageBody
+from .. import utils
 
 
-__all__ = [
-	"get_annotations",
-	"validate_annotations",
-	"extract_parameter_positions"
-]
-
-
-def get_annotations(func: t.Any) -> dict:
-	key: str = "__annotations__"
-	anno = getattr(func, key, None)
-	if anno is None and hasattr(func, "__dict__"):
-		anno = func.__dict__.get(key, None)
-	return anno or dict()
+__all__ = ["validate_annotations"]
 
 
 def validate_annotations(name: str, func: DecoratedCallable) -> dict:
-	anno = get_annotations(func)
+	anno = utils.get_annotations(func)
 	for key, value in anno.items():
 		_validate_a8n_key(key, name)
 		if key == "return":
 			_validate_a8n_return(value, name)
 		elif key == "body":
 			_validate_a8n_body(key, value, name)
 		elif key == "header":
@@ -75,16 +64,7 @@
 
 def _validate_a8n_header(value: t.Any, name: str) -> None:
 	if value != XroadHeader:
 		raise ValueError(
 			f"The annotation of the 'headers' parameter of the {name} "
 			f"SOAP action must be the 'XroadHeaders' class."
 		)
-
-
-def extract_parameter_positions(anno: dict) -> dict:
-	pos = dict(body=None, header=None)
-	keys = list(anno.keys())
-	for key in ["body", "header"]:
-		if key in keys:
-			pos[key] = keys.index(key)
-	return pos
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/wsdl/__init__.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 #   Copyright (c) 2024, Centre of Registers and Information Systems
 #
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
-from .generator import generate
 from .binding import (
 	SOAPFault,
 	SOAPBody,
 	SOAPHeader,
 	WSDLFaultBinding,
 	WSDLOutputBinding,
 	WSDLInputBinding,
@@ -23,48 +22,37 @@
 	WSDLBinding
 )
 from .conditions import (
 	Enumeration,
 	RegexPattern,
 	MinInclusive,
 	MaxInclusive,
-	MinExclusive,
-	MaxExclusive,
-	FractionDigits,
 	TotalDigits,
 	Length,
 	MinLength,
 	MaxLength,
-	WhiteSpace
+	WhiteSpace,
 )
 from .definitions import (
 	WSDLTypes,
 	WSDLPart,
 	WSDLMessage,
-	WSDLDefinitions
+	WSDLDefinitions,
 )
 from .port_type import (
 	WSDLFaultPort,
 	WSDLOutputPort,
 	WSDLInputPort,
 	WSDLDocumentation,
 	WSDLOperationPort,
-	WSDLPortType
+	WSDLPortType,
 )
 from .restrictions import (
-	StringRestriction,
-	IntegerRestriction,
-	DecimalRestriction,
-	FloatRestriction,
-	DoubleRestriction,
-	DateRestriction,
-	TimeRestriction,
-	DateTimeRestriction,
-	DurationRestriction,
-	AnyURIRestriction
+	NumericTypeRestriction,
+	StringTypeRestriction
 )
 from .schema import (
 	SimpleType,
 	AnyXML,
 	Element,
 	Sequence,
 	ComplexType,
@@ -76,16 +64,14 @@
 	SOAPAddress,
 	WSDLPortBinding,
 	WSDLService
 )
 
 
 __all__ = [
-	"generate",
-
 	# binding.py
 	"SOAPFault",
 	"SOAPBody",
 	"SOAPHeader",
 	"WSDLFaultBinding",
 	"WSDLOutputBinding",
 	"WSDLInputBinding",
@@ -96,17 +82,14 @@
 	"WSDLBinding",
 
 	# conditions.py
 	"Enumeration",
 	"RegexPattern",
 	"MinInclusive",
 	"MaxInclusive",
-	"MinExclusive",
-	"MaxExclusive",
-	"FractionDigits",
 	"TotalDigits",
 	"Length",
 	"MinLength",
 	"MaxLength",
 	"WhiteSpace",
 
 	# definitions.py
@@ -120,24 +103,16 @@
 	"WSDLOutputPort",
 	"WSDLInputPort",
 	"WSDLDocumentation",
 	"WSDLOperationPort",
 	"WSDLPortType",
 
 	# restrictions.py
-	"StringRestriction",
-	"IntegerRestriction",
-	"DecimalRestriction",
-	"FloatRestriction",
-	"DoubleRestriction",
-	"DateRestriction",
-	"TimeRestriction",
-	"DateTimeRestriction",
-	"DurationRestriction",
-	"AnyURIRestriction",
+	"NumericTypeRestriction",
+	"StringTypeRestriction",
 
 	# schema.py
 	"SimpleType",
 	"AnyXML",
 	"Element",
 	"Sequence",
 	"ComplexType",
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/wsdl/binding.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/binding.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 import typing as t
 from pydantic_xml import BaseXmlModel, attr
-from ..constants import WSDL_NSMAP
+from fastapi_xroad_soap.internal.constants import WSDL_NSMAP
 
 
 __all__ = [
 	"SOAPFault",
 	"SOAPBody",
 	"SOAPHeader",
 	"WSDLFaultBinding",
@@ -46,35 +46,35 @@
 class WSDLFaultBinding(BaseXmlModel, tag="fault", ns="wsdl", nsmap=WSDL_NSMAP):
 	name: str = attr(default="FaultResponse")
 	fault: SOAPFault = SOAPFault()
 
 
 class WSDLOutputBinding(BaseXmlModel, tag="output", ns="wsdl", nsmap=WSDL_NSMAP):
 	headers: t.List[SOAPHeader] = [
-		SOAPHeader(part="client"),
-		SOAPHeader(part="service"),
-		SOAPHeader(part="id"),
 		SOAPHeader(part="userId"),
-		SOAPHeader(part="protocolVersion")
+		SOAPHeader(part="protocolVersion"),
+		SOAPHeader(part="id"),
+		SOAPHeader(part="service"),
+		SOAPHeader(part="client")
 	]
 	body: SOAPBody = SOAPBody()
 
 
 class WSDLInputBinding(BaseXmlModel, tag="input", ns="wsdl", nsmap=WSDL_NSMAP):
 	headers: t.List[SOAPHeader] = [
-		SOAPHeader(part="client"),
-		SOAPHeader(part="service"),
-		SOAPHeader(part="id"),
+		SOAPHeader(part="userId"),
 		SOAPHeader(part="protocolVersion"),
-		SOAPHeader(part="userId")
+		SOAPHeader(part="id"),
+		SOAPHeader(part="service"),
+		SOAPHeader(part="client")
 	]
 	body: SOAPBody = SOAPBody()
 
 
-class XROADVersion(BaseXmlModel, tag="version", ns="xroad", nsmap=WSDL_NSMAP):
+class XROADVersion(BaseXmlModel, tag="version", ns="xro", nsmap=WSDL_NSMAP):
 	version: str = "v1"
 
 
 class SOAPOperationBinding(BaseXmlModel, tag="operation", ns="soap", nsmap=WSDL_NSMAP):
 	soap_action: str = attr(name="soapAction")
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/wsdl/conditions.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/conditions.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,17 +13,14 @@
 
 
 __all__ = [
 	"Enumeration",
 	"RegexPattern",
 	"MinInclusive",
 	"MaxInclusive",
-	"MinExclusive",
-	"MaxExclusive",
-	"FractionDigits",
 	"TotalDigits",
 	"Length",
 	"MinLength",
 	"MaxLength",
 	"WhiteSpace"
 ]
 
@@ -40,26 +37,14 @@
 	value: str = attr()
 
 
 class MaxInclusive(BaseXmlModel, tag="maxInclusive"):
 	value: str = attr()
 
 
-class MinExclusive(BaseXmlModel, tag="minExclusive"):
-	value: str = attr()
-
-
-class MaxExclusive(BaseXmlModel, tag="maxExclusive"):
-	value: str = attr()
-
-
-class FractionDigits(BaseXmlModel, tag="fractionDigits"):
-	value: str = attr()
-
-
 class TotalDigits(BaseXmlModel, tag="totalDigits"):
 	value: str = attr()
 
 
 class Length(BaseXmlModel, tag="length"):
 	value: str = attr()
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/wsdl/definitions.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/definitions.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 import typing as t
 from pydantic_xml import BaseXmlModel, element, attr
-from ..constants import WSDL_NSMAP
+from fastapi_xroad_soap.internal.constants import WSDL_NSMAP
 from .port_type import WSDLPortType
 from .binding import WSDLBinding
 from .service import WSDLService
 from .schema import Schema
 
 
 __all__ = [
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/wsdl/port_type.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/port_type.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,51 +6,51 @@
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 import typing as t
 from pydantic_xml import BaseXmlModel, element, attr
-from ..constants import WSDL_NSMAP
+from fastapi_xroad_soap.internal.constants import WSDL_NSMAP
 
 
 __all__ = [
     "WSDLFaultPort",
     "WSDLOutputPort",
     "WSDLInputPort",
     "WSDLDocumentation",
     "WSDLOperationPort",
     "WSDLPortType"
 ]
 
 
 class WSDLFaultPort(BaseXmlModel, tag="fault", nsmap=WSDL_NSMAP):
-    message: str = attr()
-    name: str = attr()
+    message: str = attr(default="tns:FaultResponse")
+    name: str = attr(default="FaultResponse")
 
 
 class WSDLOutputPort(BaseXmlModel, tag="output", nsmap=WSDL_NSMAP):
     message: str = attr()
     name: str = attr()
 
 
 class WSDLInputPort(BaseXmlModel, tag="input", nsmap=WSDL_NSMAP):
     message: str = attr()
     name: str = attr()
 
 
 class WSDLDocumentation(BaseXmlModel, tag="documentation", nsmap=WSDL_NSMAP):
-    title: str = element(ns='xroad', nsmap=WSDL_NSMAP)
-    notes: str = element(ns='xroad', nsmap=WSDL_NSMAP)
+    title: str = element(ns='xro', nsmap=WSDL_NSMAP)
+    notes: str = element(ns='xro', nsmap=WSDL_NSMAP)
 
 
-class WSDLOperationPort(BaseXmlModel, tag="operation", ns="wsdl", nsmap=WSDL_NSMAP):
-    documentation: WSDLDocumentation
-    input: WSDLInputPort
-    output: WSDLOutputPort
-    fault: WSDLFaultPort
+class WSDLOperationPort(BaseXmlModel, tag="operation", ns="wsdl", nsmap=WSDL_NSMAP, skip_empty=True):
+    documentation: t.Optional[WSDLDocumentation] = None
+    input: t.Optional[WSDLInputPort] = None
+    output: t.Optional[WSDLOutputPort] = None
+    fault: WSDLFaultPort = WSDLFaultPort()
     name: str = attr()
 
 
 class WSDLPortType(BaseXmlModel, tag="portType", ns="wsdl", nsmap=WSDL_NSMAP):
     name: str = attr(default="servicePortType")
     operations: t.List[WSDLOperationPort]
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/wsdl/schema.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/schema.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,62 +6,38 @@
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 import typing as t
 from pydantic_xml import BaseXmlModel, attr
-from ..constants import WSDL_NSMAP
+from fastapi_xroad_soap.internal.constants import WSDL_NSMAP
 from .restrictions import (
-    StringRestriction,
-    IntegerRestriction,
-    DecimalRestriction,
-    FloatRestriction,
-    DoubleRestriction,
-    DateRestriction,
-    TimeRestriction,
-    DateTimeRestriction,
-    DurationRestriction,
-    AnyURIRestriction
+    NumericTypeRestriction,
+    StringTypeRestriction
 )
 
 
 __all__ = [
-    "SimpleType",
     "AnyXML",
     "Element",
     "Sequence",
     "ComplexType",
+    "SimpleType",
     "Import",
     "Include",
     "Schema"
 ]
 
 
-class SimpleType(BaseXmlModel, tag="simpleType"):
-    name: str = attr()
-    restriction: t.Union[
-        StringRestriction,
-        IntegerRestriction,
-        DecimalRestriction,
-        FloatRestriction,
-        DoubleRestriction,
-        DateRestriction,
-        TimeRestriction,
-        DateTimeRestriction,
-        DurationRestriction,
-        AnyURIRestriction
-    ]
-
-
 class AnyXML(BaseXmlModel, tag="any"):
-    process_contents: str = attr(default="lax")
+    process_contents: str = attr(name="processContents", default="lax")
 
 
-class Element(BaseXmlModel, tag="element"):
+class Element(BaseXmlModel, tag="element", skip_empty=True):
     name: str = attr()
     type: str = attr()
     min_occurs: t.Union[str, None] = attr(name="minOccurs", default=None)
     max_occurs: t.Union[str, None] = attr(name="maxOccurs", default=None)
 
 
 class Sequence(BaseXmlModel, tag="sequence"):
@@ -69,17 +45,25 @@
 
 
 class ComplexType(BaseXmlModel, tag="complexType"):
     name: str = attr()
     sequence: Sequence
 
 
+class SimpleType(BaseXmlModel, tag="simpleType"):
+    name: str = attr()
+    restriction: t.Union[
+        NumericTypeRestriction,
+        StringTypeRestriction
+    ]
+
+
 class Import(BaseXmlModel, tag="import"):
-    schema_loc: str = attr(name="schemaLocation")
     namespace: str = attr()
+    schema_loc: str = attr(name="schemaLocation")
 
 
 class Include(BaseXmlModel, tag="include"):
     schema_loc: str = attr(name="schemaLocation")
 
 
 class Schema(BaseXmlModel, tag="schema"):
```

### Comparing `fastapi_xroad_soap-0.2.2/fastapi_xroad_soap/internal/wsdl/service.py` & `fastapi_xroad_soap-0.3.0/fastapi_xroad_soap/internal/wsdl/models/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 from pydantic_xml import BaseXmlModel, attr
-from ..constants import WSDL_NSMAP
+from fastapi_xroad_soap.internal.constants import WSDL_NSMAP
 
 
 __all__ = [
 	"SOAPAddress",
 	"WSDLPortBinding",
 	"WSDLService"
 ]
```

### Comparing `fastapi_xroad_soap-0.2.2/pyproject.toml` & `fastapi_xroad_soap-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-xroad-soap"
-version = "0.2.2"
+version = "0.3.0"
 description = "FastAPI Extension for X-Road SOAP"
 authors = ["Zero Reports Team <zero.dev@rik.ee>"]
 license = "EUPL-1.2"
 readme = "README.md"
 keywords = ["fastapi", "xroad", "soap"]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `fastapi_xroad_soap-0.2.2/PKG-INFO` & `fastapi_xroad_soap-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-xroad-soap
-Version: 0.2.2
+Version: 0.3.0
 Summary: FastAPI Extension for X-Road SOAP
 License: EUPL-1.2
 Keywords: fastapi,xroad,soap
 Author: Zero Reports Team
 Author-email: zero.dev@rik.ee
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -36,14 +36,16 @@
 Project-URL: Bug Tracker, https://github.com/rik-ee/fastapi-xroad-soap/issues
 Project-URL: Documentation, https://github.com/rik-ee/fastapi-xroad-soap/wiki
 Project-URL: Repository, https://github.com/rik-ee/fastapi-xroad-soap
 Description-Content-Type: text/markdown
 
 # FastAPI X-Road SOAP
 
+<img src="https://raw.githubusercontent.com/rik-ee/fastapi-xroad-soap/main/media/fxs_logo.jpg" alt="Logo" width="500">
+
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fastapi-xroad-soap)](https://pypi.org/project/fastapi-xroad-soap/)
 [![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/rik-ee/fastapi-xroad-soap/build-publish.yaml)](https://github.com/rik-ee/fastapi-xroad-soap/actions/workflows/build-publish.yaml)
 [![codecov](https://codecov.io/gh/rik-ee/fastapi-xroad-soap/graph/badge.svg?token=KB58NGDC1N)](https://codecov.io/gh/rik-ee/fastapi-xroad-soap)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/fastapi-xroad-soap)](https://pypistats.org/packages/fastapi-xroad-soap)
```

