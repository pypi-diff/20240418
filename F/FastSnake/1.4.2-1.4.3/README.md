# Comparing `tmp/fastsnake-1.4.2.tar.gz` & `tmp/fastsnake-1.4.3.tar.gz`

## Comparing `fastsnake-1.4.2.tar` & `fastsnake-1.4.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fastsnake-1.4.2/requirements.txt
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 fastsnake-1.4.2/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/__init__.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/entries.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/algorithms/binary_search.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/algorithms/knapsack.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/algorithms/lower_bound.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/algorithms/mex.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/algorithms/min_coins.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/algorithms/upper_bound.py
--rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/application/application.py
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/application/arg_parser.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/application/config.py
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/application/contest.py
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/application/runner.py
--rw-r--r--   0        0        0     8838 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/structures/b_tree.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/util/codeforces.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 fastsnake-1.4.2/fastsnake/util/compiler.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/conftest.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_algorithms/test_binary_search.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_algorithms/test_knapsack.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_algorithms/test_lower_bound.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_algorithms/test_mex.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_algorithms/test_min_coins.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_algorithms/test_upper_bound.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_codeforces_tools/test_problem_loader.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_codeforces_tools/sample_1949_J/0.in
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_codeforces_tools/sample_1949_J/0.out
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_codeforces_tools/sample_1949_J/1.in
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_codeforces_tools/sample_1949_J/1.out
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_compiler/sample.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_compiler/test_compiler.py
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 fastsnake-1.4.2/tests/test_structures/test_b_tree.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 fastsnake-1.4.2/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 fastsnake-1.4.2/LICENSE
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 fastsnake-1.4.2/README.md
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 fastsnake-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 fastsnake-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fastsnake-1.4.3/requirements.txt
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 fastsnake-1.4.3/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 fastsnake-1.4.3/fastsnake/__init__.py
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 fastsnake-1.4.3/fastsnake/entries.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 fastsnake-1.4.3/fastsnake/algorithms/binary_search.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 fastsnake-1.4.3/fastsnake/algorithms/knapsack.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 fastsnake-1.4.3/fastsnake/algorithms/lower_bound.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fastsnake-1.4.3/fastsnake/algorithms/mex.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 fastsnake-1.4.3/fastsnake/algorithms/min_coins.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 fastsnake-1.4.3/fastsnake/algorithms/upper_bound.py
+-rw-r--r--   0        0        0     6641 2020-02-02 00:00:00.000000 fastsnake-1.4.3/fastsnake/application/application.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 fastsnake-1.4.3/fastsnake/application/arg_parser.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fastsnake-1.4.3/fastsnake/application/config.py
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 fastsnake-1.4.3/fastsnake/application/contest.py
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 fastsnake-1.4.3/fastsnake/application/runner.py
+-rw-r--r--   0        0        0     8838 2020-02-02 00:00:00.000000 fastsnake-1.4.3/fastsnake/structures/b_tree.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 fastsnake-1.4.3/fastsnake/util/codeforces.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 fastsnake-1.4.3/fastsnake/util/compiler.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastsnake-1.4.3/tests/conftest.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fastsnake-1.4.3/tests/test_algorithms/test_binary_search.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 fastsnake-1.4.3/tests/test_algorithms/test_knapsack.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.4.3/tests/test_algorithms/test_lower_bound.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fastsnake-1.4.3/tests/test_algorithms/test_mex.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fastsnake-1.4.3/tests/test_algorithms/test_min_coins.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.4.3/tests/test_algorithms/test_upper_bound.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 fastsnake-1.4.3/tests/test_codeforces_tools/test_problem_loader.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 fastsnake-1.4.3/tests/test_codeforces_tools/sample_1949_J/0.in
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastsnake-1.4.3/tests/test_codeforces_tools/sample_1949_J/0.out
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fastsnake-1.4.3/tests/test_codeforces_tools/sample_1949_J/1.in
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fastsnake-1.4.3/tests/test_codeforces_tools/sample_1949_J/1.out
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 fastsnake-1.4.3/tests/test_compiler/sample.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastsnake-1.4.3/tests/test_compiler/test_compiler.py
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 fastsnake-1.4.3/tests/test_structures/test_b_tree.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 fastsnake-1.4.3/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 fastsnake-1.4.3/LICENSE
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 fastsnake-1.4.3/README.md
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 fastsnake-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 fastsnake-1.4.3/PKG-INFO
```

### Comparing `fastsnake-1.4.2/.github/workflows/python-package.yml` & `fastsnake-1.4.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.2/fastsnake/entries.py` & `fastsnake-1.4.3/fastsnake/entries.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.2/fastsnake/algorithms/knapsack.py` & `fastsnake-1.4.3/fastsnake/algorithms/knapsack.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.2/fastsnake/algorithms/min_coins.py` & `fastsnake-1.4.3/fastsnake/algorithms/min_coins.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.2/fastsnake/application/application.py` & `fastsnake-1.4.3/fastsnake/application/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,18 +141,24 @@
     start_contest(solutions, test_cases, test_generators, contest_id, problems)
 
 
 def main() -> None:
     """
     Main function.
     """
-    # Print the version of the project.
+    # Print the information of the project.
     if args.version:
         print(fastsnake.__version__)
 
+    elif args.author:
+        print(fastsnake.__author__)
+
+    elif args.credits:
+        print(fastsnake.__credits__)
+
     # List algorithms and structures.
     elif args.list:
         for name in os.listdir(os.path.join(project_path, args.list)):
             if "__" not in name:
                 print(f"- {name.replace('.py', '').replace('_', ' ').title()}")
 
     # CLI Commands.
```

### Comparing `fastsnake-1.4.2/fastsnake/application/arg_parser.py` & `fastsnake-1.4.3/fastsnake/application/arg_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from argparse import ArgumentParser
 
 
 main_parser = ArgumentParser(prog="FastSnake", description="CLI Tools for Competitive Programming")
 
 main_parser.add_argument("-l", "--list", type=str, choices=["algorithms", "structures"], help="List algorithm or structure modules")
 main_parser.add_argument("-v", "--version", action="store_true", help="Print the fastsnake's version")
+main_parser.add_argument("--author", action="store_true", help="Print the author name")
+main_parser.add_argument("--credits", action="store_true", help="Print the credits of the project")
 
 command_parser = main_parser.add_subparsers(title="Fastsnake CLI Commands", dest="command")
 
 # Testing Solutions.
 test_parser = command_parser.add_parser("test", help="Test a solution for a contest problem")
 test_parser.add_argument("problem", type=str, help="Problem of the contest")
 test_parser.add_argument("-c", "--compile", action="store_true", dest="test_and_compile", help="Test and compile the solution")
```

### Comparing `fastsnake-1.4.2/fastsnake/application/contest.py` & `fastsnake-1.4.3/fastsnake/application/contest.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.2/fastsnake/application/runner.py` & `fastsnake-1.4.3/fastsnake/application/runner.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.2/fastsnake/structures/b_tree.py` & `fastsnake-1.4.3/fastsnake/structures/b_tree.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.2/fastsnake/util/codeforces.py` & `fastsnake-1.4.3/fastsnake/util/codeforces.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.2/fastsnake/util/compiler.py` & `fastsnake-1.4.3/fastsnake/util/compiler.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.2/tests/test_algorithms/test_binary_search.py` & `fastsnake-1.4.3/tests/test_algorithms/test_binary_search.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.2/tests/test_algorithms/test_knapsack.py` & `fastsnake-1.4.3/tests/test_algorithms/test_knapsack.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.2/tests/test_algorithms/test_lower_bound.py` & `fastsnake-1.4.3/tests/test_algorithms/test_lower_bound.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.2/tests/test_algorithms/test_mex.py` & `fastsnake-1.4.3/tests/test_algorithms/test_mex.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.2/tests/test_algorithms/test_upper_bound.py` & `fastsnake-1.4.3/tests/test_algorithms/test_upper_bound.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.2/tests/test_codeforces_tools/test_problem_loader.py` & `fastsnake-1.4.3/tests/test_codeforces_tools/test_problem_loader.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.2/tests/test_compiler/test_compiler.py` & `fastsnake-1.4.3/tests/test_compiler/test_compiler.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.2/tests/test_structures/test_b_tree.py` & `fastsnake-1.4.3/tests/test_structures/test_b_tree.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.2/.gitignore` & `fastsnake-1.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.2/LICENSE` & `fastsnake-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.2/README.md` & `fastsnake-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.2/pyproject.toml` & `fastsnake-1.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.2/PKG-INFO` & `fastsnake-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: FastSnake
-Version: 1.4.2
+Version: 1.4.3
 Summary: A helper for contests in Python 3
 Project-URL: Homepage, https://github.com/JeanExtreme002/FastSnake
 Author-email: Jean Loui Bernard Silva de Jesus <jeanextreme002@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: algorithms,codeforces,contest
 Classifier: Intended Audience :: Developers
```

