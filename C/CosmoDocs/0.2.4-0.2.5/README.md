# Comparing `tmp/cosmodocs-0.2.4.tar.gz` & `tmp/cosmodocs-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmodocs-0.2.4.tar", last modified: Wed Jan  3 21:55:03 2024, max compression
+gzip compressed data, was "cosmodocs-0.2.5.tar", last modified: Thu Apr 18 15:03:56 2024, max compression
```

## Comparing `cosmodocs-0.2.4.tar` & `cosmodocs-0.2.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1913 2024-01-02 05:00:20.288071 cosmodocs-0.2.4/README.md
--rw-r--r--   0        0        0      478 2024-01-03 21:55:03.418250 cosmodocs-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     8761 2024-01-03 21:54:15.230148 cosmodocs-0.2.4/src/cosmodocs/__init__.py
--rw-r--r--   0        0        0        0 2023-12-30 17:08:40.424239 cosmodocs-0.2.4/tests/__init__.py
--rw-r--r--   0        0        0     1605 2024-01-03 12:32:43.233462 cosmodocs-0.2.4/tests/data/sample_file.py
--rw-r--r--   0        0        0     3192 2024-01-03 02:17:56.067745 cosmodocs-0.2.4/tests/unit/test_cosmos_docs.py
--rw-r--r--   0        0        0     2123 1970-01-01 00:00:00.000000 cosmodocs-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1913 2024-03-16 15:13:41.596396 cosmodocs-0.2.5/README.md
+-rw-r--r--   0        0        0      478 2024-04-18 15:03:56.618555 cosmodocs-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     9126 2024-04-18 14:57:51.504519 cosmodocs-0.2.5/src/cosmodocs/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-30 17:08:40.424239 cosmodocs-0.2.5/tests/__init__.py
+-rw-r--r--   0        0        0     1605 2024-01-03 12:32:43.233462 cosmodocs-0.2.5/tests/data/sample_file.py
+-rw-r--r--   0        0        0     3192 2024-01-03 02:17:56.067745 cosmodocs-0.2.5/tests/unit/test_cosmos_docs.py
+-rw-r--r--   0        0        0     2123 1970-01-01 00:00:00.000000 cosmodocs-0.2.5/PKG-INFO
```

### Comparing `cosmodocs-0.2.4/README.md` & `cosmodocs-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `cosmodocs-0.2.4/src/cosmodocs/__init__.py` & `cosmodocs-0.2.5/src/cosmodocs/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import ast
+import re
 from typing import TypedDict
 
 
 class FunctionArg(TypedDict):
     name: str
     type: str
 
@@ -218,15 +219,23 @@
         markdown_result += "\n|"
 
         for _ in columns:
             markdown_result += " --- |"
 
         for value in values:
             markdown_result += "\n|"
+            markdown_result += "\n|"
             for item in value:
+                if not item:
+                    item = ""
+                item = item.replace("\n", "")
+                item = re.sub(r'"\s+"', "", item)
+                item = re.sub(r"\(\s+", "(", item)
+                item = re.sub(r",\s+\)", ")", item)
+                item = re.sub(r",\s+", ", ", item)
                 markdown_result += f" {item} |"
         markdown_result += "\n"
 
         return markdown_result
 
     def markdown_title(self, size: int, text: str):
         markdown_result = ""
```

### Comparing `cosmodocs-0.2.4/tests/data/sample_file.py` & `cosmodocs-0.2.5/tests/data/sample_file.py`

 * *Files identical despite different names*

### Comparing `cosmodocs-0.2.4/tests/unit/test_cosmos_docs.py` & `cosmodocs-0.2.5/tests/unit/test_cosmos_docs.py`

 * *Files identical despite different names*

### Comparing `cosmodocs-0.2.4/PKG-INFO` & `cosmodocs-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CosmoDocs
-Version: 0.2.4
+Version: 0.2.5
 Summary: A file based documentation generator for Python projects.
 Author-Email: Thiago Santa Clara <strovsk@outlook.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Cosmo Docs
```

