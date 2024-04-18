# Comparing `tmp/anclib-0.9.1.tar.gz` & `tmp/anclib-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anclib-0.9.1.tar", last modified: Fri Sep 15 20:11:18 2023, max compression
+gzip compressed data, was "anclib-0.9.2.tar", last modified: Mon Sep 18 15:19:46 2023, max compression
```

## Comparing `anclib-0.9.1.tar` & `anclib-0.9.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 agpe       (502) staff       (20)        0 2023-09-15 20:11:18.957196 anclib-0.9.1/
--rw-r--r--   0 agpe       (502) staff       (20)    35149 2022-11-10 12:08:59.000000 anclib-0.9.1/LICENSE
--rw-r--r--   0 agpe       (502) staff       (20)     2260 2023-09-15 20:11:18.957114 anclib-0.9.1/PKG-INFO
--rw-r--r--   0 agpe       (502) staff       (20)     1591 2023-09-15 20:09:03.000000 anclib-0.9.1/README.md
-drwxr-xr-x   0 agpe       (502) staff       (20)        0 2023-09-15 20:11:18.956884 anclib-0.9.1/anclib.egg-info/
--rw-r--r--   0 agpe       (502) staff       (20)     2260 2023-09-15 20:11:18.000000 anclib-0.9.1/anclib.egg-info/PKG-INFO
--rw-r--r--   0 agpe       (502) staff       (20)      201 2023-09-15 20:11:18.000000 anclib-0.9.1/anclib.egg-info/SOURCES.txt
--rw-r--r--   0 agpe       (502) staff       (20)        1 2023-09-15 20:11:18.000000 anclib-0.9.1/anclib.egg-info/dependency_links.txt
--rw-r--r--   0 agpe       (502) staff       (20)       71 2023-09-15 20:11:18.000000 anclib-0.9.1/anclib.egg-info/requires.txt
--rw-r--r--   0 agpe       (502) staff       (20)        7 2023-09-15 20:11:18.000000 anclib-0.9.1/anclib.egg-info/top_level.txt
--rw-r--r--   0 agpe       (502) staff       (20)    27542 2023-09-15 20:08:47.000000 anclib-0.9.1/anclib.py
--rw-r--r--   0 agpe       (502) staff       (20)      104 2022-11-17 13:06:18.000000 anclib-0.9.1/pyproject.toml
--rw-r--r--   0 agpe       (502) staff       (20)      668 2023-09-15 20:11:18.957457 anclib-0.9.1/setup.cfg
+drwxr-xr-x   0 agpe       (502) staff       (20)        0 2023-09-18 15:19:46.438103 anclib-0.9.2/
+-rw-r--r--   0 agpe       (502) staff       (20)    35149 2022-11-10 12:08:59.000000 anclib-0.9.2/LICENSE
+-rw-r--r--   0 agpe       (502) staff       (20)     2260 2023-09-18 15:19:46.438042 anclib-0.9.2/PKG-INFO
+-rw-r--r--   0 agpe       (502) staff       (20)     1591 2023-09-18 15:18:42.000000 anclib-0.9.2/README.md
+drwxr-xr-x   0 agpe       (502) staff       (20)        0 2023-09-18 15:19:46.437823 anclib-0.9.2/anclib.egg-info/
+-rw-r--r--   0 agpe       (502) staff       (20)     2260 2023-09-18 15:19:46.000000 anclib-0.9.2/anclib.egg-info/PKG-INFO
+-rw-r--r--   0 agpe       (502) staff       (20)      201 2023-09-18 15:19:46.000000 anclib-0.9.2/anclib.egg-info/SOURCES.txt
+-rw-r--r--   0 agpe       (502) staff       (20)        1 2023-09-18 15:19:46.000000 anclib-0.9.2/anclib.egg-info/dependency_links.txt
+-rw-r--r--   0 agpe       (502) staff       (20)       71 2023-09-18 15:19:46.000000 anclib-0.9.2/anclib.egg-info/requires.txt
+-rw-r--r--   0 agpe       (502) staff       (20)        7 2023-09-18 15:19:46.000000 anclib-0.9.2/anclib.egg-info/top_level.txt
+-rw-r--r--   0 agpe       (502) staff       (20)    27625 2023-09-18 15:18:17.000000 anclib-0.9.2/anclib.py
+-rw-r--r--   0 agpe       (502) staff       (20)      104 2022-11-17 13:06:18.000000 anclib-0.9.2/pyproject.toml
+-rw-r--r--   0 agpe       (502) staff       (20)      668 2023-09-18 15:19:46.438351 anclib-0.9.2/setup.cfg
```

### Comparing `anclib-0.9.1/LICENSE` & `anclib-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anclib-0.9.1/PKG-INFO` & `anclib-0.9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: anclib
-Version: 0.9.1
+Version: 0.9.2
 Summary: (Beginning of) library for analyzing ancestral reconstructions of DNA or protein sequences
 Home-page: https://github.com/agormp/anclib
 Author: Anders Gorm Pedersen
 Author-email: agpe@dtu.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sequencelib>=2.10.0
-Requires-Dist: phylotreelib>=1.23.3
+Requires-Dist: phylotreelib>=1.24.0
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: rpy2
 Requires-Dist: Levenshtein
 
 # anclib
 
-![](https://img.shields.io/badge/version-0.9.1-blue)
+![](https://img.shields.io/badge/version-0.9.2-blue)
 [![PyPI downloads](https://static.pepy.tech/personalized-badge/anclib?period=total&units=none&left_color=black&right_color=blue&left_text=downloads&service=github)](https://pepy.tech/project/anclib)
 
 Using classes and methods in anclib.py it is possible to parse and analyze text files containing results related to ancestral reconstruction of DNA or protein sequences. (Rudimentary - beginning of project)
 
 ## Availability
 
 The anclib.py source code is available on GitHub: https://github.com/agormp/anclib and can be installed from PyPI: https://pypi.org/project/anclib/
```

### Comparing `anclib-0.9.1/README.md` & `anclib-0.9.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # anclib
 
-![](https://img.shields.io/badge/version-0.9.1-blue)
+![](https://img.shields.io/badge/version-0.9.2-blue)
 [![PyPI downloads](https://static.pepy.tech/personalized-badge/anclib?period=total&units=none&left_color=black&right_color=blue&left_text=downloads&service=github)](https://pepy.tech/project/anclib)
 
 Using classes and methods in anclib.py it is possible to parse and analyze text files containing results related to ancestral reconstruction of DNA or protein sequences. (Rudimentary - beginning of project)
 
 ## Availability
 
 The anclib.py source code is available on GitHub: https://github.com/agormp/anclib and can be installed from PyPI: https://pypi.org/project/anclib/
```

### Comparing `anclib-0.9.1/anclib.egg-info/PKG-INFO` & `anclib-0.9.2/anclib.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: anclib
-Version: 0.9.1
+Version: 0.9.2
 Summary: (Beginning of) library for analyzing ancestral reconstructions of DNA or protein sequences
 Home-page: https://github.com/agormp/anclib
 Author: Anders Gorm Pedersen
 Author-email: agpe@dtu.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sequencelib>=2.10.0
-Requires-Dist: phylotreelib>=1.23.3
+Requires-Dist: phylotreelib>=1.24.0
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: rpy2
 Requires-Dist: Levenshtein
 
 # anclib
 
-![](https://img.shields.io/badge/version-0.9.1-blue)
+![](https://img.shields.io/badge/version-0.9.2-blue)
 [![PyPI downloads](https://static.pepy.tech/personalized-badge/anclib?period=total&units=none&left_color=black&right_color=blue&left_text=downloads&service=github)](https://pepy.tech/project/anclib)
 
 Using classes and methods in anclib.py it is possible to parse and analyze text files containing results related to ancestral reconstruction of DNA or protein sequences. (Rudimentary - beginning of project)
 
 ## Availability
 
 The anclib.py source code is available on GitHub: https://github.com/agormp/anclib and can be installed from PyPI: https://pypi.org/project/anclib/
```

### Comparing `anclib-0.9.1/anclib.py` & `anclib-0.9.2/anclib.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             seqid = ancseq.name2id[seq.name]  # Python note: not this objects responsibility!!!
             newname = str(seqid2traitid[seqid])
             seq.rename(newname)
             self.alignment.addseq(seq)
 
     ###############################################################################################
 
-    def write_tree(self, outfilename, label="branchtype", br=1):
+    def write_tree(self, outfilename, label="branchtype", br=1, label_delimiters="braces"):
         """Prints Nexus tree to outfilename, where branch labels carry information:
 
         label="branchtype": labels give same inforamtion as branchtype in branchinfo and
         branchdiff, namely traits for parent, nodefrom, nodeto (e.g., human-swine-swine)
 
         label="nodeid": nodeid used in other output functions (This means labels should
         be interpreted as belonging to the child node, not the branch)"""
@@ -79,15 +79,15 @@
                         if nodefrom != self.tree.root:
                             parent = self.tree.parent(nodefrom)
                             traitfrom_parent = self.traitdict[parent]
                         else:
                             traitfrom_parent = "None"
                         branch_type = f"{traitfrom_parent}-{traitfrom}-{traitto}"
                     out_tree.setlabel(nodefrom, nodeto, branch_type)
-            treestring = out_tree.nexus()
+            treestring = out_tree.nexus(print_leaflabels=True, label_delimiters=label_delimiters)
         elif label == "nodeid":
             # Hack: add label for root manually
             out_tree.set_nodeid_labels()
             treestring = out_tree.nexus()
             rootid = str(out_tree.root)
             treestring = treestring.replace(");", f"){rootid};")
         else:
```

### Comparing `anclib-0.9.1/setup.cfg` & `anclib-0.9.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = anclib
-version = 0.9.1
+version = 0.9.2
 author = Anders Gorm Pedersen
 author_email = agpe@dtu.dk
 description = (Beginning of) library for analyzing ancestral reconstructions of DNA or protein sequences
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/agormp/anclib
 classifiers = 
@@ -13,15 +13,15 @@
 	Operating System :: OS Independent
 
 [options]
 py_modules = anclib
 python_requires = >=3.6
 install_requires = 
 	sequencelib>=2.10.0
-	phylotreelib>=1.23.3
+	phylotreelib>=1.24.0
 	numpy
 	pandas
 	rpy2
 	Levenshtein
 
 [egg_info]
 tag_build =
```

