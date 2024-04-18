# Comparing `tmp/protobuf2pydantic-2024.1.8.tar.gz` & `tmp/protobuf2pydantic-2024.4.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protobuf2pydantic-2024.1.8.tar", last modified: Mon Jan  8 06:24:56 2024, max compression
+gzip compressed data, was "protobuf2pydantic-2024.4.18.tar", last modified: Thu Apr 18 06:30:04 2024, max compression
```

## Comparing `protobuf2pydantic-2024.1.8.tar` & `protobuf2pydantic-2024.4.18.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 06:24:56.778068 protobuf2pydantic-2024.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-01-08 06:24:44.000000 protobuf2pydantic-2024.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-01-08 06:24:56.778068 protobuf2pydantic-2024.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-01-08 06:24:44.000000 protobuf2pydantic-2024.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 06:24:56.774068 protobuf2pydantic-2024.1.8/protobuf2pydantic/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-01-08 06:24:44.000000 protobuf2pydantic-2024.1.8/protobuf2pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-01-08 06:24:44.000000 protobuf2pydantic-2024.1.8/protobuf2pydantic/biz.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-01-08 06:24:44.000000 protobuf2pydantic-2024.1.8/protobuf2pydantic/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 06:24:56.778068 protobuf2pydantic-2024.1.8/protobuf2pydantic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-01-08 06:24:56.000000 protobuf2pydantic-2024.1.8/protobuf2pydantic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-01-08 06:24:56.000000 protobuf2pydantic-2024.1.8/protobuf2pydantic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 06:24:56.000000 protobuf2pydantic-2024.1.8/protobuf2pydantic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-08 06:24:56.000000 protobuf2pydantic-2024.1.8/protobuf2pydantic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-08 06:24:56.000000 protobuf2pydantic-2024.1.8/protobuf2pydantic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-08 06:24:56.000000 protobuf2pydantic-2024.1.8/protobuf2pydantic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-08 06:24:56.778068 protobuf2pydantic-2024.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-01-08 06:24:44.000000 protobuf2pydantic-2024.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 06:24:56.778068 protobuf2pydantic-2024.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 06:24:44.000000 protobuf2pydantic-2024.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-01-08 06:24:44.000000 protobuf2pydantic-2024.1.8/tests/celery_task_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-01-08 06:24:44.000000 protobuf2pydantic-2024.1.8/tests/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-01-08 06:24:44.000000 protobuf2pydantic-2024.1.8/tests/test_biz.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-01-08 06:24:44.000000 protobuf2pydantic-2024.1.8/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    14568 2024-01-08 06:24:44.000000 protobuf2pydantic-2024.1.8/tests/test_map_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-01-08 06:24:44.000000 protobuf2pydantic-2024.1.8/tests/test_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:30:04.752966 protobuf2pydantic-2024.4.18/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-18 06:29:49.000000 protobuf2pydantic-2024.4.18/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-18 06:30:04.748966 protobuf2pydantic-2024.4.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-18 06:29:49.000000 protobuf2pydantic-2024.4.18/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:30:04.748966 protobuf2pydantic-2024.4.18/protobuf2pydantic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-18 06:29:49.000000 protobuf2pydantic-2024.4.18/protobuf2pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-18 06:29:49.000000 protobuf2pydantic-2024.4.18/protobuf2pydantic/biz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-18 06:29:49.000000 protobuf2pydantic-2024.4.18/protobuf2pydantic/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:30:04.748966 protobuf2pydantic-2024.4.18/protobuf2pydantic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-18 06:30:04.000000 protobuf2pydantic-2024.4.18/protobuf2pydantic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-18 06:30:04.000000 protobuf2pydantic-2024.4.18/protobuf2pydantic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 06:30:04.000000 protobuf2pydantic-2024.4.18/protobuf2pydantic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-18 06:30:04.000000 protobuf2pydantic-2024.4.18/protobuf2pydantic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-18 06:30:04.000000 protobuf2pydantic-2024.4.18/protobuf2pydantic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-18 06:30:04.000000 protobuf2pydantic-2024.4.18/protobuf2pydantic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 06:30:04.752966 protobuf2pydantic-2024.4.18/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-18 06:29:49.000000 protobuf2pydantic-2024.4.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:30:04.748966 protobuf2pydantic-2024.4.18/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:29:49.000000 protobuf2pydantic-2024.4.18/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-04-18 06:29:49.000000 protobuf2pydantic-2024.4.18/tests/celery_task_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-18 06:29:49.000000 protobuf2pydantic-2024.4.18/tests/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-18 06:29:49.000000 protobuf2pydantic-2024.4.18/tests/test_biz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-18 06:29:49.000000 protobuf2pydantic-2024.4.18/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14568 2024-04-18 06:29:49.000000 protobuf2pydantic-2024.4.18/tests/test_map_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-18 06:29:49.000000 protobuf2pydantic-2024.4.18/tests/test_pb2.py
```

### Comparing `protobuf2pydantic-2024.1.8/LICENSE` & `protobuf2pydantic-2024.4.18/LICENSE`

 * *Files identical despite different names*

### Comparing `protobuf2pydantic-2024.1.8/PKG-INFO` & `protobuf2pydantic-2024.4.18/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protobuf2pydantic
-Version: 2024.1.8
+Version: 2024.4.18
 Summary: Generate a file which include pydantic models by protobuf.pb2 file
 Home-page: https://github.com/Ed-XCF/protobuf2pydantic
 Author: Ed__xu__Ed
 Author-email: m.tofu@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `protobuf2pydantic-2024.1.8/README.md` & `protobuf2pydantic-2024.4.18/README.md`

 * *Files identical despite different names*

### Comparing `protobuf2pydantic-2024.1.8/protobuf2pydantic/__init__.py` & `protobuf2pydantic-2024.4.18/protobuf2pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `protobuf2pydantic-2024.1.8/protobuf2pydantic/biz.py` & `protobuf2pydantic-2024.4.18/protobuf2pydantic/biz.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from os import linesep
-from typing import List
+from typing import List, Optional
 from functools import partial
 
 from google.protobuf.reflection import GeneratedProtocolMessageType
 from google.protobuf.descriptor import Descriptor, FieldDescriptor, EnumDescriptor
 
 message_metaclasses = [GeneratedProtocolMessageType]
 try:
@@ -57,15 +57,15 @@
     try:
         defined_classes[level]
     except KeyError:
         defined_classes[level] = []
     defined_classes[level].append(class_name)
         
 
-def convert_field(level: int, field: FieldDescriptor) -> str | None:
+def convert_field(level: int, field: FieldDescriptor) -> Optional[str]:
     level += 1
     field_type = field.type
     field_label = field.label
     was_mapping = False
     extra = None
 
     if class_already_defined(level, field):
@@ -119,15 +119,15 @@
 
 def msg2pydantic(level: int, msg: Descriptor) -> str:
     class_statement = f"{tab * level}class {msg.name}(BaseModel):"
     add_defined_class(level, msg.name)
     if msg.fields:
         field_statements = map(partial(convert_field, level), msg.fields)
     else:
-        field_statements = [tab + "pass"]
+        field_statements = [f"{tab * (level + 1)}pass"]
     return linesep.join([class_statement, *[fs for fs in field_statements if fs]])
 
 
 def get_config(level: int):
     level += 1
     class_statement = f"{tab * level}class Config:"
     attribute_statement = f"{tab * (level + 1)}arbitrary_types_allowed = True"
```

### Comparing `protobuf2pydantic-2024.1.8/protobuf2pydantic.egg-info/PKG-INFO` & `protobuf2pydantic-2024.4.18/protobuf2pydantic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protobuf2pydantic
-Version: 2024.1.8
+Version: 2024.4.18
 Summary: Generate a file which include pydantic models by protobuf.pb2 file
 Home-page: https://github.com/Ed-XCF/protobuf2pydantic
 Author: Ed__xu__Ed
 Author-email: m.tofu@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `protobuf2pydantic-2024.1.8/setup.py` & `protobuf2pydantic-2024.4.18/setup.py`

 * *Files identical despite different names*

### Comparing `protobuf2pydantic-2024.1.8/tests/celery_task_pb2.py` & `protobuf2pydantic-2024.4.18/tests/celery_task_pb2.py`

 * *Files identical despite different names*

### Comparing `protobuf2pydantic-2024.1.8/tests/test_map_pb2.py` & `protobuf2pydantic-2024.4.18/tests/test_map_pb2.py`

 * *Files identical despite different names*

### Comparing `protobuf2pydantic-2024.1.8/tests/test_pb2.py` & `protobuf2pydantic-2024.4.18/tests/test_pb2.py`

 * *Files identical despite different names*

