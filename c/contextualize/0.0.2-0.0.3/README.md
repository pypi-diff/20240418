# Comparing `tmp/contextualize-0.0.2.tar.gz` & `tmp/contextualize-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contextualize-0.0.2.tar", last modified: Thu Mar 21 18:24:55 2024, max compression
+gzip compressed data, was "contextualize-0.0.3.tar", last modified: Thu Apr 18 18:57:16 2024, max compression
```

## Comparing `contextualize-0.0.2.tar` & `contextualize-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2024-03-21 18:24:55.333862 contextualize-0.0.2/
--rw-rw-r--   0 josh      (1000) josh      (1000)    34523 2024-03-21 16:21:04.000000 contextualize-0.0.2/LICENSE
--rw-rw-r--   0 josh      (1000) josh      (1000)     2316 2024-03-21 18:24:55.333862 contextualize-0.0.2/PKG-INFO
--rw-rw-r--   0 josh      (1000) josh      (1000)     2060 2024-03-21 18:21:26.000000 contextualize-0.0.2/README.md
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2024-03-21 18:24:55.333862 contextualize-0.0.2/contextualize/
--rw-rw-r--   0 josh      (1000) josh      (1000)        0 2024-03-16 14:45:26.000000 contextualize-0.0.2/contextualize/__init__.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     2690 2024-03-18 16:42:08.000000 contextualize-0.0.2/contextualize/cli.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     2875 2024-03-18 16:42:08.000000 contextualize-0.0.2/contextualize/reference.py
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2024-03-21 18:24:55.333862 contextualize-0.0.2/contextualize.egg-info/
--rw-r--r--   0 josh      (1000) josh      (1000)     2316 2024-03-21 18:24:55.000000 contextualize-0.0.2/contextualize.egg-info/PKG-INFO
--rw-rw-r--   0 josh      (1000) josh      (1000)      341 2024-03-21 18:24:55.000000 contextualize-0.0.2/contextualize.egg-info/SOURCES.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)        1 2024-03-21 18:24:55.000000 contextualize-0.0.2/contextualize.egg-info/dependency_links.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)       57 2024-03-21 18:24:55.000000 contextualize-0.0.2/contextualize.egg-info/entry_points.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)        9 2024-03-21 18:24:55.000000 contextualize-0.0.2/contextualize.egg-info/requires.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)       14 2024-03-21 18:24:55.000000 contextualize-0.0.2/contextualize.egg-info/top_level.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)        9 2024-03-18 16:42:08.000000 contextualize-0.0.2/requirements.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)       38 2024-03-21 18:24:55.333862 contextualize-0.0.2/setup.cfg
--rw-rw-r--   0 josh      (1000) josh      (1000)      653 2024-03-21 18:24:01.000000 contextualize-0.0.2/setup.py
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2024-04-18 18:57:16.373942 contextualize-0.0.3/
+-rw-rw-r--   0 josh      (1000) josh      (1000)     3409 2024-04-18 18:57:16.373942 contextualize-0.0.3/PKG-INFO
+-rw-rw-r--   0 josh      (1000) josh      (1000)     3175 2024-03-24 16:44:17.000000 contextualize-0.0.3/README.md
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2024-04-18 18:57:16.373942 contextualize-0.0.3/contextualize/
+-rw-rw-r--   0 josh      (1000) josh      (1000)        0 2024-03-16 14:45:26.000000 contextualize-0.0.3/contextualize/__init__.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     6581 2024-04-15 17:19:36.000000 contextualize-0.0.3/contextualize/cli.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     6657 2024-04-11 23:28:00.000000 contextualize-0.0.3/contextualize/external.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     3900 2024-04-15 17:28:32.000000 contextualize-0.0.3/contextualize/reference.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)      975 2024-03-22 18:49:33.000000 contextualize-0.0.3/contextualize/tokenize.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)      498 2024-04-11 23:16:13.000000 contextualize-0.0.3/contextualize/utils.py
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2024-04-18 18:57:16.373942 contextualize-0.0.3/contextualize.egg-info/
+-rw-r--r--   0 josh      (1000) josh      (1000)     3409 2024-04-18 18:57:16.000000 contextualize-0.0.3/contextualize.egg-info/PKG-INFO
+-rw-rw-r--   0 josh      (1000) josh      (1000)      391 2024-04-18 18:57:16.000000 contextualize-0.0.3/contextualize.egg-info/SOURCES.txt
+-rw-rw-r--   0 josh      (1000) josh      (1000)        1 2024-04-18 18:57:16.000000 contextualize-0.0.3/contextualize.egg-info/dependency_links.txt
+-rw-rw-r--   0 josh      (1000) josh      (1000)       57 2024-04-18 18:57:16.000000 contextualize-0.0.3/contextualize.egg-info/entry_points.txt
+-rw-rw-r--   0 josh      (1000) josh      (1000)       49 2024-04-18 18:57:16.000000 contextualize-0.0.3/contextualize.egg-info/requires.txt
+-rw-rw-r--   0 josh      (1000) josh      (1000)       14 2024-04-18 18:57:16.000000 contextualize-0.0.3/contextualize.egg-info/top_level.txt
+-rw-rw-r--   0 josh      (1000) josh      (1000)       38 2024-04-18 18:57:16.373942 contextualize-0.0.3/setup.cfg
+-rw-rw-r--   0 josh      (1000) josh      (1000)      653 2024-04-18 18:47:39.000000 contextualize-0.0.3/setup.py
```

### Comparing `contextualize-0.0.2/PKG-INFO` & `contextualize-0.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,13 @@
-Metadata-Version: 2.1
-Name: contextualize
-Version: 0.0.2
-Summary: LLM prompt/context preparation utility 
-Home-page: https://github.com/jmpaz/contextualize
-Author: jmpaz
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # contextualize
 
 `contextualize` is a package to quickly retrieve and format file contents for use with LLMs.
 
+<img src="https://github.com/jmpaz/contextualize/assets/30947643/01dbcec2-69fc-405a-8d91-0a00626f8946" width=80%>
+
 
 ## Installation
 
 You can install the package using pip:
 ```python
 pip install contextualize
 ```
@@ -26,15 +18,15 @@
 ```
 
 
 ## Usage (`reference.py`)
 
 Define `FileReference` objects for specified file paths and optional ranges.
 - set `range` to a tuple of line numbers to include only a portion of the file, e.g. `range=(1, 10)`
-- set `format` to "md" or "xml" to wrap file contents in Markdown code blocks or `<file>` tags
+- set `format` to "md" (default) or "xml" to wrap file contents in Markdown code blocks or `<file>` tags
 - set `label` to "relative" (default), "name", or "ext" to determine what label is affixed to the enclosing Markdown/XML string
     - "relative" will use the relative path from the current working directory
     - "name" will use the file name only
     - "ext" will use the file extension only
 
 Retrieve wrapped contents from the `output` attribute.
 
@@ -43,16 +35,26 @@
 
 A CLI (`cli.py`) is provided to print file contents to the console from the command line.
 - `cat`: Prepare and concatenate file references
     - `paths`: Positional arguments for target file(s) or directories
     - `--ignore`: File(s) to ignore (optional)
     - `--format`: Output format (`md` or `xml`, default is `md`)
     - `--label`: Label style (`relative` for relative file path, `name` for file name only, `ext` for file extension only; default is `relative`)
-- Example usage:
+    - `--output`: Output target (`console` (default), `clipboard`)
+    - `--output-file`: Output file path (optional, compatible with `--output clipboard`)
+- `ls`: List token counts
+    - `paths`: Positional arguments for target file(s) or directories  
+    - `--encoding`: Encoding to use for tokenization, e.g., `cl100k_base` (default), `p50k_base`, `r50k_base`
+    - `--model`: Model (e.g., `gpt-3.5-turbo`/`gpt-4` (default), `text-davinci-003`, `code-davinci-002`) to determine which encoding to use for tokenization. Not used if `encoding` is provided.
+
+#### Examples
+- `cat`:
     - `contextualize cat README.md` will print the wrapped contents of `README.md` to the console with default settings (Markdown format, relative path label).
     - `contextualize cat README.md --format xml` will print the wrapped contents of `README.md` to the console with XML format.
     - `contextualize cat contextualize/ dev/ README.md --format xml` will prepare file references for files in the `contextualize/` and `dev/` directories and `README.md`, and print each file's contents (wrapped in corresponding XML tags) to the console.
-
+- `ls`:
+    - `contextualize ls README.md` will count and print the number of tokens in `README.md` using the default `cl100k_base` encoding.
+    - `contextualize ls contextualize/ --model text-davinci-003` will count and print the number of tokens in each file in the `contextualize/` directory using the `p50k_base` encoding associated with the `text-davinci-003` model, then print the total tokens for all processed files.
 
 ## Related projects
 
 - [lumpenspace/jamall](https://github.com/lumpenspace/jamall)
```

### Comparing `contextualize-0.0.2/setup.py` & `contextualize-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     required = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="contextualize",
-    version="0.0.2",
+    version="0.0.3",
     packages=find_packages(),
     install_requires=required,
     entry_points={"console_scripts": ["contextualize = contextualize.cli:main"]},
     author="jmpaz",
     description="LLM prompt/context preparation utility ",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

