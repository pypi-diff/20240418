# Comparing `tmp/graph_validation_tests-0.0.4.tar.gz` & `tmp/graph_validation_tests-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph_validation_tests-0.0.4.tar", max compression
+gzip compressed data, was "graph_validation_tests-0.0.5.tar", max compression
```

## Comparing `graph_validation_tests-0.0.4.tar` & `graph_validation_tests-0.0.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1070 2024-04-17 04:54:03.427763 graph_validation_tests-0.0.4/LICENSE
--rw-r--r--   0        0        0    13357 2024-04-17 04:54:03.427763 graph_validation_tests-0.0.4/README.md
--rw-r--r--   0        0        0    21742 2024-04-17 04:54:03.427763 graph_validation_tests-0.0.4/graph_validation_test/__init__.py
--rw-r--r--   0        0        0    10451 2024-04-17 04:54:03.427763 graph_validation_tests-0.0.4/graph_validation_test/request.py
--rw-r--r--   0        0        0        0 2024-04-17 04:54:03.427763 graph_validation_tests-0.0.4/graph_validation_test/translator/__init__.py
--rw-r--r--   0        0        0    36673 2024-04-17 04:54:03.427763 graph_validation_tests-0.0.4/graph_validation_test/translator/registry/__init__.py
--rw-r--r--   0        0        0    10042 2024-04-17 04:54:03.427763 graph_validation_tests-0.0.4/graph_validation_test/translator/trapi/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 04:54:03.427763 graph_validation_tests-0.0.4/graph_validation_test/utils/__init__.py
--rw-r--r--   0        0        0      722 2024-04-17 04:54:03.427763 graph_validation_tests-0.0.4/graph_validation_test/utils/asyncio.py
--rw-r--r--   0        0        0      113 2024-04-17 04:54:03.431763 graph_validation_tests-0.0.4/graph_validation_test/utils/constants.py
--rw-r--r--   0        0        0      886 2024-04-17 04:54:03.431763 graph_validation_tests-0.0.4/graph_validation_test/utils/http.py
--rw-r--r--   0        0        0     4271 2024-04-17 04:54:03.431763 graph_validation_tests-0.0.4/graph_validation_test/utils/ontology_kp.py
--rw-r--r--   0        0        0     7957 2024-04-17 04:54:03.431763 graph_validation_tests-0.0.4/graph_validation_test/utils/testsuite.py
--rw-r--r--   0        0        0    18148 2024-04-17 04:54:03.431763 graph_validation_tests-0.0.4/graph_validation_test/utils/unit_test_templates.py
--rw-r--r--   0        0        0     8957 2024-04-17 04:54:03.431763 graph_validation_tests-0.0.4/one_hop_test/__init__.py
--rw-r--r--   0        0        0     2833 2024-04-17 04:54:15.507779 graph_validation_tests-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4851 2024-04-17 04:54:03.431763 graph_validation_tests-0.0.4/standards_validation_test/__init__.py
--rw-r--r--   0        0        0     1256 2024-04-17 04:54:03.431763 graph_validation_tests-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 04:54:03.431763 graph_validation_tests-0.0.4/tests/graph_validation_test/__init__.py
--rw-r--r--   0        0        0     3855 2024-04-17 04:54:03.431763 graph_validation_tests-0.0.4/tests/graph_validation_test/test_graph_validation_test.py
--rw-r--r--   0        0        0     5746 2024-04-17 04:54:03.431763 graph_validation_tests-0.0.4/tests/graph_validation_test/test_unit_test_templates.py
--rw-r--r--   0        0        0        0 2024-04-17 04:54:03.431763 graph_validation_tests-0.0.4/tests/graph_validation_test/translator/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 04:54:03.431763 graph_validation_tests-0.0.4/tests/graph_validation_test/translator/biolink/__init__.py
--rw-r--r--   0        0        0     1183 2024-04-17 04:54:03.431763 graph_validation_tests-0.0.4/tests/graph_validation_test/translator/biolink/test_ontology_kp.py
--rw-r--r--   0        0        0    18171 2024-04-17 04:54:03.431763 graph_validation_tests-0.0.4/tests/graph_validation_test/translator/test_translator_smartapi_registry.py
--rw-r--r--   0        0        0        0 2024-04-17 04:54:03.431763 graph_validation_tests-0.0.4/tests/graph_validation_test/translator/trapi/__init__.py
--rw-r--r--   0        0        0     5320 2024-04-17 04:54:03.431763 graph_validation_tests-0.0.4/tests/graph_validation_test/translator/trapi/test_trapi.py
--rw-r--r--   0        0        0        0 2024-04-17 04:54:03.431763 graph_validation_tests-0.0.4/tests/one_hop_test/__init__.py
--rw-r--r--   0        0        0     2874 2024-04-17 04:54:03.431763 graph_validation_tests-0.0.4/tests/one_hop_test/test_one_hop_test.py
--rw-r--r--   0        0        0    25697 2024-04-17 04:54:03.431763 graph_validation_tests-0.0.4/tests/one_hop_test/test_venv/Scripts/Activate.ps1
--rw-r--r--   0        0        0     2063 2024-04-17 04:54:03.431763 graph_validation_tests-0.0.4/tests/one_hop_test/test_venv/Scripts/activate
--rw-r--r--   0        0        0     1027 2024-04-17 04:54:03.431763 graph_validation_tests-0.0.4/tests/one_hop_test/test_venv/Scripts/activate.bat
--rw-r--r--   0        0        0      371 2024-04-17 04:54:03.431763 graph_validation_tests-0.0.4/tests/one_hop_test/test_venv/Scripts/deactivate.bat
--rw-r--r--   0        0        0   108460 2024-04-17 04:54:03.435763 graph_validation_tests-0.0.4/tests/one_hop_test/test_venv/Scripts/pip.exe
--rw-r--r--   0        0        0   108460 2024-04-17 04:54:03.435763 graph_validation_tests-0.0.4/tests/one_hop_test/test_venv/Scripts/pip3.10.exe
--rw-r--r--   0        0        0   108460 2024-04-17 04:54:03.435763 graph_validation_tests-0.0.4/tests/one_hop_test/test_venv/Scripts/pip3.exe
--rw-r--r--   0        0        0   268568 2024-04-17 04:54:03.435763 graph_validation_tests-0.0.4/tests/one_hop_test/test_venv/Scripts/python.exe
--rw-r--r--   0        0        0   257304 2024-04-17 04:54:03.439763 graph_validation_tests-0.0.4/tests/one_hop_test/test_venv/Scripts/pythonw.exe
--rw-r--r--   0        0        0      164 2024-04-17 04:54:03.439763 graph_validation_tests-0.0.4/tests/one_hop_test/test_venv/pyvenv.cfg
--rw-r--r--   0        0        0       70 2024-04-17 04:54:03.439763 graph_validation_tests-0.0.4/tests/scripts/one_hop_test.cmd
--rw-r--r--   0        0        0        0 2024-04-17 04:54:03.439763 graph_validation_tests-0.0.4/tests/standards_validation_test/__init__.py
--rw-r--r--   0        0        0     1467 2024-04-17 04:54:03.439763 graph_validation_tests-0.0.4/tests/standards_validation_test/test_standards_validation_test.py
--rw-r--r--   0        0        0    15403 1970-01-01 00:00:00.000000 graph_validation_tests-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-17 23:10:59.294165 graph_validation_tests-0.0.5/LICENSE
+-rw-r--r--   0        0        0    11619 2024-04-17 23:10:59.294165 graph_validation_tests-0.0.5/README.md
+-rw-r--r--   0        0        0    21742 2024-04-17 23:10:59.298165 graph_validation_tests-0.0.5/graph_validation_test/__init__.py
+-rw-r--r--   0        0        0    10451 2024-04-17 23:10:59.298165 graph_validation_tests-0.0.5/graph_validation_test/request.py
+-rw-r--r--   0        0        0        0 2024-04-17 23:10:59.298165 graph_validation_tests-0.0.5/graph_validation_test/translator/__init__.py
+-rw-r--r--   0        0        0    36673 2024-04-17 23:10:59.298165 graph_validation_tests-0.0.5/graph_validation_test/translator/registry/__init__.py
+-rw-r--r--   0        0        0    10042 2024-04-17 23:10:59.298165 graph_validation_tests-0.0.5/graph_validation_test/translator/trapi/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 23:10:59.298165 graph_validation_tests-0.0.5/graph_validation_test/utils/__init__.py
+-rw-r--r--   0        0        0      722 2024-04-17 23:10:59.298165 graph_validation_tests-0.0.5/graph_validation_test/utils/asyncio.py
+-rw-r--r--   0        0        0      113 2024-04-17 23:10:59.298165 graph_validation_tests-0.0.5/graph_validation_test/utils/constants.py
+-rw-r--r--   0        0        0      886 2024-04-17 23:10:59.298165 graph_validation_tests-0.0.5/graph_validation_test/utils/http.py
+-rw-r--r--   0        0        0     4267 2024-04-17 23:10:59.298165 graph_validation_tests-0.0.5/graph_validation_test/utils/ontology_kp.py
+-rw-r--r--   0        0        0     7957 2024-04-17 23:10:59.298165 graph_validation_tests-0.0.5/graph_validation_test/utils/testsuite.py
+-rw-r--r--   0        0        0    18148 2024-04-17 23:10:59.298165 graph_validation_tests-0.0.5/graph_validation_test/utils/unit_test_templates.py
+-rw-r--r--   0        0        0     8957 2024-04-17 23:10:59.298165 graph_validation_tests-0.0.5/one_hop_test/__init__.py
+-rw-r--r--   0        0        0     2856 2024-04-17 23:11:11.218260 graph_validation_tests-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4851 2024-04-17 23:10:59.298165 graph_validation_tests-0.0.5/standards_validation_test/__init__.py
+-rw-r--r--   0        0        0     1250 2024-04-17 23:10:59.298165 graph_validation_tests-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 23:10:59.298165 graph_validation_tests-0.0.5/tests/graph_validation_test/__init__.py
+-rw-r--r--   0        0        0     3855 2024-04-17 23:10:59.298165 graph_validation_tests-0.0.5/tests/graph_validation_test/test_graph_validation_test.py
+-rw-r--r--   0        0        0     5764 2024-04-17 23:10:59.298165 graph_validation_tests-0.0.5/tests/graph_validation_test/test_unit_test_templates.py
+-rw-r--r--   0        0        0        0 2024-04-17 23:10:59.298165 graph_validation_tests-0.0.5/tests/graph_validation_test/translator/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 23:10:59.298165 graph_validation_tests-0.0.5/tests/graph_validation_test/translator/biolink/__init__.py
+-rw-r--r--   0        0        0     1065 2024-04-17 23:10:59.298165 graph_validation_tests-0.0.5/tests/graph_validation_test/translator/biolink/test_ontology_kp.py
+-rw-r--r--   0        0        0    18030 2024-04-17 23:10:59.298165 graph_validation_tests-0.0.5/tests/graph_validation_test/translator/test_translator_smartapi_registry.py
+-rw-r--r--   0        0        0        0 2024-04-17 23:10:59.298165 graph_validation_tests-0.0.5/tests/graph_validation_test/translator/trapi/__init__.py
+-rw-r--r--   0        0        0     5061 2024-04-17 23:10:59.298165 graph_validation_tests-0.0.5/tests/graph_validation_test/translator/trapi/test_trapi.py
+-rw-r--r--   0        0        0        0 2024-04-17 23:10:59.298165 graph_validation_tests-0.0.5/tests/one_hop_test/__init__.py
+-rw-r--r--   0        0        0     3149 2024-04-17 23:10:59.298165 graph_validation_tests-0.0.5/tests/one_hop_test/test_one_hop_test.py
+-rw-r--r--   0        0        0    25697 2024-04-17 23:10:59.302165 graph_validation_tests-0.0.5/tests/one_hop_test/test_venv/Scripts/Activate.ps1
+-rw-r--r--   0        0        0     2063 2024-04-17 23:10:59.302165 graph_validation_tests-0.0.5/tests/one_hop_test/test_venv/Scripts/activate
+-rw-r--r--   0        0        0     1027 2024-04-17 23:10:59.302165 graph_validation_tests-0.0.5/tests/one_hop_test/test_venv/Scripts/activate.bat
+-rw-r--r--   0        0        0      371 2024-04-17 23:10:59.302165 graph_validation_tests-0.0.5/tests/one_hop_test/test_venv/Scripts/deactivate.bat
+-rw-r--r--   0        0        0   108460 2024-04-17 23:10:59.302165 graph_validation_tests-0.0.5/tests/one_hop_test/test_venv/Scripts/pip.exe
+-rw-r--r--   0        0        0   108460 2024-04-17 23:10:59.302165 graph_validation_tests-0.0.5/tests/one_hop_test/test_venv/Scripts/pip3.10.exe
+-rw-r--r--   0        0        0   108460 2024-04-17 23:10:59.302165 graph_validation_tests-0.0.5/tests/one_hop_test/test_venv/Scripts/pip3.exe
+-rw-r--r--   0        0        0   268568 2024-04-17 23:10:59.306165 graph_validation_tests-0.0.5/tests/one_hop_test/test_venv/Scripts/python.exe
+-rw-r--r--   0        0        0   257304 2024-04-17 23:10:59.306165 graph_validation_tests-0.0.5/tests/one_hop_test/test_venv/Scripts/pythonw.exe
+-rw-r--r--   0        0        0      164 2024-04-17 23:10:59.306165 graph_validation_tests-0.0.5/tests/one_hop_test/test_venv/pyvenv.cfg
+-rw-r--r--   0        0        0       70 2024-04-17 23:10:59.306165 graph_validation_tests-0.0.5/tests/scripts/one_hop_test.cmd
+-rw-r--r--   0        0        0        0 2024-04-17 23:10:59.306165 graph_validation_tests-0.0.5/tests/standards_validation_test/__init__.py
+-rw-r--r--   0        0        0     1567 2024-04-17 23:10:59.306165 graph_validation_tests-0.0.5/tests/standards_validation_test/test_standards_validation_test.py
+-rw-r--r--   0        0        0    13665 1970-01-01 00:00:00.000000 graph_validation_tests-0.0.5/PKG-INFO
```

### Comparing `graph_validation_tests-0.0.4/LICENSE` & `graph_validation_tests-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.4/graph_validation_test/__init__.py` & `graph_validation_tests-0.0.5/graph_validation_test/__init__.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.4/graph_validation_test/request.py` & `graph_validation_tests-0.0.5/graph_validation_test/request.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.4/graph_validation_test/translator/registry/__init__.py` & `graph_validation_tests-0.0.5/graph_validation_test/translator/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.4/graph_validation_test/translator/trapi/__init__.py` & `graph_validation_tests-0.0.5/graph_validation_test/translator/trapi/__init__.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.4/graph_validation_test/utils/asyncio.py` & `graph_validation_tests-0.0.5/graph_validation_test/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.4/graph_validation_test/utils/http.py` & `graph_validation_tests-0.0.5/graph_validation_test/utils/http.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.4/graph_validation_test/utils/ontology_kp.py` & `graph_validation_tests-0.0.5/graph_validation_test/utils/ontology_kp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Ontology KP interface
 """
 from typing import Optional
 from reasoner_validator.biolink import get_biolink_model_toolkit
 from graph_validation_test.utils.http import post_query
 
-ONTOLOGY_KP_TRAPI_SERVER = "https://automat.renci.org/ubergraph/1.4/query"
+ONTOLOGY_KP_TRAPI_SERVER = "https://automat.renci.org/ubergraph/query"
 NODE_NORMALIZER_SERVER = "https://nodenormalization-sri.renci.org/get_normalized_nodes"
 
 
 def convert_to_preferred(curie, allowed_list):
     """
     :param curie
     :param allowed_list
```

### Comparing `graph_validation_tests-0.0.4/graph_validation_test/utils/testsuite.py` & `graph_validation_tests-0.0.5/graph_validation_test/utils/testsuite.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.4/graph_validation_test/utils/unit_test_templates.py` & `graph_validation_tests-0.0.5/graph_validation_test/utils/unit_test_templates.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.4/one_hop_test/__init__.py` & `graph_validation_tests-0.0.5/one_hop_test/__init__.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.4/pyproject.toml` & `graph_validation_tests-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graph-validation-tests"
-version = "0.0.4"
+version = "0.0.5"
 description = "Validation of Translator Knowledge Graphs - TRAPI, Biolink Model and One Hop navigation"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Chris Bizon <bizon.renci.org>",
     "Tim Putnam <tim@tislab>"
 ]
 maintainers = ["Richard Bruskiewich <richard.bruskiewich@delphinai.com>"]
@@ -49,16 +49,16 @@
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 deepdiff = "^6.7.1"
 
 #reasoner-validator = { git = "https://github.com/NCATSTranslator/reasoner-validator.git", branch = "graph-validation-test-revisions" }
 reasoner-validator = "^4.0.0"
 
-#translator-testing-model = { git = "https://github.com/TranslatorSRI/TranslatorTestingModel.git", branch = "main" }
-translator-testing-model = "^0.2.5"
+#translator-testing-model = { git = "https://github.com/TranslatorSRI/TranslatorTestingModel.git", branch = "add_missing_test_objectives" }
+translator-testing-model = "^0.2.6"
 
 pytest = "^7.4.2"
 pytest-asyncio = "^0.23.3"
 fastapi = "^0.110.0"
 httpx = "^0.27.0"
 tqdm = "^4.66.2"
 reasoner-pydantic = "^4.1.6"
```

### Comparing `graph_validation_tests-0.0.4/standards_validation_test/__init__.py` & `graph_validation_tests-0.0.5/standards_validation_test/__init__.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.4/tests/__init__.py` & `graph_validation_tests-0.0.5/tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 DEFAULT_TRAPI_VERSION = get_latest_version("1")
 DEFAULT_BMT: Toolkit = get_biolink_model_toolkit()
 SAMPLE_TEST_INPUT_1 = {
     # One test edge (asset)
     "subject_id": "DRUGBANK:DB01592",
     "subject_category": "biolink:SmallMolecule",
-    "predicate_id": "biolink:ameliorates_condition",
+    "predicate_id": "biolink:has_side_effect",
     "object_id": "MONDO:0011426",
     "object_category": "biolink:Disease",
     #
     #     "environment": environment, # Optional[TestEnvEnum] = None; default: 'TestEnvEnum.ci' if not given
     #     "components": components,  # Optional[str] = None; default: 'ars' if not given
     #     "trapi_version": trapi_version,  # Optional[str] = None; latest community release if not given
     #     "biolink_version": biolink_version,  # Optional[str] = None; current Biolink Toolkit default if not given
```

### Comparing `graph_validation_tests-0.0.4/tests/graph_validation_test/test_graph_validation_test.py` & `graph_validation_tests-0.0.5/tests/graph_validation_test/test_graph_validation_test.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.4/tests/graph_validation_test/test_unit_test_templates.py` & `graph_validation_tests-0.0.5/tests/graph_validation_test/test_unit_test_templates.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     invert_association,
 )
 
 
 TEST_ASSET_1 = {
     "subject_id": "DRUGBANK:DB01592",
     "subject_category": "biolink:SmallMolecule",
-    "predicate_id": "biolink:treats",
+    "predicate_id": "biolink:has_side_effect",
     "object_id": "MONDO:0011426",
     "object_category": "biolink:Disease"
 }
 
 TEST_TRAPI_TEMPLATE = {
     "message": {
         "query_graph": {
@@ -33,15 +33,15 @@
                     "categories": ["biolink:Disease"]
                 },
             },
             "edges": {
                 "ab": {
                     "subject": "a",
                     "object": "b",
-                    "predicates": ["biolink:treats"]
+                    "predicates": ["biolink:has_side_effect"]
                 }
             }
         },
         "knowledge_graph": {
             "nodes": {}, "edges": {},
         },
         "results": []
```

### Comparing `graph_validation_tests-0.0.4/tests/graph_validation_test/translator/biolink/test_ontology_kp.py` & `graph_validation_tests-0.0.5/tests/graph_validation_test/translator/biolink/test_ontology_kp.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
 from typing import Optional
 from graph_validation_test.utils.ontology_kp import get_parent_concept
 
 import pytest
 
 
-@pytest.mark.skip("Ubergraph offline on April 16th, 2024, but need to deploy this project without unit test failure")
 @pytest.mark.parametrize(
     "curie,category,result",
     [
         (   # Query 0 - chemical compounds are NOT in an ontology hierarchy
             "CHEMBL.COMPOUND:CHEMBL2333026",
             "biolink:SmallMolecule",
             None
```

### Comparing `graph_validation_tests-0.0.4/tests/graph_validation_test/translator/test_translator_smartapi_registry.py` & `graph_validation_tests-0.0.5/tests/graph_validation_test/translator/test_translator_smartapi_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -472,25 +472,22 @@
         assert 'url' in resource_metadata
         assert url in resource_metadata['url']
         assert x_maturity in resource_metadata['x_maturity']
     else:
         assert not resource_metadata
 
 
-@pytest.mark.skip(
-    "Translator endpoints in transition on April 16th, 2024, but need to deploy this project without unit test failure"
-)
 @pytest.mark.parametrize(
     "component,environment,result",
     [
         ("arax", "dev", "https://arax.ncats.io/beta/api/arax/v1.4"),
         ("aragorn", "ci", "https://aragorn.ci.transltr.io/aragorn"),
         ("biothings-explorer", "test", "https://bte.test.transltr.io/v1"),
         ("improving-agent", "test", "https://ia.test.transltr.io/api/v1.4/"),
-        ("molepro", "ci", "https://molepro-trapi.ci.transltr.io/molepro/trapi/v1.4"),
+        ("molepro", "ci", "https://molepro-trapi.ci.transltr.io/molepro/trapi/v1.5"),
         ("foobar", "ci", None)
     ]
 )
 def test_get_component_endpoint_from_registry(
         component: str,
         environment: str,
         result: Optional[str]
```

### Comparing `graph_validation_tests-0.0.4/tests/graph_validation_test/translator/trapi/test_trapi.py` & `graph_validation_tests-0.0.5/tests/graph_validation_test/translator/trapi/test_trapi.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,29 +34,26 @@
         ("molepro", "molepro")
     ]
 )
 def test_get_get_component_infores_object_id(component: str, infores: str):
     assert get_component_infores_object_id(component=component) == infores
 
 
-@pytest.mark.skip(
-    "Translator endpoints in transition on April 16th, 2024, but need to deploy this project without unit test failure"
-)
 @pytest.mark.parametrize(
     "component,environment,result",
     [
         (None, None, f"https://ars.ci.transltr.io/ars/api/"),
         ("ars", None, f"https://ars.ci.transltr.io/ars/api/"),
         ("ars", "non-environment", None),
         ("ars", "test", f"https://ars.test.transltr.io/ars/api/"),
         ("arax", "dev", "https://arax.ncats.io/beta/api/arax/v1.4"),
         ("aragorn", "ci", "https://aragorn.ci.transltr.io/aragorn"),
         ("biothings-explorer", "test", "https://bte.test.transltr.io/v1"),
         ("improving-agent", "test", "https://ia.test.transltr.io/api/v1.4/"),
-        ("molepro", "ci", "https://molepro-trapi.ci.transltr.io/molepro/trapi/v1.4"),
+        ("molepro", "ci", "https://molepro-trapi.ci.transltr.io/molepro/trapi/v1.5"),
         ("foobar", "ci", None),
         ("arax", "non-environment", None),
     ]
 )
 def test_resolve_component_endpoint(
         component: Optional[str],
         environment: Optional[str],
@@ -68,15 +65,14 @@
             environment=environment,
             target_trapi_version=None,
             target_biolink_version=None
         )
     assert endpoint == result
 
 
-@pytest.mark.skip("Ubergraph offline on April 16th, 2024, but need to deploy this project without unit test failure")
 @pytest.mark.parametrize(
     "curie,category,result",
     [
         (   # Query 0 - chemical compounds are NOT in ontology hierarchy
             "CHEMBL.COMPOUND:CHEMBL2333026",
             "biolink:SmallMolecule",
             None
```

### Comparing `graph_validation_tests-0.0.4/tests/one_hop_test/test_one_hop_test.py` & `graph_validation_tests-0.0.5/tests/one_hop_test/test_one_hop_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         raise_object_entity,
         raise_object_by_subject,
         raise_predicate_by_subject
     ]
     results: Dict = await OneHopTest.run_tests(
         **SAMPLE_TEST_INPUT_1,
         trapi_generators=trapi_generators,
-        environment=TestEnvEnum.ci,
+        environment=TestEnvEnum.prod,
         components="arax,molepro"
     )
     dump(results, stderr, indent=4)
 
 
 # ARS tests not yet supported so yes... results will
 # always be empty, with a logger message to inform why
@@ -53,37 +53,49 @@
         raise_object_entity,
         raise_object_by_subject,
         raise_predicate_by_subject
     ]
     results: Dict = await OneHopTest.run_tests(
         **SAMPLE_TEST_INPUT_1,
         trapi_generators=trapi_generators,
-        environment=TestEnvEnum.ci
+        environment=TestEnvEnum.prod
     )
     assert not results
 
 
 @pytest.mark.asyncio
 async def test_run_one_hop_tests():
-    results: Dict = await run_one_hop_tests(**SAMPLE_TEST_INPUT_1, components="arax,molepro")
+    results: Dict = await run_one_hop_tests(
+        **SAMPLE_TEST_INPUT_1,
+        environment=TestEnvEnum.prod,
+        components="arax,molepro"
+    )
     assert results
+    dump(results, stderr, indent=4)
 
 
 @pytest.mark.asyncio
 async def test_run_one_hop_tests_with_runner_parameters():
-    results: Dict = await run_one_hop_tests(**SAMPLE_TEST_INPUT_1, components="arax,molepro")
+    results: Dict = await run_one_hop_tests(
+        **SAMPLE_TEST_INPUT_1,
+        environment=TestEnvEnum.prod,
+        components="arax,molepro",
+        strict_validation=True
+    )
     assert results
+    dump(results, stderr, indent=4)
 
 
 # subprocess.run(
 #     args, *, stdin=None, input=None, stdout=None, stderr=None,
 #     capture_output=False, shell=False, cwd=None, timeout=None,
 #     check=False, encoding=None, errors=None, text=None, env=None,
 #     universal_newlines=None, **other_popen_kwargs
 # )
+@pytest.mark.skip("Not yet fully implemented")
 def test_one_hop_cli():
     # command: List = ["python", "-m", "one_hop_test.__init__"]
     # args: Dict = SAMPLE_TEST_INPUT_1.copy()
     # args["components"] = "arax,molepro"
     # [command.extend([f"--{flag}", value]) for flag, value in args.items()]
     # results = check_output(command)
     # results = check_output(["dir"])
```

### Comparing `graph_validation_tests-0.0.4/tests/one_hop_test/test_venv/Scripts/Activate.ps1` & `graph_validation_tests-0.0.5/tests/one_hop_test/test_venv/Scripts/Activate.ps1`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.4/tests/one_hop_test/test_venv/Scripts/activate` & `graph_validation_tests-0.0.5/tests/one_hop_test/test_venv/Scripts/activate`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.4/tests/one_hop_test/test_venv/Scripts/activate.bat` & `graph_validation_tests-0.0.5/tests/one_hop_test/test_venv/Scripts/activate.bat`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.4/tests/one_hop_test/test_venv/Scripts/pip.exe` & `graph_validation_tests-0.0.5/tests/one_hop_test/test_venv/Scripts/pip.exe`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.4/tests/one_hop_test/test_venv/Scripts/pip3.10.exe` & `graph_validation_tests-0.0.5/tests/one_hop_test/test_venv/Scripts/pip3.10.exe`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.4/tests/one_hop_test/test_venv/Scripts/pip3.exe` & `graph_validation_tests-0.0.5/tests/one_hop_test/test_venv/Scripts/pip3.exe`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.4/tests/one_hop_test/test_venv/Scripts/python.exe` & `graph_validation_tests-0.0.5/tests/one_hop_test/test_venv/Scripts/python.exe`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.4/tests/one_hop_test/test_venv/Scripts/pythonw.exe` & `graph_validation_tests-0.0.5/tests/one_hop_test/test_venv/Scripts/pythonw.exe`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.4/tests/standards_validation_test/test_standards_validation_test.py` & `graph_validation_tests-0.0.5/tests/standards_validation_test/test_standards_validation_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     trapi_generators = [
         by_subject,
         by_object
     ]
     results: Dict = await StandardsValidationTest.run_tests(
         **SAMPLE_TEST_INPUT_1,
         trapi_generators=trapi_generators,
-        environment=TestEnvEnum.ci,
+        environment=TestEnvEnum.prod,
         components="arax,molepro"
     )
     dump(results, stderr, indent=4)
 
 
 # ARS tests not yet supported so yes... results will
 # always be empty, with a logger message to inform why
@@ -34,16 +34,21 @@
     trapi_generators = [
         by_subject,
         by_object
     ]
     results: Dict = await StandardsValidationTest.run_tests(
         **SAMPLE_TEST_INPUT_1,
         trapi_generators=trapi_generators,
-        environment=TestEnvEnum.ci
+        environment=TestEnvEnum.prod
     )
     assert not results
 
 
 @pytest.mark.asyncio
 async def test_run_standards_validation_tests():
-    results: Dict = await run_standards_validation_tests(**SAMPLE_TEST_INPUT_1, components="arax,molepro")
+    results: Dict = await run_standards_validation_tests(
+        **SAMPLE_TEST_INPUT_1,
+        environment=TestEnvEnum.prod,
+        components="arax,molepro"
+    )
     assert results
+    dump(results, stderr, indent=4)
```

### Comparing `graph_validation_tests-0.0.4/PKG-INFO` & `graph_validation_tests-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graph-validation-tests
-Version: 0.0.4
+Version: 0.0.5
 Summary: Validation of Translator Knowledge Graphs - TRAPI, Biolink Model and One Hop navigation
 Home-page: https://github.com/TranslatorSRI
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
@@ -28,15 +28,15 @@
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
 Requires-Dist: pytest (>=7.4.2,<8.0.0)
 Requires-Dist: pytest-asyncio (>=0.23.3,<0.24.0)
 Requires-Dist: reasoner-pydantic (>=4.1.6,<5.0.0)
 Requires-Dist: reasoner-validator (>=4.0.0,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
-Requires-Dist: translator-testing-model (>=0.2.5,<0.3.0)
+Requires-Dist: translator-testing-model (>=0.2.6,<0.3.0)
 Project-URL: Bug Tracker, https://github.com/TranslatorSRI/GraphValidationTests/issues
 Project-URL: Change Log, https://github.com/TranslatorSRI/GraphValidationTests/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/TranslatorSRI/GraphValidationTests/blob/main/README.md
 Project-URL: Repository, https://github.com/TranslatorSRI/GraphValidationTests
 Description-Content-Type: text/markdown
 
 # Graph Validation Tests
@@ -136,15 +136,15 @@
 import asyncio
 from standards_validation_test import run_standards_validation_tests
 
 test_data = {
     # One test edge (asset)
     "subject_id": "DRUGBANK:DB01592",
     "subject_category": "biolink:SmallMolecule",
-    "predicate_id": "biolink:treats",
+    "predicate_id": "biolink:has_side_effect",
     "object_id": "MONDO:0011426",
     "object_category": "biolink:Disease",
     "components": "arax,molepro"
     #     "environment": environment, # Optional[TestEnvEnum] = None; default: 'TestEnvEnum.ci' if not given
     #     "trapi_version": trapi_version,  # Optional[str] = None; latest community release if not given
     #     "biolink_version": biolink_version,  # Optional[str] = None; current Biolink Toolkit default if not given
     #     "runner_settings": asset.test_runner_settings,  # Optional[List[str]] = None
@@ -162,15 +162,15 @@
 import asyncio
 from one_hop_test import run_one_hop_tests
 
 test_data = {
     # One test edge (asset)
     "subject_id": "DRUGBANK:DB01592",
     "subject_category": "biolink:SmallMolecule",
-    "predicate_id": "biolink:treats",
+    "predicate_id": "biolink:has_side_effect",
     "object_id": "MONDO:0011426",
     "object_category": "biolink:Disease",
     "components": "arax,molepro"
     #
     #     "environment": environment, # Optional[TestEnvEnum] = None; default: 'TestEnvEnum.ci' if not given
     #     "trapi_version": trapi_version,  # Optional[str] = None; latest community release if not given
     #     "biolink_version": biolink_version,  # Optional[str] = None; current Biolink Toolkit default if not given
@@ -197,15 +197,15 @@
     raise_predicate_by_subject
 )
 
 test_data = {
     # One test edge (asset)
     "subject_id": "DRUGBANK:DB01592",
     "subject_category": "biolink:SmallMolecule",
-    "predicate_id": "biolink:treats",
+    "predicate_id": "biolink:has_side_effect",
     "object_id": "MONDO:0011426",
     "object_category": "biolink:Disease",
     "components": "arax,molepro",
     "environment": TestEnvEnum.test,
     "trapi_version": "1.5.0-beta",
     "biolink_version": "4.1.6",
     "runner_settings": "Inferred"
@@ -246,84 +246,40 @@
                     "by_subject": {
                         "info": {},
                         "skipped": {},
                         "warning": {},
                         "error": {
                             "error.trapi.response.knowledge_graph.missing_expected_edge": {
                                 "global": {
-                                    "TestAsset:00001|(DRUGBANK:DB01592#biolink:SmallMolecule)-[biolink:treats]->(MONDO:0011426#biolink:Disease)": null
+                                    "TestAsset:00001|(DRUGBANK:DB01592#biolink:SmallMolecule)-[biolink:has_side_effect]->(MONDO:0011426#biolink:Disease)": null
                                 }
                             }
                         },
                         "critical": {}
                     }
                 }
             },
-            {
-                "arax": {
-                    "inverse_by_new_subject": {
-                        "info": {},
-                        "skipped": {},
-                        "warning": {},
-                        "error": {},
-                        "critical": {
-                            "critical.trapi.request.invalid": {
-                                "global": {
-                                    "predicate 'biolink:treats'": [
-                                        {
-                                            "context": "inverse_by_new_subject",
-                                            "reason": "is an unknown or has no inverse?"
-                                        }
-                                    ]
-                                }
-                            }
-                        }
-                    }
-                }
-            },
 etc ...
             {
                 "molepro": {
                     "by_subject": {
                         "info": {},
                         "skipped": {},
                         "warning": {},
                         "error": {
                             "error.trapi.response.knowledge_graph.missing_expected_edge": {
                                 "global": {
-                                    "TestAsset:00001|(DRUGBANK:DB01592#biolink:SmallMolecule)-[biolink:treats]->(MONDO:0011426#biolink:Disease)": null
+                                    "TestAsset:00001|(DRUGBANK:DB01592#biolink:SmallMolecule)-[biolink:has_side_effect]->(MONDO:0011426#biolink:Disease)": null
                                 }
                             }
                         },
                         "critical": {}
                     }
                 }
             },
-            {
-                "molepro": {
-                    "inverse_by_new_subject": {
-                        "info": {},
-                        "skipped": {},
-                        "warning": {},
-                        "error": {},
-                        "critical": {
-                            "critical.trapi.request.invalid": {
-                                "global": {
-                                    "predicate 'biolink:treats'": [
-                                        {
-                                            "context": "inverse_by_new_subject",
-                                            "reason": "is an unknown or has no inverse?"
-                                        }
-                                    ]
-                                }
-                            }
-                        }
-                    }
-                }
-            },
 etc...
         ]
     ]
 }
 ```
 
 ## Releases
```

