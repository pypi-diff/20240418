# Comparing `tmp/markdown_convert-1.0.9.tar.gz` & `tmp/markdown_convert-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_convert-1.0.9.tar", max compression
+gzip compressed data, was "markdown_convert-1.1.0.tar", max compression
```

## Comparing `markdown_convert-1.0.9.tar` & `markdown_convert-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    18092 2023-10-23 17:37:06.761873 markdown_convert-1.0.9/LICENSE
--rw-r--r--   0        0        0     1763 2024-04-10 11:53:43.195866 markdown_convert-1.0.9/README.md
--rw-r--r--   0        0        0      213 2024-04-10 10:59:42.869680 markdown_convert-1.0.9/markdown_convert/__init__.py
--rwxr-xr-x   0        0        0     2815 2024-04-09 12:12:31.637276 markdown_convert-1.0.9/markdown_convert/__main__.py
--rw-r--r--   0        0        0     4935 2024-04-08 12:12:18.468503 markdown_convert-1.0.9/markdown_convert/code.css
--rw-r--r--   0        0        0     5344 2024-04-10 06:55:23.607495 markdown_convert-1.0.9/markdown_convert/default.css
--rw-r--r--   0        0        0       65 2024-04-10 10:59:51.693837 markdown_convert-1.0.9/markdown_convert/modules/__init__.py
--rw-r--r--   0        0        0      429 2024-04-10 20:54:32.247070 markdown_convert-1.0.9/markdown_convert/modules/constants.py
--rw-r--r--   0        0        0     5711 2024-04-16 12:03:21.481233 markdown_convert-1.0.9/markdown_convert/modules/convert.py
--rw-r--r--   0        0        0     2258 2024-04-09 12:12:32.309271 markdown_convert-1.0.9/markdown_convert/modules/resources.py
--rw-r--r--   0        0        0      655 2024-04-10 10:56:40.081145 markdown_convert-1.0.9/markdown_convert/modules/utils.py
--rw-r--r--   0        0        0     1487 2024-04-08 14:48:42.000577 markdown_convert-1.0.9/markdown_convert/modules/validate.py
--rw-r--r--   0        0        0      680 2024-04-16 12:07:15.948931 markdown_convert-1.0.9/pyproject.toml
--rw-r--r--   0        0        0     2667 1970-01-01 00:00:00.000000 markdown_convert-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-10-23 17:37:06.761873 markdown_convert-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2367 2024-04-18 13:52:43.702629 markdown_convert-1.1.0/README.md
+-rw-r--r--   0        0        0      213 2024-04-10 10:59:42.869680 markdown_convert-1.1.0/markdown_convert/__init__.py
+-rwxr-xr-x   0        0        0     2815 2024-04-09 12:12:31.637276 markdown_convert-1.1.0/markdown_convert/__main__.py
+-rw-r--r--   0        0        0     4935 2024-04-08 12:12:18.468503 markdown_convert-1.1.0/markdown_convert/code.css
+-rw-r--r--   0        0        0     5344 2024-04-10 06:55:23.607495 markdown_convert-1.1.0/markdown_convert/default.css
+-rw-r--r--   0        0        0       65 2024-04-10 10:59:51.693837 markdown_convert-1.1.0/markdown_convert/modules/__init__.py
+-rw-r--r--   0        0        0      429 2024-04-10 20:54:32.247070 markdown_convert-1.1.0/markdown_convert/modules/constants.py
+-rw-r--r--   0        0        0     5711 2024-04-16 12:03:21.481233 markdown_convert-1.1.0/markdown_convert/modules/convert.py
+-rw-r--r--   0        0        0     2258 2024-04-09 12:12:32.309271 markdown_convert-1.1.0/markdown_convert/modules/resources.py
+-rw-r--r--   0        0        0      655 2024-04-10 10:56:40.081145 markdown_convert-1.1.0/markdown_convert/modules/utils.py
+-rw-r--r--   0        0        0     1487 2024-04-08 14:48:42.000577 markdown_convert-1.1.0/markdown_convert/modules/validate.py
+-rw-r--r--   0        0        0      680 2024-04-18 13:54:52.923563 markdown_convert-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3271 1970-01-01 00:00:00.000000 markdown_convert-1.1.0/PKG-INFO
```

### Comparing `markdown_convert-1.0.9/LICENSE` & `markdown_convert-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.9/README.md` & `markdown_convert-1.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # markdown-convert
 
 _Convert Markdown files to PDF from your command line._
 
 ### `pip install markdown-convert`
 
+[<kbd> <br> 🐱 GitHub <br> </kbd>](https://github.com/Julynx/markdown-convert) [<kbd> <br> 📦 PyPi <br> </kbd>](https://pypi.org/project/markdown_convert) 
+
 <img src='https://i.imgur.com/SZIz2gY.png' width='80%'>
 
 `markdown-convert` is an elegant command-line tool that converts Markdown files to PDF, powered by the amazing `markdown2` and `weasyprint` libraries.
 
 Unlike other similar tools, it relies solely on Python packages to do the job, eliminating the need for any external system-level dependencies when running on Linux.
 
 If you're running Windows, you only need to install the GTK-3 runtime from the following link: [GTK-3 Runtime](https://github.com/tschoonj/GTK-for-Windows-Runtime-Environment-Installer/releases).
@@ -17,14 +19,16 @@
 - ⚡️ Supports live compilation, so you can preview your PDF in real-time as you type.
 - 🌸 Comes with beautiful CSS out of the box, making your documents look great from the start.
 - 🎨 Syntax highlighting for code blocks included.
 - 🪐 Designed for the 21st century, with relative links, pipe tables, and modern CSS paged media features.
 
 ### Usage
 
+> Note: If you just installed the package, you may need to log out and log back in for the `markdown-convert` command to be registered to your PATH.
+
 Run `markdown-convert -h` right from your terminal to check out the available options:
 
 ```bash
 Usage:
   markdown-convert [markdown_file_path] [options]
 
 Options:
@@ -43,7 +47,11 @@
 
 # Convert your Markdown file to PDF once
 convert('README.md', 'style.css', 'README.pdf')
 
 # Convert your Markdown file to PDF every time it changes
 live_convert('README.md', 'style.css', 'README.pdf')
 ```
+
+### Integrations
+
+Right click a Markdown file and `Convert to PDF` with the [markdown_convert_explorer](https://github.com/Julynx/markdown_convert_explorer) and [markdown_convert_nautilus](https://github.com/Julynx/markdown_convert_nautilus) extensions for Windows and Linux.
```

### Comparing `markdown_convert-1.0.9/markdown_convert/__main__.py` & `markdown_convert-1.1.0/markdown_convert/__main__.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.9/markdown_convert/code.css` & `markdown_convert-1.1.0/markdown_convert/code.css`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.9/markdown_convert/default.css` & `markdown_convert-1.1.0/markdown_convert/default.css`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.9/markdown_convert/modules/convert.py` & `markdown_convert-1.1.0/markdown_convert/modules/convert.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.9/markdown_convert/modules/resources.py` & `markdown_convert-1.1.0/markdown_convert/modules/resources.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.9/markdown_convert/modules/utils.py` & `markdown_convert-1.1.0/markdown_convert/modules/utils.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.9/markdown_convert/modules/validate.py` & `markdown_convert-1.1.0/markdown_convert/modules/validate.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.9/pyproject.toml` & `markdown_convert-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "markdown_convert"
-version = "1.0.9"
+version = "1.1.0"
 description = "Convert Markdown files to PDF from your command line."
 authors = ["Julio Cabria <juliocabria@tutanota.com>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 homepage = "https://github.com/Julynx/markdown_convert"
 include = ["markdown_convert/default.css", "markdown_convert/code.css"]
```

