# Comparing `tmp/ained-0.1.0.tar.gz` & `tmp/ained-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ained-0.1.0.tar", max compression
+gzip compressed data, was "ained-0.2.0.tar", max compression
```

## Comparing `ained-0.1.0.tar` & `ained-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     2642 2024-04-16 10:17:00.460106 ained-0.1.0/README.md
--rw-r--r--   0        0        0      654 2024-04-17 12:37:04.163437 ained-0.1.0/ained/Data/exampleData.json
--rw-r--r--   0        0        0     1208 2024-04-17 12:37:04.163437 ained-0.1.0/ained/Data/jasonSchema.json
--rw-r--r--   0        0        0    29149 2024-04-17 12:37:04.163437 ained-0.1.0/ained/Samples/Sample1.txt
--rw-r--r--   0        0        0      294 2024-04-17 12:37:04.163437 ained-0.1.0/ained/Samples/Sample2.txt
--rw-r--r--   0        0        0      397 2024-04-17 12:37:04.163437 ained-0.1.0/ained/TauswortheInC/README.md
--rwxr-xr-x   0        0        0    15800 2024-04-17 12:37:04.163437 ained-0.1.0/ained/TauswortheInC/libtausworthe.so
--rw-r--r--   0        0        0      924 2024-04-17 12:37:04.163437 ained-0.1.0/ained/TauswortheInC/tausworthe.c
--rw-r--r--   0        0        0      110 2024-04-17 12:37:04.163437 ained-0.1.0/ained/TauswortheInC/tausworthe_wrapper.c
--rw-r--r--   0        0        0       26 2024-04-17 12:37:04.163437 ained-0.1.0/ained/Test_Data/random_nums.txt
--rw-r--r--   0        0        0        0 2024-04-17 12:37:04.163437 ained-0.1.0/ained/__init__.py
--rw-r--r--   0        0        0     2622 2024-04-17 12:37:04.163437 ained-0.1.0/ained/board.py
--rw-r--r--   0        0        0     3765 2024-04-17 12:37:04.163437 ained-0.1.0/ained/calculator.py
--rw-r--r--   0        0        0     2293 2024-04-17 12:37:04.163437 ained-0.1.0/ained/dipole.py
--rw-r--r--   0        0        0     5666 2024-04-17 12:41:24.076991 ained-0.1.0/ained/display.py
--rw-r--r--   0        0        0      573 2024-04-17 12:37:04.163437 ained-0.1.0/ained/fixedpoint_config.py
--rw-r--r--   0        0        0     1742 2024-04-17 12:37:04.163437 ained-0.1.0/ained/generator.py
--rw-r--r--   0        0        0     1116 2024-04-17 12:37:04.163437 ained-0.1.0/ained/historymanager.py
--rw-r--r--   0        0        0     2014 2024-04-17 12:37:04.163437 ained-0.1.0/ained/main.py
--rw-r--r--   0        0        0      317 2024-04-17 12:37:04.163437 ained-0.1.0/ained/number_gen.py
--rw-r--r--   0        0        0     2002 2024-04-17 12:37:04.163437 ained-0.1.0/ained/processJson.py
--rw-r--r--   0        0        0       26 2024-04-17 12:37:04.163437 ained-0.1.0/ained/test/Test_Data/random_nums.txt
--rw-r--r--   0        0        0     2337 2024-04-17 12:37:04.163437 ained-0.1.0/ained/test/__pycache__/test_board.cpython-310-pytest-8.1.1.pyc
--rw-r--r--   0        0        0     3429 2024-04-17 12:37:04.163437 ained-0.1.0/ained/test/__pycache__/test_dipole.cpython-310-pytest-8.1.1.pyc
--rw-r--r--   0        0        0     4663 2024-04-17 12:37:04.163437 ained-0.1.0/ained/test/__pycache__/test_fixedpoint.cpython-310-pytest-8.1.1.pyc
--rw-r--r--   0        0        0     1789 2024-04-17 12:37:04.163437 ained-0.1.0/ained/test/__pycache__/test_generator.cpython-310-pytest-8.1.1.pyc
--rw-r--r--   0        0        0     8355 2024-04-17 12:37:04.163437 ained-0.1.0/ained/test/__pycache__/test_utils.cpython-310-pytest-8.1.1.pyc
--rw-r--r--   0        0        0     1952 2024-04-17 12:37:04.167437 ained-0.1.0/ained/test/test_board.py
--rw-r--r--   0        0        0      734 2024-04-17 12:37:04.167437 ained-0.1.0/ained/test/test_dipole.py
--rw-r--r--   0        0        0     1307 2024-04-17 12:37:04.167437 ained-0.1.0/ained/test/test_fixedpoint.py
--rw-r--r--   0        0        0      754 2024-04-17 12:37:04.167437 ained-0.1.0/ained/test/test_generator.py
--rw-r--r--   0        0        0     3316 2024-04-17 12:37:04.167437 ained-0.1.0/ained/test/test_utils.py
--rw-r--r--   0        0        0      423 2024-04-17 12:37:04.167437 ained-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3198 1970-01-01 00:00:00.000000 ained-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2894 2024-04-18 07:24:10.007915 ained-0.2.0/README.md
+-rw-r--r--   0        0        0      654 2024-04-17 12:37:04.163437 ained-0.2.0/ained/Data/exampleData.json
+-rw-r--r--   0        0        0     1208 2024-04-17 12:37:04.163437 ained-0.2.0/ained/Data/jasonSchema.json
+-rw-r--r--   0        0        0    29149 2024-04-17 12:37:04.163437 ained-0.2.0/ained/Samples/Sample1.txt
+-rw-r--r--   0        0        0      294 2024-04-17 12:37:04.163437 ained-0.2.0/ained/Samples/Sample2.txt
+-rw-r--r--   0        0        0      397 2024-04-17 12:37:04.163437 ained-0.2.0/ained/TauswortheInC/README.md
+-rwxr-xr-x   0        0        0    15800 2024-04-17 12:37:04.163437 ained-0.2.0/ained/TauswortheInC/libtausworthe.so
+-rw-r--r--   0        0        0      924 2024-04-17 12:37:04.163437 ained-0.2.0/ained/TauswortheInC/tausworthe.c
+-rw-r--r--   0        0        0      110 2024-04-17 12:37:04.163437 ained-0.2.0/ained/TauswortheInC/tausworthe_wrapper.c
+-rw-r--r--   0        0        0       26 2024-04-17 12:37:04.163437 ained-0.2.0/ained/Test_Data/random_nums.txt
+-rw-r--r--   0        0        0       21 2024-04-18 07:26:09.891428 ained-0.2.0/ained/__init__.py
+-rw-r--r--   0        0        0     2622 2024-04-17 12:37:04.163437 ained-0.2.0/ained/board.py
+-rw-r--r--   0        0        0     3765 2024-04-17 12:37:04.163437 ained-0.2.0/ained/calculator.py
+-rw-r--r--   0        0        0     2293 2024-04-17 12:37:04.163437 ained-0.2.0/ained/dipole.py
+-rw-r--r--   0        0        0     5666 2024-04-17 12:41:24.076991 ained-0.2.0/ained/display.py
+-rw-r--r--   0        0        0      573 2024-04-17 12:37:04.163437 ained-0.2.0/ained/fixedpoint_config.py
+-rw-r--r--   0        0        0     1742 2024-04-17 12:37:04.163437 ained-0.2.0/ained/generator.py
+-rw-r--r--   0        0        0     1116 2024-04-17 12:37:04.163437 ained-0.2.0/ained/historymanager.py
+-rw-r--r--   0        0        0     2014 2024-04-17 12:37:04.163437 ained-0.2.0/ained/main.py
+-rw-r--r--   0        0        0      317 2024-04-17 12:37:04.163437 ained-0.2.0/ained/number_gen.py
+-rw-r--r--   0        0        0     2002 2024-04-17 12:37:04.163437 ained-0.2.0/ained/processJson.py
+-rw-r--r--   0        0        0       26 2024-04-17 12:37:04.163437 ained-0.2.0/ained/test/Test_Data/random_nums.txt
+-rw-r--r--   0        0        0     2337 2024-04-17 12:37:04.163437 ained-0.2.0/ained/test/__pycache__/test_board.cpython-310-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0     3429 2024-04-17 12:37:04.163437 ained-0.2.0/ained/test/__pycache__/test_dipole.cpython-310-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0     4663 2024-04-17 12:37:04.163437 ained-0.2.0/ained/test/__pycache__/test_fixedpoint.cpython-310-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0     1789 2024-04-17 12:37:04.163437 ained-0.2.0/ained/test/__pycache__/test_generator.cpython-310-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0     8355 2024-04-17 12:37:04.163437 ained-0.2.0/ained/test/__pycache__/test_utils.cpython-310-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0     1952 2024-04-17 12:37:04.167437 ained-0.2.0/ained/test/test_board.py
+-rw-r--r--   0        0        0      734 2024-04-17 12:37:04.167437 ained-0.2.0/ained/test/test_dipole.py
+-rw-r--r--   0        0        0     1307 2024-04-17 12:37:04.167437 ained-0.2.0/ained/test/test_fixedpoint.py
+-rw-r--r--   0        0        0      754 2024-04-17 12:37:04.167437 ained-0.2.0/ained/test/test_generator.py
+-rw-r--r--   0        0        0     3316 2024-04-17 12:37:04.167437 ained-0.2.0/ained/test/test_utils.py
+-rw-r--r--   0        0        0      423 2024-04-18 07:25:27.051602 ained-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3450 1970-01-01 00:00:00.000000 ained-0.2.0/PKG-INFO
```

### Comparing `ained-0.1.0/README.md` & `ained-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,86 +1,96 @@
-# `AiNed`
+# Installation
+Note that because the tausworthe random number generator is a .so file the
+program can currently only run on Linux systems - Windows is not supported
+at the moment. The program can be installed 
+
+```console
+$ pip install ained
+```
+
+# ained Usage
 
 **Usage**:
 
 ```console
-$ AiNed [OPTIONS] COMMAND [ARGS]...
+$ ained [OPTIONS] COMMAND [ARGS]...
 ```
 
 **Options**:
 
 * `--install-completion`: Install completion for the current shell.
 * `--show-completion`: Show completion for the current shell, to copy it or customize the installation.
 * `--help`: Show this message and exit.
 
 **Commands**:
 
 * `generate-numbers`: Generate a file with random numbers from 0...
 * `gui`: Create a visual representation of the...
 * `process-file`: Read in a json file (input_file) with...
 
-## `AiNed generate-numbers`
+## `ained generate-numbers`
 
 Generate a file with random numbers from 0 to 100. Used for reproducible results.
 
 **Usage**:
 
 ```console
-$ AiNed generate-numbers [OPTIONS] COUNT FILEPATH
+$ ained generate-numbers [OPTIONS] COUNT FILEPATH
 ```
 
 **Arguments**:
 
 * `COUNT`: Number of random numbers to generate.  [required]
 * `FILEPATH`: File to save the random numbers to.  [required]
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
-## `AiNed gui`
+## `ained gui`
 
 Create a visual representation of the dipole grid that you can interact with via a GUI.
 
 **Usage**:
 
 ```console
-$ AiNed gui [OPTIONS] ROWS COLUMNS
+$ ained gui [OPTIONS] ROWS COLUMNS
 ```
 
 **Arguments**:
 
 * `ROWS`: Number of rows of the dipole grid.  [required]
 * `COLUMNS`: Number of columns of the dipole grid.  [required]
 
 **Options**:
 
 * `--probability FLOAT`: Strength of co-varying effect  [default: 0.7]
 * `--help`: Show this message and exit.
 
-## `AiNed process-file`
+## `ained process-file`
 
 Read in a json file (input_file) with board properties and a series of writes. Perform each write operation
 and propagate the results to neighboring bits. Save the entire history of writes and board states to (output_file)
 
 **Usage**:
 
 ```console
-$ AiNed process-file [OPTIONS] INPUT_FILE OUTPUT_FILE
+$ ained process-file [OPTIONS] INPUT_FILE OUTPUT_FILE
 ```
 
 **Arguments**:
 
 * `INPUT_FILE`: File path to JSON file to process.  [required]
 * `OUTPUT_FILE`: File path to save results to.  [required]
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
+
 ## Fixed Point Arithmetic ##
 
 Because this software is intended to be a functional model for simulating calculations
 on an FPGA the goal was to avoid floating point arithmetic since DSPs are limited on
 an FPGA. Thus the [fxpmath](https://github.com/francof2a/fxpmath)  library was used to
 enforce 16-bit fixed point arithmetic. Specifically the following precision was used:
```

### Comparing `ained-0.1.0/ained/Data/exampleData.json` & `ained-0.2.0/ained/Data/exampleData.json`

 * *Files identical despite different names*

### Comparing `ained-0.1.0/ained/Data/jasonSchema.json` & `ained-0.2.0/ained/Data/jasonSchema.json`

 * *Files identical despite different names*

### Comparing `ained-0.1.0/ained/Samples/Sample1.txt` & `ained-0.2.0/ained/Samples/Sample1.txt`

 * *Files identical despite different names*

### Comparing `ained-0.1.0/ained/TauswortheInC/libtausworthe.so` & `ained-0.2.0/ained/TauswortheInC/libtausworthe.so`

 * *Files identical despite different names*

### Comparing `ained-0.1.0/ained/TauswortheInC/tausworthe.c` & `ained-0.2.0/ained/TauswortheInC/tausworthe.c`

 * *Files identical despite different names*

### Comparing `ained-0.1.0/ained/board.py` & `ained-0.2.0/ained/board.py`

 * *Files identical despite different names*

### Comparing `ained-0.1.0/ained/calculator.py` & `ained-0.2.0/ained/calculator.py`

 * *Files identical despite different names*

### Comparing `ained-0.1.0/ained/dipole.py` & `ained-0.2.0/ained/dipole.py`

 * *Files identical despite different names*

### Comparing `ained-0.1.0/ained/display.py` & `ained-0.2.0/ained/display.py`

 * *Files identical despite different names*

### Comparing `ained-0.1.0/ained/fixedpoint_config.py` & `ained-0.2.0/ained/fixedpoint_config.py`

 * *Files identical despite different names*

### Comparing `ained-0.1.0/ained/generator.py` & `ained-0.2.0/ained/generator.py`

 * *Files identical despite different names*

### Comparing `ained-0.1.0/ained/historymanager.py` & `ained-0.2.0/ained/historymanager.py`

 * *Files identical despite different names*

### Comparing `ained-0.1.0/ained/main.py` & `ained-0.2.0/ained/main.py`

 * *Files identical despite different names*

### Comparing `ained-0.1.0/ained/processJson.py` & `ained-0.2.0/ained/processJson.py`

 * *Files identical despite different names*

### Comparing `ained-0.1.0/ained/test/__pycache__/test_board.cpython-310-pytest-8.1.1.pyc` & `ained-0.2.0/ained/test/__pycache__/test_board.cpython-310-pytest-8.1.1.pyc`

 * *Files identical despite different names*

### Comparing `ained-0.1.0/ained/test/__pycache__/test_dipole.cpython-310-pytest-8.1.1.pyc` & `ained-0.2.0/ained/test/__pycache__/test_dipole.cpython-310-pytest-8.1.1.pyc`

 * *Files identical despite different names*

### Comparing `ained-0.1.0/ained/test/__pycache__/test_fixedpoint.cpython-310-pytest-8.1.1.pyc` & `ained-0.2.0/ained/test/__pycache__/test_fixedpoint.cpython-310-pytest-8.1.1.pyc`

 * *Files identical despite different names*

### Comparing `ained-0.1.0/ained/test/__pycache__/test_generator.cpython-310-pytest-8.1.1.pyc` & `ained-0.2.0/ained/test/__pycache__/test_generator.cpython-310-pytest-8.1.1.pyc`

 * *Files identical despite different names*

### Comparing `ained-0.1.0/ained/test/__pycache__/test_utils.cpython-310-pytest-8.1.1.pyc` & `ained-0.2.0/ained/test/__pycache__/test_utils.cpython-310-pytest-8.1.1.pyc`

 * *Files identical despite different names*

### Comparing `ained-0.1.0/ained/test/test_board.py` & `ained-0.2.0/ained/test/test_board.py`

 * *Files identical despite different names*

### Comparing `ained-0.1.0/ained/test/test_dipole.py` & `ained-0.2.0/ained/test/test_dipole.py`

 * *Files identical despite different names*

### Comparing `ained-0.1.0/ained/test/test_fixedpoint.py` & `ained-0.2.0/ained/test/test_fixedpoint.py`

 * *Files identical despite different names*

### Comparing `ained-0.1.0/ained/test/test_generator.py` & `ained-0.2.0/ained/test/test_generator.py`

 * *Files identical despite different names*

### Comparing `ained-0.1.0/ained/test/test_utils.py` & `ained-0.2.0/ained/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `ained-0.1.0/PKG-INFO` & `ained-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,103 +1,113 @@
 Metadata-Version: 2.1
 Name: ained
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: aschroede
 Author-email: aschroed@ualberta.ca
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: fxpmath (>=0.4.9,<0.5.0)
 Requires-Dist: jsonschema (>=4.21.1,<5.0.0)
 Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
 Requires-Dist: typer[all] (>=0.12.3,<0.13.0)
 Description-Content-Type: text/markdown
 
-# `AiNed`
+# Installation
+Note that because the tausworthe random number generator is a .so file the
+program can currently only run on Linux systems - Windows is not supported
+at the moment. The program can be installed 
+
+```console
+$ pip install ained
+```
+
+# ained Usage
 
 **Usage**:
 
 ```console
-$ AiNed [OPTIONS] COMMAND [ARGS]...
+$ ained [OPTIONS] COMMAND [ARGS]...
 ```
 
 **Options**:
 
 * `--install-completion`: Install completion for the current shell.
 * `--show-completion`: Show completion for the current shell, to copy it or customize the installation.
 * `--help`: Show this message and exit.
 
 **Commands**:
 
 * `generate-numbers`: Generate a file with random numbers from 0...
 * `gui`: Create a visual representation of the...
 * `process-file`: Read in a json file (input_file) with...
 
-## `AiNed generate-numbers`
+## `ained generate-numbers`
 
 Generate a file with random numbers from 0 to 100. Used for reproducible results.
 
 **Usage**:
 
 ```console
-$ AiNed generate-numbers [OPTIONS] COUNT FILEPATH
+$ ained generate-numbers [OPTIONS] COUNT FILEPATH
 ```
 
 **Arguments**:
 
 * `COUNT`: Number of random numbers to generate.  [required]
 * `FILEPATH`: File to save the random numbers to.  [required]
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
-## `AiNed gui`
+## `ained gui`
 
 Create a visual representation of the dipole grid that you can interact with via a GUI.
 
 **Usage**:
 
 ```console
-$ AiNed gui [OPTIONS] ROWS COLUMNS
+$ ained gui [OPTIONS] ROWS COLUMNS
 ```
 
 **Arguments**:
 
 * `ROWS`: Number of rows of the dipole grid.  [required]
 * `COLUMNS`: Number of columns of the dipole grid.  [required]
 
 **Options**:
 
 * `--probability FLOAT`: Strength of co-varying effect  [default: 0.7]
 * `--help`: Show this message and exit.
 
-## `AiNed process-file`
+## `ained process-file`
 
 Read in a json file (input_file) with board properties and a series of writes. Perform each write operation
 and propagate the results to neighboring bits. Save the entire history of writes and board states to (output_file)
 
 **Usage**:
 
 ```console
-$ AiNed process-file [OPTIONS] INPUT_FILE OUTPUT_FILE
+$ ained process-file [OPTIONS] INPUT_FILE OUTPUT_FILE
 ```
 
 **Arguments**:
 
 * `INPUT_FILE`: File path to JSON file to process.  [required]
 * `OUTPUT_FILE`: File path to save results to.  [required]
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
+
 ## Fixed Point Arithmetic ##
 
 Because this software is intended to be a functional model for simulating calculations
 on an FPGA the goal was to avoid floating point arithmetic since DSPs are limited on
 an FPGA. Thus the [fxpmath](https://github.com/francof2a/fxpmath)  library was used to
 enforce 16-bit fixed point arithmetic. Specifically the following precision was used:
```

