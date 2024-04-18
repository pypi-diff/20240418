# Comparing `tmp/thymus_ast-0.1.6.tar.gz` & `tmp/thymus_ast-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thymus_ast-0.1.6.tar", max compression
+gzip compressed data, was "thymus_ast-0.1.7.tar", max compression
```

## Comparing `thymus_ast-0.1.6.tar` & `thymus_ast-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1093 2023-09-19 16:12:05.290498 thymus_ast-0.1.6/LICENSE
--rw-r--r--   0        0        0      492 2023-12-08 13:57:17.473054 thymus_ast-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      544 2023-12-09 12:09:08.370980 thymus_ast-0.1.6/README.md
--rw-r--r--   0        0        0        2 2023-09-19 21:16:45.075801 thymus_ast-0.1.6/thymus_ast/__init__.py
--rw-r--r--   0        0        0      342 2023-06-17 13:40:41.547409 thymus_ast-0.1.6/thymus_ast/ios/__init__.py
--rw-r--r--   0        0        0    14383 2023-12-09 12:03:57.299512 thymus_ast-0.1.6/thymus_ast/ios/ios.py
--rw-r--r--   0        0        0      702 2023-09-12 12:44:08.921526 thymus_ast-0.1.6/thymus_ast/junos/__init__.py
--rw-r--r--   0        0        0    15718 2023-12-08 14:01:14.503719 thymus_ast-0.1.6/thymus_ast/junos/junos.py
--rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 thymus_ast-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-09-19 16:12:05.290498 thymus_ast-0.1.7/LICENSE
+-rw-r--r--   0        0        0      492 2024-04-12 09:04:25.834401 thymus_ast-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      544 2023-12-09 12:09:08.370980 thymus_ast-0.1.7/README.md
+-rw-r--r--   0        0        0        2 2023-09-19 21:16:45.075801 thymus_ast-0.1.7/thymus_ast/__init__.py
+-rw-r--r--   0        0        0      342 2023-06-17 13:40:41.547409 thymus_ast-0.1.7/thymus_ast/ios/__init__.py
+-rw-r--r--   0        0        0    14638 2024-04-18 19:36:07.707768 thymus_ast-0.1.7/thymus_ast/ios/ios.py
+-rw-r--r--   0        0        0      702 2024-04-18 19:38:59.977723 thymus_ast-0.1.7/thymus_ast/junos/__init__.py
+-rw-r--r--   0        0        0    15718 2024-04-18 19:39:06.920916 thymus_ast-0.1.7/thymus_ast/junos/junos.py
+-rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 thymus_ast-0.1.7/PKG-INFO
```

### Comparing `thymus_ast-0.1.6/LICENSE` & `thymus_ast-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `thymus_ast-0.1.6/README.md` & `thymus_ast-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `thymus_ast-0.1.6/thymus_ast/ios/ios.py` & `thymus_ast-0.1.7/thymus_ast/ios/ios.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,29 +86,27 @@
             current = new_node
         else:
             current = child
     current.is_accessible = True
     return current
 
 
-def step_back(node: Node, steps: int) -> Node:
+def step_back(node: Node, config: list[str], steps: int) -> Optional[Root | Node]:
     current: Node | Root = node
-    reverse: list[Node] = []
     while True:
-        if current.name == 'root':
+        if type(current) is Root:
             break
+        assert type(current) is Node
         current = current.parent
         if current.is_accessible:
-            reverse.append(current)
-    if len(reverse) == 1 and reverse[0].name == 'root':
-        return reverse[0]
-    if len(reverse) <= steps:
-        return reverse[-1]
-    offset = (steps + 1) * -1
-    return reverse[offset]
+            line = config[current.begin - 1][:-1]
+            spaces = get_spaces(line)
+            if steps > spaces:
+                return current
+    return None
 
 
 def chop_tree(node: Node) -> None:
     marked: list[int] = []
     for number, child in enumerate(node.heuristics):
         if len(child.stubs) <= 1:
             marked.append(number)
@@ -311,14 +309,15 @@
         children=[],
         heuristics=[],
         stubs=[],
         begin=0,
         end=0,
         is_accessible=True,
     )
+    root = current
     bom_symbol = '\ufeff'
     prev_line: str = ''
     step: int = 0  # step tells how deep the next section is
     final: int = 0
     if not is_promisc:
         for index in range(len(config) - 1, 0, -1):
             if config[index] == '\n':
@@ -369,15 +368,23 @@
                     current.stubs.append(c_buffer)
                     c_buffer = ''
                     c_block = False
                 else:
                     return None
             current.end = number
             temp = current
-            current = step_back(current, (prev_spaces - spaces) // step)
+            if current.name == 'root':
+                return None
+            if not spaces:
+                # We are definitely heading the root
+                current = root
+            else:
+                current = step_back(current, config, prev_spaces - step)
+            if not current:
+                return None
             if current.name == 'root':
                 last_end = temp.end
                 while temp.name != 'root':
                     if temp.is_accessible and not temp.end:
                         temp.end = last_end
                     temp = temp.parent
         else:
```

### Comparing `thymus_ast-0.1.6/thymus_ast/junos/__init__.py` & `thymus_ast-0.1.7/thymus_ast/junos/__init__.py`

 * *Files identical despite different names*

### Comparing `thymus_ast-0.1.6/thymus_ast/junos/junos.py` & `thymus_ast-0.1.7/thymus_ast/junos/junos.py`

 * *Files identical despite different names*

### Comparing `thymus_ast-0.1.6/PKG-INFO` & `thymus_ast-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thymus-ast
-Version: 0.1.6
+Version: 0.1.7
 Summary: A set of tools to build ASTs for different NOS
 Author: Igor Malyushkin
 Author-email: gmalyushkin@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

