# Comparing `tmp/mustrd-0.1.7.tar.gz` & `tmp/mustrd-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mustrd-0.1.7.tar", max compression
+gzip compressed data, was "mustrd-0.1.8.tar", max compression
```

## Comparing `mustrd-0.1.7.tar` & `mustrd-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,30 @@
--rw-r--r--   0        0        0     1099 2024-02-26 13:34:46.564344 mustrd-0.1.7/LICENSE
--rw-r--r--   0        0        0        0 2023-01-04 15:17:21.216939 mustrd-0.1.7/mustrd/__init__.py
--rw-r--r--   0        0        0     1630 2024-03-25 13:41:52.297143 mustrd-0.1.7/mustrd/logger_setup.py
--rw-r--r--   0        0        0     9709 2024-02-26 13:34:46.565338 mustrd-0.1.7/mustrd/model/mustrdShapes.ttl
--rw-r--r--   0        0        0    17226 2024-02-26 13:34:46.566843 mustrd-0.1.7/mustrd/model/ontology.ttl
--rw-r--r--   0        0        0     1558 2024-02-26 13:34:46.567852 mustrd-0.1.7/mustrd/model/test-resources/resources.ttl
--rw-r--r--   0        0        0    34109 2024-03-26 10:30:15.658796 mustrd-0.1.7/mustrd/mustrd.py
--rw-r--r--   0        0        0    11822 2024-03-26 11:44:28.031509 mustrd-0.1.7/mustrd/mustrdAnzo.py
--rw-r--r--   0        0        0     5599 2024-03-25 13:41:56.824150 mustrd-0.1.7/mustrd/mustrdGraphDb.py
--rw-r--r--   0        0        0     2129 2024-03-25 13:41:56.397230 mustrd-0.1.7/mustrd/mustrdRdfLib.py
--rw-r--r--   0        0        0    11784 2024-03-26 15:45:24.143136 mustrd-0.1.7/mustrd/mustrdTestPlugin.py
--rw-r--r--   0        0        0     3326 2024-03-25 13:41:55.946266 mustrd-0.1.7/mustrd/namespace.py
--rw-r--r--   0        0        0    11803 2024-02-26 13:34:46.570852 mustrd-0.1.7/mustrd/README.adoc
--rw-r--r--   0        0        0     4366 2024-03-25 13:45:02.349067 mustrd-0.1.7/mustrd/run.py
--rw-r--r--   0        0        0    32487 2024-03-25 14:41:03.222617 mustrd-0.1.7/mustrd/spec_component.py
--rw-r--r--   0        0        0     7430 2024-03-25 13:45:25.985161 mustrd-0.1.7/mustrd/steprunner.py
--rw-r--r--   0        0        0      526 2024-03-20 09:48:11.954650 mustrd-0.1.7/mustrd/templates/md_ResultList_leaf_template.jinja
--rw-r--r--   0        0        0      211 2024-03-20 09:44:31.704239 mustrd-0.1.7/mustrd/templates/md_ResultList_template.jinja
--rw-r--r--   0        0        0      157 2024-03-20 09:11:57.505980 mustrd-0.1.7/mustrd/templates/md_stats_template.jinja
--rw-r--r--   0        0        0     4986 2024-03-25 17:16:42.304350 mustrd-0.1.7/mustrd/TestResult.py
--rw-r--r--   0        0        0     1424 2024-03-25 14:51:20.065163 mustrd-0.1.7/mustrd/utils.py
--rw-r--r--   0        0        0     1493 2024-03-26 16:10:31.745289 mustrd-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2724 2024-02-26 13:34:46.565338 mustrd-0.1.7/README.adoc
--rw-r--r--   0        0        0     4130 1970-01-01 00:00:00.000000 mustrd-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1099 2024-02-26 13:34:46.564344 mustrd-0.1.8/LICENSE
+-rw-r--r--   0        0        0        0 2024-03-28 15:41:42.375415 mustrd-0.1.8/mustrd/__init__.py
+-rw-r--r--   0        0        0     1630 2024-03-28 15:41:42.377427 mustrd-0.1.8/mustrd/logger_setup.py
+-rw-r--r--   0        0        0      386 2024-04-03 15:10:48.653712 mustrd-0.1.8/mustrd/model/catalog-v001.xml
+-rw-r--r--   0        0        0     9709 2024-03-28 15:41:42.379427 mustrd-0.1.8/mustrd/model/mustrdShapes.ttl
+-rw-r--r--   0        0        0     2034 2024-04-15 09:12:19.357864 mustrd-0.1.8/mustrd/model/mustrdTestOntology.ttl
+-rw-r--r--   0        0        0      842 2024-04-15 14:03:22.329614 mustrd-0.1.8/mustrd/model/mustrdTestShapes.ttl
+-rw-r--r--   0        0        0    17303 2024-04-03 16:12:05.425128 mustrd-0.1.8/mustrd/model/ontology.ttl
+-rw-r--r--   0        0        0     1558 2024-03-28 15:41:42.381426 mustrd-0.1.8/mustrd/model/test-resources/resources.ttl
+-rw-r--r--   0        0        0     6199 2024-04-03 16:11:22.263000 mustrd-0.1.8/mustrd/model/triplestoreOntology.ttl
+-rw-r--r--   0        0        0     1876 2024-04-16 14:08:01.101076 mustrd-0.1.8/mustrd/model/triplestoreshapes.ttl
+-rw-r--r--   0        0        0    35099 2024-04-17 14:58:51.079865 mustrd-0.1.8/mustrd/mustrd.py
+-rw-r--r--   0        0        0    11822 2024-03-28 15:41:42.398480 mustrd-0.1.8/mustrd/mustrdAnzo.py
+-rw-r--r--   0        0        0     5599 2024-03-28 15:41:42.399480 mustrd-0.1.8/mustrd/mustrdGraphDb.py
+-rw-r--r--   0        0        0     2129 2024-03-28 15:41:42.400481 mustrd-0.1.8/mustrd/mustrdRdfLib.py
+-rw-r--r--   0        0        0    15035 2024-04-18 08:48:16.471480 mustrd-0.1.8/mustrd/mustrdTestPlugin.py
+-rw-r--r--   0        0        0     3765 2024-04-17 13:27:21.126688 mustrd-0.1.8/mustrd/namespace.py
+-rw-r--r--   0        0        0    11995 2024-04-03 09:39:22.688671 mustrd-0.1.8/mustrd/README.adoc
+-rw-r--r--   0        0        0     4380 2024-04-17 12:56:01.295904 mustrd-0.1.8/mustrd/run.py
+-rw-r--r--   0        0        0    32546 2024-04-17 13:39:30.911945 mustrd-0.1.8/mustrd/spec_component.py
+-rw-r--r--   0        0        0     7555 2024-04-17 13:40:53.882724 mustrd-0.1.8/mustrd/steprunner.py
+-rw-r--r--   0        0        0      526 2024-03-28 15:41:42.440938 mustrd-0.1.8/mustrd/templates/md_ResultList_leaf_template.jinja
+-rw-r--r--   0        0        0      211 2024-03-28 15:41:42.445469 mustrd-0.1.8/mustrd/templates/md_ResultList_template.jinja
+-rw-r--r--   0        0        0      157 2024-03-28 15:41:42.450987 mustrd-0.1.8/mustrd/templates/md_stats_template.jinja
+-rw-r--r--   0        0        0      129 2024-04-12 16:21:29.119938 mustrd-0.1.8/mustrd/test/test_mustrd.py
+-rw-r--r--   0        0        0     4986 2024-03-28 15:41:42.458004 mustrd-0.1.8/mustrd/TestResult.py
+-rw-r--r--   0        0        0     1424 2024-03-28 15:41:42.462005 mustrd-0.1.8/mustrd/utils.py
+-rw-r--r--   0        0        0     1493 2024-04-18 09:37:19.554639 mustrd-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2724 2024-02-26 13:34:46.565338 mustrd-0.1.8/README.adoc
+-rw-r--r--   0        0        0     4130 1970-01-01 00:00:00.000000 mustrd-0.1.8/PKG-INFO
```

### Comparing `mustrd-0.1.7/LICENSE` & `mustrd-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.7/mustrd/logger_setup.py` & `mustrd-0.1.8/mustrd/logger_setup.py`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.7/mustrd/model/mustrdShapes.ttl` & `mustrd-0.1.8/mustrd/model/mustrdShapes.ttl`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.7/mustrd/model/ontology.ttl` & `mustrd-0.1.8/mustrd/model/ontology.ttl`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 @prefix foaf: <http://xmlns.com/foaf/spec/> .
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix skos: <http://www.w3.org/2004/02/skos/core#> .
 @base <https://mustrd.com/model/> .
 
 <https://mustrd.com/model> rdf:type owl:Ontology ;
-                            owl:imports rdf: ,
+                            owl:imports <https://mustrd.com/triplestore/> ,
+                                        rdf: ,
                                         rdfs: ;
                             rdfs:comment "" ;
                             rdfs:label "Mustrd" .
 
 #################################################################
 #    Object Properties
 #################################################################
```

### Comparing `mustrd-0.1.7/mustrd/model/test-resources/resources.ttl` & `mustrd-0.1.8/mustrd/model/test-resources/resources.ttl`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.7/mustrd/mustrd.py` & `mustrd-0.1.8/mustrd/mustrd.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,21 +36,21 @@
 from requests import ConnectionError, ConnectTimeout, HTTPError, RequestException
 
 from rdflib import Graph, URIRef, RDF, XSD, SH, Literal
 
 from rdflib.compare import isomorphic, graph_diff
 import pandas
 
-from .namespace import MUST
+from .namespace import MUST, TRIPLESTORE
 import requests
 import json
 from pandas import DataFrame
 
 from .spec_component import TableThenSpec, parse_spec_component, WhenSpec, ThenSpec
-from .utils import  is_json
+from .utils import  is_json,get_mustrd_root
 from colorama import Fore, Style
 from tabulate import tabulate
 from collections import defaultdict
 from pyshacl import validate
 import logging 
 from http.client import HTTPConnection
 from .steprunner import upload_given, run_when
@@ -89,14 +89,15 @@
 @dataclass
 class Specification:
     spec_uri: URIRef
     triple_store: dict
     given: Graph
     when: WhenSpec
     then: ThenSpec
+    spec_file_name: str = "default.mustrd.ttl"
 
 
 @dataclass
 class GraphComparison:
     in_expected_not_in_actual: Graph
     in_actual_not_in_expected: Graph
     in_both: Graph
@@ -148,14 +149,15 @@
 class TripleStoreConnectionError(SpecResult):
     exception: ConnectionError
 
 
 @dataclass
 class SpecSkipped(SpecResult):
     message: str
+    spec_file_name: str = "default.mustrd.ttl"
 
 
 @dataclass
 class SparqlAction:
     query: str
 
 
@@ -172,24 +174,23 @@
 @dataclass
 class UpdateSparqlQuery(SparqlAction):
     pass
 
 
 # https://github.com/Semantic-partners/mustrd/issues/19
 
-def validate_specs(run_config: dict, triple_stores: List, shacl_graph: Graph, ont_graph: Graph)\
+def validate_specs(run_config: dict, triple_stores: List, shacl_graph: Graph, ont_graph: Graph, file_name: str = "*")\
         -> Tuple[List, Graph, List]:
     spec_graph = Graph()
     subject_uris = set()
     focus_uris = set()
     invalid_specs = []
-  #  ttl_files = list(spec_path.glob('**/*.mustrd.ttl'))
-    ttl_files = list(run_config['spec_path'].glob('**/*.mustrd.ttl'))
+    ttl_files = list(run_config['spec_path'].glob(f'**/{file_name}.mustrd.ttl'))
     ttl_files.sort()
-    log.info(f"Found {len(ttl_files)} mustrd.ttl files in {run_config['spec_path']}")
+    log.info(f"Found {len(ttl_files)} {file_name}.mustrd.ttl files in {run_config['spec_path']}")
 
     for file in ttl_files:
         error_messages = []
 
         log.info(f"Parse: {file}")
         try:
             file_graph = Graph().parse(file)
@@ -229,29 +230,28 @@
             if subject_uri in subject_uris:
                 log.warning(f"Duplicate subject URI found: {file.name} {subject_uri}. File will not be parsed.")
                 error_messages += [f"Duplicate subject URI found in {file.name}."]
                 subject_uri = URIRef(str(subject_uri) + "_DUPLICATE")
             if len(error_messages) > 0:
                 error_messages.sort()
                 error_message = "\n".join(msg for msg in error_messages)
-                invalid_specs += [SpecSkipped(subject_uri, triple_store["type"], error_message) for triple_store in
+                invalid_specs += [SpecSkipped(subject_uri, triple_store["type"], error_message, file.name) for triple_store in
                                 triple_stores]
             else:
                 subject_uris.add(subject_uri)
                 this_spec_graph = Graph()
                 this_spec_graph.parse(file)
                 spec_uris_in_this_file = list(this_spec_graph.subjects(RDF.type, MUST.TestSpec))
                 for spec in spec_uris_in_this_file:
-                    tripleToAdd = [spec, MUST.specSourceFile, Literal(file)]
                     # print(f"adding {tripleToAdd}")
-                    this_spec_graph.add(tripleToAdd)
+                    this_spec_graph.add([spec, MUST.specSourceFile, Literal(file)])
+                    this_spec_graph.add([spec, MUST.specFileName, Literal(file.name)])
                 # print(f"beforeadd: {spec_graph}" )
                 # print(f"beforeadd: {str(this_spec_graph.serialize())}" )
                 spec_graph += this_spec_graph
-                # print(f"afteradd: {str(spec_graph.serialize())}" )
 
 
     sourceFiles = list(spec_graph.subject_objects(MUST.specSourceFile))
     # print(f"sourceFiles: {sourceFiles}")
 
     valid_spec_uris = list(spec_graph.subjects(RDF.type, MUST.TestSpec))
 
@@ -272,22 +272,22 @@
               run_config: dict):
     specs = []
     skipped_results = []
     try:
         for triple_store in triple_stores:
             if "error" in triple_store:
                 log.error(f"{triple_store['error']}. No specs run for this triple store.")
-                skipped_results += [SpecSkipped(spec_uri, triple_store['type'], triple_store['error']) for spec_uri in
+                skipped_results += [SpecSkipped(spec_uri, triple_store['type'], triple_store['error'], get_spec_file(spec_uri, spec_graph)) for spec_uri in
                                     spec_uris]
             else:
                 for spec_uri in spec_uris:
                     try:
                         specs += [get_spec(spec_uri, spec_graph, run_config, triple_store)]
                     except (ValueError, FileNotFoundError, ConnectionError) as e:
-                        skipped_results += [SpecSkipped(spec_uri, triple_store['type'], e)]
+                        skipped_results += [SpecSkipped(spec_uri, triple_store['type'], e, get_spec_file(spec_uri, spec_graph))]
 
     except (BadSyntax, FileNotFoundError) as e:
         template = "An exception of type {0} occurred when trying to parse the triple store configuration file. " \
                    "Arguments:\n{1!r}"
         message = template.format(type(e).__name__, e.args)
         log.error(message)
         log.error("No specifications will be run.")
@@ -299,30 +299,33 @@
 def run_specs(specs) -> List[SpecResult]:
     results = []
     # https://github.com/Semantic-partners/mustrd/issues/115
     for specification in specs:
         results.append(run_spec(specification))
     return results
 
+def get_spec_file(spec_uri: URIRef, spec_graph: Graph):
+    test =  str(spec_graph.value(subject = spec_uri, predicate = MUST.specFileName, default = "default.mustrd.ttl"))
+    return test
 
 def get_spec(spec_uri: URIRef, spec_graph: Graph, run_config: dict, mustrd_triple_store: dict = None) -> Specification:
     try:
         if mustrd_triple_store is None:
-            mustrd_triple_store = {"type": MUST.RdfLib}
+            mustrd_triple_store = {"type": TRIPLESTORE.RdfLib}
         components = []
         for predicate in MUST.given, MUST.when, MUST.then:
             components.append(parse_spec_component(subject=spec_uri,
                                                 predicate=predicate,
                                                 spec_graph=spec_graph,
                                                 run_config=run_config,
                                                 mustrd_triple_store=mustrd_triple_store))
 
-
+        spec_file_name = get_spec_file(spec_uri, spec_graph)
         # https://github.com/Semantic-partners/mustrd/issues/92
-        return Specification(spec_uri, mustrd_triple_store, components[0].value, components[1], components[2])
+        return Specification(spec_uri, mustrd_triple_store, components[0].value, components[1], components[2], spec_file_name)
     
     except (ValueError, FileNotFoundError) as e:
         template = "An exception of type {0} occurred. Arguments:\n{1!r}"
         message = template.format(type(e).__name__, e.args)
         log.exception(message)
         raise
     except ConnectionError as e:
@@ -350,15 +353,15 @@
     # close_connection = True
     log.debug(f"run_when {spec_uri=}, {triple_store=}, {spec.given=}, {spec.when=}, {spec.then=}")
     if spec.given:
         given_as_turtle = spec.given.serialize(format="turtle")
         log.debug(f"{given_as_turtle}")
         upload_given(triple_store, spec.given)
     else:
-        if triple_store['type'] == MUST.RdfLib:
+        if triple_store['type'] == TRIPLESTORE.RdfLib:
             return SpecSkipped(spec_uri, triple_store['type'], "Unable to run Inherited State tests on Rdflib")
     try:
         for when in spec.when:
             log.info(f"Running {when.queryType} spec {spec_uri} on {triple_store['type']}")
             try:
                 result = run_when(spec_uri, triple_store, when)
             except ParseException as e:
@@ -382,65 +385,72 @@
     #         mustrd_triple_store.clear_graph()
 
 def get_triple_store_graph(triple_store_graph_path: Path, secrets: str):
     if secrets:
         return Graph().parse(triple_store_graph_path).parse(data = secrets)
     else:
         secret_path = triple_store_graph_path.parent / Path(triple_store_graph_path.stem + "_secrets" + triple_store_graph_path.suffix)
-        return Graph().parse(triple_store_graph_path).parse(source = secret_path)
+        return Graph().parse(triple_store_graph_path).parse(secret_path)
     
 
 def get_triple_stores(triple_store_graph: Graph) -> list[dict]:
     triple_stores = []
+    shacl_graph = Graph().parse(Path(os.path.join(get_mustrd_root(), "model/triplestoreshapes.ttl")))
+    ont_graph = Graph().parse(Path(os.path.join(get_mustrd_root(), "model/triplestoreOntology.ttl")))
+    conforms, results_graph, results_text = validate(
+            data_graph= triple_store_graph,
+            shacl_graph = shacl_graph,
+            ont_graph  = ont_graph,
+            advanced= True,
+            inference= 'none'
+        )
+    if not conforms:
+        raise ValueError(f"Triple store configuration not conform to the shapes. SHACL report: {results_text}", results_graph)
     for triple_store_config, rdf_type, triple_store_type in triple_store_graph.triples((None, RDF.type, None)):
         triple_store = {}
-        # Local rdf lib triple store
-        if triple_store_type == MUST.RdfLibConfig:
-            triple_store["type"] = MUST.RdfLib
+        triple_store["type"] = triple_store_type
+        triple_store["uri"] = triple_store_config
         # Anzo graph via anzo
-        elif triple_store_type == MUST.AnzoConfig:
-            triple_store["type"] = MUST.Anzo
-            triple_store["url"] = triple_store_graph.value(subject=triple_store_config, predicate=MUST.url)
-            triple_store["port"] = triple_store_graph.value(subject=triple_store_config, predicate=MUST.port)
+        if triple_store_type == TRIPLESTORE.Anzo:
+            triple_store["url"] = triple_store_graph.value(subject=triple_store_config, predicate=TRIPLESTORE.url)
+            triple_store["port"] = triple_store_graph.value(subject=triple_store_config, predicate=TRIPLESTORE.port)
             try:
-                triple_store["username"] = str(triple_store_graph.value(subject=triple_store_config, predicate=MUST.username))
-                triple_store["password"] = str(triple_store_graph.value(subject=triple_store_config, predicate=MUST.password))
+                triple_store["username"] = str(triple_store_graph.value(subject=triple_store_config, predicate=TRIPLESTORE.username))
+                triple_store["password"] = str(triple_store_graph.value(subject=triple_store_config, predicate=TRIPLESTORE.password))
             except (FileNotFoundError, ValueError) as e:
                 triple_store["error"] = e
-            triple_store["gqe_uri"] = triple_store_graph.value(subject=triple_store_config, predicate=MUST.gqeURI)
+            triple_store["gqe_uri"] = triple_store_graph.value(subject=triple_store_config, predicate=TRIPLESTORE.gqeURI)
             triple_store["input_graph"] = triple_store_graph.value(subject=triple_store_config,
-                                                                   predicate=MUST.inputGraph)
+                                                                   predicate=TRIPLESTORE.inputGraph)
             triple_store["output_graph"] = triple_store_graph.value(subject=triple_store_config,
-                                                                   predicate=MUST.outputGraph)
+                                                                   predicate=TRIPLESTORE.outputGraph)
             try:
                 check_triple_store_params(triple_store, ["url", "port", "username", "password", "input_graph"])
             except ValueError as e:
                 triple_store["error"] = e
         # GraphDB
-        elif triple_store_type == MUST.GraphDbConfig:
-            triple_store["type"] = MUST.GraphDb
-            triple_store["url"] = triple_store_graph.value(subject=triple_store_config, predicate=MUST.url)
-            triple_store["port"] = triple_store_graph.value(subject=triple_store_config, predicate=MUST.port)
+        elif triple_store_type == TRIPLESTORE.GraphDb:
+            triple_store["url"] = triple_store_graph.value(subject=triple_store_config, predicate=TRIPLESTORE.url)
+            triple_store["port"] = triple_store_graph.value(subject=triple_store_config, predicate=TRIPLESTORE.port)
             try:
-                triple_store["username"] = str(triple_store_graph.value(subject=triple_store_config, predicate=MUST.username))
-                triple_store["password"] = str(triple_store_graph.value(subject=triple_store_config, predicate=MUST.password))
+                triple_store["username"] = str(triple_store_graph.value(subject=triple_store_config, predicate=TRIPLESTORE.username))
+                triple_store["password"] = str(triple_store_graph.value(subject=triple_store_config, predicate=TRIPLESTORE.password))
             except (FileNotFoundError, ValueError) as e:
                 log.error(f"Credential retrieval failed {e}")
                 triple_store["error"] = e
             triple_store["repository"] = triple_store_graph.value(subject=triple_store_config,
-                                                                  predicate=MUST.repository)
+                                                                  predicate=TRIPLESTORE.repository)
             triple_store["input_graph"] = triple_store_graph.value(subject=triple_store_config,
-                                                                   predicate=MUST.inputGraph)
+                                                                   predicate=TRIPLESTORE.inputGraph)
 
             try:
                 check_triple_store_params(triple_store, ["url", "port", "repository"])
             except ValueError as e:
                 triple_store["error"] = e
-        else:
-            triple_store["type"] = triple_store_type
+        elif triple_store_type != TRIPLESTORE.RdfLib:
             triple_store["error"] = f"Triple store not implemented: {triple_store_type}"
 
         triple_stores.append(triple_store)
     return triple_stores
 
 
 def check_triple_store_params(triple_store: dict, required_params: List[str]):
```

### Comparing `mustrd-0.1.7/mustrd/mustrdAnzo.py` & `mustrd-0.1.8/mustrd/mustrdAnzo.py`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.7/mustrd/mustrdGraphDb.py` & `mustrd-0.1.8/mustrd/mustrdGraphDb.py`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.7/mustrd/mustrdRdfLib.py` & `mustrd-0.1.8/mustrd/mustrdRdfLib.py`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.7/mustrd/mustrdTestPlugin.py` & `mustrd-0.1.8/mustrd/mustrdTestPlugin.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,146 +25,213 @@
 from dataclasses import dataclass
 import pytest
 import os
 from pathlib import Path
 from rdflib.namespace import Namespace
 from rdflib import Graph, RDF
 from pytest import Session
-from typing import Dict
 
 from mustrd.TestResult import ResultList, TestResult, get_result_list
 from mustrd.utils import get_mustrd_root
 from mustrd.mustrd import get_triple_store_graph, get_triple_stores
-from mustrd.mustrd import SpecSkipped, validate_specs, get_specs, SpecPassed, run_spec
-from mustrd.namespace import MUST
-from collections import defaultdict
+from mustrd.mustrd import Specification, SpecSkipped, validate_specs, get_specs, SpecPassed, run_spec
+from mustrd.namespace import MUST, TRIPLESTORE, MUSTRDTEST
+from typing import Union
+from pyshacl import validate
 
 spnamespace = Namespace("https://semanticpartners.com/data/test/")
 
 mustrd_root = get_mustrd_root()
 
+MUSTRD_PYTEST_PATH = "mustrd_tests/"
+
 
 def pytest_addoption(parser):
-    group = parser.getgroup("md summary")
+    group = parser.getgroup("mustrd option")
+    group.addoption(
+        "--mustrd",
+        action="store_true",
+        dest="mustrd",
+        help="Activate/deactivate mustrd test generation.",
+    )
     group.addoption(
         "--md",
         action="store",
         dest="mdpath",
         metavar="pathToMdSummary",
         default=None,
         help="create md summary file at that path.",
     )
     group.addoption(
         "--config",
         action="store",
         dest="configpath",
         metavar="pathToTestConfig",
         default=None,
-        required=True,
         help="Ttl file containing the list of test to construct.",
     )
     group.addoption(
         "--secrets",
         action="store",
         dest="secrets",
         metavar="Secrets",
         default=None,
-        required=False,
         help="Give the secrets by command line in order to be able to store secrets safely in CI tools",
     )
     return
 
 
 def pytest_configure(config) -> None:
     # Read configuration file
-    test_configs: Dict[str, TestConfig] = defaultdict(lambda: defaultdict(list))
-    config_graph = Graph().parse(config.getoption("configpath"))
-    for test_config_subject in config_graph.subjects(predicate=RDF.type, object=MUST.TestConfig):
-        test_function = get_config_param(config_graph, test_config_subject, MUST.hasTestFunction, str)
-        spec_path = get_config_param(config_graph, test_config_subject, MUST.hasSpecPath, str)
-        data_path = get_config_param(config_graph, test_config_subject, MUST.hasDataPath, str)
-        triplestore_spec_path = get_config_param(config_graph, test_config_subject, MUST.triplestoreSpecPath, str)
+    if config.getoption("mustrd"):
+        test_configs = parse_config(config.getoption("configpath"))
+        config.pluginmanager.register(MustrdTestPlugin(config.getoption("mdpath"),
+                                                    test_configs, config.getoption("secrets")))
+    
+def parse_config(config_path):
+    test_configs = []
+    config_graph = Graph().parse(config_path)
+    shacl_graph = Graph().parse(Path(os.path.join(mustrd_root, "model/mustrdTestShapes.ttl")))
+    ont_graph = Graph().parse(Path(os.path.join(mustrd_root, "model/mustrdTestOntology.ttl")))
+    conforms, results_graph, results_text = validate(
+            data_graph= config_graph,
+            shacl_graph = shacl_graph,
+            ont_graph  = ont_graph,
+            advanced= True,
+            inference= 'none'
+        )
+    if not conforms:
+        raise ValueError(f"Mustrd test configuration not conform to the shapes. SHACL report: {results_text}", results_graph)
+        
+    for test_config_subject in config_graph.subjects(predicate=RDF.type, object=MUSTRDTEST.MustrdTest):
+        spec_path = get_config_param(config_graph, test_config_subject, MUSTRDTEST.hasSpecPath, str)
+        data_path = get_config_param(config_graph, test_config_subject, MUSTRDTEST.hasDataPath, str)
+        triplestore_spec_path = get_config_param(config_graph, test_config_subject, MUSTRDTEST.triplestoreSpecPath, str)
+        pytest_path = get_config_param(config_graph, test_config_subject, MUSTRDTEST.hasPytestPath, str)
         filter_on_tripleStore = list(config_graph.objects(subject=test_config_subject,
-                                                          predicate=MUST.filterOnTripleStore))
+                                                        predicate=MUSTRDTEST.filterOnTripleStore))
 
-        test_configs[test_function] = TestConfig(test_function=test_function,
-                                                 spec_path=spec_path, data_path=data_path,
-                                                 triplestore_spec_path=triplestore_spec_path,
-                                                 filter_on_tripleStore=filter_on_tripleStore)
-
-    config.pluginmanager.register(MustrdTestPlugin(config.getoption("mdpath"),
-                                                   test_configs, config.getoption("secrets")))
+        test_configs.append(TestConfig(spec_path=spec_path, data_path=data_path,
+                                                triplestore_spec_path=triplestore_spec_path,
+                                                pytest_path = pytest_path,
+                                                filter_on_tripleStore=filter_on_tripleStore))
+    return test_configs
+    
 
 
 def get_config_param(config_graph, config_subject, config_param, convert_function):
     raw_value = config_graph.value(subject=config_subject, predicate=config_param, any=True)
     return convert_function(raw_value) if raw_value else None
 
 
 @dataclass
 class TestConfig:
-    test_function: str
     spec_path: str
     data_path: str
     triplestore_spec_path: str
-    filter_on_tripleStore: str
-
-    def __init__(self, test_function: str, spec_path: str, data_path: str, triplestore_spec_path: str,
-                 filter_on_tripleStore: str = None):
-        self.test_function = test_function
-        self.spec_path = spec_path
-        self.data_path = data_path
-        self.triplestore_spec_path = triplestore_spec_path
-        self.filter_on_tripleStore = filter_on_tripleStore
+    pytest_path: str
+    filter_on_tripleStore: str = None
+        
 
+@dataclass
+class TestParamWrapper:
+    test_config: TestConfig
+    unit_test: Union[Specification, SpecSkipped]
 
 class MustrdTestPlugin:
     md_path: str
-    test_configs: Dict[str, TestConfig]
+    test_configs: list
     secrets: str
+    unit_tests: Union[Specification, SpecSkipped]
+    items: list
 
     def __init__(self, md_path, test_configs, secrets):
         self.md_path = md_path
         self.test_configs = test_configs
         self.secrets = secrets
+        self.items = []
+    
+    @pytest.hookimpl(tryfirst=True)
+    def pytest_collection(self, session):
+        self.unit_tests = []
+        args = session.config.args
+        if len(args) > 0:
+            file_name = self.get_file_name_from_arg(args[0])
+            # Filter test to collect only specified path
+            config_to_collect = list(filter(lambda config: 
+                                            # Case we want to collect everything
+                                            MUSTRD_PYTEST_PATH not in args[0]
+                                            # Case we want to collect a test or sub test
+                                            or (config.pytest_path or "") in args[0]
+                                            # Case we want to collect a whole test folder
+                                            or args[0].replace(f"./{MUSTRD_PYTEST_PATH}", "") in config.pytest_path,
+                                            self.test_configs))
+                
+            # Redirect everything to test_mustrd.py, no need to filter on specified test: Only specified test will be collected anyway
+            session.config.args[0] = os.path.join(mustrd_root, "test/test_mustrd.py")
+        # Collecting only relevant tests
+        
+        for one_test_config in config_to_collect: 
+            triple_stores = self.get_triple_stores_from_file(one_test_config)
+
+            if one_test_config.filter_on_tripleStore and not triple_stores:
+                self.unit_tests.extend(list(map(lambda triple_store:
+                                TestParamWrapper(test_config = one_test_config, unit_test=SpecSkipped(MUST.TestSpec, triple_store, "No triplestore found")),
+                                one_test_config.filter_on_tripleStore)))
+            else:
+                specs = self.generate_tests_for_config({"spec_path": Path(one_test_config.spec_path),
+                                                            "data_path": Path(one_test_config.data_path)},
+                                                            triple_stores, file_name)
+                self.unit_tests.extend(list(map(lambda spec: TestParamWrapper(test_config = one_test_config, unit_test=spec),specs)))
+        
+    def get_file_name_from_arg(self, arg):
+        if arg and len(arg) > 0 and "[" in arg and ".mustrd.ttl@" in arg:
+            return arg[arg.index("[") + 1: arg.index(".mustrd.ttl@")]
+        return None
+        
+        
+    @pytest.hookimpl(hookwrapper=True)
+    def pytest_pycollect_makeitem(self, collector, name, obj):
+        report = yield
+        if name == "test_unit":
+            items = report.get_result()
+            new_results = []
+            for item in items:
+                virtual_path =  MUSTRD_PYTEST_PATH + (item.callspec.params["unit_tests"].test_config.pytest_path or "default")
+                item.fspath = Path(virtual_path)
+                item._nodeid = virtual_path + "::" + item.name
+                self.items.append(item)
+                new_results.append(item)
+            return new_results
+        
 
     # Hook called at collection time: reads the configuration of the tests, and generate pytests from it
     def pytest_generate_tests(self, metafunc):
-
         if len(metafunc.fixturenames) > 0:
-            if metafunc.function.__name__ in self.test_configs:
-                one_test_config = self.test_configs[metafunc.function.__name__]
-
-                triple_stores = self.get_triple_stores_from_file(one_test_config)
-
-                unit_tests = []
-                if one_test_config.filter_on_tripleStore and not triple_stores:
-                    unit_tests = list(map(lambda triple_store:
-                                      SpecSkipped(MUST.TestSpec, triple_store, "No triplestore found"),
-                                      one_test_config.filter_on_tripleStore))
-                else:
-                    unit_tests = self.generate_tests_for_config({"spec_path": Path(one_test_config.spec_path),
-                                                                "data_path": Path(one_test_config.data_path)},
-                                                                triple_stores)
-
+            if metafunc.function.__name__  == "test_unit":
                 # Create the test in itself
-                if unit_tests:
-                    metafunc.parametrize(metafunc.fixturenames[0], unit_tests, ids=self.get_test_name)
+                if self.unit_tests:
+                    metafunc.parametrize(metafunc.fixturenames[0], self.unit_tests,
+                                         ids=lambda test_param: (test_param.unit_test.spec_file_name or "") + "@" +
+                                         (test_param.test_config.pytest_path or ""))
             else:
                 metafunc.parametrize(metafunc.fixturenames[0],
                                      [SpecSkipped(MUST.TestSpec, None, "No triplestore found")],
                                      ids=lambda x: "No configuration found for this test")
+    
+                
+            
 
     # Generate test for each triple store available
-    def generate_tests_for_config(self, config, triple_stores):
+    def generate_tests_for_config(self, config, triple_stores, file_name):
 
         shacl_graph = Graph().parse(Path(os.path.join(mustrd_root, "model/mustrdShapes.ttl")))
         ont_graph = Graph().parse(Path(os.path.join(mustrd_root, "model/ontology.ttl")))
         valid_spec_uris, spec_graph, invalid_spec_results = validate_specs(config, triple_stores,
-                                                                           shacl_graph, ont_graph)
+                                                                           shacl_graph, ont_graph, file_name or "*")
 
         specs, skipped_spec_results = \
             get_specs(valid_spec_uris, spec_graph, triple_stores, config)
 
         # Return normal specs + skipped results
         return specs + skipped_spec_results + invalid_spec_results
 
@@ -182,23 +249,23 @@
     # Get triple store configuration or default
     def get_triple_stores_from_file(self, test_config):
         if test_config.triplestore_spec_path:
             try:
                 triple_stores = get_triple_stores(get_triple_store_graph(Path(test_config.triplestore_spec_path),
                                                                          self.secrets))
             except Exception as e:
-                print(f"""No triple store configuration found at {test_config.triplestore_spec_path}.
-                    Fall back: only embedded rdflib will be executed""", e)
-                triple_stores = [{'type': MUST.RdfLib}]
+                print(f"""Triplestore configuration parsing failed {test_config.triplestore_spec_path}.
+                    Only rdflib will be executed""", e)
+                triple_stores = [{'type': TRIPLESTORE.RdfLib, 'uri': TRIPLESTORE.RdfLib}]
         else:
             print("No triple store configuration required: using embedded rdflib")
-            triple_stores = [{'type': MUST.RdfLib}]
+            triple_stores = [{'type': TRIPLESTORE.RdfLib, 'uri': TRIPLESTORE.RdfLib}]
 
         if test_config.filter_on_tripleStore:
-            triple_stores = list(filter(lambda triple_store: (triple_store["type"] in test_config.filter_on_tripleStore),
+            triple_stores = list(filter(lambda triple_store: (triple_store["uri"] in test_config.filter_on_tripleStore),
                                         triple_stores))
         return triple_stores
 
     # Hook function. Initialize the list of result in session
     def pytest_sessionstart(self, session):
         session.results = dict()
```

### Comparing `mustrd-0.1.7/mustrd/namespace.py` & `mustrd-0.1.8/mustrd/namespace.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,41 +21,31 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from rdflib import URIRef
 from rdflib.namespace import DefinedNamespace, Namespace
 
-
+# Namespace for the test specifications
 class MUST(DefinedNamespace):
     _NS = Namespace("https://mustrd.com/model/")
-
-    # test configuration
-    TestConfig: URIRef
-    hasTestFunction: URIRef
-    hasSpecPath: URIRef
-    hasDataPath: URIRef
-    triplestoreSpecPath: URIRef
-    filterOnTripleStore: URIRef
-
+    
     # Specification classes
     TestSpec: URIRef
     SelectSparql: URIRef
     ConstructSparql: URIRef
     UpdateSparql: URIRef
     AnzoQueryDrivenUpdateSparql: URIRef
     AskSparql: URIRef
     DescribeSparql: URIRef
 
     # Specification properties
     given: URIRef
     when: URIRef
     then: URIRef
-    inputGraph: URIRef 
-    outputGraph: URIRef # anzo specials? 
     dataSource: URIRef
     file: URIRef
     fileName: URIRef
     queryFolder: URIRef
     queryName: URIRef
     dataSourceUrl: URIRef
     queryText: URIRef
@@ -80,39 +70,56 @@
     EmptyTable: URIRef
     InheritedDataset: URIRef
 
     # runner uris
     fileSource: URIRef
     loadedFromFile: URIRef
     specSourceFile: URIRef
+    specFileName: URIRef
 
     # Triple store config parameters
-    url: URIRef
-    port: URIRef
-    username: URIRef
-    password: URIRef
-    inputGraph: URIRef
-    repository: URIRef
-
-    # RDFLib
-    RdfLib: URIRef
-    RdfLibConfig: URIRef
-
     # Anzo
-    Anzo: URIRef
-    AnzoConfig: URIRef
     AnzoGraphmartDataset: URIRef
     AnzoQueryBuilderSparqlSource: URIRef
     AnzoGraphmartStepSparqlSource: URIRef
     AnzoGraphmartLayerSparqlSource: URIRef
     AnzoGraphmartQueryDrivenTemplatedStepSparqlSource: URIRef
     anzoQueryStep: URIRef
     anzoGraphmartLayer: URIRef
-
     
     graphmart: URIRef
     layer: URIRef
-    gqeURI: URIRef
 
-    # GraphDb
+    
+    # FIXME: There is nothing to do that by default?
+    @classmethod
+    def get_local_name(cls, uri: URIRef):
+        return str(uri).split(cls._NS)[1]
+
+# Namespace for triplestores
+class TRIPLESTORE(DefinedNamespace):
+    _NS = Namespace("https://mustrd.com/triplestore/")
+    RdfLib: URIRef
     GraphDb: URIRef
-    GraphDbConfig: URIRef
+    Anzo: URIRef
+    ExternalTripleStore: URIRef
+    InternalTripleStore: URIRef
+    
+    gqeURI: URIRef
+    inputGraph: URIRef 
+    outputGraph: URIRef # anzo specials?     # Triple store config parameters
+    url: URIRef
+    port: URIRef
+    username: URIRef
+    password: URIRef
+    repository: URIRef
+
+# namespace for pytest_mustrd config
+class MUSTRDTEST(DefinedNamespace):
+    _NS = Namespace("https://mustrd.com/mustrdTest/")
+    MustrdTest: URIRef
+    hasSpecPath: URIRef
+    hasDataPath: URIRef
+    triplestoreSpecPath: URIRef
+    hasPytestPath: URIRef
+    filterOnTripleStore: URIRef
+
```

### Comparing `mustrd-0.1.7/mustrd/README.adoc` & `mustrd-0.1.8/mustrd/README.adoc`

 * *Files 2% similar despite different names*

```diff
@@ -174,24 +174,24 @@
 
 The configuration file should be serialised RDF. An example in Turtle format is included below for GraphDB. For Anzo the *must:repository* value is replaced with a *must:gqeURI*.
 ----
 @prefix must:      <https://mustrd.com/model/> .
 must:GraphDbConfig1  a must:GraphDbConfig ;
         must:url "http://localhost";
         must:port "7200";
-        must:username "test/triplestore_config/tripleStoreCredentials.toml" ;
-        must:password "test/triplestore_config/tripleStoreCredentials.toml" ;
         must:inputGraph "http://localhost:7200/test-graph" ;
         must:repository "mustrd" .
 ----
-The triplestore credentials are held in a separate TOML file so that configurations can be shared without sharing credentials.
+To avoid versioning secrets when you want to version triplestore configuration (for example in case you want to run mustrd in CI), you have to configure user/password in a different file.
+This file must be named as the triple store configuration file, but with "_secrets" just before the extension. For example triplestores.ttl -> triplestores_secrets.ttl
+Subjects in the two files must match, no need to redefine the type, for example:
 ----
-["https://mustrd.com/model/GraphDbConfig1"]
-"username"="<username>"
-"password"="<password>"
+@prefix must:      <https://mustrd.com/model/> .
+must:GraphDbConfig1  must:username 'test' ;
+              must:password 'test' .
 ----
 
 == Additional Notes for Developers
 Mustrd remains very much under development. It is anticipated that additional functionality and triplestore support will be added over time. The project uses https://python-poetry.org/docs/[Poetry] to manage dependencies so it will be necessary to have this installed to contribute towards the project. The link contains instructions on how to install and use this.
 As the project is actually built from the requirements.txt file at the project root, it is necessary to export dependencies from poetry to this file before committing and pushing changes to the repository, using the following command.
 
 `poetry export -f requirements.txt --without-hashes > requirements.txt`
```

### Comparing `mustrd-0.1.7/mustrd/run.py` & `mustrd-0.1.8/mustrd/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import argparse
 import logger_setup
 import sys
 import os
 from rdflib import Graph
 from .mustrd import get_triple_store_graph, run_specs, get_triple_stores, review_results, validate_specs, get_specs
 from pathlib import Path
-from .namespace import MUST
+from .namespace import TRIPLESTORE
 from .utils import get_project_root
 import logging 
 log = logger_setup.setup_logger(__name__)
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser()
@@ -64,15 +64,15 @@
 
     if args.config:
         triplestore_spec_path = Path(args.config)
         log.info(f"Path for triple store configuration is {triplestore_spec_path}")
         triple_stores = get_triple_stores(get_triple_store_graph(triplestore_spec_path))
     else:
         log.info(f"No triple store configuration added, running default configuration")
-        triple_stores = [{'type': MUST.RdfLib}]
+        triple_stores = [{'type': TRIPLESTORE.RdfLib}]
     log.info("Triple Stores: " + str(triple_stores))
     if args.data:
         run_config["data_path"] = Path(args.data)
     else:
         run_config["data_path"] = Path(args.put)
     log.info(f"Path for test data folder is {run_config['data_path']}")
```

### Comparing `mustrd-0.1.7/mustrd/spec_component.py` & `mustrd-0.1.8/mustrd/spec_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from rdflib import RDF, Graph, URIRef, Variable, Literal, XSD, util
 from rdflib.exceptions import ParserError
 from rdflib.term import Node
 import logging 
 
 from . import logger_setup
 from .mustrdAnzo import get_queries_for_layer, get_queries_from_templated_step, get_spec_component_from_graphmart, get_query_from_querybuilder, get_query_from_step
-from .namespace import MUST
+from .namespace import MUST, TRIPLESTORE
 from multimethods import MultiMethod, Default
 
 log = logger_setup.setup_logger(__name__)
 
 
 @dataclass
 class SpecComponent:
@@ -413,95 +413,95 @@
 
 
 @get_spec_component.method((MUST.AnzoGraphmartDataset, MUST.given))
 @get_spec_component.method((MUST.AnzoGraphmartDataset, MUST.then))
 def _get_spec_component_AnzoGraphmartDataset(spec_component_details: SpecComponentDetails) -> SpecComponent:
     spec_component = init_spec_component(spec_component_details.predicate)
 
-    if spec_component_details.mustrd_triple_store["type"] == MUST.Anzo:
+    if spec_component_details.mustrd_triple_store["type"] == TRIPLESTORE.Anzo:
         # Get GIVEN or THEN from anzo graphmart
         graphmart = spec_component_details.spec_graph.value(subject=spec_component_details.spec_component_node,
                                                             predicate=MUST.graphmart)
         layer = spec_component_details.spec_graph.value(subject=spec_component_details.spec_component_node,
                                                         predicate=MUST.layer)
         spec_component.value = get_spec_component_from_graphmart(
             triple_store=spec_component_details.mustrd_triple_store,
             graphmart=graphmart,
             layer=layer)
     else:
-        raise ValueError(f"You must define {MUST.AnzoConfig} to use {MUST.AnzoGraphmartDataset}")
+        raise ValueError(f"You must define {TRIPLESTORE.Anzo} to use {MUST.AnzoGraphmartDataset}")
 
     return spec_component
 
 
 @get_spec_component.method((MUST.AnzoQueryBuilderSparqlSource, MUST.when))
 def _get_spec_component_AnzoQueryBuilderSparqlSource(spec_component_details: SpecComponentDetails) -> SpecComponent:
     spec_component = init_spec_component(spec_component_details.predicate)
 
     # Get WHEN specComponent from query builder
-    if spec_component_details.mustrd_triple_store["type"] == MUST.Anzo:
+    if spec_component_details.mustrd_triple_store["type"] == TRIPLESTORE.Anzo:
         query_folder = spec_component_details.spec_graph.value(subject=spec_component_details.spec_component_node,
                                                                predicate=MUST.queryFolder)
         query_name = spec_component_details.spec_graph.value(subject=spec_component_details.spec_component_node,
                                                              predicate=MUST.queryName)
         spec_component.value = get_query_from_querybuilder(triple_store=spec_component_details.mustrd_triple_store,
                                                            folder_name=query_folder,
                                                            query_name=query_name)
     # If anzo specific function is called but no anzo defined
     else:
-        raise ValueError(f"You must define {MUST.AnzoConfig} to use {MUST.AnzoQueryBuilderSparqlSource}")
+        raise ValueError(f"You must define {TRIPLESTORE.Anzo} to use {MUST.AnzoQueryBuilderSparqlSource}")
 
     spec_component.queryType = spec_component_details.spec_graph.value(subject=spec_component_details.spec_component_node,
                                                                        predicate=MUST.queryType)
     return spec_component
 
 
 @get_spec_component.method((MUST.AnzoGraphmartStepSparqlSource, MUST.when))
 def _get_spec_component_AnzoGraphmartStepSparqlSource(spec_component_details: SpecComponentDetails) -> SpecComponent:
     spec_component = init_spec_component(spec_component_details.predicate)
 
     # Get WHEN specComponent from query builder
-    if spec_component_details.mustrd_triple_store["type"] == MUST.Anzo:
+    if spec_component_details.mustrd_triple_store["type"] == TRIPLESTORE.Anzo:
         query_step_uri = spec_component_details.spec_graph.value(subject=spec_component_details.spec_component_node,
                                                              predicate=MUST.anzoQueryStep)
         spec_component.value = get_query_from_step(triple_store=spec_component_details.mustrd_triple_store,
                                                     query_step_uri=query_step_uri)
     # If anzo specific function is called but no anzo defined
     else:
-        raise ValueError(f"You must define {MUST.AnzoConfig} to use {MUST.AnzoGraphmartStepSparqlSource}")
+        raise ValueError(f"You must define {TRIPLESTORE.Anzo} to use {MUST.AnzoGraphmartStepSparqlSource}")
 
     spec_component.queryType = spec_component_details.spec_graph.value(subject=spec_component_details.spec_component_node,
                                                                        predicate=MUST.queryType)
     return spec_component
 
 @get_spec_component.method((MUST.AnzoGraphmartQueryDrivenTemplatedStepSparqlSource, MUST.when))
 def _get_spec_component_AnzoGraphmartQueryDrivenTemplatedStepSparqlSource(spec_component_details: SpecComponentDetails) -> SpecComponent:
     spec_component = init_spec_component(spec_component_details.predicate, spec_component_details.mustrd_triple_store["type"] )
 
     # Get WHEN specComponent from query builder
-    if spec_component_details.mustrd_triple_store["type"] == MUST.Anzo:
+    if spec_component_details.mustrd_triple_store["type"] == TRIPLESTORE.Anzo:
         query_step_uri = spec_component_details.spec_graph.value(subject=spec_component_details.spec_component_node,
                                                              predicate=MUST.anzoQueryStep)
         queries = get_queries_from_templated_step(triple_store=spec_component_details.mustrd_triple_store,
                                                     query_step_uri=query_step_uri)
         spec_component.paramQuery= queries["param_query"]
         spec_component.queryTemplate = queries["query_template"]
     # If anzo specific function is called but no anzo defined
     else:
-        raise ValueError(f"You must define {MUST.AnzoConfig} to use {MUST.AnzoGraphmartQueryDrivenTemplatedStepSparqlSource}")
+        raise ValueError(f"You must define {TRIPLESTORE.Anzo} to use {MUST.AnzoGraphmartQueryDrivenTemplatedStepSparqlSource}")
 
     spec_component.queryType = spec_component_details.spec_graph.value(subject=spec_component_details.spec_component_node,
                                                                        predicate=MUST.queryType)
     return spec_component
 
 @get_spec_component.method((MUST.AnzoGraphmartLayerSparqlSource, MUST.when))
 def _get_spec_component_AnzoGraphmartLayerSparqlSource(spec_component_details: SpecComponentDetails) -> list:
     spec_components = []
     # Get the ordered  WHEN specComponents which is the transform and query driven template queries for the Layer
-    if spec_component_details.mustrd_triple_store["type"] == MUST.Anzo:
+    if spec_component_details.mustrd_triple_store["type"] == TRIPLESTORE.Anzo:
         graphmart_layer_uri = spec_component_details.spec_graph.value(subject=spec_component_details.spec_component_node,
                                                              predicate=MUST.anzoGraphmartLayer)
         queries = get_queries_for_layer(triple_store=spec_component_details.mustrd_triple_store,
                                                     graphmart_layer_uri=graphmart_layer_uri)
     # If anzo specific function is called but no anzo defined
     else:
         raise ValueError(f"This test specification is specific to Anzo and can only be run against that platform.")
@@ -525,15 +525,15 @@
         f"spec component ({spec_component_details.predicate})")
 
 
 def init_spec_component(predicate: URIRef, triple_store_type: URIRef = None ) -> GivenSpec | WhenSpec | ThenSpec | TableThenSpec:
     if predicate == MUST.given:
         spec_component = GivenSpec()
     elif predicate == MUST.when:
-        if triple_store_type == MUST.Anzo:
+        if triple_store_type == TRIPLESTORE.Anzo:
             spec_component = AnzoWhenSpec()
         else:
             spec_component = WhenSpec()
     elif predicate == MUST.then:
         spec_component = ThenSpec()
     else:
         spec_component = SpecComponent()
```

### Comparing `mustrd-0.1.7/mustrd/steprunner.py` & `mustrd-0.1.8/mustrd/steprunner.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 SOFTWARE.
 """
 
 import json
 
 from . import logger_setup
 from multimethods import MultiMethod, Default
-from .namespace import MUST
+from .namespace import MUST, TRIPLESTORE
 from rdflib import Graph, URIRef
 from .mustrdRdfLib import execute_select as execute_select_rdflib
 from .mustrdRdfLib import execute_construct as execute_construct_rdflib
 from .mustrdRdfLib import execute_update as execute_update_rdflib
 from .mustrdAnzo import upload_given as upload_given_anzo
 from .mustrdAnzo import execute_update as execute_update_anzo
 from .mustrdAnzo import execute_construct as execute_construct_anzo
@@ -49,85 +49,85 @@
     log.info(f"dispatch_upload_given to {ts}")
     return ts
 
 
 upload_given = MultiMethod('upload_given', dispatch_upload_given)
 
 
-@upload_given.method(MUST.RdfLib)
+@upload_given.method(TRIPLESTORE.RdfLib)
 def _upload_given_rdflib(triple_store: dict, given: Graph):
     triple_store["given"] = given
 
 
-@upload_given.method(MUST.GraphDb)
+@upload_given.method(TRIPLESTORE.GraphDb)
 def _upload_given_graphdb(triple_store: dict, given: Graph):
     upload_given_graphdb(triple_store, given)
 
 
-@upload_given.method(MUST.Anzo)
+@upload_given.method(TRIPLESTORE.Anzo)
 def _upload_given_anzo(triple_store: dict, given: Graph):
     upload_given_anzo(triple_store, given)
 
 
 def dispatch_run_when(spec_uri: URIRef, triple_store: dict, when: WhenSpec):
     ts = triple_store['type']
     query_type = when.queryType
     log.info(f"dispatch_run_when to SPARQL type {query_type} to {ts}")
     return ts, query_type
 
 
 run_when = MultiMethod('run_when', dispatch_run_when)
 
 
-@run_when.method((MUST.Anzo, MUST.UpdateSparql))
+@run_when.method((TRIPLESTORE.Anzo, MUST.UpdateSparql))
 def _anzo_run_when_update(spec_uri: URIRef, triple_store: dict, when: AnzoWhenSpec):
     return execute_update_anzo(triple_store, when.value, when.bindings)
 
 
-@run_when.method((MUST.Anzo, MUST.ConstructSparql))
+@run_when.method((TRIPLESTORE.Anzo, MUST.ConstructSparql))
 def _anzo_run_when_construct(spec_uri: URIRef, triple_store: dict, when: AnzoWhenSpec):
     return execute_construct_anzo(triple_store, when.value, when.bindings)
 
 
-@run_when.method((MUST.Anzo, MUST.SelectSparql))
+@run_when.method((TRIPLESTORE.Anzo, MUST.SelectSparql))
 def _anzo_run_when_select(spec_uri: URIRef, triple_store: dict, when: AnzoWhenSpec):
     return execute_select_anzo(triple_store, when.value, when.bindings)
 
 
-@run_when.method((MUST.GraphDb, MUST.UpdateSparql))
+@run_when.method((TRIPLESTORE.GraphDb, MUST.UpdateSparql))
 def _graphdb_run_when_update(spec_uri: URIRef, triple_store: dict, when: WhenSpec):
     return execute_update_graphdb(triple_store, when.value, when.bindings)
 
 
-@run_when.method((MUST.GraphDb, MUST.ConstructSparql))
+@run_when.method((TRIPLESTORE.GraphDb, MUST.ConstructSparql))
 def _graphdb_run_when_construct(spec_uri: URIRef, triple_store: dict, when: WhenSpec):
     return execute_construct_graphdb(triple_store, when.value, when.bindings)
 
 
-@run_when.method((MUST.GraphDb, MUST.SelectSparql))
+@run_when.method((TRIPLESTORE.GraphDb, MUST.SelectSparql))
 def _graphdb_run_when_select(spec_uri: URIRef, triple_store: dict, when: WhenSpec):
     return execute_select_graphdb(triple_store, when.value, when.bindings)
 
 
-@run_when.method((MUST.RdfLib, MUST.UpdateSparql))
+@run_when.method((TRIPLESTORE.RdfLib, MUST.UpdateSparql))
 def _rdflib_run_when_update(spec_uri: URIRef, triple_store: dict, when: WhenSpec):
     return execute_update_rdflib(triple_store, triple_store["given"], when.value, when.bindings)
 
 
-@run_when.method((MUST.RdfLib, MUST.ConstructSparql))
+@run_when.method((TRIPLESTORE.RdfLib, MUST.ConstructSparql))
 def _rdflib_run_when_construct(spec_uri: URIRef, triple_store: dict, when: WhenSpec):
     return execute_construct_rdflib(triple_store, triple_store["given"], when.value, when.bindings)
 
 
-@run_when.method((MUST.RdfLib, MUST.SelectSparql))
+@run_when.method((TRIPLESTORE.RdfLib, MUST.SelectSparql))
 def _rdflib_run_when_select(spec_uri: URIRef, triple_store: dict, when: WhenSpec):
     return execute_select_rdflib(triple_store, triple_store["given"], when.value, when.bindings)
 
 
-@run_when.method((MUST.Anzo, MUST.AnzoQueryDrivenUpdateSparql))
+@run_when.method((TRIPLESTORE.Anzo, MUST.AnzoQueryDrivenUpdateSparql))
 def _multi_run_when_anzo_query_driven_update(spec_uri: URIRef, triple_store: dict, when: AnzoWhenSpec):
     # run the parameters query to obtain the values for the template step and put them into a dictionary
     query_parameters = json.loads(execute_select_anzo(triple_store, when.paramQuery, None))
     if len(query_parameters['results']['bindings']) > 0:
         # replace the anzo query placeholders with the input and output graphs
         when_template = when.queryTemplate.replace(
             "${usingSources}",
@@ -154,13 +154,13 @@
 def _multi_run_when_default(spec_uri: URIRef, triple_store: dict, when: WhenSpec):
     if when.queryType == MUST.AskSparql:
         log.warning(f"Skipping {spec_uri}, SPARQL ASK not implemented.")
         msg = "SPARQL ASK not implemented."
     elif when.queryType == MUST.DescribeSparql:
         log.warning(f"Skipping {spec_uri}, SPARQL DESCRIBE not implemented.")
         msg = "SPARQL DESCRIBE not implemented."
-    elif triple_store['type'] not in [MUST.Anzo, MUST.GraphDb, MUST.RdfLib]:
+    elif triple_store['type'] not in [TRIPLESTORE.Anzo, TRIPLESTORE.GraphDb, TRIPLESTORE.RdfLib]:
         msg = f"{when.queryType} not implemented for {triple_store['type']}"
     else:
         log.warning(f"Skipping {spec_uri},  {when.queryType} is not a valid SPARQL query type.")
         msg = f"{when.queryType} is not a valid SPARQL query type."
     raise NotImplementedError(msg)
```

### Comparing `mustrd-0.1.7/mustrd/templates/md_ResultList_leaf_template.jinja` & `mustrd-0.1.8/mustrd/templates/md_ResultList_leaf_template.jinja`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.7/mustrd/TestResult.py` & `mustrd-0.1.8/mustrd/TestResult.py`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.7/mustrd/utils.py` & `mustrd-0.1.8/mustrd/utils.py`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.7/pyproject.toml` & `mustrd-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mustrd"
-version = "0.1.7"
+version = "0.1.8"
 description = "A Spec By Example framework for RDF and SPARQL, Inspired by Cucumber."
 authors = ["John Placek <john.placek@semanticpartners.com>",
     "Juliane Piñeiro-Winkler <juliane.pineiro-winkler@semanticpartners.com>",
     "Aymeric Picou <aymeric.picou@semanticpartners.com>",
     "Lance Paine <lance.paine@semanticpartners.com>",
     "Andrew Large <andy.large@semanticpartners.com>", ]
 classifiers = [
```

### Comparing `mustrd-0.1.7/README.adoc` & `mustrd-0.1.8/README.adoc`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.7/PKG-INFO` & `mustrd-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mustrd
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Spec By Example framework for RDF and SPARQL, Inspired by Cucumber.
 Home-page: https://github.com/Semantic-partners/mustrd
 License: MIT
 Author: John Placek
 Author-email: john.placek@semanticpartners.com
 Requires-Python: ==3.11.7
 Classifier: Framework :: Pytest
```

