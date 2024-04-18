# Comparing `tmp/hipopy-1.2.4.tar.gz` & `tmp/hipopy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hipopy-1.2.4.tar", max compression
+gzip compressed data, was "hipopy-1.3.0.tar", max compression
```

## Comparing `hipopy-1.2.4.tar` & `hipopy-1.3.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1098 2022-05-27 15:19:00.119583 hipopy-1.2.4/LICENSE
--rw-r--r--   0        0        0      817 2022-05-27 15:18:58.965901 hipopy-1.2.4/README.md
--rw-r--r--   0        0        0      108 2023-02-07 16:10:21.136237 hipopy-1.2.4/hipopy/__init__.py
--rw-r--r--   0        0        0    30262 2023-02-07 16:08:17.890801 hipopy-1.2.4/hipopy/hipopy.py
--rw-r--r--   0        0        0      566 2023-02-07 16:10:05.862417 hipopy-1.2.4/pyproject.toml
--rw-r--r--   0        0        0     1584 1970-01-01 00:00:00.000000 hipopy-1.2.4/setup.py
--rw-r--r--   0        0        0     1614 1970-01-01 00:00:00.000000 hipopy-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-11 20:15:48.863986 hipopy-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1001 2024-04-11 20:15:48.864143 hipopy-1.3.0/README.md
+-rw-r--r--   0        0        0      108 2024-04-18 20:16:20.203572 hipopy-1.3.0/hipopy/__init__.py
+-rw-r--r--   0        0        0    30484 2024-04-17 18:03:08.077803 hipopy-1.3.0/hipopy/hipopy.py
+-rw-r--r--   0        0        0      513 2024-04-18 20:15:36.420722 hipopy-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1849 1970-01-01 00:00:00.000000 hipopy-1.3.0/PKG-INFO
```

### Comparing `hipopy-1.2.4/LICENSE` & `hipopy-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hipopy-1.2.4/README.md` & `hipopy-1.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 # HIPOPy: UpROOT-like I/O Interface for CLAS12 HIPO Files
 
-## Installation
+## Prerequisites
 
-To install from source:
-```bash
-git clone https://github.com/mfmceneaney/hipopy.git
-```
+* Python >=3.7.3
+* A compiler with C++11 support
+* Pip 10+ or CMake >= 3.4 (or 3.14+ on Windows, which was the first version to support VS 2019)
+* Ninja or Pip 10+
 
-Then add to following to your startup script:
-```bash
-export PYTHONPATH=$PYTHONPATH:/path/to/hipopy
-```
 You will also need to install the project dependencies:
 * [numpy](https://numpy.org)
 * [awkward](https://awkward-array.readthedocs.io/en/latest/)
 * [hipopybind](https://github.com/mfmceneaney/hipopybind.git)
 
 (All available with pip.)
 
+## Installation
+
 To install with pip:
 ```bash
 pip install hipopy
 ```
 
+To install from source:
+```bash
+git clone https://github.com/mfmceneaney/hipopy.git
+```
+
+Then add to following to your startup script:
+```bash
+export PYTHONPATH=$PYTHONPATH:/path/to/hipopy
+```
+
 ## Getting Started
 
 Check out the example scripts in `tutorials`.  More functionality coming soon!
 
 ## Documentation
 
 Full documentation available on [Read the Docs](https://hipopy.readthedocs.io/en/latest/index.html)!
```

### Comparing `hipopy-1.2.4/hipopy/hipopy.py` & `hipopy-1.3.0/hipopy/hipopy.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,20 @@
         Description
         -----------
         Open a HIPO file to read, write (from scratch), or append data.
         IMPORTANT:  Make sure you add schema before opening a file to write!
         """
 
         if self.mode=="r":
-            if self.tags is not None: self.reader.setTags(self.tags) #NOTE: Only set tags for files to read since not yet tested for writing files.
+            if self.tags is not None:
+                if type(self.tags)==int:
+                    self.reader.setTags(self.tags) #NOTE: Only set tags for files to read since not yet tested for writing files.
+                else:
+                    for tag in self.tags:
+                        self.reader.setTags(tag)
             self.reader.open(self.filename)
             self.reader.readDictionary(self.dictionary)
         elif self.mode=="w": self.writer.open(self.filename)
         elif self.mode=="a" and self.buffname is None:
 
             # Open with reader first
             self.reader.open(self.filename)
@@ -389,15 +394,15 @@
     def newTree(self,bank,bankdict,group=None,item=None):
         """
         Parameters
         ----------
         bank : string, required
             Bank name
         bankdict : dictionary, required
-            Dictionary of bank entry names to data types ("D", "F", "I")
+            Dictionary of bank entry names to data types ("D":double, "F":float, "I":int, "B":byte, "S":short, "L":long)
         group : int, optional
             Group identifier for bank (must be unique)
             Default : None
         item : int, optional
             Item identifier for bank (does not have to be unique)
             Default : None
```

### Comparing `hipopy-1.2.4/pyproject.toml` & `hipopy-1.3.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [tool.poetry]
 name = "hipopy"
-version = "1.2.4"
+version = "1.3.0"
 license = "MIT"
 description = "UpROOT-Like I/O Interface for CLAS12 HIPO Files"
 authors = ["Matthew McEneaney <matthew.mceneaney@duke.edu>"]
 repository = "https://github.com/mfmceneaney/hipopy.git"
 readme = "README.md"
-include = ["hipo/libhipo4.so","hipo/libhipo4.dylib"]
 
 [tool.poetry.dependencies]
 python = "^3.7.3"
 awkward = "^1.3.0"
 numpy = "^1.19.2"
-hipopybind = ">=0.1.1"
+hipopybind = ">=1.0.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hipopy-1.2.4/PKG-INFO` & `hipopy-1.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,62 @@
 Metadata-Version: 2.1
 Name: hipopy
-Version: 1.2.4
+Version: 1.3.0
 Summary: UpROOT-Like I/O Interface for CLAS12 HIPO Files
 Home-page: https://github.com/mfmceneaney/hipopy.git
 License: MIT
 Author: Matthew McEneaney
 Author-email: matthew.mceneaney@duke.edu
 Requires-Python: >=3.7.3,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: awkward (>=1.3.0,<2.0.0)
-Requires-Dist: hipopybind (>=0.1.1)
+Requires-Dist: hipopybind (>=1.0.1)
 Requires-Dist: numpy (>=1.19.2,<2.0.0)
 Project-URL: Repository, https://github.com/mfmceneaney/hipopy.git
 Description-Content-Type: text/markdown
 
 # HIPOPy: UpROOT-like I/O Interface for CLAS12 HIPO Files
 
-## Installation
+## Prerequisites
 
-To install from source:
-```bash
-git clone https://github.com/mfmceneaney/hipopy.git
-```
+* Python >=3.7.3
+* A compiler with C++11 support
+* Pip 10+ or CMake >= 3.4 (or 3.14+ on Windows, which was the first version to support VS 2019)
+* Ninja or Pip 10+
 
-Then add to following to your startup script:
-```bash
-export PYTHONPATH=$PYTHONPATH:/path/to/hipopy
-```
 You will also need to install the project dependencies:
 * [numpy](https://numpy.org)
 * [awkward](https://awkward-array.readthedocs.io/en/latest/)
 * [hipopybind](https://github.com/mfmceneaney/hipopybind.git)
 
 (All available with pip.)
 
+## Installation
+
 To install with pip:
 ```bash
 pip install hipopy
 ```
 
+To install from source:
+```bash
+git clone https://github.com/mfmceneaney/hipopy.git
+```
+
+Then add to following to your startup script:
+```bash
+export PYTHONPATH=$PYTHONPATH:/path/to/hipopy
+```
+
 ## Getting Started
 
 Check out the example scripts in `tutorials`.  More functionality coming soon!
 
 ## Documentation
 
 Full documentation available on [Read the Docs](https://hipopy.readthedocs.io/en/latest/index.html)!
```

