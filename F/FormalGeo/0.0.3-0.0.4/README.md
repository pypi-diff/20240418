# Comparing `tmp/FormalGeo-0.0.3.tar.gz` & `tmp/formalgeo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FormalGeo-0.0.3.tar", last modified: Wed Jan  3 07:52:43 2024, max compression
+gzip compressed data, was "formalgeo-0.0.4.tar", last modified: Thu Apr 18 04:47:04 2024, max compression
```

## Comparing `FormalGeo-0.0.3.tar` & `formalgeo-0.0.4.tar`

### file list

```diff
@@ -1,43 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-01-03 07:52:43.512161 FormalGeo-0.0.3/
--rw-rw-rw-   0        0        0     2825 2023-11-06 06:56:17.000000 FormalGeo-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     6219 2024-01-03 07:52:43.512161 FormalGeo-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5491 2024-01-03 07:50:58.000000 FormalGeo-0.0.3/README.md
--rw-rw-rw-   0        0        0      788 2024-01-03 07:41:44.000000 FormalGeo-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-03 07:52:43.512161 FormalGeo-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-03 07:52:43.186112 FormalGeo-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-01-03 07:52:43.512161 FormalGeo-0.0.3/src/FormalGeo.egg-info/
--rw-rw-rw-   0        0        0     6219 2024-01-03 07:52:43.000000 FormalGeo-0.0.3/src/FormalGeo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      918 2024-01-03 07:52:43.000000 FormalGeo-0.0.3/src/FormalGeo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-03 07:52:43.000000 FormalGeo-0.0.3/src/FormalGeo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2024-01-03 07:52:43.000000 FormalGeo-0.0.3/src/FormalGeo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-01-03 07:52:43.000000 FormalGeo-0.0.3/src/FormalGeo.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-01-03 07:52:43.248566 FormalGeo-0.0.3/src/formalgeo/
--rw-rw-rw-   0        0        0      270 2023-12-21 13:40:21.000000 FormalGeo-0.0.3/src/formalgeo/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-03 07:52:43.279860 FormalGeo-0.0.3/src/formalgeo/core/
--rw-rw-rw-   0        0        0      532 2023-11-10 12:01:44.000000 FormalGeo-0.0.3/src/formalgeo/core/__init__.py
--rw-rw-rw-   0        0        0    38257 2023-12-26 05:47:36.000000 FormalGeo-0.0.3/src/formalgeo/core/engine.py
-drwxrwxrwx   0        0        0        0 2024-01-03 07:52:43.314630 FormalGeo-0.0.3/src/formalgeo/data/
--rw-rw-rw-   0        0        0      425 2023-11-10 12:01:44.000000 FormalGeo-0.0.3/src/formalgeo/data/__init__.py
--rw-rw-rw-   0        0        0    12468 2023-12-29 05:59:28.000000 FormalGeo-0.0.3/src/formalgeo/data/data.py
-drwxrwxrwx   0        0        0        0 2024-01-03 07:52:43.355766 FormalGeo-0.0.3/src/formalgeo/parse/
--rw-rw-rw-   0        0        0      980 2023-11-10 12:01:44.000000 FormalGeo-0.0.3/src/formalgeo/parse/__init__.py
--rw-rw-rw-   0        0        0     8491 2023-11-02 12:13:07.000000 FormalGeo-0.0.3/src/formalgeo/parse/basic.py
--rw-rw-rw-   0        0        0     5907 2023-11-03 02:36:11.000000 FormalGeo-0.0.3/src/formalgeo/parse/inverse_parse_m2f.py
--rw-rw-rw-   0        0        0     4333 2023-11-02 12:03:23.000000 FormalGeo-0.0.3/src/formalgeo/parse/parse_cdl.py
--rw-rw-rw-   0        0        0     4935 2023-11-02 12:03:23.000000 FormalGeo-0.0.3/src/formalgeo/parse/parse_pgdl.py
--rw-rw-rw-   0        0        0    10893 2023-12-23 09:51:21.000000 FormalGeo-0.0.3/src/formalgeo/parse/parse_tgdl.py
-drwxrwxrwx   0        0        0        0 2024-01-03 07:52:43.371574 FormalGeo-0.0.3/src/formalgeo/problem/
--rw-rw-rw-   0        0        0      439 2023-11-10 12:01:44.000000 FormalGeo-0.0.3/src/formalgeo/problem/__init__.py
--rw-rw-rw-   0        0        0     7952 2023-11-03 03:17:50.000000 FormalGeo-0.0.3/src/formalgeo/problem/condition.py
--rw-rw-rw-   0        0        0    33071 2023-12-26 06:17:54.000000 FormalGeo-0.0.3/src/formalgeo/problem/problem.py
-drwxrwxrwx   0        0        0        0 2024-01-03 07:52:43.402813 FormalGeo-0.0.3/src/formalgeo/solver/
--rw-rw-rw-   0        0        0      666 2023-11-10 12:01:44.000000 FormalGeo-0.0.3/src/formalgeo/solver/__init__.py
--rw-rw-rw-   0        0        0    28738 2023-11-30 07:11:44.000000 FormalGeo-0.0.3/src/formalgeo/solver/backward_search.py
--rw-rw-rw-   0        0        0    19452 2023-12-23 09:31:47.000000 FormalGeo-0.0.3/src/formalgeo/solver/forward_search.py
--rw-rw-rw-   0        0        0    12057 2023-12-26 05:40:04.000000 FormalGeo-0.0.3/src/formalgeo/solver/interactive.py
-drwxrwxrwx   0        0        0        0 2024-01-03 07:52:43.465200 FormalGeo-0.0.3/src/formalgeo/tools/
--rw-rw-rw-   0        0        0      889 2023-12-26 13:29:25.000000 FormalGeo-0.0.3/src/formalgeo/tools/__init__.py
--rw-rw-rw-   0        0        0    16575 2023-12-29 07:29:27.000000 FormalGeo-0.0.3/src/formalgeo/tools/output.py
--rw-rw-rw-   0        0        0     1396 2023-11-19 02:20:51.000000 FormalGeo-0.0.3/src/formalgeo/tools/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-03 07:52:43.465200 FormalGeo-0.0.3/tests/
--rw-rw-rw-   0        0        0    20813 2024-01-03 06:14:22.000000 FormalGeo-0.0.3/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-04-18 04:47:04.550917 formalgeo-0.0.4/
+-rw-rw-rw-   0        0        0     2825 2024-04-16 10:38:21.000000 formalgeo-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     5475 2024-04-18 04:47:04.549889 formalgeo-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4747 2024-04-18 04:36:20.000000 formalgeo-0.0.4/README.md
+-rw-rw-rw-   0        0        0      788 2024-04-18 04:35:10.000000 formalgeo-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-18 04:47:04.550917 formalgeo-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-18 04:47:04.507176 formalgeo-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-18 04:47:04.549889 formalgeo-0.0.4/src/FormalGeo.egg-info/
+-rw-rw-rw-   0        0        0     5475 2024-04-18 04:47:04.000000 formalgeo-0.0.4/src/FormalGeo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      904 2024-04-18 04:47:04.000000 formalgeo-0.0.4/src/FormalGeo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 04:47:04.000000 formalgeo-0.0.4/src/FormalGeo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2024-04-18 04:47:04.000000 formalgeo-0.0.4/src/FormalGeo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-18 04:47:04.000000 formalgeo-0.0.4/src/FormalGeo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 04:47:04.534032 formalgeo-0.0.4/src/formalgeo/
+-rw-rw-rw-   0        0        0      295 2024-04-18 04:35:10.000000 formalgeo-0.0.4/src/formalgeo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 04:47:04.535440 formalgeo-0.0.4/src/formalgeo/core/
+-rw-rw-rw-   0        0        0      532 2024-01-12 04:53:44.000000 formalgeo-0.0.4/src/formalgeo/core/__init__.py
+-rw-rw-rw-   0        0        0    38257 2023-12-26 05:47:38.000000 formalgeo-0.0.4/src/formalgeo/core/engine.py
+drwxrwxrwx   0        0        0        0 2024-04-18 04:47:04.536648 formalgeo-0.0.4/src/formalgeo/data/
+-rw-rw-rw-   0        0        0      425 2024-01-12 04:53:44.000000 formalgeo-0.0.4/src/formalgeo/data/__init__.py
+-rw-rw-rw-   0        0        0     9768 2024-04-18 04:39:54.000000 formalgeo-0.0.4/src/formalgeo/data/data.py
+drwxrwxrwx   0        0        0        0 2024-04-18 04:47:04.541695 formalgeo-0.0.4/src/formalgeo/parse/
+-rw-rw-rw-   0        0        0      980 2024-01-12 04:53:44.000000 formalgeo-0.0.4/src/formalgeo/parse/__init__.py
+-rw-rw-rw-   0        0        0     8491 2024-04-16 10:38:21.000000 formalgeo-0.0.4/src/formalgeo/parse/basic.py
+-rw-rw-rw-   0        0        0     5907 2024-04-16 10:38:21.000000 formalgeo-0.0.4/src/formalgeo/parse/inverse_parse_m2f.py
+-rw-rw-rw-   0        0        0     4333 2024-04-16 10:38:21.000000 formalgeo-0.0.4/src/formalgeo/parse/parse_cdl.py
+-rw-rw-rw-   0        0        0     4935 2024-04-16 10:38:21.000000 formalgeo-0.0.4/src/formalgeo/parse/parse_pgdl.py
+-rw-rw-rw-   0        0        0    10893 2024-04-16 10:38:21.000000 formalgeo-0.0.4/src/formalgeo/parse/parse_tgdl.py
+drwxrwxrwx   0        0        0        0 2024-04-18 04:47:04.543912 formalgeo-0.0.4/src/formalgeo/problem/
+-rw-rw-rw-   0        0        0      439 2024-01-12 04:53:44.000000 formalgeo-0.0.4/src/formalgeo/problem/__init__.py
+-rw-rw-rw-   0        0        0     7952 2024-04-16 10:38:21.000000 formalgeo-0.0.4/src/formalgeo/problem/condition.py
+-rw-rw-rw-   0        0        0    33071 2024-04-16 10:38:21.000000 formalgeo-0.0.4/src/formalgeo/problem/problem.py
+drwxrwxrwx   0        0        0        0 2024-04-18 04:47:04.546426 formalgeo-0.0.4/src/formalgeo/solver/
+-rw-rw-rw-   0        0        0      666 2024-01-12 04:53:44.000000 formalgeo-0.0.4/src/formalgeo/solver/__init__.py
+-rw-rw-rw-   0        0        0    28738 2024-04-16 10:38:21.000000 formalgeo-0.0.4/src/formalgeo/solver/backward_search.py
+-rw-rw-rw-   0        0        0    19452 2024-04-16 10:38:21.000000 formalgeo-0.0.4/src/formalgeo/solver/forward_search.py
+-rw-rw-rw-   0        0        0    12057 2024-04-16 10:38:21.000000 formalgeo-0.0.4/src/formalgeo/solver/interactive.py
+drwxrwxrwx   0        0        0        0 2024-04-18 04:47:04.548738 formalgeo-0.0.4/src/formalgeo/tools/
+-rw-rw-rw-   0        0        0      889 2024-01-12 04:53:44.000000 formalgeo-0.0.4/src/formalgeo/tools/__init__.py
+-rw-rw-rw-   0        0        0    16575 2024-04-16 10:38:21.000000 formalgeo-0.0.4/src/formalgeo/tools/output.py
+-rw-rw-rw-   0        0        0     1396 2024-04-16 10:38:21.000000 formalgeo-0.0.4/src/formalgeo/tools/utils.py
```

### Comparing `FormalGeo-0.0.3/LICENSE` & `formalgeo-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `FormalGeo-0.0.3/PKG-INFO` & `formalgeo-0.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FormalGeo
-Version: 0.0.3
+Version: 0.0.4
 Summary: Formal representation and solving for Euclidean plane geometry problems.
 Author-email: Xiaokai Zhang <xiaokaizhang1999@163.com>
 Project-URL: Homepage, https://github.com/FormalGeo/FormalGeo
 Project-URL: Bug Tracker, https://github.com/FormalGeo/FormalGeo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 Requires-Dist: func-timeout>=4.3
 Requires-Dist: requests>=2.31
 Requires-Dist: tqdm>=4.66.1
 Requires-Dist: graphviz>=0.20.1
 
 # FormalGeo
 
-[![Version](https://img.shields.io/badge/Version-0.0.3-brightgreen)](https://github.com/FormalGeo/FormalGeo)
+[![Version](https://img.shields.io/badge/Version-0.0.4-brightgreen)](https://github.com/FormalGeo/FormalGeo)
 [![License](https://img.shields.io/badge/License-MIT-green)](https://opensource.org/licenses/MIT)
 [![Survey](https://img.shields.io/badge/Survey-FormalGeo-blue)](https://github.com/FormalGeo/FormalGeo)
 
 Formal representation and solving for Euclidean plane geometry problems. Our goal is to build a crucial bridge between
 IMO-level plane geometry challenges and readable AI automated reasoning.  
 More information about FormalGeo will be found in [homepage](https://formalgeo.github.io/). FormalGeo is in its early
 stages and brimming with potential. We welcome anyone to join us in this exciting endeavor.
@@ -86,31 +86,14 @@
 
 ## Bugs
 
 Our bug reporting platform is available at [here](https://github.com/FormalGeo/FormalGeo/issues). We encourage you to
 report any issues you encounter. Or even better, fork our repository on GitHub and submit a pull request. We appreciate
 contributions of all sizes and are happy to assist newcomers to git with their pull requests.
 
-## Related Projects
-
-**Datasets**  
-URL: https://github.com/FormalGeo/Datasets  
-Intro: This project is used for the design and release of geometry formal systems and datasets. It currently includes 2
-formal systems, GFS-BASIC and GFS-IMO, and the corresponding datasets formalgeo7k and formalgeo-imo.
-
-**FGPS**  
-URL: https://github.com/BitSecret/FGPS  
-Intro: This project has implemented an automated solving algorithm for geometric problems based on search, including
-forward search and backward search. FGPS is capable of adopting various search strategies, such as breadth-first search,
-depth-first search, random search and beam search.
-
-**FGeoDRL**  
-URL: https://github.com/PersonNoName/FGeoDRL
-Intro: coming soon...
-
 ## Citation
 
 To cite FormalGeo in publications use:
 > Xiaokai, Zhang., Na, Zhu., Yiming, He., Jia, Zou., ... & Tuo, Leng. (2023). FormalGeo: The First Step Toward
 > Human-like IMO-level Geometric Automated Reasoning. arXiv preprint arXiv:2310.18021.
 
 A BibTeX entry for LaTeX users is:
```

### Comparing `FormalGeo-0.0.3/README.md` & `formalgeo-0.0.4/src/FormalGeo.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,29 @@
+Metadata-Version: 2.1
+Name: FormalGeo
+Version: 0.0.4
+Summary: Formal representation and solving for Euclidean plane geometry problems.
+Author-email: Xiaokai Zhang <xiaokaizhang1999@163.com>
+Project-URL: Homepage, https://github.com/FormalGeo/FormalGeo
+Project-URL: Bug Tracker, https://github.com/FormalGeo/FormalGeo/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: sympy>=1.10
+Requires-Dist: func-timeout>=4.3
+Requires-Dist: requests>=2.31
+Requires-Dist: tqdm>=4.66.1
+Requires-Dist: graphviz>=0.20.1
+
 # FormalGeo
 
-[![Version](https://img.shields.io/badge/Version-0.0.3-brightgreen)](https://github.com/FormalGeo/FormalGeo)
+[![Version](https://img.shields.io/badge/Version-0.0.4-brightgreen)](https://github.com/FormalGeo/FormalGeo)
 [![License](https://img.shields.io/badge/License-MIT-green)](https://opensource.org/licenses/MIT)
 [![Survey](https://img.shields.io/badge/Survey-FormalGeo-blue)](https://github.com/FormalGeo/FormalGeo)
 
 Formal representation and solving for Euclidean plane geometry problems. Our goal is to build a crucial bridge between
 IMO-level plane geometry challenges and readable AI automated reasoning.  
 More information about FormalGeo will be found in [homepage](https://formalgeo.github.io/). FormalGeo is in its early
 stages and brimming with potential. We welcome anyone to join us in this exciting endeavor.
@@ -67,31 +86,14 @@
 
 ## Bugs
 
 Our bug reporting platform is available at [here](https://github.com/FormalGeo/FormalGeo/issues). We encourage you to
 report any issues you encounter. Or even better, fork our repository on GitHub and submit a pull request. We appreciate
 contributions of all sizes and are happy to assist newcomers to git with their pull requests.
 
-## Related Projects
-
-**Datasets**  
-URL: https://github.com/FormalGeo/Datasets  
-Intro: This project is used for the design and release of geometry formal systems and datasets. It currently includes 2
-formal systems, GFS-BASIC and GFS-IMO, and the corresponding datasets formalgeo7k and formalgeo-imo.
-
-**FGPS**  
-URL: https://github.com/BitSecret/FGPS  
-Intro: This project has implemented an automated solving algorithm for geometric problems based on search, including
-forward search and backward search. FGPS is capable of adopting various search strategies, such as breadth-first search,
-depth-first search, random search and beam search.
-
-**FGeoDRL**  
-URL: https://github.com/PersonNoName/FGeoDRL
-Intro: coming soon...
-
 ## Citation
 
 To cite FormalGeo in publications use:
 > Xiaokai, Zhang., Na, Zhu., Yiming, He., Jia, Zou., ... & Tuo, Leng. (2023). FormalGeo: The First Step Toward
 > Human-like IMO-level Geometric Automated Reasoning. arXiv preprint arXiv:2310.18021.
 
 A BibTeX entry for LaTeX users is:
@@ -104,8 +106,8 @@
 > eprint={2310.18021},  
 > archivePrefix={arXiv},  
 > primaryClass={cs.AI}  
 > }
 
 FormalGeo is MIT licensed, so you are free to use it whatever you like, be it academic, commercial, creating forks or
 derivatives, as long as you copy the MIT statement if you redistribute it (see the LICENSE file for details). That said,
-if it is convenient for you, please cite FormalGeo when using it in your work.
+if it is convenient for you, please cite FormalGeo when using it in your work.
```

### Comparing `FormalGeo-0.0.3/pyproject.toml` & `formalgeo-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "FormalGeo"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name = "Xiaokai Zhang", email = "xiaokaizhang1999@163.com" },
 ]
 description = "Formal representation and solving for Euclidean plane geometry problems."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `FormalGeo-0.0.3/src/FormalGeo.egg-info/PKG-INFO` & `formalgeo-0.0.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,10 @@
-Metadata-Version: 2.1
-Name: FormalGeo
-Version: 0.0.3
-Summary: Formal representation and solving for Euclidean plane geometry problems.
-Author-email: Xiaokai Zhang <xiaokaizhang1999@163.com>
-Project-URL: Homepage, https://github.com/FormalGeo/FormalGeo
-Project-URL: Bug Tracker, https://github.com/FormalGeo/FormalGeo/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: sympy>=1.10
-Requires-Dist: func-timeout>=4.3
-Requires-Dist: requests>=2.31
-Requires-Dist: tqdm>=4.66.1
-Requires-Dist: graphviz>=0.20.1
-
 # FormalGeo
 
-[![Version](https://img.shields.io/badge/Version-0.0.3-brightgreen)](https://github.com/FormalGeo/FormalGeo)
+[![Version](https://img.shields.io/badge/Version-0.0.4-brightgreen)](https://github.com/FormalGeo/FormalGeo)
 [![License](https://img.shields.io/badge/License-MIT-green)](https://opensource.org/licenses/MIT)
 [![Survey](https://img.shields.io/badge/Survey-FormalGeo-blue)](https://github.com/FormalGeo/FormalGeo)
 
 Formal representation and solving for Euclidean plane geometry problems. Our goal is to build a crucial bridge between
 IMO-level plane geometry challenges and readable AI automated reasoning.  
 More information about FormalGeo will be found in [homepage](https://formalgeo.github.io/). FormalGeo is in its early
 stages and brimming with potential. We welcome anyone to join us in this exciting endeavor.
@@ -86,31 +67,14 @@
 
 ## Bugs
 
 Our bug reporting platform is available at [here](https://github.com/FormalGeo/FormalGeo/issues). We encourage you to
 report any issues you encounter. Or even better, fork our repository on GitHub and submit a pull request. We appreciate
 contributions of all sizes and are happy to assist newcomers to git with their pull requests.
 
-## Related Projects
-
-**Datasets**  
-URL: https://github.com/FormalGeo/Datasets  
-Intro: This project is used for the design and release of geometry formal systems and datasets. It currently includes 2
-formal systems, GFS-BASIC and GFS-IMO, and the corresponding datasets formalgeo7k and formalgeo-imo.
-
-**FGPS**  
-URL: https://github.com/BitSecret/FGPS  
-Intro: This project has implemented an automated solving algorithm for geometric problems based on search, including
-forward search and backward search. FGPS is capable of adopting various search strategies, such as breadth-first search,
-depth-first search, random search and beam search.
-
-**FGeoDRL**  
-URL: https://github.com/PersonNoName/FGeoDRL
-Intro: coming soon...
-
 ## Citation
 
 To cite FormalGeo in publications use:
 > Xiaokai, Zhang., Na, Zhu., Yiming, He., Jia, Zou., ... & Tuo, Leng. (2023). FormalGeo: The First Step Toward
 > Human-like IMO-level Geometric Automated Reasoning. arXiv preprint arXiv:2310.18021.
 
 A BibTeX entry for LaTeX users is:
@@ -123,8 +87,8 @@
 > eprint={2310.18021},  
 > archivePrefix={arXiv},  
 > primaryClass={cs.AI}  
 > }
 
 FormalGeo is MIT licensed, so you are free to use it whatever you like, be it academic, commercial, creating forks or
 derivatives, as long as you copy the MIT statement if you redistribute it (see the LICENSE file for details). That said,
-if it is convenient for you, please cite FormalGeo when using it in your work.
+if it is convenient for you, please cite FormalGeo when using it in your work.
```

### Comparing `FormalGeo-0.0.3/src/FormalGeo.egg-info/SOURCES.txt` & `formalgeo-0.0.4/src/FormalGeo.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 src/formalgeo/problem/problem.py
 src/formalgeo/solver/__init__.py
 src/formalgeo/solver/backward_search.py
 src/formalgeo/solver/forward_search.py
 src/formalgeo/solver/interactive.py
 src/formalgeo/tools/__init__.py
 src/formalgeo/tools/output.py
-src/formalgeo/tools/utils.py
-tests/test.py
+src/formalgeo/tools/utils.py
```

### Comparing `FormalGeo-0.0.3/src/formalgeo/core/__init__.py` & `formalgeo-0.0.4/src/formalgeo/core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022-2023 FormalGeo Development Team
+# Copyright (C) 2022-2024 FormalGeo Development Team
 # Author: Xiaokai Zhang
 # Contact: formalgeo@gmail.com
 
 """
 'core' responsible for GPL statements executing, which consists of 2 submodules.
 'GeometryPredicateLogicExecutor' responsible for GPL statements parsing and relational inference.
 'EquationKiller' responsible for symbolic and algebraic computation.
```

### Comparing `FormalGeo-0.0.3/src/formalgeo/core/engine.py` & `formalgeo-0.0.4/src/formalgeo/core/engine.py`

 * *Files identical despite different names*

### Comparing `FormalGeo-0.0.3/src/formalgeo/data/data.py` & `formalgeo-0.0.4/src/formalgeo/data/data.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,34 +3,25 @@
 import requests
 from tqdm import tqdm
 import json
 import tarfile
 import shutil
 import random
 
-remote = "https://raw.githubusercontent.com/Formalgeo/Datasets/main/released/"
-
 
 def get_datasets_path(datasets_path):
     if datasets_path is None:
         datasets_path = os.path.join(os.path.dirname(os.path.dirname(os.path.abspath(__file__))), "datasets")
     if not os.path.exists(datasets_path):
         os.makedirs(datasets_path)
     return datasets_path
 
 
-def format_json(path_datasets):
-    for path, _, files in os.walk(path_datasets):
-        for file in files:
-            if file.endswith(".json"):  # format json
-                save_json(load_json(os.path.join(path, file)), os.path.join(path, file))
-
-
 def get_remote_datasets():
-    response = requests.get(os.path.join(remote, "released.json"))
+    response = requests.get("https://raw.githubusercontent.com/FormalGeo/Datasets/main/released.json")
     if response.status_code == 200:
         return json.loads(response.content)
     return None
 
 
 def get_local_datasets(datasets_path):
     local_datasets = {}
@@ -42,70 +33,63 @@
     return local_datasets
 
 
 def show_available_datasets(datasets_path=None):
     datasets_path = get_datasets_path(datasets_path)
     remote_datasets = get_remote_datasets()
     local_datasets = get_local_datasets(datasets_path)
-    text = "{0:<12}{1:<10}{2:<15}{3:<15}{4:<15}{5:<15}{6:<15}{7:<22}{8:}"
-    print(text.format("Location", "Status", "Name", "Version", "Formalgeo", "GDL", "GDL-Version", "Release", "Description"))
+    text = "{0:<12}{1:<10}{2:<20}{3:<15}{4:<15}{5:<15}{6:<22}{7:}"
+    print(text.format("Location", "Status", "Name", "Formalgeo", "GDL", "GDL-Version", "Release",
+                      "Description"))
 
     if remote_datasets is None:
         for dataset in local_datasets:
-            print(text.format("local", "U",
-                              local_datasets[dataset]["dataset_name"],
-                              local_datasets[dataset]["dataset_version"],
+            print(text.format("local", "-",
+                              dataset,
                               local_datasets[dataset]["formalgeo_version"],
                               local_datasets[dataset]["gdl_name"],
                               local_datasets[dataset]["gdl_version"],
                               local_datasets[dataset]["release_datetime"],
                               local_datasets[dataset]["short_description"]))
         print("\nFailed to get the remote datasets, displaying local datasets.")
         print("Please check your network connection and try again.")
         return
 
     for dataset in local_datasets:
         if dataset in remote_datasets:
             if local_datasets[dataset]["release_datetime"] == remote_datasets[dataset]["release_datetime"]:
-                status = "A"
+                status = "latest"
             else:
-                status = "B"
+                status = "old"
             print(text.format("local", status,
-                              local_datasets[dataset]["dataset_name"],
-                              local_datasets[dataset]["dataset_version"],
+                              dataset,
                               local_datasets[dataset]["formalgeo_version"],
                               local_datasets[dataset]["gdl_name"],
                               local_datasets[dataset]["gdl_version"],
                               local_datasets[dataset]["release_datetime"],
                               local_datasets[dataset]["short_description"]))
         else:
-            print(text.format("local", "C",
-                              local_datasets[dataset]["dataset_name"],
-                              local_datasets[dataset]["dataset_version"],
+            print(text.format("local", "-",
+                              dataset,
                               local_datasets[dataset]["formalgeo_version"],
                               local_datasets[dataset]["gdl_name"],
                               local_datasets[dataset]["gdl_version"],
                               local_datasets[dataset]["release_datetime"],
                               local_datasets[dataset]["short_description"]))
 
     for dataset in remote_datasets:
-        print(text.format("remote", "R",
-                          remote_datasets[dataset]["dataset_name"],
-                          remote_datasets[dataset]["dataset_version"],
+        print(text.format("remote", "-",
+                          dataset,
                           remote_datasets[dataset]["formalgeo_version"],
                           remote_datasets[dataset]["gdl_name"],
                           remote_datasets[dataset]["gdl_version"],
                           remote_datasets[dataset]["release_datetime"],
                           remote_datasets[dataset]["short_description"]))
 
-    print("\n<A> indicates that the local version is in sync with the remote version.")
-    print("<B> indicates the remote dataset has updates.")
-    print("<C> represents the local dataset not in the remote repository.")
-    print("<D> represents the remote dataset that can be downloaded.")
-    print("<R> represents the remote datasets.")
+    print()
     print("Run 'formalgeo.data.download_dataset()' to download the remote dataset.")
 
 
 def download_dataset(dataset_name, datasets_path=None):
     datasets_path = get_datasets_path(datasets_path)
     remote_datasets = get_remote_datasets()
     local_datasets = get_local_datasets(datasets_path)
@@ -122,15 +106,15 @@
     if dataset_name in local_datasets:
         if local_datasets[dataset_name]["release_datetime"] == remote_datasets[dataset_name]["release_datetime"]:
             print("Datasets '{}' already exits in '{}'.".format(dataset_name, datasets_path))
             if get_user_input("Do you want to update?") == "n":
                 return False
         remove_dataset(dataset_name, datasets_path)
 
-    response = requests.get(os.path.join(remote, "{}.tar.gz".format(dataset_name)), stream=True)
+    response = requests.get(remote_datasets[dataset_name]["downloads"], stream=True)
     if response.status_code == 200:
         pbar = tqdm(
             total=int(response.headers.get('content-length', 0)),
             unit='iB',
             unit_scale=True,
             desc="Download dataset '{}'".format(dataset_name)
         )
@@ -140,97 +124,75 @@
                 file.write(data)
         pbar.close()
 
         print("Extracting files ...")
         with tarfile.open(os.path.join(datasets_path, "{}.tar.gz".format(dataset_name)), "r:gz") as tar_file:  # extract
             tar_file.extractall(os.path.join(datasets_path, dataset_name))
 
-        format_json(os.path.join(datasets_path, dataset_name))
-
         shutil.copy(os.path.join(datasets_path, dataset_name, "info.json"),
                     os.path.join(datasets_path, "{}.json".format(dataset_name)))
 
         os.remove(os.path.join(datasets_path, "{}.tar.gz".format(dataset_name)))
 
         return True
 
-    msg = "Network error. Fail to download '{}'.".format(
-        os.path.join(remote, os.path.join(remote, "{}.tar.gz".format(dataset_name))))
-    raise Exception(msg)
+    raise Exception("Network error. Fail to download '{}'.".format(remote_datasets[dataset_name]["downloads"]))
 
 
 def remove_dataset(dataset_name, datasets_path=None):
     datasets_path = get_datasets_path(datasets_path)
     local_datasets = get_local_datasets(datasets_path)
 
     if dataset_name not in local_datasets:
         print("No dataset '{}' in '{}'. please check your inputs.".format(dataset_name, datasets_path))
         return
 
     print("Removing dataset '{}'...".format(dataset_name))
     if os.path.isdir(os.path.join(datasets_path, dataset_name)):
-        shutil.rmtree(os.path.join(datasets_path, dataset_name), ignore_errors=True)
+        shutil.rmtree(os.path.join(datasets_path, dataset_name), ignore_errors=True)  # json文件也要移除吧
+        os.remove(os.path.join(datasets_path, f"{dataset_name}.json"))
 
 
 class DatasetLoader:
 
     def __init__(self, dataset_name, datasets_path=None):
         datasets_path = get_datasets_path(datasets_path)
         local_datasets = get_local_datasets(datasets_path)
         if dataset_name not in local_datasets:
-            msg = "No dataset dir named '{}'. run 'formalgeo.data.show_available_datasets()' for more info.".format(
+            msg = "No dataset named '{}'. run 'formalgeo.data.show_available_datasets()' for more info.".format(
                 dataset_name)
             raise Exception(msg)
 
         self.dataset_path = os.path.join(datasets_path, dataset_name)
 
         self.info = load_json(os.path.join(self.dataset_path, "info.json"))
         self.predicate_GDL = load_json(os.path.join(self.dataset_path, "gdl", "predicate_GDL.json"))
         self.theorem_GDL = load_json(os.path.join(self.dataset_path, "gdl", "theorem_GDL.json"))
-        self.pid_mapping = self.load_file("pid_mapping.json")
 
     def show(self):
         for item in self.info:
             print("{}: {}".format(item, self.info[item]))
         print("dataset_path: {}".format(self.dataset_path))
         print("files: {}".format(os.listdir(os.path.join(self.dataset_path, "files"))))
 
     def get_problem(self, pid):
         if pid <= self.info["problem_number"]:
-            return load_json(os.path.join(self.dataset_path, "problems", "{}.json".format(pid)))
-        elif pid <= self.info["expanded_problem_number"]:
-            raw_pid = self.pid_mapping[str(pid)]
-            raw_problem = load_json(os.path.join(self.dataset_path, "problems", "{}.json".format(raw_pid)))
-            expanded = load_json(os.path.join(self.dataset_path, "expanded", "{}.json".format(raw_pid)))[str(pid)]
-            raw_problem["problem_id"] = expanded["problem_id"]
-            raw_problem["text_cdl"] += expanded["added_cdl"]
-            raw_problem["goal_cdl"] = expanded["goal_cdl"]
-            raw_problem["problem_answer"] = expanded["problem_answer"]
-            raw_problem["theorem_seqs"] = expanded["theorem_seqs"]
-            raw_problem["theorem_seqs_dag"] = expanded["theorem_seqs_dag"]
-            raw_problem["problem_level"] = len(expanded["theorem_seqs"])
-            return raw_problem
+            return load_json(os.path.join(self.dataset_path, "problems", f"{pid}.json"))
         else:
             msg = "No problem named {}.".format(pid)
             raise Exception(msg)
 
-    def get_problem_split(self, expanded=False):
+    def get_problem_split(self, split_msg=None):
         file_path = os.path.join(self.dataset_path, "files")
-        if expanded:
-            split_msg = self.info["expanded_problem_split"]
-            filename = "expanded_problem_split_{}_{}_{}_{}.json".format(
-                split_msg[0], split_msg[1], split_msg[2], split_msg[3]
-            )
-            problem_number = self.info["expanded_problem_number"]
-        else:
+
+        if split_msg is None:
             split_msg = self.info["problem_split"]
-            filename = "problem_split_{}_{}_{}_{}.json".format(
-                split_msg[0], split_msg[1], split_msg[2], split_msg[3]
-            )
-            problem_number = self.info["problem_number"]
+
+        filename = f"problem_split_{split_msg[0]}_{split_msg[1]}_{split_msg[2]}_{split_msg[3]}.json"
+        problem_number = self.info["problem_number"]
 
         if filename in os.listdir(file_path):
             return load_json(os.path.join(file_path, filename))
 
         total = split_msg[0] + split_msg[1] + split_msg[2]
         random.seed(split_msg[3])
         data = list(range(1, problem_number + 1))
@@ -260,22 +222,12 @@
             }
         }
 
         save_json(data, os.path.join(file_path, filename))
 
         return data
 
-    def load_file(self, filename):
-        file_path = os.path.join(self.dataset_path, "files")
-        if filename not in os.listdir(file_path):
-            msg = "No file named {} in {}.".format(filename, file_path)
-            raise Exception(msg)
-
-        if filename.endswith(".json"):
-            return load_json(os.path.join(file_path, filename))
-        else:
-            with open(os.path.join(file_path, filename)) as f:
-                return f.read()
-
 
 if __name__ == '__main__':
-    show_available_datasets("F:/test/datasets")
+    show_available_datasets("D:/Projects/dataset")
+    # download_dataset("formalgeo7k_v1", "D:/Projects/dataset")
+    # remove_dataset("formalgeo7k_v1", "D:/Projects/dataset")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `FormalGeo-0.0.3/src/formalgeo/parse/__init__.py` & `formalgeo-0.0.4/src/formalgeo/parse/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022-2023 FormalGeo Development Team
+# Copyright (C) 2022-2024 FormalGeo Development Team
 # Author: Xiaokai Zhang
 # Contact: formalgeo@gmail.com
 
 """
 'parse' responsible for statements parsing and inverse parsing, building a bridge
 between natural language, formal language, and machine language.
 """
```

### Comparing `FormalGeo-0.0.3/src/formalgeo/parse/basic.py` & `formalgeo-0.0.4/src/formalgeo/parse/basic.py`

 * *Files identical despite different names*

### Comparing `FormalGeo-0.0.3/src/formalgeo/parse/inverse_parse_m2f.py` & `formalgeo-0.0.4/src/formalgeo/parse/inverse_parse_m2f.py`

 * *Files identical despite different names*

### Comparing `FormalGeo-0.0.3/src/formalgeo/parse/parse_cdl.py` & `formalgeo-0.0.4/src/formalgeo/parse/parse_cdl.py`

 * *Files identical despite different names*

### Comparing `FormalGeo-0.0.3/src/formalgeo/parse/parse_pgdl.py` & `formalgeo-0.0.4/src/formalgeo/parse/parse_pgdl.py`

 * *Files identical despite different names*

### Comparing `FormalGeo-0.0.3/src/formalgeo/parse/parse_tgdl.py` & `formalgeo-0.0.4/src/formalgeo/parse/parse_tgdl.py`

 * *Files identical despite different names*

### Comparing `FormalGeo-0.0.3/src/formalgeo/problem/condition.py` & `formalgeo-0.0.4/src/formalgeo/problem/condition.py`

 * *Files identical despite different names*

### Comparing `FormalGeo-0.0.3/src/formalgeo/problem/problem.py` & `formalgeo-0.0.4/src/formalgeo/problem/problem.py`

 * *Files identical despite different names*

### Comparing `FormalGeo-0.0.3/src/formalgeo/solver/__init__.py` & `formalgeo-0.0.4/src/formalgeo/solver/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022-2023 FormalGeo Development Team
+# Copyright (C) 2022-2024 FormalGeo Development Team
 # Author: Xiaokai Zhang
 # Contact: formalgeo@gmail.com
 
 """
 'solver' invokes other modules to enable interactive problem-solving and automated problem-solving.
 The automated problem-solving implements both forward search and backward search, allowing for the
 configuration of various search strategies (breadth-first, depth-first, random, beam).
```

### Comparing `FormalGeo-0.0.3/src/formalgeo/solver/backward_search.py` & `formalgeo-0.0.4/src/formalgeo/solver/backward_search.py`

 * *Files identical despite different names*

### Comparing `FormalGeo-0.0.3/src/formalgeo/solver/forward_search.py` & `formalgeo-0.0.4/src/formalgeo/solver/forward_search.py`

 * *Files identical despite different names*

### Comparing `FormalGeo-0.0.3/src/formalgeo/solver/interactive.py` & `formalgeo-0.0.4/src/formalgeo/solver/interactive.py`

 * *Files identical despite different names*

### Comparing `FormalGeo-0.0.3/src/formalgeo/tools/__init__.py` & `formalgeo-0.0.4/src/formalgeo/tools/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022-2023 FormalGeo Development Team
+# Copyright (C) 2022-2024 FormalGeo Development Team
 # Author: Xiaokai Zhang
 # Contact: formalgeo@gmail.com
 
 """
 'tools' provides some practical tools, such as problem-solving process outputting.
 """
```

### Comparing `FormalGeo-0.0.3/src/formalgeo/tools/output.py` & `formalgeo-0.0.4/src/formalgeo/tools/output.py`

 * *Files identical despite different names*

### Comparing `FormalGeo-0.0.3/src/formalgeo/tools/utils.py` & `formalgeo-0.0.4/src/formalgeo/tools/utils.py`

 * *Files identical despite different names*

