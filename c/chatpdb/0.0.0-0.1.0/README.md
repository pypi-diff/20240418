# Comparing `tmp/chatpdb-0.0.0.tar.gz` & `tmp/chatpdb-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatpdb-0.0.0.tar", last modified: Wed Apr 17 01:25:48 2024, max compression
+gzip compressed data, was "chatpdb-0.1.0.tar", last modified: Thu Apr 18 02:41:54 2024, max compression
```

## Comparing `chatpdb-0.0.0.tar` & `chatpdb-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,34 @@
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-17 01:25:48.925054 chatpdb-0.0.0/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)    35149 2024-04-17 01:18:02.000000 chatpdb-0.0.0/LICENSE
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1180 2024-04-17 01:25:48.924811 chatpdb-0.0.0/PKG-INFO
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-17 01:25:48.924560 chatpdb-0.0.0/chatpdb.egg-info/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1180 2024-04-17 01:25:48.000000 chatpdb-0.0.0/chatpdb.egg-info/PKG-INFO
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      176 2024-04-17 01:25:48.000000 chatpdb-0.0.0/chatpdb.egg-info/SOURCES.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-17 01:25:48.000000 chatpdb-0.0.0/chatpdb.egg-info/dependency_links.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       29 2024-04-17 01:25:48.000000 chatpdb-0.0.0/chatpdb.egg-info/requires.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-17 01:25:48.000000 chatpdb-0.0.0/chatpdb.egg-info/top_level.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1353 2024-04-17 01:24:59.000000 chatpdb-0.0.0/pyproject.toml
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       38 2024-04-17 01:25:48.925104 chatpdb-0.0.0/setup.cfg
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 02:41:54.130261 chatpdb-0.1.0/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)    35149 2024-04-17 01:18:02.000000 chatpdb-0.1.0/LICENSE
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     4287 2024-04-18 02:41:54.129955 chatpdb-0.1.0/PKG-INFO
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2916 2024-04-18 02:40:12.000000 chatpdb-0.1.0/README.md
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 02:41:54.125334 chatpdb-0.1.0/chatpdb/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      657 2024-04-17 22:36:33.000000 chatpdb-0.1.0/chatpdb/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)    10988 2024-04-17 20:47:59.000000 chatpdb-0.1.0/chatpdb/__main__.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 02:41:54.126741 chatpdb-0.1.0/chatpdb/chat/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      126 2024-04-17 20:46:43.000000 chatpdb-0.1.0/chatpdb/chat/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1206 2024-04-18 02:40:12.000000 chatpdb-0.1.0/chatpdb/chat/interface.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 02:41:54.127508 chatpdb-0.1.0/chatpdb/chat/llm/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      132 2024-04-17 20:46:43.000000 chatpdb-0.1.0/chatpdb/chat/llm/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1233 2024-04-17 22:36:33.000000 chatpdb-0.1.0/chatpdb/chat/llm/interface.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1678 2024-04-18 02:40:12.000000 chatpdb-0.1.0/chatpdb/chat/llm/openai.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 02:41:54.128325 chatpdb-0.1.0/chatpdb/chat/prompts/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      243 2024-04-17 20:46:43.000000 chatpdb-0.1.0/chatpdb/chat/prompts/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1753 2024-04-18 02:40:12.000000 chatpdb-0.1.0/chatpdb/chat/prompts/ask.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1901 2024-04-18 02:40:12.000000 chatpdb-0.1.0/chatpdb/chat/prompts/explain.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      546 2024-04-18 02:40:12.000000 chatpdb-0.1.0/chatpdb/chat/prompts/system.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1625 2024-04-18 02:40:12.000000 chatpdb-0.1.0/chatpdb/debugger.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1431 2024-04-18 02:40:12.000000 chatpdb-0.1.0/chatpdb/frame.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1041 2024-04-17 21:33:19.000000 chatpdb-0.1.0/chatpdb/stdout.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 02:41:54.129368 chatpdb-0.1.0/chatpdb.egg-info/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     4287 2024-04-18 02:41:54.000000 chatpdb-0.1.0/chatpdb.egg-info/PKG-INFO
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      608 2024-04-18 02:41:54.000000 chatpdb-0.1.0/chatpdb.egg-info/SOURCES.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-18 02:41:54.000000 chatpdb-0.1.0/chatpdb.egg-info/dependency_links.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       74 2024-04-18 02:41:54.000000 chatpdb-0.1.0/chatpdb.egg-info/requires.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        8 2024-04-18 02:41:54.000000 chatpdb-0.1.0/chatpdb.egg-info/top_level.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1626 2024-04-18 02:40:12.000000 chatpdb-0.1.0/pyproject.toml
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       38 2024-04-18 02:41:54.130315 chatpdb-0.1.0/setup.cfg
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 02:41:54.129003 chatpdb-0.1.0/tests/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      452 2024-04-18 02:40:12.000000 chatpdb-0.1.0/tests/test_debugger.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      432 2024-04-18 02:40:12.000000 chatpdb-0.1.0/tests/test_fixtures.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      454 2024-04-18 02:40:12.000000 chatpdb-0.1.0/tests/test_frame.py
```

### Comparing `chatpdb-0.0.0/LICENSE` & `chatpdb-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chatpdb-0.0.0/pyproject.toml` & `chatpdb-0.1.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,56 @@
 [project]
 name = "chatpdb"
-version = "0.0.0"
+version = "0.1.0"
 authors = [
   { name="Caelean Barnes", email="caeleanb@gmail.com" },
   { name="Evan Doyle", email="evanmdoyle@gmail.com" },
 ]
 description = "A chatgpt enabled python debugger"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 keywords = ['python', 'chatgpt', 'pdb', 'ai', 'chat', 'debugger']
 dependencies = [
     "ipdb==0.13.13",
-    "openai==1.20.0",
+    "openai==1.21.0",
+    "pydantic==2.5.3",
+    "tenacity==8.2.3",
+    "rich==13.7.1"
 ]
 [project.urls]
 Homepage = "https://github.com/never-over/chatpdb"
 Issues = "https://github.com/never-over/chatpdb/issues"
 
 [tool.pyright]
 include = ["chatpdb"]
-exclude = ["**/__pycache__", '**/.venv']
+exclude = [
+    "**/__pycache__",
+    "**/.venv",
+    "chatpdb/__main__.py",
+    "chatpdb/stdout.py",
+    "tests/"
+]
 reportMissingTypeStubs = false
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
+
+[tool.setuptools]
+packages = ["chatpdb"]
```

