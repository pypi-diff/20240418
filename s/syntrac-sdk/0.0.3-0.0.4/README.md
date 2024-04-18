# Comparing `tmp/syntrac_sdk-0.0.3.tar.gz` & `tmp/syntrac_sdk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntrac_sdk-0.0.3.tar", max compression
+gzip compressed data, was "syntrac_sdk-0.0.4.tar", max compression
```

## Comparing `syntrac_sdk-0.0.3.tar` & `syntrac_sdk-0.0.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      606 2024-04-16 14:38:01.555391 syntrac_sdk-0.0.3/README.md
--rw-r--r--   0        0        0     2125 2024-04-16 14:38:01.574774 syntrac_sdk-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     7767 2024-04-16 14:38:01.558526 syntrac_sdk-0.0.3/syntrac/sdk/__init__.py
--rw-r--r--   0        0        0      358 2024-04-16 14:38:01.560515 syntrac_sdk-0.0.3/syntrac/sdk/config/__init__.py
--rw-r--r--   0        0        0     1117 2024-04-16 14:38:01.560884 syntrac_sdk-0.0.3/syntrac/sdk/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    11612 2024-04-16 14:38:01.561217 syntrac_sdk-0.0.3/syntrac/sdk/decorators/__init__.py
--rw-r--r--   0        0        0    16396 2024-04-16 14:38:01.561774 syntrac_sdk-0.0.3/syntrac/sdk/decorators/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4393 2024-04-16 14:38:01.561938 syntrac_sdk-0.0.3/syntrac/sdk/fetcher.py
--rw-r--r--   0        0        0      465 2024-04-16 14:38:01.562061 syntrac_sdk-0.0.3/syntrac/sdk/instruments.py
--rw-r--r--   0        0        0        0 2024-04-16 14:38:01.562239 syntrac_sdk-0.0.3/syntrac/sdk/metrics/__init__.py
--rw-r--r--   0        0        0      202 2024-04-16 14:38:01.562485 syntrac_sdk-0.0.3/syntrac/sdk/metrics/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3677 2024-04-16 14:38:01.562722 syntrac_sdk-0.0.3/syntrac/sdk/metrics/__pycache__/metrics.cpython-311.pyc
--rw-r--r--   0        0        0     2346 2024-04-16 14:38:01.562933 syntrac_sdk-0.0.3/syntrac/sdk/metrics/metrics.py
--rw-r--r--   0        0        0     2721 2024-04-16 14:38:01.563267 syntrac_sdk-0.0.3/syntrac/sdk/otlp/json/__init__.py
--rw-r--r--   0        0        0     2638 2024-04-16 14:38:01.563673 syntrac_sdk-0.0.3/syntrac/sdk/otlp/json/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      226 2024-04-16 14:38:01.563858 syntrac_sdk-0.0.3/syntrac/sdk/otlp/json/__pycache__/version.cpython-311.pyc
--rw-r--r--   0        0        0     7151 2024-04-16 14:38:01.564092 syntrac_sdk-0.0.3/syntrac/sdk/otlp/json/trace_exporter/__init__.py
--rw-r--r--   0        0        0     9678 2024-04-16 14:38:01.564348 syntrac_sdk-0.0.3/syntrac/sdk/otlp/json/trace_exporter/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      607 2024-04-16 14:38:01.564564 syntrac_sdk-0.0.3/syntrac/sdk/otlp/json/version.py
--rw-r--r--   0        0        0      152 2024-04-16 14:38:01.564795 syntrac_sdk-0.0.3/syntrac/sdk/prompts/__init__.py
--rw-r--r--   0        0        0      514 2024-04-16 14:38:01.565056 syntrac_sdk-0.0.3/syntrac/sdk/prompts/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     9274 2024-04-16 14:38:01.565260 syntrac_sdk-0.0.3/syntrac/sdk/prompts/__pycache__/client.cpython-311.pyc
--rw-r--r--   0        0        0     4571 2024-04-16 14:38:01.565471 syntrac_sdk-0.0.3/syntrac/sdk/prompts/__pycache__/model.cpython-311.pyc
--rw-r--r--   0        0        0     1345 2024-04-16 14:38:01.565624 syntrac_sdk-0.0.3/syntrac/sdk/prompts/__pycache__/registry.cpython-311.pyc
--rw-r--r--   0        0        0     5583 2024-04-16 14:38:01.565750 syntrac_sdk-0.0.3/syntrac/sdk/prompts/client.py
--rw-r--r--   0        0        0     1558 2024-04-16 14:38:01.565860 syntrac_sdk-0.0.3/syntrac/sdk/prompts/model.py
--rw-r--r--   0        0        0      408 2024-04-16 14:38:01.565970 syntrac_sdk-0.0.3/syntrac/sdk/prompts/registry.py
--rw-r--r--   0        0        0     2424 2024-04-16 14:38:01.566111 syntrac_sdk-0.0.3/syntrac/sdk/telemetry.py
--rw-r--r--   0        0        0     6148 2024-04-16 14:38:01.566528 syntrac_sdk-0.0.3/syntrac/sdk/tracing/.DS_Store
--rw-r--r--   0        0        0      137 2024-04-16 14:38:01.566632 syntrac_sdk-0.0.3/syntrac/sdk/tracing/__init__.py
--rw-r--r--   0        0        0      406 2024-04-16 14:38:01.566870 syntrac_sdk-0.0.3/syntrac/sdk/tracing/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1969 2024-04-16 14:38:01.567017 syntrac_sdk-0.0.3/syntrac/sdk/tracing/__pycache__/content_allow_list.cpython-311.pyc
--rw-r--r--   0        0        0      877 2024-04-16 14:38:01.567157 syntrac_sdk-0.0.3/syntrac/sdk/tracing/__pycache__/context_manager.cpython-311.pyc
--rw-r--r--   0        0        0    29507 2024-04-16 14:38:01.567374 syntrac_sdk-0.0.3/syntrac/sdk/tracing/__pycache__/tracing.cpython-311.pyc
--rw-r--r--   0        0        0      846 2024-04-16 14:38:01.567502 syntrac_sdk-0.0.3/syntrac/sdk/tracing/content_allow_list.py
--rw-r--r--   0        0        0      297 2024-04-16 14:38:01.567605 syntrac_sdk-0.0.3/syntrac/sdk/tracing/context_manager.py
--rw-r--r--   0        0        0    23992 2024-04-16 14:38:01.567725 syntrac_sdk-0.0.3/syntrac/sdk/tracing/tracing.py
--rw-r--r--   0        0        0      604 2024-04-16 14:38:01.567937 syntrac_sdk-0.0.3/syntrac/sdk/utils/__init__.py
--rw-r--r--   0        0        0     1487 2024-04-16 14:38:01.568145 syntrac_sdk-0.0.3/syntrac/sdk/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2112 2024-04-16 14:38:01.568274 syntrac_sdk-0.0.3/syntrac/sdk/utils/in_memory_span_exporter.py
--rw-r--r--   0        0        0       22 2024-04-16 14:38:01.568401 syntrac_sdk-0.0.3/syntrac/sdk/version.py
--rw-r--r--   0        0        0     3221 1970-01-01 00:00:00.000000 syntrac_sdk-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      606 2024-04-17 07:21:56.906601 syntrac_sdk-0.0.4/README.md
+-rw-r--r--   0        0        0     2072 2024-04-17 07:21:56.924991 syntrac_sdk-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     7767 2024-04-17 07:21:56.909160 syntrac_sdk-0.0.4/syntrac/sdk/__init__.py
+-rw-r--r--   0        0        0      358 2024-04-17 07:21:56.910554 syntrac_sdk-0.0.4/syntrac/sdk/config/__init__.py
+-rw-r--r--   0        0        0     1117 2024-04-17 07:21:56.910886 syntrac_sdk-0.0.4/syntrac/sdk/config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    11612 2024-04-17 07:21:56.911131 syntrac_sdk-0.0.4/syntrac/sdk/decorators/__init__.py
+-rw-r--r--   0        0        0    16396 2024-04-17 07:21:56.911462 syntrac_sdk-0.0.4/syntrac/sdk/decorators/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4393 2024-04-17 07:21:56.911647 syntrac_sdk-0.0.4/syntrac/sdk/fetcher.py
+-rw-r--r--   0        0        0      465 2024-04-17 07:21:56.911771 syntrac_sdk-0.0.4/syntrac/sdk/instruments.py
+-rw-r--r--   0        0        0        0 2024-04-17 07:21:56.912063 syntrac_sdk-0.0.4/syntrac/sdk/metrics/__init__.py
+-rw-r--r--   0        0        0      202 2024-04-17 07:21:56.912312 syntrac_sdk-0.0.4/syntrac/sdk/metrics/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3362 2024-04-17 07:21:56.912531 syntrac_sdk-0.0.4/syntrac/sdk/metrics/__pycache__/metrics.cpython-311.pyc
+-rw-r--r--   0        0        0     2109 2024-04-17 07:21:56.912697 syntrac_sdk-0.0.4/syntrac/sdk/metrics/metrics.py
+-rw-r--r--   0        0        0     2721 2024-04-17 07:21:56.913041 syntrac_sdk-0.0.4/syntrac/sdk/otlp/json/__init__.py
+-rw-r--r--   0        0        0     2638 2024-04-17 07:21:56.913251 syntrac_sdk-0.0.4/syntrac/sdk/otlp/json/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      225 2024-04-17 07:21:56.913377 syntrac_sdk-0.0.4/syntrac/sdk/otlp/json/__pycache__/version.cpython-311.pyc
+-rw-r--r--   0        0        0     7151 2024-04-17 07:21:56.913804 syntrac_sdk-0.0.4/syntrac/sdk/otlp/json/trace_exporter/__init__.py
+-rw-r--r--   0        0        0     9686 2024-04-17 07:21:56.914080 syntrac_sdk-0.0.4/syntrac/sdk/otlp/json/trace_exporter/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      607 2024-04-17 07:21:56.914312 syntrac_sdk-0.0.4/syntrac/sdk/otlp/json/version.py
+-rw-r--r--   0        0        0      152 2024-04-17 07:21:56.914551 syntrac_sdk-0.0.4/syntrac/sdk/prompts/__init__.py
+-rw-r--r--   0        0        0      514 2024-04-17 07:21:56.914794 syntrac_sdk-0.0.4/syntrac/sdk/prompts/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     9274 2024-04-17 07:21:56.914960 syntrac_sdk-0.0.4/syntrac/sdk/prompts/__pycache__/client.cpython-311.pyc
+-rw-r--r--   0        0        0     4571 2024-04-17 07:21:56.915142 syntrac_sdk-0.0.4/syntrac/sdk/prompts/__pycache__/model.cpython-311.pyc
+-rw-r--r--   0        0        0     1345 2024-04-17 07:21:56.915262 syntrac_sdk-0.0.4/syntrac/sdk/prompts/__pycache__/registry.cpython-311.pyc
+-rw-r--r--   0        0        0     5583 2024-04-17 07:21:56.915383 syntrac_sdk-0.0.4/syntrac/sdk/prompts/client.py
+-rw-r--r--   0        0        0     1558 2024-04-17 07:21:56.915497 syntrac_sdk-0.0.4/syntrac/sdk/prompts/model.py
+-rw-r--r--   0        0        0      408 2024-04-17 07:21:56.915609 syntrac_sdk-0.0.4/syntrac/sdk/prompts/registry.py
+-rw-r--r--   0        0        0     2424 2024-04-17 07:21:56.915746 syntrac_sdk-0.0.4/syntrac/sdk/telemetry.py
+-rw-r--r--   0        0        0     6148 2024-04-17 07:21:56.916179 syntrac_sdk-0.0.4/syntrac/sdk/tracing/.DS_Store
+-rw-r--r--   0        0        0      137 2024-04-17 07:21:56.916296 syntrac_sdk-0.0.4/syntrac/sdk/tracing/__init__.py
+-rw-r--r--   0        0        0      406 2024-04-17 07:21:56.916482 syntrac_sdk-0.0.4/syntrac/sdk/tracing/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1969 2024-04-17 07:21:56.916631 syntrac_sdk-0.0.4/syntrac/sdk/tracing/__pycache__/content_allow_list.cpython-311.pyc
+-rw-r--r--   0        0        0      877 2024-04-17 07:21:56.916763 syntrac_sdk-0.0.4/syntrac/sdk/tracing/__pycache__/context_manager.cpython-311.pyc
+-rw-r--r--   0        0        0    29511 2024-04-17 07:21:56.916922 syntrac_sdk-0.0.4/syntrac/sdk/tracing/__pycache__/tracing.cpython-311.pyc
+-rw-r--r--   0        0        0      846 2024-04-17 07:21:56.917060 syntrac_sdk-0.0.4/syntrac/sdk/tracing/content_allow_list.py
+-rw-r--r--   0        0        0      297 2024-04-17 07:21:56.917484 syntrac_sdk-0.0.4/syntrac/sdk/tracing/context_manager.py
+-rw-r--r--   0        0        0    23992 2024-04-17 07:21:56.917636 syntrac_sdk-0.0.4/syntrac/sdk/tracing/tracing.py
+-rw-r--r--   0        0        0      604 2024-04-17 07:21:56.917890 syntrac_sdk-0.0.4/syntrac/sdk/utils/__init__.py
+-rw-r--r--   0        0        0     1487 2024-04-17 07:21:56.918096 syntrac_sdk-0.0.4/syntrac/sdk/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2112 2024-04-17 07:21:56.918255 syntrac_sdk-0.0.4/syntrac/sdk/utils/in_memory_span_exporter.py
+-rw-r--r--   0        0        0       22 2024-04-17 07:21:56.918391 syntrac_sdk-0.0.4/syntrac/sdk/version.py
+-rw-r--r--   0        0        0     3149 1970-01-01 00:00:00.000000 syntrac_sdk-0.0.4/PKG-INFO
```

### Comparing `syntrac_sdk-0.0.3/README.md` & `syntrac_sdk-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.3/pyproject.toml` & `syntrac_sdk-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.coverage.report]
 exclude_lines = [ "if TYPE_CHECKING:" ]
 show_missing = true
 
 [tool.poetry]
 name = "syntrac-sdk"
-version = "0.0.3"
+version = "0.0.4"
 description = "Syntrac Software Development Kit (SDK) for Python"
 authors = [ "Vuong Ngo <vuongngo.pd@gmail.com>" ]
 repository = "https://github.com/syntracAI/syntrac"
 documentation = "https://syntrac.com/docs/openllmetry"
 license = "Apache-2.0"
 readme = "README.md"
 
@@ -20,15 +20,14 @@
   include = "syntrac/sdk"
 
   [tool.poetry.dependencies]
   python = ">=3.9,<4"
   opentelemetry-api = "^1.23.0"
   opentelemetry-sdk = "^1.20.0"
   opentelemetry-exporter-otlp-proto-http = "^1.20.0"
-  opentelemetry-exporter-otlp-proto-grpc = "^1.20.0"
   opentelemetry-instrumentation-requests = "0.44b0"
   opentelemetry-instrumentation-sqlalchemy = "0.44b0"
   opentelemetry-instrumentation-urllib3 = "0.44b0"
   syntrac-opentelemetry-semantic-conventions-ai = "0.0.1"
   syntrac-opentelemetry-instrumentation-openai = "0.0.2"
   syntrac-opentelemetry-instrumentation-anthropic = "0.0.2"
   syntrac-opentelemetry-instrumentation-cohere = "0.0.2"
```

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/__init__.py` & `syntrac_sdk-0.0.4/syntrac/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/config/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.4/syntrac/sdk/config/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/decorators/__init__.py` & `syntrac_sdk-0.0.4/syntrac/sdk/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/decorators/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.4/syntrac/sdk/decorators/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/fetcher.py` & `syntrac_sdk-0.0.4/syntrac/sdk/fetcher.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/metrics/__pycache__/metrics.cpython-311.pyc` & `syntrac_sdk-0.0.4/syntrac/sdk/metrics/__pycache__/metrics.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,23 +1,22 @@
 magic:    0xa70d0d0a
-moddate:  0xcf850766 (Sat Mar 30 03:23:59 2024 UTC)
-files sz: 2346
+moddate:  0x3a731f66 (Wed Apr 17 06:59:06 2024 UTC)
+files sz: 2109
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
       036c046d055a050100640064046c066d075a076d085a080100640064056c
-      096d0a5a0b0100640064056c0c6d0a5a0d0100640064066c0e6d0f5a0f01
-      00020047006407840064086510a6030000ab0300000000000000005a1164
-      096512640a650f65126512660219000000000000000000640b6508660664
-      0c84045a1309006411640e6508640f6514640b65056606641084055a1564
-      0d5300
+      096d0a5a0b0100640064066c0c6d0d5a0d01000200470064078400640865
+      0ea6030000ab0300000000000000005a0f64096510640a650d6510651066
+      0219000000000000000000640b65086606640c84045a1109006411640e65
+      08640f6512640b65056606641084055a13640d5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('metrics',))
                  6 IMPORT_NAME              0 (opentelemetry)
                  8 IMPORT_FROM              1 (metrics)
                 10 STORE_NAME               1 (metrics)
@@ -44,77 +43,70 @@
                 46 STORE_NAME               7 (PeriodicExportingMetricReader)
                 48 IMPORT_FROM              8 (MetricExporter)
                 50 STORE_NAME               8 (MetricExporter)
                 52 POP_TOP
    
      6          54 LOAD_CONST               0 (0)
                 56 LOAD_CONST               5 (('OTLPMetricExporter',))
-                58 IMPORT_NAME              9 (opentelemetry.exporter.otlp.proto.grpc.metric_exporter)
+                58 IMPORT_NAME              9 (opentelemetry.exporter.otlp.proto.http.metric_exporter)
                 60 IMPORT_FROM             10 (OTLPMetricExporter)
-                62 STORE_NAME              11 (GRPCExporter)
+                62 STORE_NAME              11 (HTTPExporter)
                 64 POP_TOP
    
      9          66 LOAD_CONST               0 (0)
-                68 LOAD_CONST               5 (('OTLPMetricExporter',))
-                70 IMPORT_NAME             12 (opentelemetry.exporter.otlp.proto.http.metric_exporter)
-                72 IMPORT_FROM             10 (OTLPMetricExporter)
-                74 STORE_NAME              13 (HTTPExporter)
+                68 LOAD_CONST               6 (('Dict',))
+                70 IMPORT_NAME             12 (typing)
+                72 IMPORT_FROM             13 (Dict)
+                74 STORE_NAME              13 (Dict)
                 76 POP_TOP
    
-    12          78 LOAD_CONST               0 (0)
-                80 LOAD_CONST               6 (('Dict',))
-                82 IMPORT_NAME             14 (typing)
-                84 IMPORT_FROM             15 (Dict)
-                86 STORE_NAME              15 (Dict)
-                88 POP_TOP
-   
-    15          90 PUSH_NULL
-                92 LOAD_BUILD_CLASS
-                94 LOAD_CONST               7 (<code object MetricsWrapper, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/metrics/metrics.py", line 15>)
-                96 MAKE_FUNCTION            0
-                98 LOAD_CONST               8 ('MetricsWrapper')
-               100 LOAD_NAME               16 (object)
-               102 PRECALL                  3
-               106 CALL                     3
-               116 STORE_NAME              17 (MetricsWrapper)
-   
-    50         118 LOAD_CONST               9 ('endpoint')
-               120 LOAD_NAME               18 (str)
-               122 LOAD_CONST              10 ('headers')
-               124 LOAD_NAME               15 (Dict)
-               126 LOAD_NAME               18 (str)
-               128 LOAD_NAME               18 (str)
-               130 BUILD_TUPLE              2
-               132 BINARY_SUBSCR
-               142 LOAD_CONST              11 ('return')
-               144 LOAD_NAME                8 (MetricExporter)
-               146 BUILD_TUPLE              6
-               148 LOAD_CONST              12 (<code object init_metrics_exporter, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/metrics/metrics.py", line 50>)
-               150 MAKE_FUNCTION            4 (annotations)
-               152 STORE_NAME              19 (init_metrics_exporter)
-   
-    58         154 NOP
-   
-    57         156 LOAD_CONST              17 ((None,))
-               158 LOAD_CONST              14 ('exporter')
-               160 LOAD_NAME                8 (MetricExporter)
-               162 LOAD_CONST              15 ('resource_attributes')
-   
-    58         164 LOAD_NAME               20 (dict)
-   
-    57         166 LOAD_CONST              11 ('return')
-   
-    58         168 LOAD_NAME                5 (MeterProvider)
-   
-    57         170 BUILD_TUPLE              6
-               172 LOAD_CONST              16 (<code object init_metrics_provider, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/metrics/metrics.py", line 57>)
-               174 MAKE_FUNCTION            5 (defaults, annotations)
-               176 STORE_NAME              21 (init_metrics_provider)
-               178 LOAD_CONST              13 (None)
-               180 RETURN_VALUE
+    12          78 PUSH_NULL
+                80 LOAD_BUILD_CLASS
+                82 LOAD_CONST               7 (<code object MetricsWrapper, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/metrics/metrics.py", line 12>)
+                84 MAKE_FUNCTION            0
+                86 LOAD_CONST               8 ('MetricsWrapper')
+                88 LOAD_NAME               14 (object)
+                90 PRECALL                  3
+                94 CALL                     3
+               104 STORE_NAME              15 (MetricsWrapper)
+   
+    47         106 LOAD_CONST               9 ('endpoint')
+               108 LOAD_NAME               16 (str)
+               110 LOAD_CONST              10 ('headers')
+               112 LOAD_NAME               13 (Dict)
+               114 LOAD_NAME               16 (str)
+               116 LOAD_NAME               16 (str)
+               118 BUILD_TUPLE              2
+               120 BINARY_SUBSCR
+               130 LOAD_CONST              11 ('return')
+               132 LOAD_NAME                8 (MetricExporter)
+               134 BUILD_TUPLE              6
+               136 LOAD_CONST              12 (<code object init_metrics_exporter, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/metrics/metrics.py", line 47>)
+               138 MAKE_FUNCTION            4 (annotations)
+               140 STORE_NAME              17 (init_metrics_exporter)
+   
+    52         142 NOP
+   
+    51         144 LOAD_CONST              17 ((None,))
+               146 LOAD_CONST              14 ('exporter')
+               148 LOAD_NAME                8 (MetricExporter)
+               150 LOAD_CONST              15 ('resource_attributes')
+   
+    52         152 LOAD_NAME               18 (dict)
+   
+    51         154 LOAD_CONST              11 ('return')
+   
+    52         156 LOAD_NAME                5 (MeterProvider)
+   
+    51         158 BUILD_TUPLE              6
+               160 LOAD_CONST              16 (<code object init_metrics_provider, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/metrics/metrics.py", line 51>)
+               162 MAKE_FUNCTION            5 (defaults, annotations)
+               164 STORE_NAME              19 (init_metrics_provider)
+               166 LOAD_CONST              13 (None)
+               168 RETURN_VALUE
    consts
       0
       ('metrics',)
       ('Resource',)
       ('MeterProvider',)
       ('PeriodicExportingMetricReader', 'MetricExporter')
       ('OTLPMetricExporter',)
@@ -129,88 +121,88 @@
             025a066507650564033c00000069005a0865096507650766021900000000
             0000000000650564043c00000064096405650a6406640066048800660164
             07840d5a0b650c6401650464036507640465096507650766021900000000
             000000000064066402660864088404a6000000ab0000000000000000005a
             0d880078015a0e5300
                        0 MAKE_CELL                0 (__class__)
          
-          15           2 RESUME                   0
+          12           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('MetricsWrapper')
                       10 STORE_NAME               2 (__qualname__)
                       12 SETUP_ANNOTATIONS
          
-          16          14 BUILD_MAP                0
+          13          14 BUILD_MAP                0
                       16 STORE_NAME               3 (resource_attributes)
                       18 LOAD_NAME                4 (dict)
                       20 LOAD_NAME                5 (__annotations__)
                       22 LOAD_CONST               1 ('resource_attributes')
                       24 STORE_SUBSCR
          
-          17          28 LOAD_CONST               2 (None)
+          14          28 LOAD_CONST               2 (None)
                       30 STORE_NAME               6 (endpoint)
                       32 LOAD_NAME                7 (str)
                       34 LOAD_NAME                5 (__annotations__)
                       36 LOAD_CONST               3 ('endpoint')
                       38 STORE_SUBSCR
          
-          19          42 BUILD_MAP                0
+          16          42 BUILD_MAP                0
                       44 STORE_NAME               8 (headers)
                       46 LOAD_NAME                9 (Dict)
                       48 LOAD_NAME                7 (str)
                       50 LOAD_NAME                7 (str)
                       52 BUILD_TUPLE              2
                       54 BINARY_SUBSCR
                       64 LOAD_NAME                5 (__annotations__)
                       66 LOAD_CONST               4 ('headers')
                       68 STORE_SUBSCR
          
-          21          72 LOAD_CONST               9 ((None,))
+          18          72 LOAD_CONST               9 ((None,))
                       74 LOAD_CONST               5 ('exporter')
                       76 LOAD_NAME               10 (MetricExporter)
                       78 LOAD_CONST               6 ('return')
                       80 LOAD_CONST               0 ('MetricsWrapper')
                       82 BUILD_TUPLE              4
                       84 LOAD_CLOSURE             0 (__class__)
                       86 BUILD_TUPLE              1
-                      88 LOAD_CONST               7 (<code object __new__, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/metrics/metrics.py", line 21>)
+                      88 LOAD_CONST               7 (<code object __new__, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/metrics/metrics.py", line 18>)
                       90 MAKE_FUNCTION           13 (defaults, annotations, closure)
                       92 STORE_NAME              11 (__new__)
          
-          39          94 LOAD_NAME               12 (staticmethod)
+          36          94 LOAD_NAME               12 (staticmethod)
          
-          40          96 LOAD_CONST               1 ('resource_attributes')
+          37          96 LOAD_CONST               1 ('resource_attributes')
          
-          41          98 LOAD_NAME                4 (dict)
+          38          98 LOAD_NAME                4 (dict)
          
-          40         100 LOAD_CONST               3 ('endpoint')
+          37         100 LOAD_CONST               3 ('endpoint')
          
-          42         102 LOAD_NAME                7 (str)
+          39         102 LOAD_NAME                7 (str)
          
-          40         104 LOAD_CONST               4 ('headers')
+          37         104 LOAD_CONST               4 ('headers')
          
-          43         106 LOAD_NAME                9 (Dict)
+          40         106 LOAD_NAME                9 (Dict)
                      108 LOAD_NAME                7 (str)
                      110 LOAD_NAME                7 (str)
                      112 BUILD_TUPLE              2
                      114 BINARY_SUBSCR
          
-          40         124 LOAD_CONST               6 ('return')
+          37         124 LOAD_CONST               6 ('return')
          
-          44         126 LOAD_CONST               2 (None)
+          41         126 LOAD_CONST               2 (None)
          
-          40         128 BUILD_TUPLE              8
-                     130 LOAD_CONST               8 (<code object set_static_params, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/metrics/metrics.py", line 39>)
+          37         128 BUILD_TUPLE              8
+                     130 LOAD_CONST               8 (<code object set_static_params, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/metrics/metrics.py", line 36>)
                      132 MAKE_FUNCTION            4 (annotations)
          
-          39         134 PRECALL                  0
+          36         134 PRECALL                  0
                      138 CALL                     0
          
-          40         148 STORE_NAME              13 (set_static_params)
+          37         148 STORE_NAME              13 (set_static_params)
                      150 LOAD_CLOSURE             0 (__class__)
                      152 COPY                     1
                      154 STORE_NAME              14 (__classcell__)
                      156 RETURN_VALUE
          consts
             'MetricsWrapper'
             'resource_attributes'
@@ -235,192 +227,164 @@
                   0000006a070000000000000000a6020000ab0200000000000000007c025f
                   0800000000000000007413000000000000000000007c026a080000000000
                   0000007404000000000000000000006a0a0000000000000000a6020000ab
                   0200000000000000007c025f0b00000000000000007c006a040000000000
                   0000005300
                              0 COPY_FREE_VARS           1
                
-                21           2 RESUME                   0
+                18           2 RESUME                   0
                
-                22           4 LOAD_GLOBAL              1 (NULL + hasattr)
+                19           4 LOAD_GLOBAL              1 (NULL + hasattr)
                             16 LOAD_FAST                0 (cls)
                             18 LOAD_CONST               1 ('instance')
                             20 PRECALL                  2
                             24 CALL                     2
                             34 POP_JUMP_FORWARD_IF_TRUE   142 (to 320)
                
-                23          36 LOAD_GLOBAL              3 (NULL + super)
+                20          36 LOAD_GLOBAL              3 (NULL + super)
                             48 LOAD_GLOBAL              4 (MetricsWrapper)
                             60 LOAD_FAST                0 (cls)
                             62 PRECALL                  2
                             66 CALL                     2
                             76 LOAD_METHOD              3 (__new__)
                             98 LOAD_FAST                0 (cls)
                            100 PRECALL                  1
                            104 CALL                     1
                            114 COPY                     1
                            116 STORE_FAST               2 (obj)
                            118 LOAD_FAST                0 (cls)
                            120 STORE_ATTR               4 (instance)
                
-                24         130 LOAD_GLOBAL              4 (MetricsWrapper)
+                21         130 LOAD_GLOBAL              4 (MetricsWrapper)
                            142 LOAD_ATTR                5 (endpoint)
                            152 POP_JUMP_FORWARD_IF_TRUE     2 (to 158)
                
-                25         154 LOAD_FAST                2 (obj)
+                22         154 LOAD_FAST                2 (obj)
                            156 RETURN_VALUE
                
-                28     >>  158 LOAD_FAST                1 (exporter)
+                25     >>  158 LOAD_FAST                1 (exporter)
                            160 POP_JUMP_FORWARD_IF_FALSE     2 (to 166)
                            162 LOAD_FAST                1 (exporter)
                            164 JUMP_FORWARD            35 (to 236)
                
-                29     >>  166 LOAD_GLOBAL             13 (NULL + init_metrics_exporter)
+                26     >>  166 LOAD_GLOBAL             13 (NULL + init_metrics_exporter)
                
-                30         178 LOAD_GLOBAL              4 (MetricsWrapper)
+                27         178 LOAD_GLOBAL              4 (MetricsWrapper)
                            190 LOAD_ATTR                5 (endpoint)
                            200 LOAD_GLOBAL              4 (MetricsWrapper)
                            212 LOAD_ATTR                7 (headers)
                
-                29         222 PRECALL                  2
+                26         222 PRECALL                  2
                            226 CALL                     2
                
-                27     >>  236 LOAD_FAST                2 (obj)
+                24     >>  236 LOAD_FAST                2 (obj)
                            238 STORE_ATTR               8 (_MetricsWrapper__metrics_exporter)
                
-                34         248 LOAD_GLOBAL             19 (NULL + init_metrics_provider)
+                31         248 LOAD_GLOBAL             19 (NULL + init_metrics_provider)
                            260 LOAD_FAST                2 (obj)
                            262 LOAD_ATTR                8 (_MetricsWrapper__metrics_exporter)
                
-                35         272 LOAD_GLOBAL              4 (MetricsWrapper)
+                32         272 LOAD_GLOBAL              4 (MetricsWrapper)
                            284 LOAD_ATTR               10 (resource_attributes)
                
-                34         294 PRECALL                  2
+                31         294 PRECALL                  2
                            298 CALL                     2
                            308 LOAD_FAST                2 (obj)
                            310 STORE_ATTR              11 (_MetricsWrapper__metrics_provider)
                
-                37     >>  320 LOAD_FAST                0 (cls)
+                34     >>  320 LOAD_FAST                0 (cls)
                            322 LOAD_ATTR                4 (instance)
                            332 RETURN_VALUE
                consts
                   None
                   'instance'
                names      ('hasattr', 'super', 'MetricsWrapper', '__new__', 'instance', 'endpoint', 'init_metrics_exporter', 'headers', '_MetricsWrapper__metrics_exporter', 'init_metrics_provider', 'resource_attributes', '_MetricsWrapper__metrics_provider')
                varnames   ('cls', 'exporter', 'obj')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/metrics/metrics.py'
                name       '__new__'
-               firstlineno 21
+               firstlineno 18
                lnotab 0x040120015e011801040308010c012cff0efe0c07180116ff1a03
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 2
                flags     : 3
                code
                   0x97007c007400000000000000000000005f0100000000000000007c0174
                   00000000000000000000005f0200000000000000007c0274000000000000
                   00000000005f03000000000000000064005300
-                39           0 RESUME                   0
+                36           0 RESUME                   0
                
-                45           2 LOAD_FAST                0 (resource_attributes)
+                42           2 LOAD_FAST                0 (resource_attributes)
                              4 LOAD_GLOBAL              0 (MetricsWrapper)
                             16 STORE_ATTR               1 (resource_attributes)
                
-                46          26 LOAD_FAST                1 (endpoint)
+                43          26 LOAD_FAST                1 (endpoint)
                             28 LOAD_GLOBAL              0 (MetricsWrapper)
                             40 STORE_ATTR               2 (endpoint)
                
-                47          50 LOAD_FAST                2 (headers)
+                44          50 LOAD_FAST                2 (headers)
                             52 LOAD_GLOBAL              0 (MetricsWrapper)
                             64 STORE_ATTR               3 (headers)
                             74 LOAD_CONST               0 (None)
                             76 RETURN_VALUE
                consts
                   None
                names      ('MetricsWrapper', 'resource_attributes', 'endpoint', 'headers')
                varnames   ('resource_attributes', 'endpoint', 'headers')
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/metrics/metrics.py'
                name       'set_static_params'
-               firstlineno 39
+               firstlineno 36
                lnotab 0x020618011801
             (None,)
          names      ('__name__', '__module__', '__qualname__', 'resource_attributes', 'dict', '__annotations__', 'endpoint', 'str', 'headers', 'Dict', 'MetricExporter', '__new__', 'staticmethod', 'set_static_params', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/metrics/metrics.py'
          name       'MetricsWrapper'
-         firstlineno 15
+         firstlineno 12
          lnotab
             0x0e010e010e021e0216120201020102ff020202fe020312fd020402fc06
             ff0e01
       'MetricsWrapper'
       'endpoint'
       'headers'
       'return'
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
-            0x970064017c00a0000000000000000000000000000000000000000000a6
-            000000ab0000000000000000007600731664027c00a00000000000000000
-            00000000000000000000000000a6000000ab000000000000000000760072
-            107403000000000000000000007c00ac03a6010000ab0100000000000000
-            0053007405000000000000000000007c00ac03a6010000ab010000000000
+            0x97007401000000000000000000007c00ac01a6010000ab010000000000
             0000005300
-          50           0 RESUME                   0
+          47           0 RESUME                   0
          
-          51           2 LOAD_CONST               1 ('http')
-                       4 LOAD_FAST                0 (endpoint)
-                       6 LOAD_METHOD              0 (lower)
-                      28 PRECALL                  0
-                      32 CALL                     0
-                      42 CONTAINS_OP              0
-                      44 POP_JUMP_FORWARD_IF_TRUE    22 (to 90)
-                      46 LOAD_CONST               2 ('https')
-                      48 LOAD_FAST                0 (endpoint)
-                      50 LOAD_METHOD              0 (lower)
-                      72 PRECALL                  0
-                      76 CALL                     0
-                      86 CONTAINS_OP              0
-                      88 POP_JUMP_FORWARD_IF_FALSE    16 (to 122)
-         
-          52     >>   90 LOAD_GLOBAL              3 (NULL + HTTPExporter)
-                     102 LOAD_FAST                0 (endpoint)
-                     104 KW_NAMES                 3
-                     106 PRECALL                  1
-                     110 CALL                     1
-                     120 RETURN_VALUE
-         
-          54     >>  122 LOAD_GLOBAL              5 (NULL + GRPCExporter)
-                     134 LOAD_FAST                0 (endpoint)
-                     136 KW_NAMES                 3
-                     138 PRECALL                  1
-                     142 CALL                     1
-                     152 RETURN_VALUE
+          48           2 LOAD_GLOBAL              1 (NULL + HTTPExporter)
+                      14 LOAD_FAST                0 (endpoint)
+                      16 KW_NAMES                 1
+                      18 PRECALL                  1
+                      22 CALL                     1
+                      32 RETURN_VALUE
          consts
             None
-            'http'
-            'https'
             ('endpoint',)
-         names      ('lower', 'HTTPExporter', 'GRPCExporter')
+         names      ('HTTPExporter',)
          varnames   ('endpoint', 'headers')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/metrics/metrics.py'
          name       'init_metrics_exporter'
-         firstlineno 50
-         lnotab 0x020158012002
+         firstlineno 47
+         lnotab 0x0201
       None
       'exporter'
       'resource_attributes'
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 4
@@ -429,69 +393,69 @@
             0x97007c0172147401000000000000000000006a0100000000000000007c
             01a6010000ab0100000000000000006e127401000000000000000000006a
             010000000000000000a6000000ab0000000000000000007d027405000000
             000000000000007c00a6010000ab0100000000000000007d037407000000
             000000000000007c0367017c02ac01a6020000ab0200000000000000007d
             047409000000000000000000006a0500000000000000007c04a6010000ab
             01000000000000000001007c045300
-          57           0 RESUME                   0
+          51           0 RESUME                   0
          
-          59           2 LOAD_FAST                1 (resource_attributes)
+          53           2 LOAD_FAST                1 (resource_attributes)
                        4 POP_JUMP_FORWARD_IF_FALSE    20 (to 46)
                        6 LOAD_GLOBAL              1 (NULL + Resource)
                       18 LOAD_ATTR                1 (create)
                       28 LOAD_FAST                1 (resource_attributes)
                       30 PRECALL                  1
                       34 CALL                     1
                       44 JUMP_FORWARD            18 (to 82)
                  >>   46 LOAD_GLOBAL              1 (NULL + Resource)
                       58 LOAD_ATTR                1 (create)
                       68 PRECALL                  0
                       72 CALL                     0
                  >>   82 STORE_FAST               2 (resource)
          
-          60          84 LOAD_GLOBAL              5 (NULL + PeriodicExportingMetricReader)
+          54          84 LOAD_GLOBAL              5 (NULL + PeriodicExportingMetricReader)
                       96 LOAD_FAST                0 (exporter)
                       98 PRECALL                  1
                      102 CALL                     1
                      112 STORE_FAST               3 (reader)
          
-          61         114 LOAD_GLOBAL              7 (NULL + MeterProvider)
+          55         114 LOAD_GLOBAL              7 (NULL + MeterProvider)
                      126 LOAD_FAST                3 (reader)
                      128 BUILD_LIST               1
                      130 LOAD_FAST                2 (resource)
                      132 KW_NAMES                 1
                      134 PRECALL                  2
                      138 CALL                     2
                      148 STORE_FAST               4 (provider)
          
-          62         150 LOAD_GLOBAL              9 (NULL + metrics)
+          56         150 LOAD_GLOBAL              9 (NULL + metrics)
                      162 LOAD_ATTR                5 (set_meter_provider)
                      172 LOAD_FAST                4 (provider)
                      174 PRECALL                  1
                      178 CALL                     1
                      188 POP_TOP
          
-          63         190 LOAD_FAST                4 (provider)
+          57         190 LOAD_FAST                4 (provider)
                      192 RETURN_VALUE
          consts
             None
             ('metric_readers', 'resource')
          names      ('Resource', 'create', 'PeriodicExportingMetricReader', 'MeterProvider', 'metrics', 'set_meter_provider')
          varnames   ('exporter', 'resource_attributes', 'resource', 'reader', 'provider')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/metrics/metrics.py'
          name       'init_metrics_provider'
-         firstlineno 57
+         firstlineno 51
          lnotab 0x020252011e0124012801
       (None,)
-   names      ('opentelemetry', 'metrics', 'opentelemetry.sdk.resources', 'Resource', 'opentelemetry.sdk.metrics', 'MeterProvider', 'opentelemetry.sdk.metrics.export', 'PeriodicExportingMetricReader', 'MetricExporter', 'opentelemetry.exporter.otlp.proto.grpc.metric_exporter', 'OTLPMetricExporter', 'GRPCExporter', 'opentelemetry.exporter.otlp.proto.http.metric_exporter', 'HTTPExporter', 'typing', 'Dict', 'object', 'MetricsWrapper', 'str', 'init_metrics_exporter', 'dict', 'init_metrics_provider')
+   names      ('opentelemetry', 'metrics', 'opentelemetry.sdk.resources', 'Resource', 'opentelemetry.sdk.metrics', 'MeterProvider', 'opentelemetry.sdk.metrics.export', 'PeriodicExportingMetricReader', 'MetricExporter', 'opentelemetry.exporter.otlp.proto.http.metric_exporter', 'OTLPMetricExporter', 'HTTPExporter', 'typing', 'Dict', 'object', 'MetricsWrapper', 'str', 'init_metrics_exporter', 'dict', 'init_metrics_provider')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/metrics/metrics.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c010c010c0210010c030c030c031c23240802ff080102ff02
-      0102ff
+      0x00ff02010c010c010c0210010c030c031c23240502ff080102ff020102
+      ff
```

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/metrics/metrics.py` & `syntrac_sdk-0.0.4/syntrac/sdk/metrics/metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from opentelemetry import metrics
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.metrics import MeterProvider
 
 from opentelemetry.sdk.metrics.export import PeriodicExportingMetricReader, MetricExporter
-from opentelemetry.exporter.otlp.proto.grpc.metric_exporter import (
-    OTLPMetricExporter as GRPCExporter
-)
 from opentelemetry.exporter.otlp.proto.http.metric_exporter import (
     OTLPMetricExporter as HTTPExporter
 )
 from typing import Dict
 
 
 class MetricsWrapper(object):
@@ -44,18 +41,15 @@
     ) -> None:
         MetricsWrapper.resource_attributes = resource_attributes
         MetricsWrapper.endpoint = endpoint
         MetricsWrapper.headers = headers
 
 
 def init_metrics_exporter(endpoint: str, headers: Dict[str, str]) -> MetricExporter:
-    if "http" in endpoint.lower() or "https" in endpoint.lower():
-        return HTTPExporter(endpoint=endpoint)
-    else:
-        return GRPCExporter(endpoint=endpoint)
+    return HTTPExporter(endpoint=endpoint)
 
 
 def init_metrics_provider(exporter: MetricExporter,
                           resource_attributes: dict = None) -> MeterProvider:
     resource = Resource.create(resource_attributes) if resource_attributes else Resource.create()
     reader = PeriodicExportingMetricReader(exporter)
     provider = MeterProvider(metric_readers=[reader], resource=resource)
```

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/otlp/json/__init__.py` & `syntrac_sdk-0.0.4/syntrac/sdk/otlp/json/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/otlp/json/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.4/syntrac/sdk/otlp/json/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/otlp/json/trace_exporter/__init__.py` & `syntrac_sdk-0.0.4/syntrac/sdk/otlp/json/trace_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/otlp/json/trace_exporter/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.4/syntrac/sdk/otlp/json/trace_exporter/__pycache__/__init__.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xcf850766 (Sat Mar 30 03:23:59 2024 UTC)
-files sz: 7147
+moddate:  0xae090966 (Sun Mar 31 06:58:54 2024 UTC)
+files sz: 7151
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
@@ -125,15 +125,15 @@
                178 IMPORT_NAME             31 (opentelemetry.sdk.trace)
                180 IMPORT_FROM             32 (ReadableSpan)
                182 STORE_NAME              32 (ReadableSpan)
                184 POP_TOP
    
     41         186 LOAD_CONST               0 (0)
                188 LOAD_CONST              10 (('_OTLP_HTTP_HEADERS', 'DEFAULT_ENDPOINT', 'Compression'))
-               190 IMPORT_NAME             33 (syntrac.otlp.json)
+               190 IMPORT_NAME             33 (syntrac.sdk.otlp.json)
                192 IMPORT_FROM             34 (_OTLP_HTTP_HEADERS)
                194 STORE_NAME              34 (_OTLP_HTTP_HEADERS)
                196 IMPORT_FROM             35 (DEFAULT_ENDPOINT)
                198 STORE_NAME              35 (DEFAULT_ENDPOINT)
                200 IMPORT_FROM             36 (Compression)
                202 STORE_NAME              36 (Compression)
                204 POP_TOP
@@ -172,35 +172,35 @@
                290 LOAD_NAME               40 (__name__)
                292 PRECALL                  1
                296 CALL                     1
                306 STORE_NAME              47 (logger)
    
     58         308 PUSH_NULL
                310 LOAD_BUILD_CLASS
-               312 LOAD_CONST              15 (<code object OTLPSpanExporter, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/otlp/json/trace_exporter/__init__.py", line 58>)
+               312 LOAD_CONST              15 (<code object OTLPSpanExporter, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 58>)
                314 MAKE_FUNCTION            0
                316 LOAD_CONST              16 ('OTLPSpanExporter')
                318 LOAD_NAME               29 (SpanExporter)
                320 PRECALL                  3
                324 CALL                     3
                334 STORE_NAME              48 (OTLPSpanExporter)
    
    189         336 LOAD_CONST              17 ('return')
                338 LOAD_NAME               36 (Compression)
                340 BUILD_TUPLE              2
-               342 LOAD_CONST              18 (<code object _compression_from_env, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/otlp/json/trace_exporter/__init__.py", line 189>)
+               342 LOAD_CONST              18 (<code object _compression_from_env, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 189>)
                344 MAKE_FUNCTION            4 (annotations)
                346 STORE_NAME              49 (_compression_from_env)
    
    201         348 LOAD_CONST              19 ('endpoint')
                350 LOAD_NAME               50 (str)
                352 LOAD_CONST              17 ('return')
                354 LOAD_NAME               50 (str)
                356 BUILD_TUPLE              4
-               358 LOAD_CONST              20 (<code object _append_trace_path, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/otlp/json/trace_exporter/__init__.py", line 201>)
+               358 LOAD_CONST              20 (<code object _append_trace_path, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 201>)
                360 MAKE_FUNCTION            4 (annotations)
                362 STORE_NAME              51 (_append_trace_path)
                364 LOAD_CONST               1 (None)
                366 RETURN_VALUE
    consts
       0
       None
@@ -289,59 +289,59 @@
          
           66         122 LOAD_NAME                3 (Optional)
                      124 LOAD_NAME                8 (requests)
                      126 LOAD_ATTR                9 (Session)
                      136 BINARY_SUBSCR
          
           59         146 BUILD_TUPLE             12
-                     148 LOAD_CONST               8 (<code object __init__, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/otlp/json/trace_exporter/__init__.py", line 59>)
+                     148 LOAD_CONST               8 (<code object __init__, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 59>)
                      150 MAKE_FUNCTION            5 (defaults, annotations)
                      152 STORE_NAME              10 (__init__)
          
           99         154 LOAD_CONST               9 ('spans')
                      156 LOAD_NAME               11 (Sequence)
                      158 LOAD_NAME               12 (ReadableSpan)
                      160 BINARY_SUBSCR
                      170 LOAD_CONST              10 ('return')
                      172 LOAD_NAME               13 (SpanExportResult)
                      174 BUILD_TUPLE              4
-                     176 LOAD_CONST              11 (<code object export, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/otlp/json/trace_exporter/__init__.py", line 99>)
+                     176 LOAD_CONST              11 (<code object export, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 99>)
                      178 MAKE_FUNCTION            4 (annotations)
                      180 STORE_NAME              14 (export)
          
          120         182 LOAD_CONST              21 (('return', None))
-                     184 LOAD_CONST              12 (<code object shutdown, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/otlp/json/trace_exporter/__init__.py", line 120>)
+                     184 LOAD_CONST              12 (<code object shutdown, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 120>)
                      186 MAKE_FUNCTION            4 (annotations)
                      188 STORE_NAME              15 (shutdown)
          
          127         190 LOAD_CONST              22 ((30000,))
                      192 LOAD_CONST              14 ('timeout_millis')
                      194 LOAD_NAME                6 (int)
                      196 LOAD_CONST              10 ('return')
                      198 LOAD_NAME               16 (bool)
                      200 BUILD_TUPLE              4
-                     202 LOAD_CONST              15 (<code object force_flush, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/otlp/json/trace_exporter/__init__.py", line 127>)
+                     202 LOAD_CONST              15 (<code object force_flush, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 127>)
                      204 MAKE_FUNCTION            5 (defaults, annotations)
                      206 STORE_NAME              17 (force_flush)
          
          131         208 LOAD_CONST              16 ('serialized_data')
                      210 LOAD_NAME                4 (str)
                      212 BUILD_TUPLE              2
-                     214 LOAD_CONST              17 (<code object _export, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/otlp/json/trace_exporter/__init__.py", line 131>)
+                     214 LOAD_CONST              17 (<code object _export, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 131>)
                      216 MAKE_FUNCTION            4 (annotations)
                      218 STORE_NAME              18 (_export)
          
          148         220 LOAD_CONST              18 ('sdk_spans')
                      222 LOAD_NAME               11 (Sequence)
                      224 LOAD_NAME               12 (ReadableSpan)
                      226 BINARY_SUBSCR
                      236 LOAD_CONST              10 ('return')
                      238 LOAD_NAME                4 (str)
                      240 BUILD_TUPLE              4
-                     242 LOAD_CONST              19 (<code object _serialize_spans, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/otlp/json/trace_exporter/__init__.py", line 148>)
+                     242 LOAD_CONST              19 (<code object _serialize_spans, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 148>)
                      244 MAKE_FUNCTION            4 (annotations)
                      246 STORE_NAME              19 (_serialize_spans)
                      248 LOAD_CONST               1 (None)
                      250 RETURN_VALUE
          consts
             'OTLPSpanExporter'
             None
@@ -552,15 +552,15 @@
                   ''
                   'Content-Encoding'
                   False
                names      ('environ', 'get', 'OTEL_EXPORTER_OTLP_TRACES_ENDPOINT', '_append_trace_path', 'OTEL_EXPORTER_OTLP_ENDPOINT', 'DEFAULT_ENDPOINT', '_endpoint', 'OTEL_EXPORTER_OTLP_TRACES_CERTIFICATE', 'OTEL_EXPORTER_OTLP_CERTIFICATE', '_certificate_file', 'OTEL_EXPORTER_OTLP_TRACES_HEADERS', 'OTEL_EXPORTER_OTLP_HEADERS', 'parse_env_headers', '_headers', 'int', 'OTEL_EXPORTER_OTLP_TRACES_TIMEOUT', 'OTEL_EXPORTER_OTLP_TIMEOUT', 'DEFAULT_TIMEOUT', '_timeout', '_compression_from_env', '_compression', 'requests', 'Session', '_session', 'headers', 'update', '_OTLP_HTTP_HEADERS', 'Compression', 'NoCompression', 'value', '_shutdown')
                varnames   ('self', 'endpoint', 'certificate_file', 'headers', 'timeout', 'compression', 'session', 'headers_string')
                freevars   ()
                cellvars   ()
-               filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/otlp/json/trace_exporter/__init__.py'
+               filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py'
                name       '__init__'
                firstlineno 59
                lnotab
                   0x02091a010c010c013cff0efe1a061a010c0132fe1a0416010c0132fe10
                   042c01100116010c013cfe0eff1a062a0134014801480126012c011aff10
                   03
             'spans'
@@ -643,15 +643,15 @@
                   None
                   'Exporter already shutdown, ignoring batch'
                   'Failed to export batch code: %s, reason: %s'
                names      ('_shutdown', 'logger', 'warning', 'SpanExportResult', 'FAILURE', '_serialize_spans', '_export', 'ok', 'SUCCESS', '_logger', 'error', 'status_code', 'text')
                varnames   ('self', 'spans', 'serialized_data', 'resp')
                freevars   ()
                cellvars   ()
-               filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/otlp/json/trace_exporter/__init__.py'
+               filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py'
                name       'export'
                firstlineno 99
                lnotab 0x02030e01340118022a012a030e011802220102010c010cfd1005
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
@@ -694,15 +694,15 @@
                   None
                   'Exporter already shutdown, ignoring call'
                   True
                names      ('_shutdown', 'logger', 'warning', '_session', 'close')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/otlp/json/trace_exporter/__init__.py'
+               filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py'
                name       'shutdown'
                firstlineno 120
                lnotab 0x02010e01340104013201
             30000
             'timeout_millis'
             code
                argcount  : 2
@@ -717,15 +717,15 @@
                consts
                   'Nothing is buffered in this exporter, so this method does nothing.'
                   True
                names      ()
                varnames   ('self', 'timeout_millis')
                freevars   ()
                cellvars   ()
-               filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/otlp/json/trace_exporter/__init__.py'
+               filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py'
                name       'force_flush'
                firstlineno 127
                lnotab 0x0202
             'serialized_data'
             code
                argcount  : 2
                nlocals   : 5
@@ -853,15 +853,15 @@
                   'w'
                   ('fileobj', 'mode')
                   ('url', 'data', 'verify', 'timeout')
                names      ('_compression', 'Compression', 'Gzip', 'BytesIO', 'gzip', 'GzipFile', 'write', 'getvalue', 'Deflate', 'zlib', 'compress', 'bytes', '_session', 'post', '_endpoint', '_certificate_file', '_timeout')
                varnames   ('self', 'serialized_data', 'data', 'gzip_data', 'gzip_stream')
                freevars   ()
                cellvars   ()
-               filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/otlp/json/trace_exporter/__init__.py'
+               filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py'
                name       '_export'
                firstlineno 131
                lnotab
                   0x020104012a011c012e012aff2e022a012a01420222010c0102010c010c
                   fc
             'sdk_spans'
             code
@@ -888,15 +888,15 @@
                   000000000000000000a6000000ab000000000000000000a6010000ab0100
                   000000000000007c0864049c02a6010000ab01000000000000000001008c
                   a464057c0669017d09740b000000000000000000006a0800000000000000
                   007c09a6010000ab0100000000000000005300
                148           0 RESUME                   0
                
                160           2 LOAD_GLOBAL              1 (NULL + defaultdict)
-                            14 LOAD_CONST               1 (<code object <lambda>, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/otlp/json/trace_exporter/__init__.py", line 160>)
+                            14 LOAD_CONST               1 (<code object <lambda>, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 160>)
                             16 MAKE_FUNCTION            0
                             18 PRECALL                  1
                             22 CALL                     1
                             32 STORE_FAST               2 (sdk_resource_spans)
                
                161          34 LOAD_FAST                1 (sdk_spans)
                             36 GET_ITER
@@ -957,15 +957,15 @@
                            292 LOAD_FAST                5 (sdk_instrumentation)
                            294 LOAD_METHOD              7 (to_json)
                            316 PRECALL                  0
                            320 CALL                     0
                            330 PRECALL                  1
                            334 CALL                     1
                
-               173         344 LOAD_CONST               2 (<code object <listcomp>, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/otlp/json/trace_exporter/__init__.py", line 173>)
+               173         344 LOAD_CONST               2 (<code object <listcomp>, file "/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py", line 173>)
                            346 MAKE_FUNCTION            0
                            348 LOAD_FAST                1 (sdk_spans)
                            350 GET_ITER
                            352 PRECALL                  0
                            356 CALL                     0
                
                171         366 LOAD_CONST               3 (('scope', 'spans'))
@@ -1028,15 +1028,15 @@
                                   40 RETURN_VALUE
                      consts
                         None
                      names      ('defaultdict', 'list')
                      varnames   ()
                      freevars   ()
                      cellvars   ()
-                     filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/otlp/json/trace_exporter/__init__.py'
+                     filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py'
                      name       '<lambda>'
                      firstlineno 160
                      lnotab 0x
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 6
@@ -1063,39 +1063,39 @@
                                   86 JUMP_BACKWARD           41 (to 6)
                              >>   88 RETURN_VALUE
                      consts
                      names      ('json', 'loads', 'to_json')
                      varnames   ('.0', 'sdk_span')
                      freevars   ()
                      cellvars   ()
-                     filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/otlp/json/trace_exporter/__init__.py'
+                     filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py'
                      name       '<listcomp>'
                      firstlineno 173
                      lnotab 0x
                   ('scope', 'spans')
                   ('resource', 'scope_spans')
                   'resource_spans'
                names      ('defaultdict', 'resource', 'instrumentation_scope', 'append', 'items', 'json', 'loads', 'to_json', 'dumps')
                varnames   ('self', 'sdk_spans', 'sdk_resource_spans', 'sdk_span', 'sdk_resource', 'sdk_instrumentation', 'resource_spans', 'sdk_instrumentations', 'scope_spans', 'data')
                freevars   ()
                cellvars   ()
-               filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/otlp/json/trace_exporter/__init__.py'
+               filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py'
                name       '_serialize_spans'
                firstlineno 148
                lnotab
                   0x020c200108010e010e014402040132010401320118024a0116fe04ff12
                   0618024a0102fe04ff120804ff0403
             (None, None, None, None, None, None)
             ('return', None)
             (30000,)
          names      ('__name__', '__module__', '__qualname__', 'Optional', 'str', 'Dict', 'int', 'Compression', 'requests', 'Session', '__init__', 'Sequence', 'ReadableSpan', 'SpanExportResult', 'export', 'shutdown', 'bool', 'force_flush', '_export', '_serialize_spans')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/otlp/json/trace_exporter/__init__.py'
+         filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py'
          name       'OTLPSpanExporter'
          firstlineno 58
          lnotab
             0x0a030201020102010201020102f904020efe02030efd02041efc02050e
             fb02060efa020718f908281c15080712040c11
       'OTLPSpanExporter'
       'return'
@@ -1147,15 +1147,15 @@
          consts
             None
             'none'
          names      ('environ', 'get', 'OTEL_EXPORTER_OTLP_TRACES_COMPRESSION', 'OTEL_EXPORTER_OTLP_COMPRESSION', 'lower', 'strip', 'Compression')
          varnames   ('compression',)
          freevars   ()
          cellvars   ()
-         filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/otlp/json/trace_exporter/__init__.py'
+         filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py'
          name       '_compression_from_env'
          firstlineno 189
          lnotab 0x020216010c0132fe0e04240124fa0208
       'endpoint'
       code
          argcount  : 1
          nlocals   : 1
@@ -1190,21 +1190,21 @@
          consts
             None
             '/'
          names      ('endswith', 'DEFAULT_TRACES_EXPORT_PATH')
          varnames   ('endpoint',)
          freevars   ()
          cellvars   ()
-         filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/otlp/json/trace_exporter/__init__.py'
+         filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py'
          name       '_append_trace_path'
          firstlineno 201
          lnotab 0x02012a011401
-   names      ('gzip', 'logging', 'zlib', 'io', 'BytesIO', 'collections', 'defaultdict', 'os', 'environ', 'typing', 'Dict', 'Optional', 'Sequence', 'json', 'requests', 'opentelemetry.sdk.environment_variables', 'OTEL_EXPORTER_OTLP_TRACES_CERTIFICATE', 'OTEL_EXPORTER_OTLP_TRACES_COMPRESSION', 'OTEL_EXPORTER_OTLP_TRACES_ENDPOINT', 'OTEL_EXPORTER_OTLP_TRACES_HEADERS', 'OTEL_EXPORTER_OTLP_TRACES_TIMEOUT', 'OTEL_EXPORTER_OTLP_CERTIFICATE', 'OTEL_EXPORTER_OTLP_COMPRESSION', 'OTEL_EXPORTER_OTLP_ENDPOINT', 'OTEL_EXPORTER_OTLP_HEADERS', 'OTEL_EXPORTER_OTLP_TIMEOUT', 'opentelemetry.sdk.resources', 'SERVICE_NAME', 'opentelemetry.sdk.trace.export', 'SpanExporter', 'SpanExportResult', 'opentelemetry.sdk.trace', 'ReadableSpan', 'syntrac.otlp.json', '_OTLP_HTTP_HEADERS', 'DEFAULT_ENDPOINT', 'Compression', 'opentelemetry.util.re', 'parse_env_headers', 'getLogger', '__name__', '_logger', 'NoCompression', 'DEFAULT_COMPRESSION', 'DEFAULT_TRACES_EXPORT_PATH', 'DEFAULT_TIMEOUT', 'REQUESTS_SUCCESS_STATUS_CODES', 'logger', 'OTLPSpanExporter', '_compression_from_env', 'str', '_append_trace_path')
+   names      ('gzip', 'logging', 'zlib', 'io', 'BytesIO', 'collections', 'defaultdict', 'os', 'environ', 'typing', 'Dict', 'Optional', 'Sequence', 'json', 'requests', 'opentelemetry.sdk.environment_variables', 'OTEL_EXPORTER_OTLP_TRACES_CERTIFICATE', 'OTEL_EXPORTER_OTLP_TRACES_COMPRESSION', 'OTEL_EXPORTER_OTLP_TRACES_ENDPOINT', 'OTEL_EXPORTER_OTLP_TRACES_HEADERS', 'OTEL_EXPORTER_OTLP_TRACES_TIMEOUT', 'OTEL_EXPORTER_OTLP_CERTIFICATE', 'OTEL_EXPORTER_OTLP_COMPRESSION', 'OTEL_EXPORTER_OTLP_ENDPOINT', 'OTEL_EXPORTER_OTLP_HEADERS', 'OTEL_EXPORTER_OTLP_TIMEOUT', 'opentelemetry.sdk.resources', 'SERVICE_NAME', 'opentelemetry.sdk.trace.export', 'SpanExporter', 'SpanExportResult', 'opentelemetry.sdk.trace', 'ReadableSpan', 'syntrac.sdk.otlp.json', '_OTLP_HTTP_HEADERS', 'DEFAULT_ENDPOINT', 'Compression', 'opentelemetry.util.re', 'parse_env_headers', 'getLogger', '__name__', '_logger', 'NoCompression', 'DEFAULT_COMPRESSION', 'DEFAULT_TRACES_EXPORT_PATH', 'DEFAULT_TIMEOUT', 'REQUESTS_SUCCESS_STATUS_CODES', 'logger', 'OTLPSpanExporter', '_compression_from_env', 'str', '_append_trace_path')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/otlp/json/trace_exporter/__init__.py'
+   filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/otlp/json/trace_exporter/__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020f0801080108010c010c010c01140108020802300c0c0110010c
       0114050c0220020e0104010401040220031c7f00040c0c
```

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/otlp/json/version.py` & `syntrac_sdk-0.0.4/syntrac/sdk/otlp/json/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
```

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/prompts/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.4/syntrac/sdk/prompts/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/prompts/__pycache__/client.cpython-311.pyc` & `syntrac_sdk-0.0.4/syntrac/sdk/prompts/__pycache__/client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/prompts/__pycache__/model.cpython-311.pyc` & `syntrac_sdk-0.0.4/syntrac/sdk/prompts/__pycache__/model.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/prompts/__pycache__/registry.cpython-311.pyc` & `syntrac_sdk-0.0.4/syntrac/sdk/prompts/__pycache__/registry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/prompts/client.py` & `syntrac_sdk-0.0.4/syntrac/sdk/prompts/client.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/prompts/model.py` & `syntrac_sdk-0.0.4/syntrac/sdk/prompts/model.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/telemetry.py` & `syntrac_sdk-0.0.4/syntrac/sdk/telemetry.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/tracing/.DS_Store` & `syntrac_sdk-0.0.4/syntrac/sdk/tracing/.DS_Store`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/tracing/__pycache__/content_allow_list.cpython-311.pyc` & `syntrac_sdk-0.0.4/syntrac/sdk/tracing/__pycache__/content_allow_list.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/tracing/__pycache__/context_manager.cpython-311.pyc` & `syntrac_sdk-0.0.4/syntrac/sdk/tracing/__pycache__/context_manager.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/tracing/__pycache__/tracing.cpython-311.pyc` & `syntrac_sdk-0.0.4/syntrac/sdk/tracing/__pycache__/tracing.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x95ac0766 (Sat Mar 30 06:09:25 2024 UTC)
-files sz: 23988
+moddate:  0x060a0966 (Sun Mar 31 07:00:22 2024 UTC)
+files sz: 23992
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 12
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
@@ -60,15 +60,15 @@
                 50 IMPORT_NAME              7 (opentelemetry)
                 52 IMPORT_FROM              8 (trace)
                 54 STORE_NAME               8 (trace)
                 56 POP_TOP
    
      9          58 LOAD_CONST               0 (0)
                 60 LOAD_CONST               4 (('OTLPSpanExporter',))
-                62 IMPORT_NAME              9 (syntrac.otlp.json.trace_exporter)
+                62 IMPORT_NAME              9 (syntrac.sdk.otlp.json.trace_exporter)
                 64 IMPORT_FROM             10 (OTLPSpanExporter)
                 66 STORE_NAME              10 (OTLPSpanExporter)
                 68 POP_TOP
    
     12          70 LOAD_CONST               0 (0)
                 72 LOAD_CONST               5 (('Resource',))
                 74 IMPORT_NAME             11 (opentelemetry.sdk.resources)
@@ -3883,15 +3883,15 @@
          varnames   ('WeaviateInstrumentor', 'instrumentor')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
          name       'init_weaviate_instrumentor'
          firstlineno 608
          lnotab 0x02013e0142010c0214010e012801
-   names      ('atexit', 'logging', 'os', 'importlib.util', 'importlib', 'colorama', 'Fore', 'opentelemetry', 'trace', 'syntrac.otlp.json.trace_exporter', 'OTLPSpanExporter', 'opentelemetry.sdk.resources', 'Resource', 'opentelemetry.sdk.trace', 'TracerProvider', 'SpanProcessor', 'opentelemetry.propagators.textmap', 'TextMapPropagator', 'opentelemetry.propagate', 'set_global_textmap', 'opentelemetry.sdk.trace.export', 'SpanExporter', 'SimpleSpanProcessor', 'BatchSpanProcessor', 'opentelemetry.trace', 'get_tracer_provider', 'ProxyTracerProvider', 'opentelemetry.context', 'get_value', 'attach', 'set_value', 'syntrac_opentelemetry.semconv.ai', 'SpanAttributes', 'syntrac.sdk', 'Telemetry', 'syntrac.sdk.instruments', 'Instruments', 'syntrac.sdk.tracing.content_allow_list', 'ContentAllowList', 'syntrac.sdk.utils', 'is_notebook', 'typing', 'Dict', 'Optional', 'Set', 'TRACER_NAME', 'EXCLUDED_URLS', 'object', 'TracerWrapper', 'str', 'set_correlation_id', 'dict', 'set_association_properties', 'set_workflow_name', 'int', 'set_prompt_tracing_context', 'bool', 'is_llm_span', 'init_spans_exporter', 'init_tracer_provider', 'init_instrumentations', 'init_openai_instrumentor', 'init_anthropic_instrumentor', 'init_cohere_instrumentor', 'init_pinecone_instrumentor', 'init_qdrant_instrumentor', 'init_chroma_instrumentor', 'init_haystack_instrumentor', 'init_langchain_instrumentor', 'init_transformers_instrumentor', 'init_llama_index_instrumentor', 'init_requests_instrumentor', 'init_urllib3_instrumentor', 'init_pymysql_instrumentor', 'init_bedrock_instrumentor', 'init_replicate_instrumentor', 'init_vertexai_instrumentor', 'init_watsonx_instrumentor', 'init_weaviate_instrumentor')
+   names      ('atexit', 'logging', 'os', 'importlib.util', 'importlib', 'colorama', 'Fore', 'opentelemetry', 'trace', 'syntrac.sdk.otlp.json.trace_exporter', 'OTLPSpanExporter', 'opentelemetry.sdk.resources', 'Resource', 'opentelemetry.sdk.trace', 'TracerProvider', 'SpanProcessor', 'opentelemetry.propagators.textmap', 'TextMapPropagator', 'opentelemetry.propagate', 'set_global_textmap', 'opentelemetry.sdk.trace.export', 'SpanExporter', 'SimpleSpanProcessor', 'BatchSpanProcessor', 'opentelemetry.trace', 'get_tracer_provider', 'ProxyTracerProvider', 'opentelemetry.context', 'get_value', 'attach', 'set_value', 'syntrac_opentelemetry.semconv.ai', 'SpanAttributes', 'syntrac.sdk', 'Telemetry', 'syntrac.sdk.instruments', 'Instruments', 'syntrac.sdk.tracing.content_allow_list', 'ContentAllowList', 'syntrac.sdk.utils', 'is_notebook', 'typing', 'Dict', 'Optional', 'Set', 'TRACER_NAME', 'EXCLUDED_URLS', 'object', 'TracerWrapper', 'str', 'set_correlation_id', 'dict', 'set_association_properties', 'set_workflow_name', 'int', 'set_prompt_tracing_context', 'bool', 'is_llm_span', 'init_spans_exporter', 'init_tracer_provider', 'init_instrumentations', 'init_openai_instrumentor', 'init_anthropic_instrumentor', 'init_cohere_instrumentor', 'init_pinecone_instrumentor', 'init_qdrant_instrumentor', 'init_chroma_instrumentor', 'init_haystack_instrumentor', 'init_langchain_instrumentor', 'init_transformers_instrumentor', 'init_llama_index_instrumentor', 'init_requests_instrumentor', 'init_urllib3_instrumentor', 'init_pymysql_instrumentor', 'init_bedrock_instrumentor', 'init_replicate_instrumentor', 'init_vertexai_instrumentor', 'init_watsonx_instrumentor', 'init_weaviate_instrumentor')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/vuongngo/workspace/syntrac/packages/python/syntrac-sdk/syntrac/sdk/tracing/tracing.py'
    name       '<module>'
    firstlineno 1
    lnotab
```

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/tracing/content_allow_list.py` & `syntrac_sdk-0.0.4/syntrac/sdk/tracing/content_allow_list.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/tracing/tracing.py` & `syntrac_sdk-0.0.4/syntrac/sdk/tracing/tracing.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/utils/__init__.py` & `syntrac_sdk-0.0.4/syntrac/sdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/utils/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.4/syntrac/sdk/utils/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.3/syntrac/sdk/utils/in_memory_span_exporter.py` & `syntrac_sdk-0.0.4/syntrac/sdk/utils/in_memory_span_exporter.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.3/PKG-INFO` & `syntrac_sdk-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syntrac-sdk
-Version: 0.0.3
+Version: 0.0.4
 Summary: Syntrac Software Development Kit (SDK) for Python
 Home-page: https://github.com/syntracAI/syntrac
 License: Apache-2.0
 Author: Vuong Ngo
 Author-email: vuongngo.pd@gmail.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,15 +13,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: deprecated (>=1.2.14,<2.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: opentelemetry-api (>=1.23.0,<2.0.0)
-Requires-Dist: opentelemetry-exporter-otlp-proto-grpc (>=1.20.0,<2.0.0)
 Requires-Dist: opentelemetry-exporter-otlp-proto-http (>=1.20.0,<2.0.0)
 Requires-Dist: opentelemetry-instrumentation-requests (==0.44b0)
 Requires-Dist: opentelemetry-instrumentation-sqlalchemy (==0.44b0)
 Requires-Dist: opentelemetry-instrumentation-urllib3 (==0.44b0)
 Requires-Dist: opentelemetry-sdk (>=1.20.0,<2.0.0)
 Requires-Dist: posthog (>=3.0.2,<4.0.0)
 Requires-Dist: pydantic (>=1)
```

