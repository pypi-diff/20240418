# Comparing `tmp/ragdaemon-0.1.8.tar.gz` & `tmp/ragdaemon-0.1.9.tar.gz`

## Comparing `ragdaemon-0.1.8.tar` & `ragdaemon-0.1.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/__main__.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/app.py
--rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/context.py
--rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/errors.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/get_paths.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/graph.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/llm.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/utils.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     7336 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/database/database.py
--rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/conftest.py
--rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/test_comments.py
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/test_context.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/test_daemon.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/test_database.py
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/test_get_paths.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/test_sample.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/data/context_message.txt
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/data/diff_graph.json
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/README.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/app.py
+-rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/context.py
+-rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/graph.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/llm.py
+-rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/utils.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/conftest.py
+-rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/test_comments.py
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/test_context.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/test_daemon.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/test_database.py
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/test_sample.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/data/context_message.txt
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/PKG-INFO
```

### Comparing `ragdaemon-0.1.8/tutorial.ipynb` & `ragdaemon-0.1.9/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/.github/workflows/run-tests.yml` & `ragdaemon-0.1.9/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/ragdaemon/app.py` & `ragdaemon-0.1.9/ragdaemon/app.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/ragdaemon/context.py` & `ragdaemon-0.1.9/ragdaemon/context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/ragdaemon/daemon.py` & `ragdaemon-0.1.9/ragdaemon/daemon.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,19 +45,19 @@
             self.graph_path = (cwd / graph_path).resolve()
         else:
             self.graph_path = self.cwd / ".ragdaemon" / "graph.json"
         self.graph_path.parent.mkdir(exist_ok=True)
         if spice_client is None:
             spice_client = Spice(
                 default_text_model=DEFAULT_COMPLETION_MODEL,
-                default_embeddings_model=DEFAULT_EMBEDDING_MODEL,
+                default_embeddings_model=model,
             )
         self.spice_client = spice_client
-        self.model = model
-        self.provider = provider
+        self.embedding_model = model
+        self.embedding_provider = provider
 
         # Initialize an empty graph
         self.graph = KnowledgeGraph()
         self.graph.graph["cwd"] = self.cwd.as_posix()
         if self.verbose:
             print("Initialized empty graph.")
 
@@ -73,16 +73,16 @@
 
     @property
     def db(self) -> Database:
         if not hasattr(self, "_db"):
             self._db = get_db(
                 self.cwd,
                 spice_client=self.spice_client,
-                model=self.model,
-                provider=self.provider,
+                embedding_model=self.embedding_model,
+                embedding_provider=self.embedding_provider,
             )
         return self._db
 
     def save(self):
         """Saves the graph to disk."""
         data = json_graph.node_link_data(self.graph)
         with open(self.graph_path, "w") as f:
@@ -127,38 +127,35 @@
 
     def get_context(
         self,
         query: str,
         context_builder: Optional[ContextBuilder] = None,
         max_tokens: int = 8000,
         auto_tokens: int = 0,
+        model: str = DEFAULT_COMPLETION_MODEL,
     ) -> ContextBuilder:
         if context_builder is None:
             context = ContextBuilder(self.graph, self.db, self.verbose)
         else:
             # TODO: Compare graph hashes, reconcile changes
             context = context_builder
         include_context_message = context.render()
-        include_tokens = self.spice_client.count_tokens(
-            include_context_message, DEFAULT_COMPLETION_MODEL
-        )
+        include_tokens = self.spice_client.count_tokens(include_context_message, model)
         if not auto_tokens or include_tokens >= max_tokens:
             return context
 
         auto_tokens = min(auto_tokens, max_tokens - include_tokens)
         results = self.search(query)
         for node in results:
             if node["type"] == "diff":
                 context.add_diff(node["id"])
             else:
                 context.add_ref(node["ref"], tags=["search-result"])
             next_context_message = context.render()
-            next_tokens = self.spice_client.count_tokens(
-                next_context_message, DEFAULT_COMPLETION_MODEL
-            )
+            next_tokens = self.spice_client.count_tokens(next_context_message, model)
             if (next_tokens - include_tokens) > auto_tokens:
                 if node["type"] == "diff":
                     context.remove_diff(node["id"])
                 else:
                     context.remove_ref(node["ref"])
                 break
         return context
```

### Comparing `ragdaemon-0.1.8/ragdaemon/get_paths.py` & `ragdaemon-0.1.9/ragdaemon/get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/ragdaemon/graph.py` & `ragdaemon-0.1.9/ragdaemon/graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/ragdaemon/annotators/__init__.py` & `ragdaemon-0.1.9/ragdaemon/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.1.9/ragdaemon/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/ragdaemon/annotators/chunker.py` & `ragdaemon-0.1.9/ragdaemon/annotators/chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.1.9/ragdaemon/annotators/chunker_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.1.9/ragdaemon/annotators/chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/ragdaemon/annotators/diff.py` & `ragdaemon-0.1.9/ragdaemon/annotators/diff.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import json
 import re
 from pathlib import Path
 
 from ragdaemon.annotators.base_annotator import Annotator
-from ragdaemon.database import (
-    DEFAULT_EMBEDDING_MODEL,
-    MAX_TOKENS_PER_EMBEDDING,
-    Database,
-)
+from ragdaemon.database import Database
 from ragdaemon.get_paths import get_git_root_for_path
 from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.errors import RagdaemonError
 from ragdaemon.utils import get_document, hash_str, parse_path_ref, truncate
 
 
 def get_chunks_from_diff(id: str, diff: str) -> dict[str, str]:
@@ -113,19 +109,15 @@
                 "checksum": checksum,
                 "chunks": json.dumps(chunks),
                 "active": False,
             }
 
             # If the full diff is too long to embed, it is truncated. Anything
             # removed will be captured in chunks.
-            document, truncate_ratio = truncate(
-                document,
-                model=DEFAULT_EMBEDDING_MODEL,
-                max_tokens=MAX_TOKENS_PER_EMBEDDING,
-            )
+            document, truncate_ratio = truncate(document, db.embedding_model)
             if truncate_ratio > 0 and self.verbose:
                 print(f"Truncated diff by {truncate_ratio:.2%}")
             db.upsert(ids=checksum, documents=document, metadatas=data)
         else:
             data = existing_records["metadatas"][0]
         data["chunks"] = json.loads(data["chunks"])
         graph.add_node(self.id, **data)
@@ -141,19 +133,15 @@
                 data = {
                     "id": chunk_id,
                     "ref": chunk_ref,
                     "type": "diff",
                     "checksum": chunk_checksum,
                     "active": False,
                 }
-                document, truncate_ratio = truncate(
-                    document,
-                    model=DEFAULT_EMBEDDING_MODEL,
-                    max_tokens=MAX_TOKENS_PER_EMBEDDING,
-                )
+                document, truncate_ratio = truncate(document, db.embedding_model)
                 if truncate_ratio < 1 and self.verbose:
                     print(f"Truncated diff chunk {chunk_id} by {truncate_ratio:.2%}")
                 add_to_db["ids"].append(chunk_checksum)
                 add_to_db["documents"].append(document)
                 add_to_db["metadatas"].append(data)
             else:
                 data = existing_records["metadatas"][0]
```

### Comparing `ragdaemon-0.1.8/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.1.9/ragdaemon/annotators/hierarchy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 from pathlib import Path
 
 from ragdaemon.annotators.base_annotator import Annotator
-from ragdaemon.database import (
-    DEFAULT_EMBEDDING_MODEL,
-    MAX_TOKENS_PER_EMBEDDING,
-    Database,
-)
+from ragdaemon.database import Database
 from ragdaemon.get_paths import get_paths_for_directory
 from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.errors import RagdaemonError
 from ragdaemon.utils import get_document, hash_str, truncate
 
 
 def get_active_checksums(
@@ -38,19 +34,15 @@
                 metadatas = {
                     "id": path_str,
                     "type": "file",
                     "ref": ref,
                     "checksum": checksum,
                     "active": False,
                 }
-                document, truncate_ratio = truncate(
-                    document,
-                    model=DEFAULT_EMBEDDING_MODEL,
-                    max_tokens=MAX_TOKENS_PER_EMBEDDING,
-                )
+                document, truncate_ratio = truncate(document, db.embedding_model)
                 if truncate_ratio > 0 and verbose:
                     print(f"Truncated {path_str} by {truncate_ratio:.2%}")
                 add_to_db["ids"].append(checksum)
                 add_to_db["documents"].append(document)
                 add_to_db["metadatas"].append(metadatas)
             checksums[path] = checksum
         except UnicodeDecodeError:  # Ignore non-text files
```

### Comparing `ragdaemon-0.1.8/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.1.9/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/ragdaemon/database/chroma_database.py` & `ragdaemon-0.1.9/ragdaemon/database/chroma_database.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 
 class ChromaDB(Database):
     def __init__(
         self,
         cwd: Path,
         db_path: Path,
         spice_client: Spice,
-        model: str,
-        provider: Optional[str] = None,
+        embedding_model: str,
+        embedding_provider: Optional[str] = None,
     ) -> None:
         self.cwd = cwd
         self.db_path = db_path
-        self.model = model
+        self.embedding_model = embedding_model
 
         import chromadb  # Imports are slow so do it lazily
         from chromadb.api.types import Embeddable, EmbeddingFunction, Embeddings  # noqa: F811
 
         class SpiceEmbeddingFunction(EmbeddingFunction[Embeddable]):
             def __call__(self, input_texts: Embeddable) -> Embeddings:
                 if not all(isinstance(item, str) for item in input_texts):
@@ -40,24 +40,24 @@
                 n_batches = (len(input_texts) - 1) // MAX_INPUTS_PER_CALL + 1
                 output: Embeddings = []
                 for batch in range(n_batches):
                     start = batch * MAX_INPUTS_PER_CALL
                     end = min((batch + 1) * MAX_INPUTS_PER_CALL, len(input_texts))
                     embeddings = spice_client.get_embeddings_sync(
                         input_texts=input_texts[start:end],
-                        model=model,
-                        provider=provider,
+                        model=embedding_model,
+                        provider=embedding_provider,
                     ).embeddings
                     output.extend(embeddings)
                 return output
 
         embedding_function = SpiceEmbeddingFunction()
 
         _client = chromadb.PersistentClient(path=str(db_path))
-        name = f"ragdaemon-{self.cwd.name}-{self.model}"
+        name = f"ragdaemon-{self.cwd.name}-{self.embedding_model}"
         self._collection = _client.get_or_create_collection(
             name=name,
             embedding_function=embedding_function,
         )
 
     def query(self, query: str, active_checksums: list[str]) -> list[dict]:
         # Flag active records
```

### Comparing `ragdaemon-0.1.8/ragdaemon/database/database.py` & `ragdaemon-0.1.9/ragdaemon/database/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from pathlib import Path
 from typing import Optional
 
 from ragdaemon.graph import KnowledgeGraph
 
 
 class Database:
+    embedding_model: str | None = None
     _collection = None  # Collection | LiteDB
 
     def __init__(self, cwd: Path, db_path: Path) -> None:
         raise NotImplementedError
 
     def __getattr__(self, name):
         """Delegate attribute access to the collection."""
```

### Comparing `ragdaemon-0.1.8/ragdaemon/database/lite_database.py` & `ragdaemon-0.1.9/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/ragdaemon/static/favicon.ico` & `ragdaemon-0.1.9/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.1.9/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/ragdaemon/static/js/main.js` & `ragdaemon-0.1.9/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.1.9/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/ragdaemon/static/js/three/node.js` & `ragdaemon-0.1.9/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.1.9/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/ragdaemon/templates/index.html` & `ragdaemon-0.1.9/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/tests/conftest.py` & `ragdaemon-0.1.9/tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 @pytest.fixture
 def cwd():
     return Path("tests/sample").resolve()
 
 
 @pytest.fixture
 def mock_db(cwd):
-    return get_db(cwd, spice_client=AsyncMock(), model=DEFAULT_EMBEDDING_MODEL)
+    return get_db(
+        cwd, spice_client=AsyncMock(), embedding_model=DEFAULT_EMBEDDING_MODEL
+    )
 
 
 @pytest.fixture
 def mock_get_llm_response():
     with patch(
         "ragdaemon.annotators.chunker_llm.ChunkerLLM.get_llm_response",
         return_value={"chunks": []},
```

### Comparing `ragdaemon-0.1.8/tests/test_comments.py` & `ragdaemon-0.1.9/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/tests/test_context.py` & `ragdaemon-0.1.9/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/tests/test_daemon.py` & `ragdaemon-0.1.9/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/tests/test_get_paths.py` & `ragdaemon-0.1.9/tests/test_get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/tests/test_sample.py` & `ragdaemon-0.1.9/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/tests/annotators/test_chunker.py` & `ragdaemon-0.1.9/tests/annotators/test_chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/tests/annotators/test_diff.py` & `ragdaemon-0.1.9/tests/annotators/test_diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/tests/annotators/test_hierarchy.py` & `ragdaemon-0.1.9/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.1.9/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/tests/data/chunker_graph.json` & `ragdaemon-0.1.9/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/tests/data/context_message.txt` & `ragdaemon-0.1.9/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/tests/data/diff_graph.json` & `ragdaemon-0.1.9/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/tests/data/hierarchy_graph.json` & `ragdaemon-0.1.9/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.1.9/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/tests/sample/src/interface.py` & `ragdaemon-0.1.9/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/LICENSE` & `ragdaemon-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.8/README.md` & `ragdaemon-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 ## 2. **Explore the knowledge graph**
 
 Install locally to visualize and query the knowledge graph directly. 
 Install using `pip install ragdaemon`, and run in your codebase's directory, e.g. `ragdaemon`. This will start a Daemon on your codebase, and an interface at `localhost:5001`. Options:
 - `--chunk-extensions <ext>[..<ext>]`: Which file extensions to chunk. If not specified, defaults to the top 20 most common code file extensions.
 - `--chunk-model`: OpenAI's `gpt-4-0215-preview` by default.
-- `--embeddings-model`: OpenAI's `text-embedding-ada-002` by default.
+- `--embeddings-model`: OpenAI's `text-embedding-3-large` by default.
 - `--diff`: A git diff to include in the knowledge graph. By default, the active diff (if any) is included with each code feature.
 
 ## 3. **Use ragdaemon Python API** 
 
 Ragdaemon is released open-source as a standalone RAG system. It includes a library of python classes to generate and query the knowledge graph. The graph itself is a NetworkX MultiDiGraph which saves/loads to a `.json` file.
 
 ```python
```

### Comparing `ragdaemon-0.1.8/pyproject.toml` & `ragdaemon-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.1.8"
+version = "0.1.9"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
```

### Comparing `ragdaemon-0.1.8/PKG-INFO` & `ragdaemon-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.1.8
+Version: 0.1.9
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -35,15 +35,15 @@
 
 ## 2. **Explore the knowledge graph**
 
 Install locally to visualize and query the knowledge graph directly. 
 Install using `pip install ragdaemon`, and run in your codebase's directory, e.g. `ragdaemon`. This will start a Daemon on your codebase, and an interface at `localhost:5001`. Options:
 - `--chunk-extensions <ext>[..<ext>]`: Which file extensions to chunk. If not specified, defaults to the top 20 most common code file extensions.
 - `--chunk-model`: OpenAI's `gpt-4-0215-preview` by default.
-- `--embeddings-model`: OpenAI's `text-embedding-ada-002` by default.
+- `--embeddings-model`: OpenAI's `text-embedding-3-large` by default.
 - `--diff`: A git diff to include in the knowledge graph. By default, the active diff (if any) is included with each code feature.
 
 ## 3. **Use ragdaemon Python API** 
 
 Ragdaemon is released open-source as a standalone RAG system. It includes a library of python classes to generate and query the knowledge graph. The graph itself is a NetworkX MultiDiGraph which saves/loads to a `.json` file.
 
 ```python
```

