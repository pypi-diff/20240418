# Comparing `tmp/ofnodes-1.5.1.tar.gz` & `tmp/ofnodes-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofnodes-1.5.1.tar", max compression
+gzip compressed data, was "ofnodes-1.6.0.tar", max compression
```

## Comparing `ofnodes-1.5.1.tar` & `ofnodes-1.6.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-04-10 08:32:12.931610 ofnodes-1.5.1/LICENSE
--rw-r--r--   0        0        0     2606 2024-04-05 21:55:30.417310 ofnodes-1.5.1/README.md
--rw-r--r--   0        0        0      590 2024-04-17 16:26:13.714358 ofnodes-1.5.1/pyproject.toml
--rw-r--r--   0        0        0      953 2024-04-05 16:17:48.873936 ofnodes-1.5.1/src/ofnodes/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.5.1/src/ofnodes/nodes/__init__.py
--rw-r--r--   0        0        0     2479 2024-04-17 16:06:36.566198 ofnodes-1.5.1/src/ofnodes/nodes/singlynode.py
--rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-1.5.1/src/ofnodes/py.typed
--rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.5.1/src/ofnodes/structures/__init__.py
--rw-r--r--   0        0        0    23695 2024-04-17 16:17:14.917972 ofnodes-1.5.1/src/ofnodes/structures/singlylinkedlist.py
--rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 ofnodes-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-10 08:32:12.931610 ofnodes-1.6.0/LICENSE
+-rw-r--r--   0        0        0     2606 2024-04-05 21:55:30.417310 ofnodes-1.6.0/README.md
+-rw-r--r--   0        0        0      590 2024-04-18 20:15:49.132482 ofnodes-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      953 2024-04-05 16:17:48.873936 ofnodes-1.6.0/src/ofnodes/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.6.0/src/ofnodes/nodes/__init__.py
+-rw-r--r--   0        0        0     2479 2024-04-17 16:06:36.566198 ofnodes-1.6.0/src/ofnodes/nodes/singlynode.py
+-rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-1.6.0/src/ofnodes/py.typed
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.6.0/src/ofnodes/structures/__init__.py
+-rw-r--r--   0        0        0    26514 2024-04-18 20:15:49.132482 ofnodes-1.6.0/src/ofnodes/structures/singlylinkedlist.py
+-rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 ofnodes-1.6.0/PKG-INFO
```

### Comparing `ofnodes-1.5.1/LICENSE` & `ofnodes-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ofnodes-1.5.1/README.md` & `ofnodes-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ofnodes-1.5.1/pyproject.toml` & `ofnodes-1.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofnodes"
-version = "1.5.1"
+version = "1.6.0"
 description = "A library of Data Structures and Algorithms written in Python"
 authors = ["Robert Portelli <github@robertportelli.com>"]
 readme = "README.md"
 packages = [{include = "ofnodes", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `ofnodes-1.5.1/src/ofnodes/__init__.py` & `ofnodes-1.6.0/src/ofnodes/__init__.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.5.1/src/ofnodes/nodes/singlynode.py` & `ofnodes-1.6.0/src/ofnodes/nodes/singlynode.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.5.1/src/ofnodes/structures/singlylinkedlist.py` & `ofnodes-1.6.0/src/ofnodes/structures/singlylinkedlist.py`

 * *Files 13% similar despite different names*

```diff
@@ -350,14 +350,63 @@
             (SinglyNode(data='1 node'), SinglyNode(data='2 node'), SinglyNode(data='4 node'))
             >>> llist.tail = "is passed to setter to become SinglyNode()"
             >>> llist.head, llist.head.next, llist.tail
             (SinglyNode(data='1 node'), SinglyNode(data='2 node'), SinglyNode(data='is passed to setter to become SinglyNode()'))
         """
         self.tail = data  # trigger the tail setter
 
+    def insert_after_target(self, target_data: Any, data_to_insert: Any) -> None:
+        """
+        steps:
+        1) the target data is validated
+        2) the head data is checked for the target
+            - if True, the linked list is checked if it's a one node list
+                - if True, simply use the tail property to insert after the head
+                - if False, the list contains more than one node
+        3) the tail data is checked for the target
+            - if True, simply use
+        """
+        self.target = target_data  # trigger the setter
+        # insert after the first encounter
+        if getattr(self._head, 'data') == self._target:
+            if self._head is self._tail:  # it's a one node list
+                self.tail = data_to_insert  # trigger the setter, tail property will validate input
+                return
+        current_node = getattr(self, '_head')  # traversal
+        while current_node is not self._tail:  # traversal
+            if current_node.data == self._target:
+                new_node = SinglyNode(data_to_insert)  # SinglyNode() will validate input
+                setattr(new_node, '_next', current_node.next)  # insert after()
+                setattr(current_node, '_next', new_node)  # insert after()
+                return
+            current_node = current_node.next  # traversal
+        if getattr(self._tail, 'data') == self.target:
+            self.tail = data_to_insert  # # trigger the setter, tail property will validate input
+
+    def insert_before_target(self, target_data, data_to_insert):
+        """The traversal doesn't have to account for head or tail because
+        each is explicitly checked before traversal.
+
+        using current_node.next for traversal accounts for a one node list
+        as .next is not set on the head of a one node list."""
+        self.target = target_data  # trigger setter
+        # insert before first occurence
+        if getattr(self._head, 'data') == self._target:
+            self.head = data_to_insert  # trigger the setter, head property will validate input
+            return
+        current_node = getattr(self, '_head')  # traversal
+        while current_node: # traversal
+            if current_node.next.data == self._target:  # peek
+                #node = current_node.next  # the node containing the target
+                new_node = SinglyNode(data_to_insert)
+                setattr(new_node, '_next', current_node.next)  # insert_before()
+                setattr(current_node, '_next', new_node)  # insert before()
+                return #node
+            current_node = current_node.next  # traversal
+
     def search(self, target_data):
         """Searches each node's data in a linked list until the first occurrence of
         the target is found.
 
         Args:
             target_data (Any): The value to search for in the linked list.
 
@@ -445,28 +494,30 @@
             >>> sllist.head, sllist.head.next, sllist.tail
             (SinglyNode(data='2 node'), None, SinglyNode(data='2 node'))
         """
 
         self.target = target_data  # trigger the setter
 
         if getattr(self._head, 'data') == self._target:
-            # node = self._head
+            # node = self._head  # the node to be removed
             self.remove_head()
             return #node
+
+        current_node = getattr(self, '_head')  # traversal
+        while current_node.next is not self._tail:  # traversal (tail already checked)
+            if current_node.next.data == self._target:  # peek
+                #node = current_node.next  # the node to be removed
+                setattr(current_node, '_next', current_node.next.next)  # remove()
+                return #node
+            current_node = current_node.next  # traversal
+
         if getattr(self._tail, 'data') == self._target:
-            # node = self._tail
+            # node = self._tail  # the node to be removed
             self.remove_tail()
             return #node
-        current_node = getattr(self, '_head')
-        while current_node.next:
-            if current_node.next.data == self._target:
-                #node = current_node.next
-                setattr(current_node, '_next', current_node.next.next)
-                return #node
-            current_node = current_node.next
 
     def remove_head(self) -> None:
         """Removes the head node from the linked list.
 
         Raises:
             ValueError: If the linked list is empty.
```

### Comparing `ofnodes-1.5.1/PKG-INFO` & `ofnodes-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofnodes
-Version: 1.5.1
+Version: 1.6.0
 Summary: A library of Data Structures and Algorithms written in Python
 Author: Robert Portelli
 Author-email: github@robertportelli.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

