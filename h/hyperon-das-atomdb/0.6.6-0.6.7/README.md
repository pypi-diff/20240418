# Comparing `tmp/hyperon_das_atomdb-0.6.6.tar.gz` & `tmp/hyperon_das_atomdb-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperon_das_atomdb-0.6.6.tar", max compression
+gzip compressed data, was "hyperon_das_atomdb-0.6.7.tar", max compression
```

## Comparing `hyperon_das_atomdb-0.6.6.tar` & `hyperon_das_atomdb-0.6.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1081 2024-04-17 13:50:45.888398 hyperon_das_atomdb-0.6.6/LICENCE
--rw-r--r--   0        0        0     2687 2024-04-17 13:50:45.888398 hyperon_das_atomdb-0.6.6/README.md
--rw-r--r--   0        0        0      306 2024-04-17 13:50:45.888398 hyperon_das_atomdb-0.6.6/hyperon_das_atomdb/__init__.py
--rw-r--r--   0        0        0      194 2024-04-17 13:50:45.892398 hyperon_das_atomdb-0.6.6/hyperon_das_atomdb/adapters/__init__.py
--rw-r--r--   0        0        0    20557 2024-04-17 13:50:45.892398 hyperon_das_atomdb-0.6.6/hyperon_das_atomdb/adapters/ram_only.py
--rw-r--r--   0        0        0    37055 2024-04-17 13:50:45.892398 hyperon_das_atomdb-0.6.6/hyperon_das_atomdb/adapters/redis_mongo_db.py
--rw-r--r--   0        0        0    12546 2024-04-17 13:50:45.892398 hyperon_das_atomdb-0.6.6/hyperon_das_atomdb/adapters/redis_postgreslobe_db.py
--rw-r--r--   0        0        0    19820 2024-04-17 13:50:45.892398 hyperon_das_atomdb-0.6.6/hyperon_das_atomdb/database.py
--rw-r--r--   0        0        0      939 2024-04-17 13:50:45.892398 hyperon_das_atomdb-0.6.6/hyperon_das_atomdb/exceptions.py
--rw-r--r--   0        0        0     1122 2024-04-17 13:50:45.892398 hyperon_das_atomdb-0.6.6/hyperon_das_atomdb/index.py
--rw-r--r--   0        0        0     1052 2024-04-17 13:50:45.892398 hyperon_das_atomdb-0.6.6/hyperon_das_atomdb/logger.py
--rw-r--r--   0        0        0        0 2024-04-17 13:50:45.892398 hyperon_das_atomdb-0.6.6/hyperon_das_atomdb/utils/__init__.py
--rw-r--r--   0        0        0     1947 2024-04-17 13:50:45.892398 hyperon_das_atomdb-0.6.6/hyperon_das_atomdb/utils/expression_hasher.py
--rw-r--r--   0        0        0     5695 2024-04-17 13:50:45.892398 hyperon_das_atomdb-0.6.6/hyperon_das_atomdb/utils/mapper.py
--rw-r--r--   0        0        0     1388 2024-04-17 13:50:45.892398 hyperon_das_atomdb-0.6.6/hyperon_das_atomdb/utils/patterns.py
--rw-r--r--   0        0        0       65 2024-04-17 13:50:45.892398 hyperon_das_atomdb-0.6.6/hyperon_das_atomdb/utils/settings.py
--rw-r--r--   0        0        0     1141 2024-04-17 13:50:57.428577 hyperon_das_atomdb-0.6.6/pyproject.toml
--rw-r--r--   0        0        0     3564 1970-01-01 00:00:00.000000 hyperon_das_atomdb-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-18 19:30:20.156326 hyperon_das_atomdb-0.6.7/LICENCE
+-rw-r--r--   0        0        0     2687 2024-04-18 19:30:20.156326 hyperon_das_atomdb-0.6.7/README.md
+-rw-r--r--   0        0        0      306 2024-04-18 19:30:20.160326 hyperon_das_atomdb-0.6.7/hyperon_das_atomdb/__init__.py
+-rw-r--r--   0        0        0      194 2024-04-18 19:30:20.160326 hyperon_das_atomdb-0.6.7/hyperon_das_atomdb/adapters/__init__.py
+-rw-r--r--   0        0        0    20567 2024-04-18 19:30:20.160326 hyperon_das_atomdb-0.6.7/hyperon_das_atomdb/adapters/ram_only.py
+-rw-r--r--   0        0        0    37515 2024-04-18 19:30:20.160326 hyperon_das_atomdb-0.6.7/hyperon_das_atomdb/adapters/redis_mongo_db.py
+-rw-r--r--   0        0        0    12546 2024-04-18 19:30:20.160326 hyperon_das_atomdb-0.6.7/hyperon_das_atomdb/adapters/redis_postgreslobe_db.py
+-rw-r--r--   0        0        0    20258 2024-04-18 19:30:20.160326 hyperon_das_atomdb-0.6.7/hyperon_das_atomdb/database.py
+-rw-r--r--   0        0        0      939 2024-04-18 19:30:20.160326 hyperon_das_atomdb-0.6.7/hyperon_das_atomdb/exceptions.py
+-rw-r--r--   0        0        0     1122 2024-04-18 19:30:20.160326 hyperon_das_atomdb-0.6.7/hyperon_das_atomdb/index.py
+-rw-r--r--   0        0        0     1052 2024-04-18 19:30:20.160326 hyperon_das_atomdb-0.6.7/hyperon_das_atomdb/logger.py
+-rw-r--r--   0        0        0        0 2024-04-18 19:30:20.160326 hyperon_das_atomdb-0.6.7/hyperon_das_atomdb/utils/__init__.py
+-rw-r--r--   0        0        0     1947 2024-04-18 19:30:20.160326 hyperon_das_atomdb-0.6.7/hyperon_das_atomdb/utils/expression_hasher.py
+-rw-r--r--   0        0        0     5695 2024-04-18 19:30:20.160326 hyperon_das_atomdb-0.6.7/hyperon_das_atomdb/utils/mapper.py
+-rw-r--r--   0        0        0     1388 2024-04-18 19:30:20.160326 hyperon_das_atomdb-0.6.7/hyperon_das_atomdb/utils/patterns.py
+-rw-r--r--   0        0        0       65 2024-04-18 19:30:20.160326 hyperon_das_atomdb-0.6.7/hyperon_das_atomdb/utils/settings.py
+-rw-r--r--   0        0        0     1141 2024-04-18 19:30:28.492392 hyperon_das_atomdb-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0     3564 1970-01-01 00:00:00.000000 hyperon_das_atomdb-0.6.7/PKG-INFO
```

### Comparing `hyperon_das_atomdb-0.6.6/LICENCE` & `hyperon_das_atomdb-0.6.7/LICENCE`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.6/README.md` & `hyperon_das_atomdb-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.6/hyperon_das_atomdb/adapters/ram_only.py` & `hyperon_das_atomdb-0.6.7/hyperon_das_atomdb/adapters/ram_only.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,15 +290,15 @@
         else:
             return [
                 key
                 for key, value in self.db.node.items()
                 if value['composite_type_hash'] == node_type_hash
             ]
 
-    def get_all_links(self, link_type: str) -> List[str]:
+    def get_all_links(self, link_type: str, **kwargs) -> List[str]:
         answer = []
         for _, link in self.db.link.items():
             if link['named_type'] == link_type:
                 answer.append(link['_id'])
         return answer
 
     def get_link_handle(self, link_type: str, target_handles: List[str]) -> str:
```

### Comparing `hyperon_das_atomdb-0.6.6/hyperon_das_atomdb/adapters/redis_mongo_db.py` & `hyperon_das_atomdb-0.6.7/hyperon_das_atomdb/adapters/redis_mongo_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,20 +377,33 @@
             return [
                 document[MongoFieldNames.ID_HASH]
                 for document in self.mongo_atoms_collection.find(
                     {MongoFieldNames.TYPE_NAME: node_type}
                 )
             ]
 
-    def get_all_links(self, link_type: str) -> List[str]:
-        links_handle = []
-        documents = self.mongo_atoms_collection.find({MongoFieldNames.TYPE_NAME: link_type})
-        for document in documents:
-            links_handle.append(document[MongoFieldNames.ID_HASH])
-        return links_handle
+    def get_all_links(self, link_type: str, **kwargs) -> Tuple[int, List[str]]:
+        pymongo_cursor = self.mongo_atoms_collection.find({MongoFieldNames.TYPE_NAME: link_type})
+
+        if kwargs.get('cursor') is not None:
+            cursor = kwargs.get('cursor')
+            chunk_size = kwargs.get('chunk_size', 500)
+            pymongo_cursor.skip(cursor).limit(chunk_size)
+
+            handles = [document[MongoFieldNames.ID_HASH] for document in pymongo_cursor]
+
+            if not handles:
+                return 0, []
+
+            if len(handles) < chunk_size:
+                return 0, handles
+            else:
+                return cursor + chunk_size, handles
+
+        return 0, [document[MongoFieldNames.ID_HASH] for document in pymongo_cursor]
 
     def get_link_handle(self, link_type: str, target_handles: List[str]) -> str:
         link_handle = self.link_handle(link_type, target_handles)
         document = self._retrieve_document(link_handle)
         if document is not None:
             return document[MongoFieldNames.ID_HASH]
         else:
@@ -423,29 +436,29 @@
     def get_matched_links(
         self, link_type: str, target_handles: List[str], **kwargs
     ) -> Union[tuple, list]:
         if link_type != WILDCARD and WILDCARD not in target_handles:
             try:
                 link_handle = self.get_link_handle(link_type, target_handles)
                 if kwargs.get('cursor') is not None:
-                    return None, [link_handle]
+                    return 0, [link_handle]
                 return [link_handle]
             except LinkDoesNotExist:
                 if kwargs.get('cursor') is not None:
-                    return None, []
+                    return 0, []
                 return []
 
         if link_type == WILDCARD:
             link_type_hash = WILDCARD
         else:
             link_type_hash = self._get_atom_type_hash(link_type)
 
         if link_type_hash is None:
             if kwargs.get('cursor') is not None:
-                return None, []
+                return 0, []
             return []
 
         if link_type in UNORDERED_LINK_TYPES:
             target_handles = sorted(target_handles)
 
         pattern_hash = ExpressionHasher.composite_hash([link_type_hash, *target_handles])
         cursor, patterns_matched = self._retrieve_pattern(pattern_hash, **kwargs)
@@ -519,19 +532,20 @@
             if "targets" in document:
                 answer["targets"] = document["targets"]
             else:
                 answer["name"] = document["name"]
         return answer
 
     def count_atoms(self) -> Tuple[int, int]:
-        atoms_count = self.mongo_atoms_collection.estimated_document_count()
         nodes_count = self.mongo_atoms_collection.count_documents(
             {MongoFieldNames.COMPOSITE_TYPE: {'$exists': False}}
         )
-        links_count = atoms_count - nodes_count
+        links_count = self.mongo_atoms_collection.count_documents(
+            {MongoFieldNames.COMPOSITE_TYPE: {'$exists': True}}
+        )
         return (nodes_count, links_count)
 
     def clear_database(self) -> None:
         """
         from the connected MongoDB and Redis databases.
 
         This method drops all collections in the MongoDB database and flushes
```

### Comparing `hyperon_das_atomdb-0.6.6/hyperon_das_atomdb/adapters/redis_postgreslobe_db.py` & `hyperon_das_atomdb-0.6.7/hyperon_das_atomdb/adapters/redis_postgreslobe_db.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.6/hyperon_das_atomdb/database.py` & `hyperon_das_atomdb-0.6.7/hyperon_das_atomdb/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -258,14 +258,27 @@
 
         Returns:
             List[str]: A list of node handles or names, depending on the value of 'names'.
         """
         ...  # pragma no cover
 
     @abstractmethod
+    def get_all_links(self, link_type: str, **kwargs) -> Union[List[str], Tuple[int, List[str]]]:
+        """
+        Get all link of a specific type.
+
+        Args:
+            link_type (str): The link type.
+
+        Returns:
+            Union[List[str], Tuple[int, List[str]]]: A list of link handles or a tuple containing the cursor number and the list of link handles.
+        """
+        ...  # pragma no cover
+
+    @abstractmethod
     def get_link_handle(self, link_type: str, target_handles: List[str]) -> str:
         """
         Get the handle of the link with the specified type and targets.
 
         Args:
             link_type (str): The link type.
             target_handles (List[str]): A list of link target identifiers.
```

### Comparing `hyperon_das_atomdb-0.6.6/hyperon_das_atomdb/exceptions.py` & `hyperon_das_atomdb-0.6.7/hyperon_das_atomdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.6/hyperon_das_atomdb/index.py` & `hyperon_das_atomdb-0.6.7/hyperon_das_atomdb/index.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.6/hyperon_das_atomdb/logger.py` & `hyperon_das_atomdb-0.6.7/hyperon_das_atomdb/logger.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.6/hyperon_das_atomdb/utils/expression_hasher.py` & `hyperon_das_atomdb-0.6.7/hyperon_das_atomdb/utils/expression_hasher.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.6/hyperon_das_atomdb/utils/mapper.py` & `hyperon_das_atomdb-0.6.7/hyperon_das_atomdb/utils/mapper.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.6/hyperon_das_atomdb/utils/patterns.py` & `hyperon_das_atomdb-0.6.7/hyperon_das_atomdb/utils/patterns.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.6/pyproject.toml` & `hyperon_das_atomdb-0.6.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperon-das-atomdb"
-version = "0.6.6"
+version = "0.6.7"
 description = "Persistence layer for Distributed AtomSpace"
 authors = ["marcocapozzoli <marcocapozzoli90@gmail.com>"]
 readme = "README.md"
 packages = [{include = "hyperon_das_atomdb"}]
 
 [tool.poetry.urls]
 "Code" = "https://github.com/singnet/das-atom-db"
```

### Comparing `hyperon_das_atomdb-0.6.6/PKG-INFO` & `hyperon_das_atomdb-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperon-das-atomdb
-Version: 0.6.6
+Version: 0.6.7
 Summary: Persistence layer for Distributed AtomSpace
 Author: marcocapozzoli
 Author-email: marcocapozzoli90@gmail.com
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

