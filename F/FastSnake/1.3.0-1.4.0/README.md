# Comparing `tmp/fastsnake-1.3.0.tar.gz` & `tmp/fastsnake-1.4.0.tar.gz`

## Comparing `fastsnake-1.3.0.tar` & `fastsnake-1.4.0.tar`

### file list

```diff
@@ -1,32 +1,36 @@
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fastsnake-1.3.0/requirements.txt
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 fastsnake-1.3.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 fastsnake-1.3.0/fastsnake/__init__.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 fastsnake-1.3.0/fastsnake/algorithms/binary_search.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 fastsnake-1.3.0/fastsnake/algorithms/knapsack.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 fastsnake-1.3.0/fastsnake/algorithms/lower_bound.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fastsnake-1.3.0/fastsnake/algorithms/mex.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 fastsnake-1.3.0/fastsnake/algorithms/min_coins.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 fastsnake-1.3.0/fastsnake/algorithms/upper_bound.py
--rw-r--r--   0        0        0     7598 2020-02-02 00:00:00.000000 fastsnake-1.3.0/fastsnake/application/application.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 fastsnake-1.3.0/fastsnake/application/arg_parser.py
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 fastsnake-1.3.0/fastsnake/util/codeforces.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 fastsnake-1.3.0/fastsnake/util/compiler.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastsnake-1.3.0/tests/conftest.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fastsnake-1.3.0/tests/test_algorithms/test_binary_search.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 fastsnake-1.3.0/tests/test_algorithms/test_knapsack.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.3.0/tests/test_algorithms/test_lower_bound.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fastsnake-1.3.0/tests/test_algorithms/test_mex.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fastsnake-1.3.0/tests/test_algorithms/test_min_coins.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.3.0/tests/test_algorithms/test_upper_bound.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 fastsnake-1.3.0/tests/test_codeforces_tools/test_problem_loader.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 fastsnake-1.3.0/tests/test_codeforces_tools/sample_1949_J/0.in
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastsnake-1.3.0/tests/test_codeforces_tools/sample_1949_J/0.out
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fastsnake-1.3.0/tests/test_codeforces_tools/sample_1949_J/1.in
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fastsnake-1.3.0/tests/test_codeforces_tools/sample_1949_J/1.out
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 fastsnake-1.3.0/tests/test_compiler/sample.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastsnake-1.3.0/tests/test_compiler/test_compiler.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 fastsnake-1.3.0/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 fastsnake-1.3.0/LICENSE
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 fastsnake-1.3.0/README.md
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 fastsnake-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 fastsnake-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fastsnake-1.4.0/requirements.txt
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 fastsnake-1.4.0/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/__init__.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/algorithms/binary_search.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/algorithms/knapsack.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/algorithms/lower_bound.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/algorithms/mex.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/algorithms/min_coins.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/algorithms/upper_bound.py
+-rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/application/application.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/application/arg_parser.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/application/config.py
+-rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/application/contest.py
+-rw-r--r--   0        0        0     5328 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/application/test_runner.py
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/structures/b_tree.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/util/codeforces.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 fastsnake-1.4.0/fastsnake/util/compiler.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/conftest.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/test_algorithms/test_binary_search.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/test_algorithms/test_knapsack.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/test_algorithms/test_lower_bound.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/test_algorithms/test_mex.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/test_algorithms/test_min_coins.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/test_algorithms/test_upper_bound.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/test_codeforces_tools/test_problem_loader.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/test_codeforces_tools/sample_1949_J/0.in
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/test_codeforces_tools/sample_1949_J/0.out
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/test_codeforces_tools/sample_1949_J/1.in
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/test_codeforces_tools/sample_1949_J/1.out
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/test_compiler/sample.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastsnake-1.4.0/tests/test_compiler/test_compiler.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 fastsnake-1.4.0/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 fastsnake-1.4.0/LICENSE
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 fastsnake-1.4.0/README.md
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 fastsnake-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 fastsnake-1.4.0/PKG-INFO
```

### Comparing `fastsnake-1.3.0/.github/workflows/python-package.yml` & `fastsnake-1.4.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `fastsnake-1.3.0/fastsnake/algorithms/knapsack.py` & `fastsnake-1.4.0/fastsnake/algorithms/knapsack.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.3.0/fastsnake/algorithms/min_coins.py` & `fastsnake-1.4.0/fastsnake/algorithms/min_coins.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.3.0/fastsnake/application/arg_parser.py` & `fastsnake-1.4.0/fastsnake/application/arg_parser.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 from argparse import ArgumentParser
 
-main_parser = ArgumentParser(
-    prog="FastSnake",
-    description="CLI Tools for Competitive Programming",
-)
-
-main_parser.add_argument("-c", "--compile", type=str, metavar="filename", default="", help="Compile a python fastsnake solution")
-main_parser.add_argument("-t", "--test", metavar="problem", type=str, help="Test the solution for a problem of the contest")
-main_parser.add_argument("-tc", metavar="problem", type=str, dest="test_and_compile", help="Test and compile the solution for a problem of the contest")
+
+main_parser = ArgumentParser(prog="FastSnake", description="CLI Tools for Competitive Programming")
+
 main_parser.add_argument("-l", "--list", type=str, choices=["algorithms", "structures"], help="List algorithm or structure modules")
 main_parser.add_argument("-v", "--version", action="store_true", help="Print the fastsnake's version")
 
-contest_parser = main_parser.add_subparsers(title="Contest Platforms", dest="contest")
+command_parser = main_parser.add_subparsers(title="Fastsnake CLI Commands", dest="command")
+
+# Testing Solutions.
+test_parser = command_parser.add_parser("test", help="Test a solution for a contest problem")
+test_parser.add_argument("problem", type=str, help="Problem of the contest")
+test_parser.add_argument("-c", "--compile", action="store_true", dest="test_and_compile", help="Test and compile the solution")
+test_parser.add_argument("-g", "--generator", type=int, metavar="n_tests", dest="generator", help="Use generator module to test the solution")
+
+# Compiling Solutions.
+compile_parser = command_parser.add_parser("compile", help="Compile a python fastsnake solution")
+compile_parser.add_argument("filename", type=str, help="Python module")
 
-codeforces_parser = contest_parser.add_parser("codeforces", help="Tools for Codeforces")
+# Tools for Contest Platforms.
+codeforces_parser = command_parser.add_parser("codeforces", help="Tools for Codeforces platform")
 codeforces_parser.add_argument("--load-all", metavar="contest_id", type=int, dest="load_all", help="Download test cases from every problem of a contest")
 codeforces_parser.add_argument("--load", metavar=("contest_id", "problem"), type=str, nargs=2, dest="load", help="Download test cases from a problem")
 codeforces_parser.add_argument("--save", metavar="directory", type=str, default="codeforces", dest="save", help="Directory for saving downloaded files")
 codeforces_parser.add_argument("-sc", "--start-contest", metavar="contest_id", type=int, dest="start_contest", help="Initialize a Codeforces contest")
+codeforces_parser.add_argument("-sg", "--start-gym", metavar="gym_id", type=int, dest="start_gym", help="Initialize a Codeforces gym")
```

### Comparing `fastsnake-1.3.0/fastsnake/util/codeforces.py` & `fastsnake-1.4.0/fastsnake/util/codeforces.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from bs4 import BeautifulSoup
 from typing import List, Tuple
 
 import os
 import requests
 
+
 headers = {
     "Sec-Ch-Ua": "\"Google Chrome\";v=\"123\", \"Not:A-Brand\";v=\"8\", \"Chromium\";v=\"123\"",
     "Sec-Ch-Ua-Arch": "\"x86\"",
     "Sec-Ch-Ua-Bitness": "\"64\"",
     "Sec-Ch-Ua-Full-Version": "\"123.0.6312.123\"",
     "Sec-Ch-Ua-Full-Version-List": "\"Google Chrome\";v=\"123.0.6312.123\", \"Not:A-Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"123.0.6312.123\"",
     "Sec-Ch-Ua-Mobile": "?0",
@@ -15,46 +16,66 @@
     "Sec-Ch-Ua-Platform": "\"Windows\"",
     "Sec-Ch-Ua-Platform-Version": "\"10.0.0\"",
     "Upgrade-Insecure-Requests": "1",
     "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36"
 }
 
 
-def get_contest_problems(contest_id: int) -> List[str]:
-    url = f"https://codeforces.com/contest/{contest_id}"
+def get_problems(id_: int, namespace: str = "contest") -> List[str]:
+    url = f"https://codeforces.com/{namespace}/{id_}"
 
     response = requests.get(url, headers=headers)
+
+    if response.status_code >= 300:
+        raise ValueError(f"{namespace.capitalize()} not found")
+
     problems = []
 
     soup = BeautifulSoup(response.content, "html.parser")
 
     table = soup.find("table", class_="problems")
 
+    if not table:
+        raise ValueError(f"{namespace.capitalize()} not found")
+
     for problem in table.find_all("tr")[1:]:
 
         problem = problem.find("td").find("a")
         data = problem.text.strip().strip("\n")
 
         problems.append(data)
 
     return problems
 
 
-def get_contest_problem_test_cases(contest_id: int, problem: str) -> Tuple[List[str], List[str]]:
-    url = f"https://codeforces.com/contest/{contest_id}/problem/{problem}"
+def get_problem_test_cases(id_: int, problem: str, namespace: str = "contest") -> Tuple[List[str], List[str]]:
+    url = f"https://codeforces.com/{namespace}/{id_}/problem/{problem}"
 
     response = requests.get(url, headers=headers)
     inputs, outputs = [], []
+
+    if response.status_code >= 300:
+        raise ValueError(f"{namespace.capitalize()} problem not found")
     
     soup = BeautifulSoup(response.content, "html.parser")
 
     for input_data in soup.find_all("div", class_="input"):        
         pre = input_data.find("pre")
 
-        string = "\n".join(data.text for data in pre.find_all("div"))
+        if not pre: continue
+        
+        divs = pre.find_all("div")
+
+        if divs:
+            string = "\n".join(data.text for data in divs)
+        else: 
+            string = pre.text
+
         inputs.append(string)
 
     for output_data in soup.find_all("div", class_="output"):
         pre = output_data.find("pre")
-        outputs.append(pre.text)
+        
+        if pre:
+            outputs.append(pre.text)
 
-    return inputs, outputs
+    return inputs, outputs
```

### Comparing `fastsnake-1.3.0/fastsnake/util/compiler.py` & `fastsnake-1.4.0/fastsnake/util/compiler.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.3.0/tests/test_algorithms/test_binary_search.py` & `fastsnake-1.4.0/tests/test_algorithms/test_binary_search.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.3.0/tests/test_algorithms/test_knapsack.py` & `fastsnake-1.4.0/tests/test_algorithms/test_knapsack.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.3.0/tests/test_algorithms/test_lower_bound.py` & `fastsnake-1.4.0/tests/test_algorithms/test_lower_bound.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.3.0/tests/test_algorithms/test_mex.py` & `fastsnake-1.4.0/tests/test_algorithms/test_mex.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.3.0/tests/test_algorithms/test_upper_bound.py` & `fastsnake-1.4.0/tests/test_algorithms/test_upper_bound.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.3.0/tests/test_codeforces_tools/test_problem_loader.py` & `fastsnake-1.4.0/tests/test_codeforces_tools/test_problem_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from fastsnake.util.codeforces import *
 import os
 
 def test_get_problems():
-    problems = get_contest_problems(1949)
+    problems = get_problems(1949)
     assert "".join(problems) == "ABCDEFGHIJK"
 
 
 def test_load_problem_test_cases():
     folder = os.path.join(os.path.dirname(__file__), "sample_1949_J")
 
     n_input = len([x for x in os.listdir(folder) if x.endswith(".in")])
     n_output = len([x for x in os.listdir(folder) if x.endswith(".out")])
 
-    inputs, outputs = get_contest_problem_test_cases(1949, "J")
+    inputs, outputs = get_problem_test_cases(1949, "J")
 
     assert len(inputs) == n_input and len(outputs) == n_output
 
     for i in range(n_input):
         with open(os.path.join(folder, f"{i}.in")) as file:
             assert file.read().strip().strip("\n") == inputs[i].strip().strip("\n")
```

### Comparing `fastsnake-1.3.0/tests/test_compiler/test_compiler.py` & `fastsnake-1.4.0/tests/test_compiler/test_compiler.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.3.0/.gitignore` & `fastsnake-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fastsnake-1.3.0/LICENSE` & `fastsnake-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastsnake-1.3.0/README.md` & `fastsnake-1.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,58 +6,62 @@
 [![Python Version](https://img.shields.io/badge/python-3.7+-8A2BE2)](https://pypi.org/project/FastSnake/)
 
 Tired of having to copy-paste your library code into every solution you write? FastSnake is a command-line tool that allows you to easily create, expand, run and test Python solutions for competitive programming problems.
 
 This project provides useful CLI tools for competitive programming, such as algorithms and data structures, and tools for Codeforces. But you will have to write your own code and library for the problems you want to solve.
 
 ## Installing FastSnake:
-**For Python with pip:**
 ```
 $ pip install FastSnake
 ```
 
 ## Basic Usage:
 Starting a contest from Codeforces...
 ```
 $ fastsnake codeforces -sc <contest_id>
 ```
 **Note:** The contest ID can be found at contest URL `https://codeforces.com/contest/<id>`
 <br>
 
 Once you have written your solution, test it.
 ```
-$ fastsnake -t <problem>
+$ fastsnake test <problem>
+```
+
+You can also create your own generator, at `test_generators` folder, to bruteforce your solution.
+```
+$ fastsnake test <problem> -g <n_tests>
 ```
 
 ### Algorithms and Structures
 
 FastSnake provides some algorithms and structures that can be injected to your final solution. See the sample below:
 
 **Python Solution:**
 ```py
 from fastsnake.algorithms.min_coins import *
 
-n = int(input())
 coins = []
 
 for x in input().split():
     coins.append(int(x))
 
 value = int(input())
 
-print(min_coins(coins, value))  # Result
+result = min_coins(coins, value)
+print(result)
 ```
 Use the argument `--list <algorithms | structures>` to see all algorithms and structures provided by FastSnake.
 
 **Injecting the algorithm to the final solution...**
 ```
-$ fastsnake -c main.py
+$ fastsnake compile main.py
 ```
 Check out the code of the generated Python module.
 <br>
 
 ### Testing and Compiling:
 You may test and compile your solution using the command below:
 ```
-$ fastsnake -tc <problem>
+$ fastsnake test <problem> -c
 ```
 If the solution was accepted at all test cases, it will be compiled.
```

### Comparing `fastsnake-1.3.0/pyproject.toml` & `fastsnake-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastsnake-1.3.0/PKG-INFO` & `fastsnake-1.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: FastSnake
-Version: 1.3.0
+Version: 1.4.0
 Summary: A helper for contests in Python 3
 Project-URL: Homepage, https://github.com/JeanExtreme002/FastSnake
 Author-email: Jean Loui Bernard Silva de Jesus <jeanextreme002@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: algorithms,codeforces,contest
 Classifier: Intended Audience :: Developers
@@ -24,58 +24,62 @@
 [![Python Version](https://img.shields.io/badge/python-3.7+-8A2BE2)](https://pypi.org/project/FastSnake/)
 
 Tired of having to copy-paste your library code into every solution you write? FastSnake is a command-line tool that allows you to easily create, expand, run and test Python solutions for competitive programming problems.
 
 This project provides useful CLI tools for competitive programming, such as algorithms and data structures, and tools for Codeforces. But you will have to write your own code and library for the problems you want to solve.
 
 ## Installing FastSnake:
-**For Python with pip:**
 ```
 $ pip install FastSnake
 ```
 
 ## Basic Usage:
 Starting a contest from Codeforces...
 ```
 $ fastsnake codeforces -sc <contest_id>
 ```
 **Note:** The contest ID can be found at contest URL `https://codeforces.com/contest/<id>`
 <br>
 
 Once you have written your solution, test it.
 ```
-$ fastsnake -t <problem>
+$ fastsnake test <problem>
+```
+
+You can also create your own generator, at `test_generators` folder, to bruteforce your solution.
+```
+$ fastsnake test <problem> -g <n_tests>
 ```
 
 ### Algorithms and Structures
 
 FastSnake provides some algorithms and structures that can be injected to your final solution. See the sample below:
 
 **Python Solution:**
 ```py
 from fastsnake.algorithms.min_coins import *
 
-n = int(input())
 coins = []
 
 for x in input().split():
     coins.append(int(x))
 
 value = int(input())
 
-print(min_coins(coins, value))  # Result
+result = min_coins(coins, value)
+print(result)
 ```
 Use the argument `--list <algorithms | structures>` to see all algorithms and structures provided by FastSnake.
 
 **Injecting the algorithm to the final solution...**
 ```
-$ fastsnake -c main.py
+$ fastsnake compile main.py
 ```
 Check out the code of the generated Python module.
 <br>
 
 ### Testing and Compiling:
 You may test and compile your solution using the command below:
 ```
-$ fastsnake -tc <problem>
+$ fastsnake test <problem> -c
 ```
 If the solution was accepted at all test cases, it will be compiled.
```

