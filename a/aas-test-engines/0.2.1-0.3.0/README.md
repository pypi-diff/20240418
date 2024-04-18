# Comparing `tmp/aas_test_engines-0.2.1.tar.gz` & `tmp/aas_test_engines-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aas_test_engines-0.2.1.tar", last modified: Mon Nov 13 15:03:56 2023, max compression
+gzip compressed data, was "aas_test_engines-0.3.0.tar", last modified: Thu Feb  1 20:33:47 2024, max compression
```

## Comparing `aas_test_engines-0.2.1.tar` & `aas_test_engines-0.3.0.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 15:03:56.780586 aas_test_engines-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2023-11-13 15:03:56.780586 aas_test_engines-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 15:03:56.776586 aas_test_engines-0.2.1/aas_test_engines/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-11-13 15:03:50.000000 aas_test_engines-0.2.1/aas_test_engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/aas_test_engines/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 15:03:56.780586 aas_test_engines-0.2.1/aas_test_engines/_api/
--rw-r--r--   0 runner    (1001) docker     (127)    13403 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/aas_test_engines/_api/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/aas_test_engines/_api/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     8746 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/aas_test_engines/_api/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/aas_test_engines/_api/parse_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/aas_test_engines/_api/resolver.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4280 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/aas_test_engines/_api/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/aas_test_engines/_api/runconf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/aas_test_engines/_api/runtime_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/aas_test_engines/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 15:03:56.776586 aas_test_engines-0.2.1/aas_test_engines/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 15:03:56.780586 aas_test_engines-0.2.1/aas_test_engines/data/api/
--rw-r--r--   0 runner    (1001) docker     (127)   567190 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/aas_test_engines/data/api/3.0.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 15:03:56.780586 aas_test_engines-0.2.1/aas_test_engines/data/api/samples/
--rw-r--r--   0 runner    (1001) docker     (127)   122762 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/aas_test_engines/data/api/samples/aas.json
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/aas_test_engines/data/api/samples/asset_info.json
--rw-r--r--   0 runner    (1001) docker     (127)        2 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/aas_test_engines/data/api/samples/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      172 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/aas_test_engines/data/api/samples/model_reference.json
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/aas_test_engines/data/api/samples/operation_request.json
--rw-r--r--   0 runner    (1001) docker     (127)      830 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/aas_test_engines/data/api/samples/shell_descriptor.json
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/aas_test_engines/data/api/samples/submodel.json
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/aas_test_engines/data/api/samples/submodel_descriptor.json
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/aas_test_engines/data/api/samples/submodel_element.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 15:03:56.780586 aas_test_engines-0.2.1/aas_test_engines/data/file/
--rw-r--r--   0 runner    (1001) docker     (127)    37460 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/aas_test_engines/data/file/3.0.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9266 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/aas_test_engines/data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/aas_test_engines/exception.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10858 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/aas_test_engines/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/aas_test_engines/result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 15:03:56.776586 aas_test_engines-0.2.1/aas_test_engines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2023-11-13 15:03:56.000000 aas_test_engines-0.2.1/aas_test_engines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2023-11-13 15:03:56.000000 aas_test_engines-0.2.1/aas_test_engines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-13 15:03:56.000000 aas_test_engines-0.2.1/aas_test_engines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-11-13 15:03:56.000000 aas_test_engines-0.2.1/aas_test_engines.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-11-13 15:03:56.000000 aas_test_engines-0.2.1/aas_test_engines.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-11-13 15:03:56.000000 aas_test_engines-0.2.1/aas_test_engines.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      726 2023-11-13 15:03:50.000000 aas_test_engines-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-13 15:03:56.780586 aas_test_engines-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 15:03:56.780586 aas_test_engines-0.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2023-11-13 15:02:19.000000 aas_test_engines-0.2.1/test/test_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 20:33:47.860152 aas_test_engines-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-02-01 20:33:47.860152 aas_test_engines-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 20:33:47.852152 aas_test_engines-0.3.0/aas_test_engines/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-01 20:33:41.000000 aas_test_engines-0.3.0/aas_test_engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/aas_test_engines/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 20:33:47.856152 aas_test_engines-0.3.0/aas_test_engines/_api/
+-rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/aas_test_engines/_api/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/aas_test_engines/_api/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8746 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/aas_test_engines/_api/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/aas_test_engines/_api/parse_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/aas_test_engines/_api/resolver.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4280 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/aas_test_engines/_api/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/aas_test_engines/_api/runconf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/aas_test_engines/_api/runtime_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/aas_test_engines/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 20:33:47.852152 aas_test_engines-0.3.0/aas_test_engines/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 20:33:47.856152 aas_test_engines-0.3.0/aas_test_engines/data/api/
+-rw-r--r--   0 runner    (1001) docker     (127)   567190 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/aas_test_engines/data/api/3.0.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 20:33:47.860152 aas_test_engines-0.3.0/aas_test_engines/data/api/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)   122762 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/aas_test_engines/data/api/samples/aas.json
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/aas_test_engines/data/api/samples/asset_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/aas_test_engines/data/api/samples/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/aas_test_engines/data/api/samples/model_reference.json
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/aas_test_engines/data/api/samples/operation_request.json
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/aas_test_engines/data/api/samples/shell_descriptor.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/aas_test_engines/data/api/samples/submodel.json
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/aas_test_engines/data/api/samples/submodel_descriptor.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/aas_test_engines/data/api/samples/submodel_element.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 20:33:47.860152 aas_test_engines-0.3.0/aas_test_engines/data/file/
+-rw-r--r--   0 runner    (1001) docker     (127)    37460 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/aas_test_engines/data/file/3.0.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/aas_test_engines/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/aas_test_engines/exception.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10846 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/aas_test_engines/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/aas_test_engines/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/aas_test_engines/result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 20:33:47.860152 aas_test_engines-0.3.0/aas_test_engines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-02-01 20:33:47.000000 aas_test_engines-0.3.0/aas_test_engines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-02-01 20:33:47.000000 aas_test_engines-0.3.0/aas_test_engines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 20:33:47.000000 aas_test_engines-0.3.0/aas_test_engines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-01 20:33:47.000000 aas_test_engines-0.3.0/aas_test_engines.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-01 20:33:47.000000 aas_test_engines-0.3.0/aas_test_engines.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-01 20:33:47.000000 aas_test_engines-0.3.0/aas_test_engines.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-02-01 20:33:41.000000 aas_test_engines-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-01 20:33:47.860152 aas_test_engines-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 20:33:47.860152 aas_test_engines-0.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-02-01 20:32:05.000000 aas_test_engines-0.3.0/test/test_file.py
```

### Comparing `aas_test_engines-0.2.1/PKG-INFO` & `aas_test_engines-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: aas_test_engines
-Version: 0.2.1
-Summary: Official test tooling for the Asset Administration Shell
-Project-URL: Homepage, https://github.com/admin-shell-io/aas-test-engines
-Keywords: asset administration shell,aas,test
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Requires-Dist: requests>=2.31
-Requires-Dist: pyyaml>=6.0
-Requires-Dist: json_schema_tool>=0.1
-Requires-Dist: jsonpath_ng>=1.5
-Requires-Dist: jsonschema>=4.19
-
 # Test Engines for the Asset Administration Shell
 
 [![Tests](https://github.com/admin-shell-io/aas-test-engines/actions/workflows/check.yml/badge.svg)](https://github.com/admin-shell-io/aas-test-engines/actions/workflows/check.yml)
 
 The Asset Administration Shell (AAS) is a standard for Digital Twins.
 More information can be found [here](https://industrialdigitaltwin.org/content-hub/downloads).
 
@@ -35,48 +19,59 @@
 
 ### Check AASX:
 ```python
 from aas_test_engines import file
 from xml.etree import ElementTree
 
 with open('aas.aasx') as f:
-    file.check_aasx_file(f)
+    result = file.check_aasx_file(f)
+# result.ok() == True
+
+result.dump()
 ```
 
 ### Check JSON:
 
 ```python
 from aas_test_engines import file
 
 # Check file
 with open('aas.json') as f:
-    file.check_json_file(f)
+    result = file.check_json_file(f)
+# result.ok() == True
 
 # Or check data directly
 aas = {
     'assetAdministrationShells': [],
     'submodels': [],
     'conceptDescriptions': []
 }
-file.check_json_data(aas)
+result = file.check_json_data(aas)
+# result.ok() == True
+
+result.dump()
 ```
 
 ### Check XML:
 ```python
 from aas_test_engines import file
 from xml.etree import ElementTree
 
 # Check file
 with open('aas.xml') as f:
-    file.check_xml_file(f)
+    result = file.check_xml_file(f)
+# result.ok() == True
 
 # Or check data directly
 data = ElementTree.fromstring(
     '<environment xmlns="https://admin-shell.io/aas/3/0" />')
-file.check_xml_data(aas)
+result = file.check_xml_data(aas)
+# result.ok() == True
+
+result.dump()
 ```
 
 ### Checking older versions
 
 By default, the `file.check...` methods check compliance to version 3.0 of the standard.
 You may want to check against older versions by passing a string containing the version to these methods.
```

### Comparing `aas_test_engines-0.2.1/README.md` & `aas_test_engines-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: aas_test_engines
+Version: 0.3.0
+Summary: Official test tooling for the Asset Administration Shell
+Project-URL: Homepage, https://github.com/admin-shell-io/aas-test-engines
+Keywords: asset administration shell,aas,test
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.31
+Requires-Dist: pyyaml>=6.0
+Requires-Dist: json_schema_tool>=0.2
+Requires-Dist: jsonpath_ng>=1.5
+Requires-Dist: jsonschema>=4.19
+
 # Test Engines for the Asset Administration Shell
 
 [![Tests](https://github.com/admin-shell-io/aas-test-engines/actions/workflows/check.yml/badge.svg)](https://github.com/admin-shell-io/aas-test-engines/actions/workflows/check.yml)
 
 The Asset Administration Shell (AAS) is a standard for Digital Twins.
 More information can be found [here](https://industrialdigitaltwin.org/content-hub/downloads).
 
@@ -19,48 +36,59 @@
 
 ### Check AASX:
 ```python
 from aas_test_engines import file
 from xml.etree import ElementTree
 
 with open('aas.aasx') as f:
-    file.check_aasx_file(f)
+    result = file.check_aasx_file(f)
+# result.ok() == True
+
+result.dump()
 ```
 
 ### Check JSON:
 
 ```python
 from aas_test_engines import file
 
 # Check file
 with open('aas.json') as f:
-    file.check_json_file(f)
+    result = file.check_json_file(f)
+# result.ok() == True
 
 # Or check data directly
 aas = {
     'assetAdministrationShells': [],
     'submodels': [],
     'conceptDescriptions': []
 }
-file.check_json_data(aas)
+result = file.check_json_data(aas)
+# result.ok() == True
+
+result.dump()
 ```
 
 ### Check XML:
 ```python
 from aas_test_engines import file
 from xml.etree import ElementTree
 
 # Check file
 with open('aas.xml') as f:
-    file.check_xml_file(f)
+    result = file.check_xml_file(f)
+# result.ok() == True
 
 # Or check data directly
 data = ElementTree.fromstring(
     '<environment xmlns="https://admin-shell.io/aas/3/0" />')
-file.check_xml_data(aas)
+result = file.check_xml_data(aas)
+# result.ok() == True
+
+result.dump()
 ```
 
 ### Checking older versions
 
 By default, the `file.check...` methods check compliance to version 3.0 of the standard.
 You may want to check against older versions by passing a string containing the version to these methods.
```

### Comparing `aas_test_engines-0.2.1/aas_test_engines/__main__.py` & `aas_test_engines-0.3.0/aas_test_engines/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,43 @@
 import argparse
 import sys
 from aas_test_engines import api, file
+from enum import Enum
 
+class Formats(Enum):
+    xml = 'xml'
+    json = 'json'
+    aasx = 'aasx'
+
+    def __str__(self):
+        return self.value
 
 def run_file_test(argv):
-    parser = argparse.ArgumentParser(description='Runs test cases')
+    parser = argparse.ArgumentParser(description='Checks a file for compliance with the AAS meta-model')
     parser.add_argument('file',
                         type=argparse.FileType('r'),
                         help='the file to check')
+    parser.add_argument('--format',
+                        type=Formats,
+                        default=Formats.aasx,
+                        choices=list(Formats))
     args = parser.parse_args(argv)
-    result = file.check_aasx_file(args.file)
-    print(result)
+    if args.format == Formats.aasx:
+        result = file.check_aasx_file(args.file)
+    elif args.format == Formats.json:
+        result = file.check_json_file(args.file)
+    elif args.format == Formats.xml:
+        result = file.check_xml_file(args.file)
+    else:
+        raise Exception(f"Invalid format {args.format}")
+    result.dump()
 
 
 def run_api_test(argv):
-    parser = argparse.ArgumentParser(description='Runs test cases')
+    parser = argparse.ArgumentParser(description='Checks a server instance for compliance with the AAS api')
     parser.add_argument('server',
                         type=str,
                         help='server to run the tests against')
     parser.add_argument('--dry',
                         action='store_true',
                         help="dry run, do not send requests")
     parser.add_argument('--suite',
```

### Comparing `aas_test_engines-0.2.1/aas_test_engines/_api/generate.py` & `aas_test_engines-0.3.0/aas_test_engines/_api/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,20 +95,23 @@
             '#/components/schemas/Identifier': 'empty.json',
             '#/components/schemas/IdentifierKeyValuePair': 'empty.json',
             '#/components/schemas/SubmodelMetadata': 'empty.json',
             '#/components/schemas/SubmodelValue': 'empty.json',
             '#/components/schemas/SubmodelElementMetadata': 'empty.json',
             '#/components/schemas/SubmodelElementValue': 'empty.json',
             '#/components/schemas/OperationRequestValueOnly': 'empty.json',
+            '#/components/schemas/GetSubmodelElementsMetadataResult': 'empty.json',
+            '#/components/schemas/GetSubmodelElementsValueResult': 'empty.json',
+            '#/components/schemas/SpecificAssetId': 'empty.json',
         }.get(ref)
         if path:
             # TODO: check if example matches the schema
             return [json.load(open(samples_dir + path, "rb"))]
         else:
-            raise Exception("Unknown ref " + schema['$ref'])
+            raise Exception("Failed to generate valid samples for " + schema['$ref'])
     type_ = schema.get('type', 'object')
     if type_ == 'array':
         return [generate_valid_samples(schema['items'])]
     elif type_ == 'boolean':
         return [True, False]
     elif type_ == 'string':
         return ["random_string"]
```

### Comparing `aas_test_engines-0.2.1/aas_test_engines/_api/graph.py` & `aas_test_engines-0.3.0/aas_test_engines/_api/graph.py`

 * *Files identical despite different names*

### Comparing `aas_test_engines-0.2.1/aas_test_engines/_api/openapi.py` & `aas_test_engines-0.3.0/aas_test_engines/_api/openapi.py`

 * *Files identical despite different names*

### Comparing `aas_test_engines-0.2.1/aas_test_engines/_api/parse_util.py` & `aas_test_engines-0.3.0/aas_test_engines/_api/parse_util.py`

 * *Files identical despite different names*

### Comparing `aas_test_engines-0.2.1/aas_test_engines/_api/resolver.py` & `aas_test_engines-0.3.0/aas_test_engines/_api/resolver.py`

 * *Files identical despite different names*

### Comparing `aas_test_engines-0.2.1/aas_test_engines/_api/run.py` & `aas_test_engines-0.3.0/aas_test_engines/_api/run.py`

 * *Files identical despite different names*

### Comparing `aas_test_engines-0.2.1/aas_test_engines/_api/runconf.py` & `aas_test_engines-0.3.0/aas_test_engines/_api/runconf.py`

 * *Files identical despite different names*

### Comparing `aas_test_engines-0.2.1/aas_test_engines/_api/runtime_expression.py` & `aas_test_engines-0.3.0/aas_test_engines/_api/runtime_expression.py`

 * *Files identical despite different names*

### Comparing `aas_test_engines-0.2.1/aas_test_engines/api.py` & `aas_test_engines-0.3.0/aas_test_engines/api.py`

 * *Files identical despite different names*

### Comparing `aas_test_engines-0.2.1/aas_test_engines/data/api/3.0.yml` & `aas_test_engines-0.3.0/aas_test_engines/data/api/3.0.yml`

 * *Files identical despite different names*

### Comparing `aas_test_engines-0.2.1/aas_test_engines/data/api/samples/aas.json` & `aas_test_engines-0.3.0/aas_test_engines/data/api/samples/aas.json`

 * *Files identical despite different names*

### Comparing `aas_test_engines-0.2.1/aas_test_engines/data/api/samples/asset_info.json` & `aas_test_engines-0.3.0/aas_test_engines/data/api/samples/asset_info.json`

 * *Files identical despite different names*

### Comparing `aas_test_engines-0.2.1/aas_test_engines/data/api/samples/shell_descriptor.json` & `aas_test_engines-0.3.0/aas_test_engines/data/api/samples/shell_descriptor.json`

 * *Files identical despite different names*

### Comparing `aas_test_engines-0.2.1/aas_test_engines/data/api/samples/submodel.json` & `aas_test_engines-0.3.0/aas_test_engines/data/api/samples/submodel.json`

 * *Files identical despite different names*

### Comparing `aas_test_engines-0.2.1/aas_test_engines/data/api/samples/submodel_descriptor.json` & `aas_test_engines-0.3.0/aas_test_engines/data/api/samples/submodel_descriptor.json`

 * *Files identical despite different names*

### Comparing `aas_test_engines-0.2.1/aas_test_engines/data/api/samples/submodel_element.json` & `aas_test_engines-0.3.0/aas_test_engines/data/api/samples/submodel_element.json`

 * *Files identical despite different names*

### Comparing `aas_test_engines-0.2.1/aas_test_engines/data/file/3.0.yml` & `aas_test_engines-0.3.0/aas_test_engines/data/file/3.0.yml`

 * *Files identical despite different names*

### Comparing `aas_test_engines-0.2.1/aas_test_engines/data_types.py` & `aas_test_engines-0.3.0/aas_test_engines/data_types.py`

 * *Files identical despite different names*

### Comparing `aas_test_engines-0.2.1/aas_test_engines/file.py` & `aas_test_engines-0.3.0/aas_test_engines/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,17 +141,17 @@
     data = ElementTree.fromstring(file.read())
     return check_xml_data(data, version)
 
 
 NS_CONTENT_TYPES = "{http://schemas.openxmlformats.org/package/2006/content-types}"
 NS_RELATIONSHIPS = "{http://schemas.openxmlformats.org/package/2006/relationships}"
 
-TYPE_AASX_ORIGIN = 'http://www.admin-shell.io/aasx/relationships/aasx-origin'
-TYPE_AASX_SPEC = 'http://www.admin-shell.io/aasx/relationships/aas-spec'
-TYPE_AASX_SUPPL = 'http://www.admin-shell.io/aasx/relationships/aas-suppl'
+TYPE_AASX_ORIGIN = 'http://admin-shell.io/aasx/relationships/aasx-origin'
+TYPE_AASX_SPEC = 'http://admin-shell.io/aasx/relationships/aas-spec'
+TYPE_AASX_SUPPL = 'http://admin-shell.io/aasx/relationships/aas-suppl'
 TYPE_THUMBNAIL = 'http://schemas.openxmlformats.org/package/2006/relationships/metadata/thumbnail'
 
 
 class Relationship:
 
     def __init__(self, type: str, target: str) -> None:
         self.type = type
```

### Comparing `aas_test_engines-0.2.1/aas_test_engines/result.py` & `aas_test_engines-0.3.0/aas_test_engines/result.py`

 * *Files identical despite different names*

### Comparing `aas_test_engines-0.2.1/aas_test_engines.egg-info/PKG-INFO` & `aas_test_engines-0.3.0/aas_test_engines.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
-Name: aas-test-engines
-Version: 0.2.1
+Name: aas_test_engines
+Version: 0.3.0
 Summary: Official test tooling for the Asset Administration Shell
 Project-URL: Homepage, https://github.com/admin-shell-io/aas-test-engines
 Keywords: asset administration shell,aas,test
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: requests>=2.31
 Requires-Dist: pyyaml>=6.0
-Requires-Dist: json_schema_tool>=0.1
+Requires-Dist: json_schema_tool>=0.2
 Requires-Dist: jsonpath_ng>=1.5
 Requires-Dist: jsonschema>=4.19
 
 # Test Engines for the Asset Administration Shell
 
 [![Tests](https://github.com/admin-shell-io/aas-test-engines/actions/workflows/check.yml/badge.svg)](https://github.com/admin-shell-io/aas-test-engines/actions/workflows/check.yml)
 
@@ -35,48 +36,59 @@
 
 ### Check AASX:
 ```python
 from aas_test_engines import file
 from xml.etree import ElementTree
 
 with open('aas.aasx') as f:
-    file.check_aasx_file(f)
+    result = file.check_aasx_file(f)
+# result.ok() == True
+
+result.dump()
 ```
 
 ### Check JSON:
 
 ```python
 from aas_test_engines import file
 
 # Check file
 with open('aas.json') as f:
-    file.check_json_file(f)
+    result = file.check_json_file(f)
+# result.ok() == True
 
 # Or check data directly
 aas = {
     'assetAdministrationShells': [],
     'submodels': [],
     'conceptDescriptions': []
 }
-file.check_json_data(aas)
+result = file.check_json_data(aas)
+# result.ok() == True
+
+result.dump()
 ```
 
 ### Check XML:
 ```python
 from aas_test_engines import file
 from xml.etree import ElementTree
 
 # Check file
 with open('aas.xml') as f:
-    file.check_xml_file(f)
+    result = file.check_xml_file(f)
+# result.ok() == True
 
 # Or check data directly
 data = ElementTree.fromstring(
     '<environment xmlns="https://admin-shell.io/aas/3/0" />')
-file.check_xml_data(aas)
+result = file.check_xml_data(aas)
+# result.ok() == True
+
+result.dump()
 ```
 
 ### Checking older versions
 
 By default, the `file.check...` methods check compliance to version 3.0 of the standard.
 You may want to check against older versions by passing a string containing the version to these methods.
```

### Comparing `aas_test_engines-0.2.1/aas_test_engines.egg-info/SOURCES.txt` & `aas_test_engines-0.3.0/aas_test_engines.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+LICENSE
 README.md
 pyproject.toml
 requirements.txt
 aas_test_engines/__init__.py
 aas_test_engines/__main__.py
 aas_test_engines/api.py
 aas_test_engines/data_types.py
 aas_test_engines/exception.py
 aas_test_engines/file.py
+aas_test_engines/py.typed
 aas_test_engines/result.py
 aas_test_engines.egg-info/PKG-INFO
 aas_test_engines.egg-info/SOURCES.txt
 aas_test_engines.egg-info/dependency_links.txt
 aas_test_engines.egg-info/entry_points.txt
 aas_test_engines.egg-info/requires.txt
 aas_test_engines.egg-info/top_level.txt
```

### Comparing `aas_test_engines-0.2.1/pyproject.toml` & `aas_test_engines-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aas_test_engines"
-version = "0.2.1"
+version = "0.3.0"
 description = "Official test tooling for the Asset Administration Shell"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["asset administration shell", "aas", "test"]
```

### Comparing `aas_test_engines-0.2.1/test/test_file.py` & `aas_test_engines-0.3.0/test/test_file.py`

 * *Files 9% similar despite different names*

```diff
@@ -70,21 +70,38 @@
     def test_unknown_filetype(self):
         z = in_memory_zipfile(os.path.join(
             script_dir, 'fixtures/aasx/invalid/unknown_filetype'))
         result = file.check_aasx_data(z)
         result.dump()
         self.assertFalse(result.ok())
 
-    def test_minimal(self):
-        z = in_memory_zipfile(os.path.join(
-            script_dir, 'fixtures/aasx/valid/simple'))
+    def test_valid_xml(self):
+        z = in_memory_zipfile(os.path.join(script_dir, 'fixtures/aasx/valid/xml'))
         result = file.check_aasx_data(z)
         result.dump()
         self.assertTrue(result.ok())
 
+    def test_valid_json(self):
+        z = in_memory_zipfile(os.path.join(script_dir, 'fixtures/aasx/valid/json'))
+        result = file.check_aasx_data(z)
+        result.dump()
+        self.assertTrue(result.ok())
+
+    def test_invalid_xml(self):
+        z = in_memory_zipfile(os.path.join(script_dir, 'fixtures/aasx/invalid/invalid_xml'))
+        result = file.check_aasx_data(z)
+        result.dump()
+        self.assertFalse(result.ok())
+
+    def test_invalid_json(self):
+        z = in_memory_zipfile(os.path.join(script_dir, 'fixtures/aasx/invalid/invalid_json'))
+        result = file.check_aasx_data(z)
+        result.dump()
+        self.assertFalse(result.ok())
+
 
 class SupportedVersionTest(TestCase):
 
     def test_invoke(self):
         s = file.supported_versions()
         for i in s:
             print(i)
```

