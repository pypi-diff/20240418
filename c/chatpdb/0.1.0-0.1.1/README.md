# Comparing `tmp/chatpdb-0.1.0.tar.gz` & `tmp/chatpdb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatpdb-0.1.0.tar", last modified: Thu Apr 18 02:41:54 2024, max compression
+gzip compressed data, was "chatpdb-0.1.1.tar", last modified: Thu Apr 18 05:33:27 2024, max compression
```

## Comparing `chatpdb-0.1.0.tar` & `chatpdb-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 02:41:54.130261 chatpdb-0.1.0/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)    35149 2024-04-17 01:18:02.000000 chatpdb-0.1.0/LICENSE
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     4287 2024-04-18 02:41:54.129955 chatpdb-0.1.0/PKG-INFO
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2916 2024-04-18 02:40:12.000000 chatpdb-0.1.0/README.md
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 02:41:54.125334 chatpdb-0.1.0/chatpdb/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      657 2024-04-17 22:36:33.000000 chatpdb-0.1.0/chatpdb/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)    10988 2024-04-17 20:47:59.000000 chatpdb-0.1.0/chatpdb/__main__.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 02:41:54.126741 chatpdb-0.1.0/chatpdb/chat/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      126 2024-04-17 20:46:43.000000 chatpdb-0.1.0/chatpdb/chat/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1206 2024-04-18 02:40:12.000000 chatpdb-0.1.0/chatpdb/chat/interface.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 02:41:54.127508 chatpdb-0.1.0/chatpdb/chat/llm/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      132 2024-04-17 20:46:43.000000 chatpdb-0.1.0/chatpdb/chat/llm/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1233 2024-04-17 22:36:33.000000 chatpdb-0.1.0/chatpdb/chat/llm/interface.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1678 2024-04-18 02:40:12.000000 chatpdb-0.1.0/chatpdb/chat/llm/openai.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 02:41:54.128325 chatpdb-0.1.0/chatpdb/chat/prompts/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      243 2024-04-17 20:46:43.000000 chatpdb-0.1.0/chatpdb/chat/prompts/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1753 2024-04-18 02:40:12.000000 chatpdb-0.1.0/chatpdb/chat/prompts/ask.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1901 2024-04-18 02:40:12.000000 chatpdb-0.1.0/chatpdb/chat/prompts/explain.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      546 2024-04-18 02:40:12.000000 chatpdb-0.1.0/chatpdb/chat/prompts/system.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1625 2024-04-18 02:40:12.000000 chatpdb-0.1.0/chatpdb/debugger.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1431 2024-04-18 02:40:12.000000 chatpdb-0.1.0/chatpdb/frame.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1041 2024-04-17 21:33:19.000000 chatpdb-0.1.0/chatpdb/stdout.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 02:41:54.129368 chatpdb-0.1.0/chatpdb.egg-info/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     4287 2024-04-18 02:41:54.000000 chatpdb-0.1.0/chatpdb.egg-info/PKG-INFO
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      608 2024-04-18 02:41:54.000000 chatpdb-0.1.0/chatpdb.egg-info/SOURCES.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-18 02:41:54.000000 chatpdb-0.1.0/chatpdb.egg-info/dependency_links.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       74 2024-04-18 02:41:54.000000 chatpdb-0.1.0/chatpdb.egg-info/requires.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        8 2024-04-18 02:41:54.000000 chatpdb-0.1.0/chatpdb.egg-info/top_level.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1626 2024-04-18 02:40:12.000000 chatpdb-0.1.0/pyproject.toml
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       38 2024-04-18 02:41:54.130315 chatpdb-0.1.0/setup.cfg
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 02:41:54.129003 chatpdb-0.1.0/tests/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      452 2024-04-18 02:40:12.000000 chatpdb-0.1.0/tests/test_debugger.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      432 2024-04-18 02:40:12.000000 chatpdb-0.1.0/tests/test_fixtures.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      454 2024-04-18 02:40:12.000000 chatpdb-0.1.0/tests/test_frame.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 05:33:27.370739 chatpdb-0.1.1/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)    35149 2024-04-17 01:18:02.000000 chatpdb-0.1.1/LICENSE
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     4287 2024-04-18 05:33:27.370380 chatpdb-0.1.1/PKG-INFO
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2916 2024-04-18 02:40:12.000000 chatpdb-0.1.1/README.md
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 05:33:27.364522 chatpdb-0.1.1/chatpdb/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      657 2024-04-17 22:36:33.000000 chatpdb-0.1.1/chatpdb/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)    10988 2024-04-17 20:47:59.000000 chatpdb-0.1.1/chatpdb/__main__.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 05:33:27.366694 chatpdb-0.1.1/chatpdb/chat/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      126 2024-04-17 20:46:43.000000 chatpdb-0.1.1/chatpdb/chat/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1206 2024-04-18 02:40:12.000000 chatpdb-0.1.1/chatpdb/chat/interface.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 05:33:27.367552 chatpdb-0.1.1/chatpdb/chat/llm/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      132 2024-04-17 20:46:43.000000 chatpdb-0.1.1/chatpdb/chat/llm/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1233 2024-04-17 22:36:33.000000 chatpdb-0.1.1/chatpdb/chat/llm/interface.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1678 2024-04-18 02:40:12.000000 chatpdb-0.1.1/chatpdb/chat/llm/openai.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 05:33:27.368568 chatpdb-0.1.1/chatpdb/chat/prompts/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      243 2024-04-17 20:46:43.000000 chatpdb-0.1.1/chatpdb/chat/prompts/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1753 2024-04-18 02:40:12.000000 chatpdb-0.1.1/chatpdb/chat/prompts/ask.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1901 2024-04-18 02:40:12.000000 chatpdb-0.1.1/chatpdb/chat/prompts/explain.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      546 2024-04-18 02:40:12.000000 chatpdb-0.1.1/chatpdb/chat/prompts/system.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1625 2024-04-18 02:40:12.000000 chatpdb-0.1.1/chatpdb/debugger.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1431 2024-04-18 02:40:12.000000 chatpdb-0.1.1/chatpdb/frame.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1041 2024-04-17 21:33:19.000000 chatpdb-0.1.1/chatpdb/stdout.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 05:33:27.369814 chatpdb-0.1.1/chatpdb.egg-info/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     4287 2024-04-18 05:33:27.000000 chatpdb-0.1.1/chatpdb.egg-info/PKG-INFO
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      608 2024-04-18 05:33:27.000000 chatpdb-0.1.1/chatpdb.egg-info/SOURCES.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-18 05:33:27.000000 chatpdb-0.1.1/chatpdb.egg-info/dependency_links.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       74 2024-04-18 05:33:27.000000 chatpdb-0.1.1/chatpdb.egg-info/requires.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        8 2024-04-18 05:33:27.000000 chatpdb-0.1.1/chatpdb.egg-info/top_level.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1626 2024-04-18 05:28:47.000000 chatpdb-0.1.1/pyproject.toml
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       38 2024-04-18 05:33:27.370819 chatpdb-0.1.1/setup.cfg
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 05:33:27.369449 chatpdb-0.1.1/tests/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      452 2024-04-18 02:40:12.000000 chatpdb-0.1.1/tests/test_debugger.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      432 2024-04-18 02:40:12.000000 chatpdb-0.1.1/tests/test_fixtures.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      454 2024-04-18 02:40:12.000000 chatpdb-0.1.1/tests/test_frame.py
```

### Comparing `chatpdb-0.1.0/LICENSE` & `chatpdb-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.0/PKG-INFO` & `chatpdb-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatpdb
-Version: 0.1.0
+Version: 0.1.1
 Summary: A chatgpt enabled python debugger
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/chatpdb
 Project-URL: Issues, https://github.com/never-over/chatpdb/issues
 Keywords: python,chatgpt,pdb,ai,chat,debugger
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `chatpdb-0.1.0/README.md` & `chatpdb-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.0/chatpdb/__init__.py` & `chatpdb-0.1.1/chatpdb/__init__.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.0/chatpdb/__main__.py` & `chatpdb-0.1.1/chatpdb/__main__.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.0/chatpdb/chat/interface.py` & `chatpdb-0.1.1/chatpdb/chat/interface.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.0/chatpdb/chat/llm/interface.py` & `chatpdb-0.1.1/chatpdb/chat/llm/interface.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.0/chatpdb/chat/llm/openai.py` & `chatpdb-0.1.1/chatpdb/chat/llm/openai.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.0/chatpdb/chat/prompts/ask.py` & `chatpdb-0.1.1/chatpdb/chat/prompts/ask.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.0/chatpdb/chat/prompts/explain.py` & `chatpdb-0.1.1/chatpdb/chat/prompts/explain.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.0/chatpdb/chat/prompts/system.py` & `chatpdb-0.1.1/chatpdb/chat/prompts/system.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.0/chatpdb/debugger.py` & `chatpdb-0.1.1/chatpdb/debugger.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.0/chatpdb/frame.py` & `chatpdb-0.1.1/chatpdb/frame.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.0/chatpdb/stdout.py` & `chatpdb-0.1.1/chatpdb/stdout.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.0/chatpdb.egg-info/PKG-INFO` & `chatpdb-0.1.1/chatpdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatpdb
-Version: 0.1.0
+Version: 0.1.1
 Summary: A chatgpt enabled python debugger
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/chatpdb
 Project-URL: Issues, https://github.com/never-over/chatpdb/issues
 Keywords: python,chatgpt,pdb,ai,chat,debugger
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `chatpdb-0.1.0/chatpdb.egg-info/SOURCES.txt` & `chatpdb-0.1.1/chatpdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.0/pyproject.toml` & `chatpdb-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "chatpdb"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Caelean Barnes", email="caeleanb@gmail.com" },
   { name="Evan Doyle", email="evanmdoyle@gmail.com" },
 ]
 description = "A chatgpt enabled python debugger"
 readme = "README.md"
 requires-python = ">=3.7"
```

