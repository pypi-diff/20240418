# Comparing `tmp/cf2tf-0.6.2.tar.gz` & `tmp/cf2tf-0.6.3a26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf2tf-0.6.2.tar", max compression
+gzip compressed data, was "cf2tf-0.6.3a26.tar", max compression
```

## Comparing `cf2tf-0.6.2.tar` & `cf2tf-0.6.3a26.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2023-11-26 17:23:35.534440 cf2tf-0.6.2/LICENSE.txt
--rw-r--r--   0        0        0     7485 2023-11-26 17:23:35.534440 cf2tf-0.6.2/README.md
--rw-r--r--   0        0        0     1087 2023-11-26 17:23:48.782528 cf2tf-0.6.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-26 17:23:35.538440 cf2tf-0.6.2/src/cf2tf/__init__.py
--rw-r--r--   0        0        0     1451 2023-11-26 17:23:35.538440 cf2tf-0.6.2/src/cf2tf/app.py
--rw-r--r--   0        0        0       46 2023-11-26 17:23:35.538440 cf2tf-0.6.2/src/cf2tf/cloudformation/__init__.py
--rw-r--r--   0        0        0     2621 2023-11-26 17:23:35.538440 cf2tf-0.6.2/src/cf2tf/cloudformation/_template.py
--rw-r--r--   0        0        0        0 2023-11-26 17:23:35.538440 cf2tf-0.6.2/src/cf2tf/conversion/__init__.py
--rw-r--r--   0        0        0    31227 2023-11-26 17:23:35.538440 cf2tf-0.6.2/src/cf2tf/conversion/expressions.py
--rw-r--r--   0        0        0     2026 2023-11-26 17:23:35.538440 cf2tf-0.6.2/src/cf2tf/conversion/overrides.py
--rw-r--r--   0        0        0    21737 2023-11-26 17:23:35.538440 cf2tf-0.6.2/src/cf2tf/convert.py
--rw-r--r--   0        0        0     2672 2023-11-26 17:23:35.538440 cf2tf-0.6.2/src/cf2tf/save.py
--rw-r--r--   0        0        0        0 2023-11-26 17:23:35.538440 cf2tf-0.6.2/src/cf2tf/terraform/__init__.py
--rw-r--r--   0        0        0      368 2023-11-26 17:23:35.538440 cf2tf-0.6.2/src/cf2tf/terraform/_configuration.py
--rw-r--r--   0        0        0     2200 2023-11-26 17:23:35.538440 cf2tf-0.6.2/src/cf2tf/terraform/blocks.py
--rw-r--r--   0        0        0     3995 2023-11-26 17:23:35.538440 cf2tf-0.6.2/src/cf2tf/terraform/code.py
--rw-r--r--   0        0        0     4674 2023-11-26 17:23:35.538440 cf2tf-0.6.2/src/cf2tf/terraform/doc_file.py
--rw-r--r--   0        0        0      304 2023-11-26 17:23:35.538440 cf2tf-0.6.2/src/cf2tf/terraform/hcl2/__init__.py
--rw-r--r--   0        0        0     2971 2023-11-26 17:23:35.538440 cf2tf-0.6.2/src/cf2tf/terraform/hcl2/_block.py
--rw-r--r--   0        0        0     1815 2023-11-26 17:23:35.538440 cf2tf-0.6.2/src/cf2tf/terraform/hcl2/complex.py
--rw-r--r--   0        0        0      868 2023-11-26 17:23:35.538440 cf2tf-0.6.2/src/cf2tf/terraform/hcl2/custom.py
--rw-r--r--   0        0        0     2673 2023-11-26 17:23:35.538440 cf2tf-0.6.2/src/cf2tf/terraform/hcl2/primitive.py
--rw-r--r--   0        0        0     8531 1970-01-01 00:00:00.000000 cf2tf-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-18 00:04:45.314821 cf2tf-0.6.3a26/LICENSE.txt
+-rw-r--r--   0        0        0     7485 2024-04-18 00:04:45.314821 cf2tf-0.6.3a26/README.md
+-rw-r--r--   0        0        0     1090 2024-04-18 00:04:54.710869 cf2tf-0.6.3a26/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-18 00:04:45.318821 cf2tf-0.6.3a26/src/cf2tf/__init__.py
+-rw-r--r--   0        0        0     1451 2024-04-18 00:04:45.318821 cf2tf-0.6.3a26/src/cf2tf/app.py
+-rw-r--r--   0        0        0       46 2024-04-18 00:04:45.318821 cf2tf-0.6.3a26/src/cf2tf/cloudformation/__init__.py
+-rw-r--r--   0        0        0     2621 2024-04-18 00:04:45.318821 cf2tf-0.6.3a26/src/cf2tf/cloudformation/_template.py
+-rw-r--r--   0        0        0        0 2024-04-18 00:04:45.318821 cf2tf-0.6.3a26/src/cf2tf/conversion/__init__.py
+-rw-r--r--   0        0        0    31228 2024-04-18 00:04:45.318821 cf2tf-0.6.3a26/src/cf2tf/conversion/expressions.py
+-rw-r--r--   0        0        0     2026 2024-04-18 00:04:45.318821 cf2tf-0.6.3a26/src/cf2tf/conversion/overrides.py
+-rw-r--r--   0        0        0    21736 2024-04-18 00:04:45.318821 cf2tf-0.6.3a26/src/cf2tf/convert.py
+-rw-r--r--   0        0        0     2673 2024-04-18 00:04:45.318821 cf2tf-0.6.3a26/src/cf2tf/save.py
+-rw-r--r--   0        0        0        0 2024-04-18 00:04:45.318821 cf2tf-0.6.3a26/src/cf2tf/terraform/__init__.py
+-rw-r--r--   0        0        0      368 2024-04-18 00:04:45.318821 cf2tf-0.6.3a26/src/cf2tf/terraform/_configuration.py
+-rw-r--r--   0        0        0     2199 2024-04-18 00:04:45.318821 cf2tf-0.6.3a26/src/cf2tf/terraform/blocks.py
+-rw-r--r--   0        0        0     3995 2024-04-18 00:04:45.318821 cf2tf-0.6.3a26/src/cf2tf/terraform/code.py
+-rw-r--r--   0        0        0     4674 2024-04-18 00:04:45.318821 cf2tf-0.6.3a26/src/cf2tf/terraform/doc_file.py
+-rw-r--r--   0        0        0      304 2024-04-18 00:04:45.318821 cf2tf-0.6.3a26/src/cf2tf/terraform/hcl2/__init__.py
+-rw-r--r--   0        0        0     2971 2024-04-18 00:04:45.318821 cf2tf-0.6.3a26/src/cf2tf/terraform/hcl2/_block.py
+-rw-r--r--   0        0        0     1815 2024-04-18 00:04:45.318821 cf2tf-0.6.3a26/src/cf2tf/terraform/hcl2/complex.py
+-rw-r--r--   0        0        0      868 2024-04-18 00:04:45.318821 cf2tf-0.6.3a26/src/cf2tf/terraform/hcl2/custom.py
+-rw-r--r--   0        0        0     2673 2024-04-18 00:04:45.318821 cf2tf-0.6.3a26/src/cf2tf/terraform/hcl2/primitive.py
+-rw-r--r--   0        0        0     8534 1970-01-01 00:00:00.000000 cf2tf-0.6.3a26/PKG-INFO
```

### Comparing `cf2tf-0.6.2/LICENSE.txt` & `cf2tf-0.6.3a26/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.2/README.md` & `cf2tf-0.6.3a26/README.md`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.2/pyproject.toml` & `cf2tf-0.6.3a26/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cf2tf"
-version = "0.6.2"
+version = "0.6.3a26"
 description = "Convert Cloudformation Templates to Terraform."
 readme = "README.md"
 authors = ["Levi Blaney <shadycuz@gmail.com>"]
 repository = "https://github.com/DontShaveTheYak/cf2tf"
 keywords = ["cloudformation", "terraform", "cf2tf", "convert", "cloud", "conversion"]
 license = "GPL-3.0-only"
 
@@ -13,25 +13,25 @@
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 cfn-flip = "^1.3.0"
 PyYAML = "^6.0"
 click = "^8.1.2"
 GitPython = "^3.1.27"
-thefuzz = {extras = ["speedup"], version = "^0.20.0"}
+thefuzz = {extras = ["speedup"], version = "^0.22.0"}
 click-log = "^0.4.0"
 requests = "^2.27.1"
-pytest = "^7.1.2"
+pytest = "^8.0.0"
 
 [tool.poetry.dev-dependencies]
-black = "^23.0.0"
-flake8 = "^6.0.0"
+black = "^24.0.0"
+flake8 = "^7.0.0"
 flake8-black = "^0.3.3"
 coverage = {extras = ["toml"], version = "^7.0.0"}
-pytest-cov = "^4.0.0"
+pytest-cov = "^5.0.0"
 mypy = "^1.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
```

### Comparing `cf2tf-0.6.2/src/cf2tf/app.py` & `cf2tf-0.6.3a26/src/cf2tf/app.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.2/src/cf2tf/cloudformation/_template.py` & `cf2tf-0.6.3a26/src/cf2tf/cloudformation/_template.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.2/src/cf2tf/conversion/expressions.py` & `cf2tf-0.6.3a26/src/cf2tf/conversion/expressions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Convert Expression
 
 This module contains the logic to convert an AWS intrinsic function/conditional to
 it's Terraform equivalent.
 """
+
 import logging
 import re
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Union
 
 import cf2tf.convert
 import cf2tf.terraform.blocks as hcl2
 import cf2tf.terraform.doc_file as doc_file
```

### Comparing `cf2tf-0.6.2/src/cf2tf/conversion/overrides.py` & `cf2tf-0.6.3a26/src/cf2tf/conversion/overrides.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.2/src/cf2tf/convert.py` & `cf2tf-0.6.3a26/src/cf2tf/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,15 +360,15 @@
                 arguments = props_to_args(overrided_values, valid_arguments, docs_path)
 
                 log.debug(f"Converted properties to {arguments}")
 
             conditional = resource_values.get("Condition")
 
             if conditional is not None:
-                condition_map = {"count": LiteralType(f"locals.{conditional} ? 1 : 0")}
+                condition_map = {"count": LiteralType(f"local.{conditional} ? 1 : 0")}
                 arguments = MapType({**condition_map, **arguments})
 
             resource = Resource(
                 tf_name, tf_type, arguments, valid_arguments, valid_attributes
             )
             tf_resources.append(resource)
```

### Comparing `cf2tf-0.6.2/src/cf2tf/save.py` & `cf2tf-0.6.3a26/src/cf2tf/save.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Save the results of the conversion.
 """
+
 import logging
 from itertools import groupby
 from pathlib import Path
 from typing import Iterable, List, Optional, Type
 
 try:
     from typing import Protocol
```

### Comparing `cf2tf-0.6.2/src/cf2tf/terraform/blocks.py` & `cf2tf-0.6.3a26/src/cf2tf/terraform/blocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Defines classes and methods for creating and interacting with HCL syntax."""
 
-
 import logging
 from typing import Any, Dict, List, Optional
 
 from cf2tf.terraform.hcl2._block import Block
 
 log = logging.getLogger("cf2tf")
```

### Comparing `cf2tf-0.6.2/src/cf2tf/terraform/code.py` & `cf2tf-0.6.3a26/src/cf2tf/terraform/code.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.2/src/cf2tf/terraform/doc_file.py` & `cf2tf-0.6.3a26/src/cf2tf/terraform/doc_file.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.2/src/cf2tf/terraform/hcl2/_block.py` & `cf2tf-0.6.3a26/src/cf2tf/terraform/hcl2/_block.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.2/src/cf2tf/terraform/hcl2/complex.py` & `cf2tf-0.6.3a26/src/cf2tf/terraform/hcl2/complex.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.2/src/cf2tf/terraform/hcl2/custom.py` & `cf2tf-0.6.3a26/src/cf2tf/terraform/hcl2/custom.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.2/src/cf2tf/terraform/hcl2/primitive.py` & `cf2tf-0.6.3a26/src/cf2tf/terraform/hcl2/primitive.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.2/PKG-INFO` & `cf2tf-0.6.3a26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf2tf
-Version: 0.6.2
+Version: 0.6.3a26
 Summary: Convert Cloudformation Templates to Terraform.
 Home-page: https://github.com/DontShaveTheYak/cf2tf
 License: GPL-3.0-only
 Keywords: cloudformation,terraform,cf2tf,convert,cloud,conversion
 Author: Levi Blaney
 Author-email: shadycuz@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
@@ -14,17 +14,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3.1.27,<4.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: cfn-flip (>=1.3.0,<2.0.0)
 Requires-Dist: click (>=8.1.2,<9.0.0)
 Requires-Dist: click-log (>=0.4.0,<0.5.0)
-Requires-Dist: pytest (>=7.1.2,<8.0.0)
+Requires-Dist: pytest (>=8.0.0,<9.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
-Requires-Dist: thefuzz[speedup] (>=0.20.0,<0.21.0)
+Requires-Dist: thefuzz[speedup] (>=0.22.0,<0.23.0)
 Project-URL: Repository, https://github.com/DontShaveTheYak/cf2tf
 Description-Content-Type: text/markdown
 
 <!-- PROJECT SHIELDS -->
 <!--
 *** I'm using markdown "reference style" links for readability.
 *** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: cf2tf Version: 0.6.2 Summary: Convert
+Metadata-Version: 2.1 Name: cf2tf Version: 0.6.3a26 Summary: Convert
 Cloudformation Templates to Terraform. Home-page: https://github.com/
 DontShaveTheYak/cf2tf License: GPL-3.0-only Keywords:
 cloudformation,terraform,cf2tf,convert,cloud,conversion Author: Levi Blaney
 Author-email: shadycuz@gmail.com Requires-Python: >=3.8.1,<4.0.0 Classifier:
 License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: GitPython
 (>=3.1.27,<4.0.0) Requires-Dist: PyYAML (>=6.0,<7.0) Requires-Dist: cfn-flip
 (>=1.3.0,<2.0.0) Requires-Dist: click (>=8.1.2,<9.0.0) Requires-Dist: click-log
-(>=0.4.0,<0.5.0) Requires-Dist: pytest (>=7.1.2,<8.0.0) Requires-Dist: requests
-(>=2.27.1,<3.0.0) Requires-Dist: thefuzz[speedup] (>=0.20.0,<0.21.0) Project-
+(>=0.4.0,<0.5.0) Requires-Dist: pytest (>=8.0.0,<9.0.0) Requires-Dist: requests
+(>=2.27.1,<3.0.0) Requires-Dist: thefuzz[speedup] (>=0.22.0,<0.23.0) Project-
 URL: Repository, https://github.com/DontShaveTheYak/cf2tf Description-Content-
 Type: text/markdown [![Python][python-shield]][pypi-url] [![Latest][version-
 shield]][pypi-url] [![Tests][test-shield]][test-url] [![Coverage][codecov-
 shield]][codecov-url] [![License][license-shield]][license-url]
                      ******** CClloouuddffoorrmmaattiioonn 22 TTeerrrraaffoorrmm ********
              Convert your Cloudformation templates to Terraform.
                        _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e Â·
```

