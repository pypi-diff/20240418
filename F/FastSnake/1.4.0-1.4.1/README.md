# Comparing `tmp/fastsnake-1.4.0.tar.gz` & `tmp/fastsnake-1.4.1.tar.gz`

## Comparing `fastsnake-1.4.0.tar` & `fastsnake-1.4.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fastsnake-1.4.0/requirements.txt
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 fastsnake-1.4.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/__init__.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/algorithms/binary_search.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/algorithms/knapsack.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/algorithms/lower_bound.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/algorithms/mex.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/algorithms/min_coins.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/algorithms/upper_bound.py
--rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/application/application.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/application/arg_parser.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/application/config.py
--rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/application/contest.py
--rw-r--r--   0        0        0     5328 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/application/test_runner.py
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/structures/b_tree.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/util/codeforces.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/util/compiler.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/conftest.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/test_algorithms/test_binary_search.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/test_algorithms/test_knapsack.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/test_algorithms/test_lower_bound.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/test_algorithms/test_mex.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/test_algorithms/test_min_coins.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/test_algorithms/test_upper_bound.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/test_codeforces_tools/test_problem_loader.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/test_codeforces_tools/sample_1949_J/0.in
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/test_codeforces_tools/sample_1949_J/0.out
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/test_codeforces_tools/sample_1949_J/1.in
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/test_codeforces_tools/sample_1949_J/1.out
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/test_compiler/sample.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/test_compiler/test_compiler.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 fastsnake-1.4.0/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 fastsnake-1.4.0/LICENSE
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 fastsnake-1.4.0/README.md
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 fastsnake-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 fastsnake-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fastsnake-1.4.1/requirements.txt
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 fastsnake-1.4.1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/__init__.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/algorithms/binary_search.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/algorithms/knapsack.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/algorithms/lower_bound.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/algorithms/mex.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/algorithms/min_coins.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/algorithms/upper_bound.py
+-rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/application/application.py
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/application/arg_parser.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/application/config.py
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/application/contest.py
+-rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/application/test_runner.py
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/structures/b_tree.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/util/codeforces.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 fastsnake-1.4.1/fastsnake/util/compiler.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/conftest.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/test_algorithms/test_binary_search.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/test_algorithms/test_knapsack.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/test_algorithms/test_lower_bound.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/test_algorithms/test_mex.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/test_algorithms/test_min_coins.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/test_algorithms/test_upper_bound.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/test_codeforces_tools/test_problem_loader.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/test_codeforces_tools/sample_1949_J/0.in
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/test_codeforces_tools/sample_1949_J/0.out
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/test_codeforces_tools/sample_1949_J/1.in
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/test_codeforces_tools/sample_1949_J/1.out
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/test_compiler/sample.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastsnake-1.4.1/tests/test_compiler/test_compiler.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 fastsnake-1.4.1/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 fastsnake-1.4.1/LICENSE
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 fastsnake-1.4.1/README.md
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 fastsnake-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 fastsnake-1.4.1/PKG-INFO
```

### Comparing `fastsnake-1.4.0/.github/workflows/python-package.yml` & `fastsnake-1.4.1/.github/workflows/python-package.yml`

 * *Files 2% similar despite different names*

```diff
@@ -29,8 +29,8 @@
         python -m pip install --upgrade pip
         pip install -r requirements.txt
     - name: Test with pytest
       run: |
         pytest tests -vv -s
     - name: Install package
       run: |
-        pip install FlightRadar24
+        pip install FastSnake
```

### Comparing `fastsnake-1.4.0/fastsnake/algorithms/knapsack.py` & `fastsnake-1.4.1/fastsnake/algorithms/knapsack.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.0/fastsnake/algorithms/min_coins.py` & `fastsnake-1.4.1/fastsnake/algorithms/min_coins.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.0/fastsnake/application/application.py` & `fastsnake-1.4.1/fastsnake/application/application.py`

 * *Files 19% similar despite different names*

```diff
@@ -102,14 +102,49 @@
     if not os.path.exists(directory):
         os.mkdir(directory)
 
     problems = load_codeforces_problems(gym_id, test_cases, namespace="gym")
     start_contest(solutions, test_cases, test_generators, gym_id, problems)
 
 
+def start_custom_contest(n_problems: int) -> None:
+    """
+    Initialize a custom contest.
+    """
+    directory = "custom_contest"
+    contest_id = "x"
+
+    solutions = os.path.join(directory, "solutions")
+    test_cases = os.path.join(directory, "test_cases")
+    test_generators = os.path.join(directory, "test_generators")
+
+    if not os.path.exists(directory):
+        os.mkdir(directory)
+
+    if not os.path.exists(test_cases):
+        os.mkdir(test_cases)
+
+    problems = [chr(ord("A")+i) for i in range(min(n_problems, 26))]
+
+    for problem in problems:
+        filename = f"contest_{contest_id}_problem_{problem}_0.in"
+        filename = os.path.join(test_cases, filename)
+
+        with open(filename, "w") as file:
+            file.write("\n")
+
+        filename = f"contest_{contest_id}_problem_{problem}_0.out"
+        filename = os.path.join(test_cases, filename)
+
+        with open(filename, "w") as file:
+            file.write("\n")
+
+    start_contest(solutions, test_cases, test_generators, contest_id, problems)
+
+
 def main() -> None:
     """
     Main function.
     """
     # Print the version of the project.
     if args.version:
         print(fastsnake.__version__)
@@ -133,14 +168,19 @@
             if result and args.test_and_compile: 
                 compile(args.problem, problem=True)
         
         # Compile a fastsnake solution.
         elif args.command == "compile":
             compile(args.filename)
 
+        # Start a custom contest.
+        elif args.command == "start-custom-contest":
+            start_custom_contest(args.n_problems)
+
+
         # Tools for Codeforces.
         elif args.command == "codeforces":
             if args.load:
                 try: 
                     contest_id, problem = int(args.load[0]), args.load[1]
                 except: 
                     contest_id, problem = int(args.load[1]), args.load[0]
```

### Comparing `fastsnake-1.4.0/fastsnake/application/arg_parser.py` & `fastsnake-1.4.1/fastsnake/application/arg_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 test_parser.add_argument("-c", "--compile", action="store_true", dest="test_and_compile", help="Test and compile the solution")
 test_parser.add_argument("-g", "--generator", type=int, metavar="n_tests", dest="generator", help="Use generator module to test the solution")
 
 # Compiling Solutions.
 compile_parser = command_parser.add_parser("compile", help="Compile a python fastsnake solution")
 compile_parser.add_argument("filename", type=str, help="Python module")
 
+# Custom Contest.
+custom_contest_parser = command_parser.add_parser("start-custom-contest", help="Start a custom contest")
+custom_contest_parser.add_argument("n_problems", type=int, help="Amount of problems")
+
 # Tools for Contest Platforms.
 codeforces_parser = command_parser.add_parser("codeforces", help="Tools for Codeforces platform")
 codeforces_parser.add_argument("--load-all", metavar="contest_id", type=int, dest="load_all", help="Download test cases from every problem of a contest")
 codeforces_parser.add_argument("--load", metavar=("contest_id", "problem"), type=str, nargs=2, dest="load", help="Download test cases from a problem")
 codeforces_parser.add_argument("--save", metavar="directory", type=str, default="codeforces", dest="save", help="Directory for saving downloaded files")
 codeforces_parser.add_argument("-sc", "--start-contest", metavar="contest_id", type=int, dest="start_contest", help="Initialize a Codeforces contest")
 codeforces_parser.add_argument("-sg", "--start-gym", metavar="gym_id", type=int, dest="start_gym", help="Initialize a Codeforces gym")
```

### Comparing `fastsnake-1.4.0/fastsnake/application/contest.py` & `fastsnake-1.4.1/fastsnake/application/contest.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,14 @@
             file.write("def generate() -> \"Generator\":  # Yield any data type (it will be converted to str later)\n")
             file.write("    # Sample code ...\n")
             file.write("    yield gen_int(0, 100)\n")
             file.write("    yield gen_int_array(10, 0, 100)\n")
             file.write("    yield gen_string(10, string.ascii_uppercase)\n")
             file.write("    yield gen_string_array(10, 1, 20, string.ascii_uppercase + string.ascii_lowercase)\n")
             file.write("\n\n")
-            file.write("def test_output(input_: str, output: str) -> bool:\n")
+            file.write("def test_output(input_: list[str], output: str) -> bool:\n")
             file.write("    raise NotImplementedError()")
             file.write("\n")
 
     # Create config file.
     with open(contest_config_filename, "w") as file:
         file.write(json.dumps(config))
```

### Comparing `fastsnake-1.4.0/fastsnake/application/test_runner.py` & `fastsnake-1.4.1/fastsnake/application/test_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,22 +101,19 @@
     if path not in sys.path:
         sys.path.append(path)
 
     generator = importlib.import_module(f"generator_{problem}")
 
     # Run the tests.
     for t in range(tests):
-        input_data = ""
-        
-        for line in generator.generate():
-            input_data += str(line) + "\n"
+        input_data = [str(line) for line in generator.generate()]
 
         # Create an input file.
         with NamedTemporaryFile("w", delete=False) as input_file:
-            input_file.write(input_data)
+            input_file.write("\n".join(input_data))
 
         # Get the absolute path for the input file.
         input_filename = os.path.abspath(input_file.name)
 
         # Copy the module, injecting a code for loading input data.
         inject = f"import sys\nsys.stdin = open(r'{input_filename}', 'r')\n\n"
 
@@ -148,15 +145,15 @@
             print("ERROR: You must implement the generator() and test_ouput() at the generator module.")
             return False
 
         # Check the output.
         if not check:
             print(f"Failed at the generated test case!!")
             print("[Input]:")
-            print(input_data)
+            print("\n".join(input_data))
             print("=" * 40)
             print("[Output]:")
             print(result if result and not error else error)
             return False
         
     print(f"SUCCESS!! Your solution was accepted at all {tests} test cases.")
     return True
```

### Comparing `fastsnake-1.4.0/fastsnake/structures/b_tree.py` & `fastsnake-1.4.1/fastsnake/structures/b_tree.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.0/fastsnake/util/codeforces.py` & `fastsnake-1.4.1/fastsnake/util/codeforces.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.0/fastsnake/util/compiler.py` & `fastsnake-1.4.1/fastsnake/util/compiler.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.0/tests/test_algorithms/test_binary_search.py` & `fastsnake-1.4.1/tests/test_algorithms/test_binary_search.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.0/tests/test_algorithms/test_knapsack.py` & `fastsnake-1.4.1/tests/test_algorithms/test_knapsack.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.0/tests/test_algorithms/test_lower_bound.py` & `fastsnake-1.4.1/tests/test_algorithms/test_lower_bound.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.0/tests/test_algorithms/test_mex.py` & `fastsnake-1.4.1/tests/test_algorithms/test_mex.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.0/tests/test_algorithms/test_upper_bound.py` & `fastsnake-1.4.1/tests/test_algorithms/test_upper_bound.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.0/tests/test_codeforces_tools/test_problem_loader.py` & `fastsnake-1.4.1/tests/test_codeforces_tools/test_problem_loader.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.0/tests/test_compiler/test_compiler.py` & `fastsnake-1.4.1/tests/test_compiler/test_compiler.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.0/.gitignore` & `fastsnake-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.0/LICENSE` & `fastsnake-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.0/README.md` & `fastsnake-1.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # FastSnake
 
 [![Python Package](https://github.com/JeanExtreme002/FastSnake/workflows/Python%20Package/badge.svg)](https://github.com/JeanExtreme002/FastSnake/actions)
 [![Pypi](https://img.shields.io/pypi/v/FastSnake?logo=pypi)](https://pypi.org/project/FastSnake/)
 [![License](https://img.shields.io/pypi/l/FastSnake)](https://github.com/JeanExtreme002/FastSnake)
-[![Python Version](https://img.shields.io/badge/python-3.7+-8A2BE2)](https://pypi.org/project/FastSnake/)
+[![Platforms](https://img.shields.io/badge/platforms-Windows%20%7C%20Linux-8A2BE2)](https://pypi.org/project/FastSnake/)
+[![Python Version](https://img.shields.io/badge/python-3.7+-yellow)](https://pypi.org/project/FastSnake/)
 
 Tired of having to copy-paste your library code into every solution you write? FastSnake is a command-line tool that allows you to easily create, expand, run and test Python solutions for competitive programming problems.
 
 This project provides useful CLI tools for competitive programming, such as algorithms and data structures, and tools for Codeforces. But you will have to write your own code and library for the problems you want to solve.
 
 ## Installing FastSnake:
 ```
```

### Comparing `fastsnake-1.4.0/pyproject.toml` & `fastsnake-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.0/PKG-INFO` & `fastsnake-1.4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: FastSnake
-Version: 1.4.0
+Version: 1.4.1
 Summary: A helper for contests in Python 3
 Project-URL: Homepage, https://github.com/JeanExtreme002/FastSnake
 Author-email: Jean Loui Bernard Silva de Jesus <jeanextreme002@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: algorithms,codeforces,contest
 Classifier: Intended Audience :: Developers
@@ -17,15 +17,16 @@
 Description-Content-Type: text/markdown
 
 # FastSnake
 
 [![Python Package](https://github.com/JeanExtreme002/FastSnake/workflows/Python%20Package/badge.svg)](https://github.com/JeanExtreme002/FastSnake/actions)
 [![Pypi](https://img.shields.io/pypi/v/FastSnake?logo=pypi)](https://pypi.org/project/FastSnake/)
 [![License](https://img.shields.io/pypi/l/FastSnake)](https://github.com/JeanExtreme002/FastSnake)
-[![Python Version](https://img.shields.io/badge/python-3.7+-8A2BE2)](https://pypi.org/project/FastSnake/)
+[![Platforms](https://img.shields.io/badge/platforms-Windows%20%7C%20Linux-8A2BE2)](https://pypi.org/project/FastSnake/)
+[![Python Version](https://img.shields.io/badge/python-3.7+-yellow)](https://pypi.org/project/FastSnake/)
 
 Tired of having to copy-paste your library code into every solution you write? FastSnake is a command-line tool that allows you to easily create, expand, run and test Python solutions for competitive programming problems.
 
 This project provides useful CLI tools for competitive programming, such as algorithms and data structures, and tools for Codeforces. But you will have to write your own code and library for the problems you want to solve.
 
 ## Installing FastSnake:
 ```
```

