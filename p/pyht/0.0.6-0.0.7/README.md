# Comparing `tmp/pyht-0.0.6.tar.gz` & `tmp/pyht-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyht-0.0.6.tar", max compression
+gzip compressed data, was "pyht-0.0.7.tar", max compression
```

## Comparing `pyht-0.0.6.tar` & `pyht-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-09-14 11:12:22.620229 pyht-0.0.6/LICENSE
--rw-r--r--   0        0        0     1394 2023-09-14 11:12:22.620229 pyht-0.0.6/README.rst
--rw-r--r--   0        0        0      139 2023-09-14 11:12:36.808685 pyht-0.0.6/pyht/__init__.py
--rw-r--r--   0        0        0     3328 2023-09-14 11:12:22.620229 pyht-0.0.6/pyht/client.py
--rw-r--r--   0        0        0      472 2023-09-14 11:12:22.620229 pyht-0.0.6/pyht/lease.py
--rw-r--r--   0        0        0        0 2023-09-14 11:12:22.620229 pyht-0.0.6/pyht/protos/.keep
--rw-r--r--   0        0        0     3435 2023-09-14 11:12:22.620229 pyht-0.0.6/pyht/protos/api_pb2.py
--rw-r--r--   0        0        0     3967 2023-09-14 11:12:22.620229 pyht-0.0.6/pyht/protos/api_pb2.pyi
--rw-r--r--   0        0        0     2283 2023-09-14 11:12:22.620229 pyht-0.0.6/pyht/protos/api_pb2_grpc.py
--rw-r--r--   0        0        0     3558 2023-09-14 11:12:36.808685 pyht-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2120 1970-01-01 00:00:00.000000 pyht-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-10-02 03:21:15.941965 pyht-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1394 2023-10-02 03:21:15.941965 pyht-0.0.7/README.rst
+-rw-r--r--   0        0        0      183 2023-10-02 03:21:33.099243 pyht-0.0.7/pyht/__init__.py
+-rw-r--r--   0        0        0     5129 2023-10-02 03:21:15.941965 pyht-0.0.7/pyht/client.py
+-rw-r--r--   0        0        0      472 2023-10-02 03:21:15.941965 pyht-0.0.7/pyht/lease.py
+-rw-r--r--   0        0        0        0 2023-10-02 03:21:15.941965 pyht-0.0.7/pyht/protos/.keep
+-rw-r--r--   0        0        0        0 2023-10-02 03:21:15.941965 pyht-0.0.7/pyht/protos/__init__.py
+-rw-r--r--   0        0        0     3422 2023-10-02 03:21:15.941965 pyht-0.0.7/pyht/protos/api_pb2.py
+-rw-r--r--   0        0        0     3951 2023-10-02 03:21:15.941965 pyht-0.0.7/pyht/protos/api_pb2.pyi
+-rw-r--r--   0        0        0     2283 2023-10-02 03:21:15.945965 pyht-0.0.7/pyht/protos/api_pb2_grpc.py
+-rw-r--r--   0        0        0     3744 2023-10-02 03:21:33.099243 pyht-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2120 1970-01-01 00:00:00.000000 pyht-0.0.7/PKG-INFO
```

### Comparing `pyht-0.0.6/LICENSE` & `pyht-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyht-0.0.6/README.rst` & `pyht-0.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `pyht-0.0.6/pyht/protos/api_pb2.py` & `pyht-0.0.7/pyht/protos/api_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,32 +9,32 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tapi.proto\x12\tplayht.v1\"A\n\nTtsRequest\x12\r\n\x05lease\x18\x01 \x01(\x0c\x12$\n\x06params\x18\x02 \x01(\x0b\x32\x14.playht.v1.TtsParams\"\\\n\x0bTtsResponse\x12\x10\n\x08sequence\x18\x01 \x01(\x05\x12\n\n\x02id\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\x12!\n\x06status\x18\x04 \x01(\x0b\x32\x11.playht.v1.Status\"\xdb\x02\n\tTtsParams\x12\x0c\n\x04text\x18\x01 \x03(\t\x12\r\n\x05voice\x18\x02 \x01(\t\x12(\n\x07quality\x18\x03 \x01(\x0e\x32\x12.playht.v1.QualityH\x00\x88\x01\x01\x12&\n\x06\x66ormat\x18\x04 \x01(\x0e\x32\x11.playht.v1.FormatH\x01\x88\x01\x01\x12\x18\n\x0bsample_rate\x18\x05 \x01(\x05H\x02\x88\x01\x01\x12\x12\n\x05speed\x18\x06 \x01(\x02H\x03\x88\x01\x01\x12\x11\n\x04seed\x18\x07 \x01(\x05H\x04\x88\x01\x01\x12\x18\n\x0btemperature\x18\x08 \x01(\x02H\x05\x88\x01\x01\x12\x12\n\x05top_p\x18\t \x01(\x02H\x06\x88\x01\x01\x12\x12\n\x05other\x18\x63 \x01(\tH\x07\x88\x01\x01\x42\n\n\x08_qualityB\t\n\x07_formatB\x0e\n\x0c_sample_rateB\x08\n\x06_speedB\x07\n\x05_seedB\x0e\n\x0c_temperatureB\x08\n\x06_top_pB\x08\n\x06_other\"8\n\x06Status\x12\x1d\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x0f.playht.v1.Code\x12\x0f\n\x07message\x18\x02 \x03(\t*h\n\x04\x43ode\x12\x14\n\x10\x43ODE_UNSPECIFIED\x10\x00\x12\x11\n\rCODE_COMPLETE\x10\x01\x12\x14\n\x10\x43ODE_IN_PROGRESS\x10\x02\x12\x11\n\rCODE_CANCELED\x10\x03\x12\x0e\n\nCODE_ERROR\x10\x04*\x81\x01\n\x07Quality\x12\x17\n\x13QUALITY_UNSPECIFIED\x10\x00\x12\x13\n\x0fQUALITY_PREMIUM\x10\x02\x12\x10\n\x0cQUALITY_HIGH\x10\x03\x12\x12\n\x0eQUALITY_MEDIUM\x10\x04\x12\x11\n\rQUALITY_DRAFT\x10\x05\x12\x0f\n\x0bQUALITY_LOW\x10\x06*s\n\x06\x46ormat\x12\x16\n\x12\x46ORMAT_UNSPECIFIED\x10\x00\x12\x0e\n\nFORMAT_MP3\x10\x01\x12\x0e\n\nFORMAT_WAV\x10\x02\x12\x0e\n\nFORMAT_OGG\x10\x03\x12\x0f\n\x0b\x46ORMAT_FLAC\x10\x04\x12\x10\n\x0c\x46ORMAT_MULAW\x10\x05\x32=\n\x03Tts\x12\x36\n\x03Tts\x12\x15.playht.v1.TtsRequest\x1a\x16.playht.v1.TtsResponse0\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tapi.proto\x12\tplayht.v1\"A\n\nTtsRequest\x12\r\n\x05lease\x18\x01 \x01(\x0c\x12$\n\x06params\x18\x02 \x01(\x0b\x32\x14.playht.v1.TtsParams\"\\\n\x0bTtsResponse\x12\x10\n\x08sequence\x18\x01 \x01(\x05\x12\n\n\x02id\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\x12!\n\x06status\x18\x04 \x01(\x0b\x32\x11.playht.v1.Status\"\xdb\x02\n\tTtsParams\x12\x0c\n\x04text\x18\x01 \x03(\t\x12\r\n\x05voice\x18\x02 \x01(\t\x12(\n\x07quality\x18\x03 \x01(\x0e\x32\x12.playht.v1.QualityH\x00\x88\x01\x01\x12&\n\x06\x66ormat\x18\x04 \x01(\x0e\x32\x11.playht.v1.FormatH\x01\x88\x01\x01\x12\x18\n\x0bsample_rate\x18\x05 \x01(\x05H\x02\x88\x01\x01\x12\x12\n\x05speed\x18\x06 \x01(\x02H\x03\x88\x01\x01\x12\x11\n\x04seed\x18\x07 \x01(\x05H\x04\x88\x01\x01\x12\x18\n\x0btemperature\x18\x08 \x01(\x02H\x05\x88\x01\x01\x12\x12\n\x05top_p\x18\t \x01(\x02H\x06\x88\x01\x01\x12\x12\n\x05other\x18\x63 \x01(\tH\x07\x88\x01\x01\x42\n\n\x08_qualityB\t\n\x07_formatB\x0e\n\x0c_sample_rateB\x08\n\x06_speedB\x07\n\x05_seedB\x0e\n\x0c_temperatureB\x08\n\x06_top_pB\x08\n\x06_other\"8\n\x06Status\x12\x1d\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x0f.playht.v1.Code\x12\x0f\n\x07message\x18\x02 \x03(\t*h\n\x04\x43ode\x12\x14\n\x10\x43ODE_UNSPECIFIED\x10\x00\x12\x11\n\rCODE_COMPLETE\x10\x01\x12\x14\n\x10\x43ODE_IN_PROGRESS\x10\x02\x12\x11\n\rCODE_CANCELED\x10\x03\x12\x0e\n\nCODE_ERROR\x10\x04*\x81\x01\n\x07Quality\x12\x17\n\x13QUALITY_UNSPECIFIED\x10\x00\x12\x13\n\x0fQUALITY_PREMIUM\x10\x02\x12\x10\n\x0cQUALITY_HIGH\x10\x03\x12\x12\n\x0eQUALITY_MEDIUM\x10\x04\x12\x11\n\rQUALITY_DRAFT\x10\x05\x12\x0f\n\x0bQUALITY_LOW\x10\x06*k\n\x06\x46ormat\x12\x0e\n\nFORMAT_RAW\x10\x00\x12\x0e\n\nFORMAT_MP3\x10\x01\x12\x0e\n\nFORMAT_WAV\x10\x02\x12\x0e\n\nFORMAT_OGG\x10\x03\x12\x0f\n\x0b\x46ORMAT_FLAC\x10\x04\x12\x10\n\x0c\x46ORMAT_MULAW\x10\x05\x32=\n\x03Tts\x12\x36\n\x03Tts\x12\x15.playht.v1.TtsRequest\x1a\x16.playht.v1.TtsResponse0\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'api_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _globals['_CODE']._serialized_start=593
   _globals['_CODE']._serialized_end=697
   _globals['_QUALITY']._serialized_start=700
   _globals['_QUALITY']._serialized_end=829
   _globals['_FORMAT']._serialized_start=831
-  _globals['_FORMAT']._serialized_end=946
+  _globals['_FORMAT']._serialized_end=938
   _globals['_TTSREQUEST']._serialized_start=24
   _globals['_TTSREQUEST']._serialized_end=89
   _globals['_TTSRESPONSE']._serialized_start=91
   _globals['_TTSRESPONSE']._serialized_end=183
   _globals['_TTSPARAMS']._serialized_start=186
   _globals['_TTSPARAMS']._serialized_end=533
   _globals['_STATUS']._serialized_start=535
   _globals['_STATUS']._serialized_end=591
-  _globals['_TTS']._serialized_start=948
-  _globals['_TTS']._serialized_end=1009
+  _globals['_TTS']._serialized_start=940
+  _globals['_TTS']._serialized_end=1001
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pyht-0.0.6/pyht/protos/api_pb2.pyi` & `pyht-0.0.7/pyht/protos/api_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     QUALITY_HIGH: _ClassVar[Quality]
     QUALITY_MEDIUM: _ClassVar[Quality]
     QUALITY_DRAFT: _ClassVar[Quality]
     QUALITY_LOW: _ClassVar[Quality]
 
 class Format(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
-    FORMAT_UNSPECIFIED: _ClassVar[Format]
+    FORMAT_RAW: _ClassVar[Format]
     FORMAT_MP3: _ClassVar[Format]
     FORMAT_WAV: _ClassVar[Format]
     FORMAT_OGG: _ClassVar[Format]
     FORMAT_FLAC: _ClassVar[Format]
     FORMAT_MULAW: _ClassVar[Format]
 CODE_UNSPECIFIED: Code
 CODE_COMPLETE: Code
@@ -38,15 +38,15 @@
 CODE_ERROR: Code
 QUALITY_UNSPECIFIED: Quality
 QUALITY_PREMIUM: Quality
 QUALITY_HIGH: Quality
 QUALITY_MEDIUM: Quality
 QUALITY_DRAFT: Quality
 QUALITY_LOW: Quality
-FORMAT_UNSPECIFIED: Format
+FORMAT_RAW: Format
 FORMAT_MP3: Format
 FORMAT_WAV: Format
 FORMAT_OGG: Format
 FORMAT_FLAC: Format
 FORMAT_MULAW: Format
 
 class TtsRequest(_message.Message):
```

### Comparing `pyht-0.0.6/pyht/protos/api_pb2_grpc.py` & `pyht-0.0.7/pyht/protos/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pyht-0.0.6/pyproject.toml` & `pyht-0.0.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
 [tool.poetry]
 name = "pyht"
-version = "0.0.6"                                  # Do not change, let poetry-dynamic-versioning handle it.
+version = "0.0.7"                                  # Do not change, let poetry-dynamic-versioning handle it.
 homepage = "https://github.com/playht/pyht"
 repository = "https://github.com/playht/pyht"
 license = "Apache-2.0"
 description = ""
 authors = ["Playht Inc. <oss@play.ht>"]
 readme = "README.rst"
 packages = [{ include = "pyht" }]
@@ -53,15 +53,15 @@
 
 [tool.poetry.group.debug.dependencies]
 ipdb = ">=0.13.9"
 line_profiler = ">=3.5.1"
 
 [tool.coverage.run]
 branch = true
-omit = ["tests/*"]
+omit = ["tests/*", "pyht/protos/*"]
 
 [tool.coverage.report]
 exclude_lines = [
     # Have to re-enable the standard pragma
     "pragma: no cover",
 
     # Don't complain about missing debug-only code:
@@ -79,14 +79,18 @@
     "if False:",
     "if __name__ == .__main__.:",
 ]
 
 [tool.pyright]
 venvPath = "."
 venv = ".venv"
+ignore = [
+    "tests/*",
+    "pyht/protos/*.py",
+]
 
 [tool.ruff]
 target-version = 'py38'
 select = [
     "B",   # flake8-bugbear
     "C4",  # flake8-comprehensions
     "D",   # pydocstyle
@@ -112,14 +116,16 @@
     "manage.py",
     "settings.py",
     "build.py",
     "env",
     ".env",
     "venv",
     ".venv",
+    "pyht/protos/*.py",
+    "demo",  # This is sample code, and not meant to build in the package.
 ]
 
 ignore = [
     "B905",   # zip strict=True; remove once python <3.10 support is dropped.
     "D100",
     "D101",
     "D102",
@@ -160,8 +166,8 @@
     "PGH001", # use of "eval"
 ]
 
 [tool.ruff.pep8-naming]
 staticmethod-decorators = ["pydantic.validator", "pydantic.root_validator"]
 
 [tool.codespell]
-skip = 'poetry.lock,'
+skip = 'poetry.lock,./pyht/protos/*.py'
```

### Comparing `pyht-0.0.6/PKG-INFO` & `pyht-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyht
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 Home-page: https://github.com/playht/pyht
 License: Apache-2.0
 Author: Playht Inc.
 Author-email: oss@play.ht
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

