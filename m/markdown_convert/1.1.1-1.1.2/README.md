# Comparing `tmp/markdown_convert-1.1.1.tar.gz` & `tmp/markdown_convert-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_convert-1.1.1.tar", max compression
+gzip compressed data, was "markdown_convert-1.1.2.tar", max compression
```

## Comparing `markdown_convert-1.1.1.tar` & `markdown_convert-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    18092 2023-10-23 17:37:06.761873 markdown_convert-1.1.1/LICENSE
--rw-r--r--   0        0        0     2339 2024-04-18 13:57:36.455111 markdown_convert-1.1.1/README.md
--rw-r--r--   0        0        0      213 2024-04-10 10:59:42.869680 markdown_convert-1.1.1/markdown_convert/__init__.py
--rwxr-xr-x   0        0        0     2815 2024-04-09 12:12:31.637276 markdown_convert-1.1.1/markdown_convert/__main__.py
--rw-r--r--   0        0        0     4935 2024-04-08 12:12:18.468503 markdown_convert-1.1.1/markdown_convert/code.css
--rw-r--r--   0        0        0     5344 2024-04-10 06:55:23.607495 markdown_convert-1.1.1/markdown_convert/default.css
--rw-r--r--   0        0        0       65 2024-04-10 10:59:51.693837 markdown_convert-1.1.1/markdown_convert/modules/__init__.py
--rw-r--r--   0        0        0      429 2024-04-10 20:54:32.247070 markdown_convert-1.1.1/markdown_convert/modules/constants.py
--rw-r--r--   0        0        0     5711 2024-04-16 12:03:21.481233 markdown_convert-1.1.1/markdown_convert/modules/convert.py
--rw-r--r--   0        0        0     2258 2024-04-09 12:12:32.309271 markdown_convert-1.1.1/markdown_convert/modules/resources.py
--rw-r--r--   0        0        0      655 2024-04-10 10:56:40.081145 markdown_convert-1.1.1/markdown_convert/modules/utils.py
--rw-r--r--   0        0        0     1487 2024-04-08 14:48:42.000577 markdown_convert-1.1.1/markdown_convert/modules/validate.py
--rw-r--r--   0        0        0      680 2024-04-18 13:57:43.063402 markdown_convert-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3243 1970-01-01 00:00:00.000000 markdown_convert-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-10-23 17:37:06.761873 markdown_convert-1.1.2/LICENSE
+-rw-r--r--   0        0        0     2312 2024-04-18 14:00:24.302419 markdown_convert-1.1.2/README.md
+-rw-r--r--   0        0        0      213 2024-04-10 10:59:42.869680 markdown_convert-1.1.2/markdown_convert/__init__.py
+-rwxr-xr-x   0        0        0     2815 2024-04-09 12:12:31.637276 markdown_convert-1.1.2/markdown_convert/__main__.py
+-rw-r--r--   0        0        0     4935 2024-04-08 12:12:18.468503 markdown_convert-1.1.2/markdown_convert/code.css
+-rw-r--r--   0        0        0     5344 2024-04-10 06:55:23.607495 markdown_convert-1.1.2/markdown_convert/default.css
+-rw-r--r--   0        0        0       65 2024-04-10 10:59:51.693837 markdown_convert-1.1.2/markdown_convert/modules/__init__.py
+-rw-r--r--   0        0        0      429 2024-04-10 20:54:32.247070 markdown_convert-1.1.2/markdown_convert/modules/constants.py
+-rw-r--r--   0        0        0     5711 2024-04-16 12:03:21.481233 markdown_convert-1.1.2/markdown_convert/modules/convert.py
+-rw-r--r--   0        0        0     2258 2024-04-09 12:12:32.309271 markdown_convert-1.1.2/markdown_convert/modules/resources.py
+-rw-r--r--   0        0        0      655 2024-04-10 10:56:40.081145 markdown_convert-1.1.2/markdown_convert/modules/utils.py
+-rw-r--r--   0        0        0     1487 2024-04-08 14:48:42.000577 markdown_convert-1.1.2/markdown_convert/modules/validate.py
+-rw-r--r--   0        0        0      680 2024-04-18 14:00:28.222589 markdown_convert-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3216 1970-01-01 00:00:00.000000 markdown_convert-1.1.2/PKG-INFO
```

### Comparing `markdown_convert-1.1.1/LICENSE` & `markdown_convert-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.1/README.md` & `markdown_convert-1.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # markdown-convert
 
 _Convert Markdown files to PDF from your command line._
 
 ### `pip install markdown-convert`
 
-[<kbd> 🐱 GitHub </kbd>](https://github.com/Julynx/markdown-convert) [<kbd> 📦 PyPi </kbd>](https://pypi.org/project/markdown_convert) 
+[ [🐱 GitHub](https://github.com/Julynx/markdown-convert) ] [ [📦 PyPi](https://pypi.org/project/markdown_convert) ]
 
 <img src='https://i.imgur.com/SZIz2gY.png' width='80%'>
 
 `markdown-convert` is an elegant command-line tool that converts Markdown files to PDF, powered by the amazing `markdown2` and `weasyprint` libraries.
 
 Unlike other similar tools, it relies solely on Python packages to do the job, eliminating the need for any external system-level dependencies when running on Linux.
```

### Comparing `markdown_convert-1.1.1/markdown_convert/__main__.py` & `markdown_convert-1.1.2/markdown_convert/__main__.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.1/markdown_convert/code.css` & `markdown_convert-1.1.2/markdown_convert/code.css`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.1/markdown_convert/default.css` & `markdown_convert-1.1.2/markdown_convert/default.css`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.1/markdown_convert/modules/convert.py` & `markdown_convert-1.1.2/markdown_convert/modules/convert.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.1/markdown_convert/modules/resources.py` & `markdown_convert-1.1.2/markdown_convert/modules/resources.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.1/markdown_convert/modules/utils.py` & `markdown_convert-1.1.2/markdown_convert/modules/utils.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.1/markdown_convert/modules/validate.py` & `markdown_convert-1.1.2/markdown_convert/modules/validate.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.1/pyproject.toml` & `markdown_convert-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "markdown_convert"
-version = "1.1.1"
+version = "1.1.2"
 description = "Convert Markdown files to PDF from your command line."
 authors = ["Julio Cabria <juliocabria@tutanota.com>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 homepage = "https://github.com/Julynx/markdown_convert"
 include = ["markdown_convert/default.css", "markdown_convert/code.css"]
```

### Comparing `markdown_convert-1.1.1/PKG-INFO` & `markdown_convert-1.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown_convert
-Version: 1.1.1
+Version: 1.1.2
 Summary: Convert Markdown files to PDF from your command line.
 Home-page: https://github.com/Julynx/markdown_convert
 License: GPL-2.0-only
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -23,15 +23,15 @@
 
 # markdown-convert
 
 _Convert Markdown files to PDF from your command line._
 
 ### `pip install markdown-convert`
 
-[<kbd> 🐱 GitHub </kbd>](https://github.com/Julynx/markdown-convert) [<kbd> 📦 PyPi </kbd>](https://pypi.org/project/markdown_convert) 
+[ [🐱 GitHub](https://github.com/Julynx/markdown-convert) ] [ [📦 PyPi](https://pypi.org/project/markdown_convert) ]
 
 <img src='https://i.imgur.com/SZIz2gY.png' width='80%'>
 
 `markdown-convert` is an elegant command-line tool that converts Markdown files to PDF, powered by the amazing `markdown2` and `weasyprint` libraries.
 
 Unlike other similar tools, it relies solely on Python packages to do the job, eliminating the need for any external system-level dependencies when running on Linux.
```

