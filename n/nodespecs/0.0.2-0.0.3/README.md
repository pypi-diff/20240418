# Comparing `tmp/nodespecs-0.0.2.tar.gz` & `tmp/nodespecs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodespecs-0.0.2.tar", last modified: Fri Apr 12 23:30:33 2024, max compression
+gzip compressed data, was "nodespecs-0.0.3.tar", last modified: Thu Apr 18 20:27:48 2024, max compression
```

## Comparing `nodespecs-0.0.2.tar` & `nodespecs-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 23:30:33.969561 nodespecs-0.0.2/
--rw-rw-rw-   0        0        0     1098 2024-04-12 22:48:35.000000 nodespecs-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     5618 2024-04-12 23:30:33.967365 nodespecs-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3737 2024-04-12 20:14:32.000000 nodespecs-0.0.2/README.md
--rw-rw-rw-   0        0        0      899 2024-04-12 23:30:15.000000 nodespecs-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 23:30:33.969561 nodespecs-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 23:30:33.937016 nodespecs-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 23:30:33.965270 nodespecs-0.0.2/src/nodespecs.egg-info/
--rw-rw-rw-   0        0        0     5618 2024-04-12 23:30:33.000000 nodespecs-0.0.2/src/nodespecs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2024-04-12 23:30:33.000000 nodespecs-0.0.2/src/nodespecs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 23:30:33.000000 nodespecs-0.0.2/src/nodespecs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-04-12 23:30:33.000000 nodespecs-0.0.2/src/nodespecs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       88 2024-04-12 23:30:33.000000 nodespecs-0.0.2/src/nodespecs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-12 23:30:33.000000 nodespecs-0.0.2/src/nodespecs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-12 23:30:33.963204 nodespecs-0.0.2/src/specs/
--rw-rw-rw-   0        0        0       91 2024-04-12 23:27:17.000000 nodespecs-0.0.2/src/specs/__init__.py
--rw-rw-rw-   0        0        0      117 2024-04-12 22:25:05.000000 nodespecs-0.0.2/src/specs/__main__.py
--rw-rw-rw-   0        0        0     1400 2024-04-12 15:15:38.000000 nodespecs-0.0.2/src/specs/cpu-benchmark.py
--rw-rw-rw-   0        0        0    86524 2024-04-12 15:14:05.000000 nodespecs-0.0.2/src/specs/cpuinfo.py
--rw-rw-rw-   0        0        0     7189 2024-04-12 22:25:26.000000 nodespecs-0.0.2/src/specs/hardware.py
+drwxrwxrwx   0        0        0        0 2024-04-18 20:27:48.230646 nodespecs-0.0.3/
+-rw-rw-rw-   0        0        0     1098 2024-04-13 00:06:04.000000 nodespecs-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     5755 2024-04-18 20:27:48.228651 nodespecs-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3874 2024-04-18 20:26:59.000000 nodespecs-0.0.3/README.md
+-rw-rw-rw-   0        0        0      899 2024-04-18 20:24:28.000000 nodespecs-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-18 20:27:48.230646 nodespecs-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-18 20:27:48.193827 nodespecs-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-18 20:27:48.227307 nodespecs-0.0.3/src/nodespecs.egg-info/
+-rw-rw-rw-   0        0        0     5755 2024-04-18 20:27:48.000000 nodespecs-0.0.3/src/nodespecs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2024-04-18 20:27:48.000000 nodespecs-0.0.3/src/nodespecs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 20:27:48.000000 nodespecs-0.0.3/src/nodespecs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-04-18 20:27:48.000000 nodespecs-0.0.3/src/nodespecs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       88 2024-04-18 20:27:48.000000 nodespecs-0.0.3/src/nodespecs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-18 20:27:48.000000 nodespecs-0.0.3/src/nodespecs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 20:27:48.224319 nodespecs-0.0.3/src/specs/
+-rw-rw-rw-   0        0        0       91 2024-04-18 20:27:13.000000 nodespecs-0.0.3/src/specs/__init__.py
+-rw-rw-rw-   0        0        0      271 2024-04-18 19:09:52.000000 nodespecs-0.0.3/src/specs/__main__.py
+-rw-rw-rw-   0        0        0      172 2024-04-18 19:56:34.000000 nodespecs-0.0.3/src/specs/cmd.py
+-rw-rw-rw-   0        0        0     1400 2024-04-12 15:15:38.000000 nodespecs-0.0.3/src/specs/cpu-benchmark.py
+-rw-rw-rw-   0        0        0    86524 2024-04-12 15:14:05.000000 nodespecs-0.0.3/src/specs/cpuinfo.py
+-rw-rw-rw-   0        0        0     7189 2024-04-12 22:25:26.000000 nodespecs-0.0.3/src/specs/hardware.py
```

### Comparing `nodespecs-0.0.2/LICENSE` & `nodespecs-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nodespecs-0.0.2/PKG-INFO` & `nodespecs-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodespecs
-Version: 0.0.2
+Version: 0.0.3
 Summary: The specs summarize utilities for computer instance
 Author-email: jinsanity <jinsanityff@gmail.com>
 License: The MIT License (MIT)
         Copyright © 2024 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -12,27 +12,38 @@
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Project-URL: Homepage, https://github.com/jinsanity07git/hardwareSummary
 Keywords: cpu,gpu,benchmark
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: psutil>=5.9.5
 Requires-Dist: tabulate>=0.9.0
 Requires-Dist: tomli; python_version < "3.11"
 Provides-Extra: dev
 Requires-Dist: GPUtil; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 
 # hardwareSummary
 Extracting and Fetching all system and hardware information such as os details, CPU and GPU information, disk and network usage in Python using platform, psutil and gputil libraries.
 
+
+
+### install and use with pip
+
+```shell
+pip install node-specs
+python -m specs
+```
+
+#### Deprecated  (install and use with git)
+
 ```
 !git clone https://github.com/jinsanity07git/hardwareSummary && python hardwareSummary/hardware.py && python hardwareSummary/cpu-benchmark.py
 
 ```
 
 ```cmd
 git clone https://github.com/jinsanity07git/hardwareSummary && python hardwareSummary/hardware.py && python hardwareSummary/cpu-benchmark.py
@@ -45,15 +56,15 @@
 git clone https://github.com/jinsanity07git/hardwareSummary && python3 hardwareSummary/hardware.py && python3 hardwareSummary/cpu-benchmark.py
 ```
 
 
 
 ### CPU collection
 
-| Brand                         | CPU                                            | Arch   | OS         | Benchmarking | Comb                                                         | Score |
+| Nickname                      | CPU                                            | Arch   | OS         | Benchmarking | Comb                                                         | Score |
 | ----------------------------- | ---------------------------------------------- | ------ | ---------- | ------------ | ------------------------------------------------------------ | ----- |
 | TC17<br />TC16                | Intel(R) Core(TM) i9-14900KF                   | AMD64  | Windows    | 15.654       | Core-i9-14900KF                                              | 39.25 |
 | TC14                          | 13th Gen Intel(R) Core(TM) i9-13900K           | AMD64  | Windows 10 | 12.991       | Core-i9-13900K                                               | 38.76 |
 | Dell Precision 3561           | 11th Gen Intel(R) Core(TM) i7-11800H @ 2.30GHz | AMD64  | Windows    | 23.852       | Core-i7-11800H                                               | 13.47 |
 | TC07                          | Intel(R) Core(TM) i7-9700K CPU @ 3.60GHz       | AMD64  | Windows    | 26.723       | Core-i7-9700K                                                | 9.45  |
 | WUYING: 8 vCPU / 16 GiB Linux | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64 | Linux      | 33.572       | [Xeon-Platinum-8163](https://versus.com/en/intel-xeon-gold-6126-vs-intel-xeon-platinum-8168) |       |
 | TC03<br />TC11                | Intel(R) Xeon(R) Gold 6248R CPU @ 3.00GHz      | AMD64  | Window     | 34.612       | Xeon-Gold-6248R                                              | 23.26 |
@@ -65,16 +76,14 @@
 
 
 
 ### GPU collection
 
 
 
-
-
 | id    | name                   | total memory | Synthetic benchmark | CUDA API |
 | ----- | ---------------------- | ------------ | ------------------- | -------- |
 | colab | Tesla T4               | 15360.0MB    | 28.16               | 70627    |
 | dell  | NVIDIA T600 Laptop GPU | 4096.0MB     | 16.69               | 26600    |
```

### Comparing `nodespecs-0.0.2/README.md` & `nodespecs-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 # hardwareSummary
 Extracting and Fetching all system and hardware information such as os details, CPU and GPU information, disk and network usage in Python using platform, psutil and gputil libraries.
 
+
+
+### install and use with pip
+
+```shell
+pip install node-specs
+python -m specs
+```
+
+#### Deprecated  (install and use with git)
+
 ```
 !git clone https://github.com/jinsanity07git/hardwareSummary && python hardwareSummary/hardware.py && python hardwareSummary/cpu-benchmark.py
 
 ```
 
 ```cmd
 git clone https://github.com/jinsanity07git/hardwareSummary && python hardwareSummary/hardware.py && python hardwareSummary/cpu-benchmark.py
@@ -17,15 +28,15 @@
 git clone https://github.com/jinsanity07git/hardwareSummary && python3 hardwareSummary/hardware.py && python3 hardwareSummary/cpu-benchmark.py
 ```
 
 
 
 ### CPU collection
 
-| Brand                         | CPU                                            | Arch   | OS         | Benchmarking | Comb                                                         | Score |
+| Nickname                      | CPU                                            | Arch   | OS         | Benchmarking | Comb                                                         | Score |
 | ----------------------------- | ---------------------------------------------- | ------ | ---------- | ------------ | ------------------------------------------------------------ | ----- |
 | TC17<br />TC16                | Intel(R) Core(TM) i9-14900KF                   | AMD64  | Windows    | 15.654       | Core-i9-14900KF                                              | 39.25 |
 | TC14                          | 13th Gen Intel(R) Core(TM) i9-13900K           | AMD64  | Windows 10 | 12.991       | Core-i9-13900K                                               | 38.76 |
 | Dell Precision 3561           | 11th Gen Intel(R) Core(TM) i7-11800H @ 2.30GHz | AMD64  | Windows    | 23.852       | Core-i7-11800H                                               | 13.47 |
 | TC07                          | Intel(R) Core(TM) i7-9700K CPU @ 3.60GHz       | AMD64  | Windows    | 26.723       | Core-i7-9700K                                                | 9.45  |
 | WUYING: 8 vCPU / 16 GiB Linux | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64 | Linux      | 33.572       | [Xeon-Platinum-8163](https://versus.com/en/intel-xeon-gold-6126-vs-intel-xeon-platinum-8168) |       |
 | TC03<br />TC11                | Intel(R) Xeon(R) Gold 6248R CPU @ 3.00GHz      | AMD64  | Window     | 34.612       | Xeon-Gold-6248R                                              | 23.26 |
@@ -37,16 +48,14 @@
 
 
 
 ### GPU collection
 
 
 
-
-
 | id    | name                   | total memory | Synthetic benchmark | CUDA API |
 | ----- | ---------------------- | ------------ | ------------------- | -------- |
 | colab | Tesla T4               | 15360.0MB    | 28.16               | 70627    |
 | dell  | NVIDIA T600 Laptop GPU | 4096.0MB     | 16.69               | 26600    |
```

### Comparing `nodespecs-0.0.2/pyproject.toml` & `nodespecs-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nodespecs"
-version = "0.0.2"
+version = "0.0.3"
 description = "The specs summarize utilities for computer instance"
 readme = "README.md"
 authors = [{ name = "jinsanity", email = "jinsanityff@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -18,15 +18,15 @@
 ]
 keywords = ["cpu", "gpu", "benchmark"]
 dependencies = [
     "psutil >= 5.9.5",
     "tabulate >= 0.9.0",
     'tomli; python_version < "3.11"',
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.6"
 
 [project.optional-dependencies]
 dev = ["GPUtil","pip-tools"]
 
 [project.urls]
 Homepage = "https://github.com/jinsanity07git/hardwareSummary"
```

### Comparing `nodespecs-0.0.2/src/nodespecs.egg-info/PKG-INFO` & `nodespecs-0.0.3/src/nodespecs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodespecs
-Version: 0.0.2
+Version: 0.0.3
 Summary: The specs summarize utilities for computer instance
 Author-email: jinsanity <jinsanityff@gmail.com>
 License: The MIT License (MIT)
         Copyright © 2024 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -12,27 +12,38 @@
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Project-URL: Homepage, https://github.com/jinsanity07git/hardwareSummary
 Keywords: cpu,gpu,benchmark
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: psutil>=5.9.5
 Requires-Dist: tabulate>=0.9.0
 Requires-Dist: tomli; python_version < "3.11"
 Provides-Extra: dev
 Requires-Dist: GPUtil; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 
 # hardwareSummary
 Extracting and Fetching all system and hardware information such as os details, CPU and GPU information, disk and network usage in Python using platform, psutil and gputil libraries.
 
+
+
+### install and use with pip
+
+```shell
+pip install node-specs
+python -m specs
+```
+
+#### Deprecated  (install and use with git)
+
 ```
 !git clone https://github.com/jinsanity07git/hardwareSummary && python hardwareSummary/hardware.py && python hardwareSummary/cpu-benchmark.py
 
 ```
 
 ```cmd
 git clone https://github.com/jinsanity07git/hardwareSummary && python hardwareSummary/hardware.py && python hardwareSummary/cpu-benchmark.py
@@ -45,15 +56,15 @@
 git clone https://github.com/jinsanity07git/hardwareSummary && python3 hardwareSummary/hardware.py && python3 hardwareSummary/cpu-benchmark.py
 ```
 
 
 
 ### CPU collection
 
-| Brand                         | CPU                                            | Arch   | OS         | Benchmarking | Comb                                                         | Score |
+| Nickname                      | CPU                                            | Arch   | OS         | Benchmarking | Comb                                                         | Score |
 | ----------------------------- | ---------------------------------------------- | ------ | ---------- | ------------ | ------------------------------------------------------------ | ----- |
 | TC17<br />TC16                | Intel(R) Core(TM) i9-14900KF                   | AMD64  | Windows    | 15.654       | Core-i9-14900KF                                              | 39.25 |
 | TC14                          | 13th Gen Intel(R) Core(TM) i9-13900K           | AMD64  | Windows 10 | 12.991       | Core-i9-13900K                                               | 38.76 |
 | Dell Precision 3561           | 11th Gen Intel(R) Core(TM) i7-11800H @ 2.30GHz | AMD64  | Windows    | 23.852       | Core-i7-11800H                                               | 13.47 |
 | TC07                          | Intel(R) Core(TM) i7-9700K CPU @ 3.60GHz       | AMD64  | Windows    | 26.723       | Core-i7-9700K                                                | 9.45  |
 | WUYING: 8 vCPU / 16 GiB Linux | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64 | Linux      | 33.572       | [Xeon-Platinum-8163](https://versus.com/en/intel-xeon-gold-6126-vs-intel-xeon-platinum-8168) |       |
 | TC03<br />TC11                | Intel(R) Xeon(R) Gold 6248R CPU @ 3.00GHz      | AMD64  | Window     | 34.612       | Xeon-Gold-6248R                                              | 23.26 |
@@ -65,16 +76,14 @@
 
 
 
 ### GPU collection
 
 
 
-
-
 | id    | name                   | total memory | Synthetic benchmark | CUDA API |
 | ----- | ---------------------- | ------------ | ------------------- | -------- |
 | colab | Tesla T4               | 15360.0MB    | 28.16               | 70627    |
 | dell  | NVIDIA T600 Laptop GPU | 4096.0MB     | 16.69               | 26600    |
```

### Comparing `nodespecs-0.0.2/src/specs/cpu-benchmark.py` & `nodespecs-0.0.3/src/specs/cpu-benchmark.py`

 * *Files identical despite different names*

### Comparing `nodespecs-0.0.2/src/specs/cpuinfo.py` & `nodespecs-0.0.3/src/specs/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `nodespecs-0.0.2/src/specs/hardware.py` & `nodespecs-0.0.3/src/specs/hardware.py`

 * *Files identical despite different names*

