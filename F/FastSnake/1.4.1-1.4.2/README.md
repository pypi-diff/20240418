# Comparing `tmp/fastsnake-1.4.1.tar.gz` & `tmp/fastsnake-1.4.2.tar.gz`

## Comparing `fastsnake-1.4.1.tar` & `fastsnake-1.4.2.tar`

### file list

```diff
@@ -1,36 +1,38 @@
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fastsnake-1.4.1/requirements.txt
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 fastsnake-1.4.1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/__init__.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/algorithms/binary_search.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/algorithms/knapsack.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/algorithms/lower_bound.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/algorithms/mex.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/algorithms/min_coins.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/algorithms/upper_bound.py
--rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/application/application.py
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/application/arg_parser.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/application/config.py
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/application/contest.py
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/application/test_runner.py
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/structures/b_tree.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/util/codeforces.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/util/compiler.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/conftest.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/test_algorithms/test_binary_search.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/test_algorithms/test_knapsack.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/test_algorithms/test_lower_bound.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/test_algorithms/test_mex.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/test_algorithms/test_min_coins.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/test_algorithms/test_upper_bound.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/test_codeforces_tools/test_problem_loader.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/test_codeforces_tools/sample_1949_J/0.in
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/test_codeforces_tools/sample_1949_J/0.out
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/test_codeforces_tools/sample_1949_J/1.in
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/test_codeforces_tools/sample_1949_J/1.out
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/test_compiler/sample.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/test_compiler/test_compiler.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 fastsnake-1.4.1/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 fastsnake-1.4.1/LICENSE
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 fastsnake-1.4.1/README.md
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 fastsnake-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 fastsnake-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fastsnake-1.4.2/requirements.txt
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 fastsnake-1.4.2/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/__init__.py
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/entries.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/algorithms/binary_search.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/algorithms/knapsack.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/algorithms/lower_bound.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/algorithms/mex.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/algorithms/min_coins.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/algorithms/upper_bound.py
+-rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/application/application.py
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/application/arg_parser.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/application/config.py
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/application/contest.py
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/application/runner.py
+-rw-r--r--   0        0        0     8838 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/structures/b_tree.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/util/codeforces.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/util/compiler.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/conftest.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_algorithms/test_binary_search.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_algorithms/test_knapsack.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_algorithms/test_lower_bound.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_algorithms/test_mex.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_algorithms/test_min_coins.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_algorithms/test_upper_bound.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_codeforces_tools/test_problem_loader.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_codeforces_tools/sample_1949_J/0.in
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_codeforces_tools/sample_1949_J/0.out
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_codeforces_tools/sample_1949_J/1.in
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_codeforces_tools/sample_1949_J/1.out
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_compiler/sample.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_compiler/test_compiler.py
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_structures/test_b_tree.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 fastsnake-1.4.2/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 fastsnake-1.4.2/LICENSE
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 fastsnake-1.4.2/README.md
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 fastsnake-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 fastsnake-1.4.2/PKG-INFO
```

### Comparing `fastsnake-1.4.1/.github/workflows/python-package.yml` & `fastsnake-1.4.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.1/fastsnake/algorithms/knapsack.py` & `fastsnake-1.4.2/fastsnake/algorithms/knapsack.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.1/fastsnake/algorithms/min_coins.py` & `fastsnake-1.4.2/fastsnake/algorithms/min_coins.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.1/fastsnake/application/application.py` & `fastsnake-1.4.2/fastsnake/application/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from fastsnake.application.arg_parser import main_parser
 from fastsnake.application.config import contest_config_filename
 from fastsnake.application.contest import start_contest
-from fastsnake.application.test_runner import run_test, run_test_generator
+from fastsnake.application.runner import run_test, run_test_generator
 from fastsnake.util.codeforces import *
 from fastsnake.util.compiler import compile_code
 
 import fastsnake
 import json
 import os
```

### Comparing `fastsnake-1.4.1/fastsnake/application/arg_parser.py` & `fastsnake-1.4.2/fastsnake/application/arg_parser.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.1/fastsnake/application/contest.py` & `fastsnake-1.4.2/fastsnake/application/contest.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,14 +27,27 @@
 
     for filename in os.listdir(config["solutions_namespace"]):
         os.remove(os.path.join(config["solutions_namespace"], filename))
 
     for problem in config["problems"]:
         with open(os.path.join(config["solutions_namespace"], problem.upper() + ".py"), "w") as file:
             file.write("# Solution for problem " + problem + "\n\n")
+            file.write("# from fastsnake.algorithms.something import *\n")
+            file.write("# from fastsnake.structures.something import *\n")
+            file.write("\n")
+            file.write("# Just remove the fastsnake code below if you will not use it.\n")
+            file.write("from fastsnake.entries import *\n")
+            file.write("inputi = input_int\n")
+            file.write("inputa = input_int_array\n")
+            file.write("inputm = input_int_matrix\n")
+            file.write("\n")
+            file.write("for test_case in range(int(input())):\n")
+            file.write("    n = int(input())\n")
+            file.write("    pass\n")
+            file.write("\n\n")
 
     # Create folder with Python modules for writting test case generators.
     if not os.path.exists(config["test_generators_namespace"]):
         os.mkdir(config["test_generators_namespace"])
 
     for filename in os.listdir(config["test_generators_namespace"]):
         os.remove(os.path.join(config["test_generators_namespace"], filename))
@@ -53,15 +66,15 @@
             file.write("\n\n")
             file.write("def gen_string(size: int, letters: str = string.ascii_lowercase):\n")
             file.write("    return ''.join(random.choice(letters) for _ in range(size))\n")
             file.write("\n\n")
             file.write("def gen_string_array(size: int, start: int, end: int, letters: str = string.ascii_lowercase):\n")
             file.write("    return ' '.join(gen_string(gen_int(start, end), letters) for _ in range(size))\n")
             file.write("\n\n")
-            file.write("def generate() -> \"Generator\":  # Yield any data type (it will be converted to str later)\n")
+            file.write("def generate(test_id: int) -> \"Generator\":  # Yield any data type (it will be converted to str later)\n")
             file.write("    # Sample code ...\n")
             file.write("    yield gen_int(0, 100)\n")
             file.write("    yield gen_int_array(10, 0, 100)\n")
             file.write("    yield gen_string(10, string.ascii_uppercase)\n")
             file.write("    yield gen_string_array(10, 1, 20, string.ascii_uppercase + string.ascii_lowercase)\n")
             file.write("\n\n")
             file.write("def test_output(input_: list[str], output: str) -> bool:\n")
```

### Comparing `fastsnake-1.4.1/fastsnake/application/test_runner.py` & `fastsnake-1.4.2/fastsnake/application/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,20 +100,20 @@
 
     if path not in sys.path:
         sys.path.append(path)
 
     generator = importlib.import_module(f"generator_{problem}")
 
     # Run the tests.
-    for t in range(tests):
-        input_data = [str(line) for line in generator.generate()]
+    for test_id in range(tests):
+        input_data = [str(line) for line in generator.generate(test_id)]
 
         # Create an input file.
         with NamedTemporaryFile("w", delete=False) as input_file:
-            input_file.write("\n".join(input_data))
+            input_file.write("\n".join(input_data) + "\n")
 
         # Get the absolute path for the input file.
         input_filename = os.path.abspath(input_file.name)
 
         # Copy the module, injecting a code for loading input data.
         inject = f"import sys\nsys.stdin = open(r'{input_filename}', 'r')\n\n"
 
@@ -143,17 +143,17 @@
             check = generator.test_output(input_data, result)
         except NotImplementedError:
             print("ERROR: You must implement the generator() and test_ouput() at the generator module.")
             return False
 
         # Check the output.
         if not check:
-            print(f"Failed at the generated test case!!")
+            print(f"Failed at the generated test #{test_id}!!")
             print("[Input]:")
             print("\n".join(input_data))
             print("=" * 40)
             print("[Output]:")
             print(result if result and not error else error)
             return False
         
-    print(f"SUCCESS!! Your solution was accepted at all {tests} test cases.")
+    print(f"SUCCESS!! Your solution was accepted at all {tests} generated tests.")
     return True
```

### Comparing `fastsnake-1.4.1/fastsnake/structures/b_tree.py` & `fastsnake-1.4.2/fastsnake/structures/b_tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Tuple
+from typing import Any, Optional, Tuple
 
 
 class BTreeNode:
 	def __init__(self, leaf = False):
 		self.leaf = leaf
 		self.keys = []
 		self.child = []
@@ -11,35 +11,36 @@
 class BTree:
 	"""
 	Example:
 	
 	B = BTree(3)
 	
 	for i in range(10):
-		B.insert((i, 2*i))
+		B.insert((i, 2*i))  # Insert (key, value [any data type])
 		
-	B.print_tree(B.root)
-	print("\n")
+	B.print_tree(B.root, "\n")
 	
 	B.delete((3,), B.root)
 	
-	if B.search(5) != None:
-		(x, i) = B.search(5)
+	result = B.search(5)
+
+	if result is not None:
+		parent_node, index = result
+		print("Found!")
 	else:
-		print("Element not found!")
-		
-	print("\n")
-	B.print_tree(B.root)
+		print("Not found!")
+
+	B.print_tree("\n", B.root)
 	"""
 	def __init__(self, minimum_degree: int):
 		"""
-		:param minimum_degree: Order of B Tree
+		:param minimum_degree: Order of B Tree (must be greater than or equal to 2)
 		"""
 		self.root = BTreeNode(True)
-		self.t = minimum_degree
+		self.t = max(2, minimum_degree)
 
 	def print_tree(self, node: Optional[BTreeNode] = None, l = 0) -> None:
 		"""
 		Print each level of the tree.
 		"""
 		if node is None:
 			node = self.root
@@ -55,15 +56,15 @@
 		l += 1
 		
 		if len(x.child) > 0:
 			for i in x.child:
 				self.print_tree(i, l)
 	
 
-	def search(self, key, position: Optional[BTreeNode] = None) -> Optional[Tuple[BTreeNode, int]]:
+	def search(self, key: int, position: Optional[BTreeNode] = None) -> Optional[Tuple[BTreeNode, int]]:
 		"""
 		Search for a key at a position.
         
 		:param key: Key to be searched
 		:param position: Node to search from
 		
 		If 'position' is not specified, then search occurs from root.
@@ -76,24 +77,24 @@
 		
 		if x != None:
 			i = 0
 			while i < len(x.keys) and k > x.keys[i][0]:
 				i += 1
 			if i < len(x.keys) and k == x.keys[i][0]:
 				return (x, i)
-			elif x.leaf:
+			elif x.leaf or i >= len(x.child):
 				return None
 			else:
 				#Search in children
 				return self.search(k, x.child[i])
 		else:
 			#Search entire tree as node not provided
 			return self.search(k, self.root)
 
-	def insert(self, key: Tuple) -> None:
+	def insert(self, key: Tuple[int, Any]) -> None:
 		"""
 		Calls helper functions to insert a key in the B-Tree.
 		
 		:param key: Key to be inserted. It must be a tuple (key, value)
 		"""
 		k = key
 		root = self.root
@@ -158,15 +159,15 @@
 		z.keys = y.keys[t : (2 * t) - 1]
 		y.keys = y.keys[0 : t - 1]
 		
 		if not y.leaf:
 			z.child = y.child[t : 2 * t]
 			y.child = y.child[0 : t - 1]
 
-	def delete(self, key, position: Optional[BTreeNode] = None) -> None:
+	def delete(self, key: Tuple[int, Any], position: Optional[BTreeNode] = None) -> None:
 		"""
 		Calls helper functions to delete the key after searching from node 'position'
 
 		:param key: Key to be deleted
 		:param position: Node, according to whose relative position, helper functions are called
 		"""
 		if position is None:
```

### Comparing `fastsnake-1.4.1/fastsnake/util/codeforces.py` & `fastsnake-1.4.2/fastsnake/util/codeforces.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.1/fastsnake/util/compiler.py` & `fastsnake-1.4.2/fastsnake/util/compiler.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,19 +2,25 @@
 
 path = os.path.join(os.path.dirname(__file__), "..")
 
 
 def compile_code(input_filename: str, output_filename: str) -> None:
     
     string = ""
+
+    valid_imports = [
+        "from fastsnake.algorithms",
+        "from fastsnake.structures",
+        "from fastsnake.entries"
+    ]
     
     with open(input_filename) as file:
         for line in file:
             # Check if the line contains an import statement for algorithms or structures.
-            if not line.startswith("from fastsnake.algorithms") and not line.startswith("from fastsnake.structures"):
+            if not any([line.startswith(x) for x in valid_imports]):
                 string += line
                 continue
 
             # Clean the line and get the module name.
             line = line.replace("\n", "").replace(" ", "")
             importing = line.replace("from", "").replace("import*", "").split(".")[1:]
```

### Comparing `fastsnake-1.4.1/tests/test_algorithms/test_binary_search.py` & `fastsnake-1.4.2/tests/test_algorithms/test_binary_search.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.1/tests/test_algorithms/test_knapsack.py` & `fastsnake-1.4.2/tests/test_algorithms/test_knapsack.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.1/tests/test_algorithms/test_lower_bound.py` & `fastsnake-1.4.2/tests/test_algorithms/test_lower_bound.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.1/tests/test_algorithms/test_mex.py` & `fastsnake-1.4.2/tests/test_algorithms/test_mex.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.1/tests/test_algorithms/test_upper_bound.py` & `fastsnake-1.4.2/tests/test_algorithms/test_upper_bound.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.1/tests/test_codeforces_tools/test_problem_loader.py` & `fastsnake-1.4.2/tests/test_codeforces_tools/test_problem_loader.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.1/tests/test_compiler/test_compiler.py` & `fastsnake-1.4.2/tests/test_compiler/test_compiler.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.1/.gitignore` & `fastsnake-1.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.1/LICENSE` & `fastsnake-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.1/README.md` & `fastsnake-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.1/pyproject.toml` & `fastsnake-1.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.1/PKG-INFO` & `fastsnake-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: FastSnake
-Version: 1.4.1
+Version: 1.4.2
 Summary: A helper for contests in Python 3
 Project-URL: Homepage, https://github.com/JeanExtreme002/FastSnake
 Author-email: Jean Loui Bernard Silva de Jesus <jeanextreme002@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: algorithms,codeforces,contest
 Classifier: Intended Audience :: Developers
```

