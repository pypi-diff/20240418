# Comparing `tmp/repo_parser-0.0.1.tar.gz` & `tmp/repo_parser-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repo_parser-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "repo_parser-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `repo_parser-0.0.1.tar` & `repo_parser-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1088 2023-12-31 03:16:34.254152 repo_parser-0.0.1/LICENSE
--rw-r--r--   0        0        0     1026 2024-03-18 01:48:41.698685 repo_parser-0.0.1/README.md
--rw-r--r--   0        0        0      490 2024-03-18 01:48:41.702685 repo_parser-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      282 2023-12-31 05:51:46.903805 repo_parser-0.0.1/repo_parser/__init__.py
--rw-r--r--   0        0        0     2035 2024-03-18 01:48:41.702685 repo_parser-0.0.1/repo_parser/filesystem.py
--rw-r--r--   0        0        0      500 2023-12-31 05:50:09.104660 repo_parser-0.0.1/repo_parser/processor.py
--rw-r--r--   0        0        0     2961 2024-02-03 20:54:01.084399 repo_parser-0.0.1/repo_parser/resource.py
--rw-r--r--   0        0        0     1380 1970-01-01 00:00:00.000000 repo_parser-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-12-31 03:16:34.254152 repo_parser-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1026 2024-03-18 01:48:41.698685 repo_parser-0.0.2/README.md
+-rw-r--r--   0        0        0      490 2024-03-18 01:48:41.702685 repo_parser-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      283 2024-04-18 12:17:56.556469 repo_parser-0.0.2/repo_parser/__init__.py
+-rw-r--r--   0        0        0     3615 2024-04-13 22:38:15.278087 repo_parser-0.0.2/repo_parser/filesystem.py
+-rw-r--r--   0        0        0      217 2024-04-13 22:38:15.278087 repo_parser-0.0.2/repo_parser/processor.py
+-rw-r--r--   0        0        0     3474 2024-04-13 22:38:15.278087 repo_parser-0.0.2/repo_parser/resource.py
+-rw-r--r--   0        0        0     1380 1970-01-01 00:00:00.000000 repo_parser-0.0.2/PKG-INFO
```

### Comparing `repo_parser-0.0.1/LICENSE` & `repo_parser-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `repo_parser-0.0.1/README.md` & `repo_parser-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `repo_parser-0.0.1/PKG-INFO` & `repo_parser-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo-parser
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for extracting metadata out of a source repository.
 Author-email: William Lachance <wlach@protonmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: GitPython
 Project-URL: Home, https://github.com/wlach/repo-parser
```

