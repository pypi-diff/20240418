# Comparing `tmp/TestY_rust-0.1.2.tar.gz` & `tmp/TestY_rust-0.1.3.tar.gz`

## Comparing `TestY_rust-0.1.2.tar` & `TestY_rust-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      333 1970-01-01 00:00:00.000000 TestY_rust-0.1.2/Cargo.toml
--rw-r--r--   0     1001      127     3567 2024-04-15 09:13:12.000000 TestY_rust-0.1.2/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      677 2024-04-15 09:13:12.000000 TestY_rust-0.1.2/.gitignore
--rw-r--r--   0     1001      127        7 2024-04-15 09:13:12.000000 TestY_rust-0.1.2/README.md
--rw-r--r--   0     1001      127     1009 2024-04-15 09:13:12.000000 TestY_rust-0.1.2/__init__.pyi
--rw-r--r--   0     1001      127      213 2024-04-15 09:13:12.000000 TestY_rust-0.1.2/pysrc/rusty/__init__.py
--rw-r--r--   0     1001      127      293 2024-04-15 09:13:12.000000 TestY_rust-0.1.2/pysrc/rusty/constants.py
--rw-r--r--   0     1001      127      444 2024-04-15 09:13:12.000000 TestY_rust-0.1.2/pysrc/rusty/types.py
--rw-r--r--   0     1001      127      266 2024-04-15 09:13:12.000000 TestY_rust-0.1.2/src/lib.rs
--rw-r--r--   0     1001      127     6082 2024-04-15 09:13:12.000000 TestY_rust-0.1.2/src/serialization.rs
--rw-r--r--   0     1001      127     4460 2024-04-15 09:13:12.000000 TestY_rust-0.1.2/src/sql.rs
--rw-r--r--   0     1001      127    28006 2024-04-15 09:13:12.000000 TestY_rust-0.1.2/Cargo.lock
--rw-r--r--   0     1001      127      520 2024-04-15 09:13:12.000000 TestY_rust-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      336 1970-01-01 00:00:00.000000 TestY_rust-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      333 1970-01-01 00:00:00.000000 TestY_rust-0.1.3/Cargo.toml
+-rw-r--r--   0     1001      127     3567 2024-04-18 11:21:54.000000 TestY_rust-0.1.3/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      685 2024-04-18 11:21:54.000000 TestY_rust-0.1.3/.gitignore
+-rw-r--r--   0     1001      127        7 2024-04-18 11:21:54.000000 TestY_rust-0.1.3/README.md
+-rw-r--r--   0     1001      127      255 2024-04-18 11:21:54.000000 TestY_rust-0.1.3/pysrc/rusty/__init__.py
+-rw-r--r--   0     1001      127     1193 2024-04-18 11:21:54.000000 TestY_rust-0.1.3/pysrc/rusty/__init__.pyi
+-rw-r--r--   0     1001      127      139 2024-04-18 11:21:54.000000 TestY_rust-0.1.3/pysrc/rusty/constants.py
+-rw-r--r--   0     1001      127      444 2024-04-18 11:21:54.000000 TestY_rust-0.1.3/pysrc/rusty/types.py
+-rw-r--r--   0     1001      127      266 2024-04-18 11:21:54.000000 TestY_rust-0.1.3/src/lib.rs
+-rw-r--r--   0     1001      127     6082 2024-04-18 11:21:54.000000 TestY_rust-0.1.3/src/serialization.rs
+-rw-r--r--   0     1001      127     3838 2024-04-18 11:21:54.000000 TestY_rust-0.1.3/src/sql.rs
+-rw-r--r--   0     1001      127    28006 2024-04-18 11:21:54.000000 TestY_rust-0.1.3/Cargo.lock
+-rw-r--r--   0     1001      127      520 2024-04-18 11:21:54.000000 TestY_rust-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      336 1970-01-01 00:00:00.000000 TestY_rust-0.1.3/PKG-INFO
```

### Comparing `TestY_rust-0.1.2/.github/workflows/CI.yml` & `TestY_rust-0.1.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `TestY_rust-0.1.2/.gitignore` & `TestY_rust-0.1.3/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+target/
 # Byte-compiled / optimized / DLL files
 __pycache__/
 .pytest_cache/
 *.py[cod]
 
 # C extensions
 *.so
```

### Comparing `TestY_rust-0.1.2/__init__.pyi` & `TestY_rust-0.1.3/pysrc/rusty/__init__.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 from typing import Any
 
-from rusty.types import DataSetObject, CaseSearchQueryParams, Prefetch
+from .constants import *
+from .rusty import *
+from .types import *
+
+__all__ = (
+    "CASES_SEARCH_SUITE_FIELDS",
+    "CASES_SEARCH_CASE_FIELDS",
+    "CaseSearchQueryParams",
+    "Prefetch",
+    "DataSetObject",
+    "serialize_tree",
+    "cases_search",
+)
 
 
 def serialize_tree(
     data_set_object: DataSetObject,
     prefetch_objects: list[Prefetch],
     is_tree: bool,
 ) -> list[dict[str, Any]]:
```

### Comparing `TestY_rust-0.1.2/src/serialization.rs` & `TestY_rust-0.1.3/src/serialization.rs`

 * *Files identical despite different names*

### Comparing `TestY_rust-0.1.2/src/sql.rs` & `TestY_rust-0.1.3/src/sql.rs`

 * *Files 14% similar despite different names*

```diff
@@ -24,23 +24,15 @@
     id: i64,
     name: String,
 }
 
 #[derive(Clone, Serialize)]
 struct TestSuite {
     id: i64,
-    name: String,
-    project: i64,
-    description: Option<String>,
     parent_id: Option<i64>,
-    descendant_count: f64,
-    cases_count: Option<i64>,
-    total_cases_count: Option<i64>,
-    estimates: Option<i64>,
-    total_estimates: Option<i64>,
     title: String,
     children: Vec<TestSuite>,
     parent: Option<Parent>,
     test_cases: Vec<TestCase>,
 }
 
 #[derive(Serialize, Clone)]
@@ -92,23 +84,15 @@
         .query(&query_params.suites_query, &[])
         .expect("Error occurred in suites query")
     {
         let id: i64 = row.get("id");
         let parent_id = row.get("parent_id");
         let suite = TestSuite {
             id: id,
-            name: row.get("name"),
-            project: row.get("project_id"),
-            description: row.get("description"),
             parent_id: parent_id,
-            descendant_count: row.get("descendant_count"),
-            cases_count: row.get("cases_count"),
-            total_cases_count: row.get("total_cases_count"),
-            estimates: row.get("estimates"),
-            total_estimates: row.get("total_estimates"),
             title: row.get("title"),
             children: vec![],
             parent: None,
             test_cases: vec![],
         };
         let node = Node {
             id,
@@ -135,15 +119,15 @@
     for node in suite_map.values() {
         let mut borrowed_node = node.borrow_mut();
         if let Some(parent_id) = borrowed_node.parent_id {
             if let Some(parent) = suite_map.get(&parent_id) {
                 let mut borrowed_parent = parent.borrow_mut();
                 borrowed_node.object.parent = Option::from(Parent {
                     id: borrowed_parent.id,
-                    name: borrowed_parent.object.name.clone(),
+                    name: borrowed_parent.object.title.clone(),
                 });
                 borrowed_parent.children.push(Rc::clone(node));
             }
         } else {
             root_refs.push(Rc::clone(node))
         }
     }
```

### Comparing `TestY_rust-0.1.2/Cargo.lock` & `TestY_rust-0.1.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -579,15 +579,15 @@
 name = "rustc-demangle"
 version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
 
 [[package]]
 name = "rusty"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "postgres",
  "pyo3",
  "serde",
  "serde_json",
 ]
```

### Comparing `TestY_rust-0.1.2/pyproject.toml` & `TestY_rust-0.1.3/pyproject.toml`

 * *Files identical despite different names*

