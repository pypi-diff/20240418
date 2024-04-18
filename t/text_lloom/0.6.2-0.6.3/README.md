# Comparing `tmp/text_lloom-0.6.2.tar.gz` & `tmp/text_lloom-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_lloom-0.6.2.tar", max compression
+gzip compressed data, was "text_lloom-0.6.3.tar", max compression
```

## Comparing `text_lloom-0.6.2.tar` & `text_lloom-0.6.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       39 2024-02-02 13:27:07.282735 text_lloom-0.6.2/README.md
--rw-r--r--   0        0        0      572 2024-04-18 03:53:24.735632 text_lloom-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     2019 2024-04-16 10:45:54.173463 text_lloom-0.6.2/src/text_lloom/__init__.py
--rw-r--r--   0        0        0      738 2024-02-28 09:09:42.891236 text_lloom-0.6.2/src/text_lloom/concept.py
--rw-r--r--   0        0        0    57603 2024-04-18 02:00:30.123241 text_lloom-0.6.2/src/text_lloom/concept_induction.py
--rw-r--r--   0        0        0    12290 2024-03-08 09:30:26.443347 text_lloom-0.6.2/src/text_lloom/llm.py
--rw-r--r--   0        0        0     8416 2024-04-13 23:28:08.093682 text_lloom-0.6.2/src/text_lloom/prompts.py
--rw-r--r--   0        0        0     1263 2024-04-15 01:19:42.816858 text_lloom-0.6.2/src/text_lloom/static/index.css
--rw-r--r--   0        0        0   455935 2024-04-15 01:19:42.816860 text_lloom-0.6.2/src/text_lloom/static/index.js
--rw-r--r--   0        0        0      707 2024-04-15 01:19:38.799003 text_lloom-0.6.2/src/text_lloom/static/index_select.css
--rw-r--r--   0        0        0    11241 2024-04-15 01:19:38.799013 text_lloom-0.6.2/src/text_lloom/static/index_select.js
--rw-r--r--   0        0        0    28029 2024-04-18 03:52:37.534292 text_lloom-0.6.2/src/text_lloom/workbench.py
--rw-r--r--   0        0        0     1025 1970-01-01 00:00:00.000000 text_lloom-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-02-02 13:27:07.282735 text_lloom-0.6.3/README.md
+-rw-r--r--   0        0        0      572 2024-04-18 04:13:54.234178 text_lloom-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     2019 2024-04-16 10:45:54.173463 text_lloom-0.6.3/src/text_lloom/__init__.py
+-rw-r--r--   0        0        0      738 2024-02-28 09:09:42.891236 text_lloom-0.6.3/src/text_lloom/concept.py
+-rw-r--r--   0        0        0    57603 2024-04-18 02:00:30.123241 text_lloom-0.6.3/src/text_lloom/concept_induction.py
+-rw-r--r--   0        0        0    12290 2024-03-08 09:30:26.443347 text_lloom-0.6.3/src/text_lloom/llm.py
+-rw-r--r--   0        0        0     8416 2024-04-13 23:28:08.093682 text_lloom-0.6.3/src/text_lloom/prompts.py
+-rw-r--r--   0        0        0     1263 2024-04-15 01:19:42.816858 text_lloom-0.6.3/src/text_lloom/static/index.css
+-rw-r--r--   0        0        0   455935 2024-04-15 01:19:42.816860 text_lloom-0.6.3/src/text_lloom/static/index.js
+-rw-r--r--   0        0        0      707 2024-04-15 01:19:38.799003 text_lloom-0.6.3/src/text_lloom/static/index_select.css
+-rw-r--r--   0        0        0    11241 2024-04-15 01:19:38.799013 text_lloom-0.6.3/src/text_lloom/static/index_select.js
+-rw-r--r--   0        0        0    28031 2024-04-18 04:09:53.773126 text_lloom-0.6.3/src/text_lloom/workbench.py
+-rw-r--r--   0        0        0     1025 1970-01-01 00:00:00.000000 text_lloom-0.6.3/PKG-INFO
```

### Comparing `text_lloom-0.6.2/pyproject.toml` & `text_lloom-0.6.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "text_lloom"
-version = "0.6.2"
+version = "0.6.3"
 description = "Concept Induction to analyze unstructured text"
 authors = ["Michelle Lam <mlam4@cs.stanford.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 bertopic = "^0.16.0"
```

### Comparing `text_lloom-0.6.2/src/text_lloom/__init__.py` & `text_lloom-0.6.3/src/text_lloom/__init__.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.6.2/src/text_lloom/concept.py` & `text_lloom-0.6.3/src/text_lloom/concept.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.6.2/src/text_lloom/concept_induction.py` & `text_lloom-0.6.3/src/text_lloom/concept_induction.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.6.2/src/text_lloom/llm.py` & `text_lloom-0.6.3/src/text_lloom/llm.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.6.2/src/text_lloom/prompts.py` & `text_lloom-0.6.3/src/text_lloom/prompts.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.6.2/src/text_lloom/static/index.css` & `text_lloom-0.6.3/src/text_lloom/static/index.css`

 * *Files identical despite different names*

### Comparing `text_lloom-0.6.2/src/text_lloom/static/index.js` & `text_lloom-0.6.3/src/text_lloom/static/index.js`

 * *Files identical despite different names*

### Comparing `text_lloom-0.6.2/src/text_lloom/static/index_select.css` & `text_lloom-0.6.3/src/text_lloom/static/index_select.css`

 * *Files identical despite different names*

### Comparing `text_lloom-0.6.2/src/text_lloom/static/index_select.js` & `text_lloom-0.6.3/src/text_lloom/static/index_select.js`

 * *Files identical despite different names*

### Comparing `text_lloom-0.6.2/src/text_lloom/workbench.py` & `text_lloom-0.6.3/src/text_lloom/workbench.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,17 +113,17 @@
 
     # Printed text formatting
     def bold_txt(self, s):
         return f"\033[1m{s}\033[0m"
 
     def highlight_txt(self, s, color="yellow"):
         if color == "yellow":
-            return f"\x1b[48;5;228m{s}\x1b[m"
+            return f"\x1b[48;5;228m{s}\x1b[0m"
         elif color == "blue":
-            return f"\x1b[48;5;117m{s}\x1b[m"
+            return f"\x1b[48;5;117m{s}\x1b[0m"
 
     def bold_highlight_txt(self, s):
         return self.bold_txt(self.highlight_txt(s))
     
     # def spinner_wrapper(self, step_name):
     #     format_step_name = f"{self.highlight_txt(step_name, color='blue')}"
     #     return yaspin(text=format_step_name, color="yellow")
```

### Comparing `text_lloom-0.6.2/PKG-INFO` & `text_lloom-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text_lloom
-Version: 0.6.2
+Version: 0.6.3
 Summary: Concept Induction to analyze unstructured text
 Author: Michelle Lam
 Author-email: mlam4@cs.stanford.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

