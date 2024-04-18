# Comparing `tmp/nullspace_optimizer-1.2.2-py3-none-any.whl.zip` & `tmp/nullspace_optimizer-1.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 21385 bytes, number of entries: 10
+Zip file size: 21303 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx     1107 b- defN 23-Nov-07 08:38 nullspace_optimizer/__init__.py
 -rw-rw-r--  2.0 unx     6649 b- defN 24-Feb-23 09:54 nullspace_optimizer/inout.py
--rw-rw-r--  2.0 unx     6240 b- defN 23-Nov-07 08:38 nullspace_optimizer/utils.py
+-rw-rw-r--  2.0 unx     6240 b- defN 24-Apr-18 07:48 nullspace_optimizer/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-02 14:40 nullspace_optimizer/examples/__init__.py
 -rw-rw-r--  2.0 unx      241 b- defN 24-Feb-22 16:16 nullspace_optimizer/examples/run_all.py
--rw-r--r--  2.0 unx    35149 b- defN 24-Feb-23 13:11 nullspace_optimizer-1.2.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3904 b- defN 24-Feb-23 13:11 nullspace_optimizer-1.2.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Feb-23 13:11 nullspace_optimizer-1.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 24-Feb-23 13:11 nullspace_optimizer-1.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      894 b- defN 24-Feb-23 13:11 nullspace_optimizer-1.2.2.dist-info/RECORD
-10 files, 54296 bytes uncompressed, 19833 bytes compressed:  63.5%
+-rw-r--r--  2.0 unx    35149 b- defN 24-Apr-18 08:43 nullspace_optimizer-1.2.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3746 b- defN 24-Apr-18 08:43 nullspace_optimizer-1.2.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-18 08:43 nullspace_optimizer-1.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 24-Apr-18 08:43 nullspace_optimizer-1.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      894 b- defN 24-Apr-18 08:43 nullspace_optimizer-1.2.3.dist-info/RECORD
+10 files, 54138 bytes uncompressed, 19751 bytes compressed:  63.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: nullspace_optimizer/examples/__init__.py
 Comment: 
 
 Filename: nullspace_optimizer/examples/run_all.py
 Comment: 
 
-Filename: nullspace_optimizer-1.2.2.dist-info/LICENSE
+Filename: nullspace_optimizer-1.2.3.dist-info/LICENSE
 Comment: 
 
-Filename: nullspace_optimizer-1.2.2.dist-info/METADATA
+Filename: nullspace_optimizer-1.2.3.dist-info/METADATA
 Comment: 
 
-Filename: nullspace_optimizer-1.2.2.dist-info/WHEEL
+Filename: nullspace_optimizer-1.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: nullspace_optimizer-1.2.2.dist-info/top_level.txt
+Filename: nullspace_optimizer-1.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: nullspace_optimizer-1.2.2.dist-info/RECORD
+Filename: nullspace_optimizer-1.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `nullspace_optimizer-1.2.2.dist-info/LICENSE` & `nullspace_optimizer-1.2.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `nullspace_optimizer-1.2.2.dist-info/METADATA` & `nullspace_optimizer-1.2.3.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: nullspace-optimizer
-Version: 1.2.2
+Version: 1.2.3
 Summary: Null space algorithm for nonlinear constrained optimization
 Home-page: https://null-space-optimizer.readthedocs.io/en/latest/
 Author: Florian Feppon
 Author-email: florian.feppon@kuleuven.be
 License: GNU GPL version 3
 Keywords: nonlinear constrained optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy >=1.26.4
 Requires-Dist: scipy >=1.11.4
 Requires-Dist: matplotlib >=3.8.3
 Requires-Dist: cvxopt >=1.3.2
 Requires-Dist: osqp >=0.6.2
@@ -67,18 +67,17 @@
 Please cite either of the following references when using this source:
 
 > Feppon F., Allaire G. and Dapogny C. *Null space gradient flows for
 > constrained optimization with applications to shape optimization.*
 > 2020. ESAIM: COCV, 26 90
 > [doi:10.1051/cocv/2020015](https://doi.org/10.1051/cocv/2020015)
 
-> Feppon F. *Density based topology optimization with the Null Space
-> Optimizer: a tutorial and a comparison* (2023). Submitted. HAL
-> preprint
-> [hal-04155507](https://hal.archives-ouvertes.fr/hal-04155507/document).
+> Feppon F. *Density based topology optimization with the Null Space Optimizer: a
+> tutorial and a comparison* (2024).   
+> [Structural and Multidisciplinary Optimization, 67(4), 1-34](https://link.springer.com/article/10.1007/s00158-023-03710-w).
 
 ``` bibtex
 @article{feppon2020optim,
    author = {{Feppon, F.} and {Allaire, G.} and {Dapogny, C.}},
    doi = {10.1051/cocv/2020015},
    journal = {ESAIM: COCV},
    pages = {90},
@@ -86,25 +85,24 @@
    url = {https://doi.org/10.1051/cocv/2020015},
    volume = 26,
    year = 2020
 }
 ```
 
 ``` bibtex
-@unpublished{feppon:hal-04155507,
-   TITLE = {{Density based topology optimization  with the Null Space Optimizer: a tutorial and a comparison}},
-   AUTHOR = {Feppon, F},
-   URL = {https://hal.science/hal-04155507},
-   NOTE = {working paper or preprint},
-   YEAR = {2023},
-   MONTH = Jul,
-   KEYWORDS = {Nonlinear constrained optimization ; density based topology optimization ; Null space gradient flows ; Python},
-   PDF = {https://hal.science/hal-04155507/file/bound_constraints%20%281%29.pdf},
-   HAL_ID = {hal-04155507},
-   HAL_VERSION = {v1},
+@article{Feppon2024density,
+  title     = "Density-based topology optimization with the Null Space Optimizer: a tutorial and a comparison",
+  author    = "Feppon, Florian",
+  journal   = "Structural and Multidisciplinary Optimization",
+  publisher = "Springer",
+  volume    =  67,
+  number    =  1,
+  pages     = "1--34",
+  month     =  jan,
+  year      =  2024
 }
 ```
 
 ## Licence
 
 The Null Space Optimizer is a free software distributed under the terms
 of the GNU General Public Licence
```

