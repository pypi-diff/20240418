# Comparing `tmp/chatpdb-0.1.2.tar.gz` & `tmp/chatpdb-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatpdb-0.1.2.tar", last modified: Thu Apr 18 05:36:46 2024, max compression
+gzip compressed data, was "chatpdb-0.1.3.tar", last modified: Thu Apr 18 05:41:06 2024, max compression
```

## Comparing `chatpdb-0.1.2.tar` & `chatpdb-0.1.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 05:36:46.429484 chatpdb-0.1.2/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)    35149 2024-04-17 01:18:02.000000 chatpdb-0.1.2/LICENSE
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     4287 2024-04-18 05:36:46.429235 chatpdb-0.1.2/PKG-INFO
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2916 2024-04-18 02:40:12.000000 chatpdb-0.1.2/README.md
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 05:36:46.425656 chatpdb-0.1.2/chatpdb/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      657 2024-04-17 22:36:33.000000 chatpdb-0.1.2/chatpdb/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)    10988 2024-04-17 20:47:59.000000 chatpdb-0.1.2/chatpdb/__main__.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 05:36:46.427017 chatpdb-0.1.2/chatpdb/chat/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      126 2024-04-17 20:46:43.000000 chatpdb-0.1.2/chatpdb/chat/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1206 2024-04-18 02:40:12.000000 chatpdb-0.1.2/chatpdb/chat/interface.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 05:36:46.427663 chatpdb-0.1.2/chatpdb/chat/llm/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      132 2024-04-17 20:46:43.000000 chatpdb-0.1.2/chatpdb/chat/llm/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1233 2024-04-17 22:36:33.000000 chatpdb-0.1.2/chatpdb/chat/llm/interface.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1678 2024-04-18 02:40:12.000000 chatpdb-0.1.2/chatpdb/chat/llm/openai.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 05:36:46.428297 chatpdb-0.1.2/chatpdb/chat/prompts/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      243 2024-04-17 20:46:43.000000 chatpdb-0.1.2/chatpdb/chat/prompts/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1753 2024-04-18 02:40:12.000000 chatpdb-0.1.2/chatpdb/chat/prompts/ask.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1901 2024-04-18 02:40:12.000000 chatpdb-0.1.2/chatpdb/chat/prompts/explain.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      546 2024-04-18 02:40:12.000000 chatpdb-0.1.2/chatpdb/chat/prompts/system.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1625 2024-04-18 02:40:12.000000 chatpdb-0.1.2/chatpdb/debugger.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1431 2024-04-18 02:40:12.000000 chatpdb-0.1.2/chatpdb/frame.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1041 2024-04-17 21:33:19.000000 chatpdb-0.1.2/chatpdb/stdout.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 05:36:46.428967 chatpdb-0.1.2/chatpdb.egg-info/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     4287 2024-04-18 05:36:46.000000 chatpdb-0.1.2/chatpdb.egg-info/PKG-INFO
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      608 2024-04-18 05:36:46.000000 chatpdb-0.1.2/chatpdb.egg-info/SOURCES.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-18 05:36:46.000000 chatpdb-0.1.2/chatpdb.egg-info/dependency_links.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       74 2024-04-18 05:36:46.000000 chatpdb-0.1.2/chatpdb.egg-info/requires.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        8 2024-04-18 05:36:46.000000 chatpdb-0.1.2/chatpdb.egg-info/top_level.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1626 2024-04-18 05:36:34.000000 chatpdb-0.1.2/pyproject.toml
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       38 2024-04-18 05:36:46.429537 chatpdb-0.1.2/setup.cfg
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 05:36:46.428760 chatpdb-0.1.2/tests/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      452 2024-04-18 02:40:12.000000 chatpdb-0.1.2/tests/test_debugger.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      432 2024-04-18 02:40:12.000000 chatpdb-0.1.2/tests/test_fixtures.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      454 2024-04-18 02:40:12.000000 chatpdb-0.1.2/tests/test_frame.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 05:41:06.303852 chatpdb-0.1.3/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)    35149 2024-04-17 01:18:02.000000 chatpdb-0.1.3/LICENSE
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     4287 2024-04-18 05:41:06.303628 chatpdb-0.1.3/PKG-INFO
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2916 2024-04-18 02:40:12.000000 chatpdb-0.1.3/README.md
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 05:41:06.299170 chatpdb-0.1.3/chatpdb/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      657 2024-04-17 22:36:33.000000 chatpdb-0.1.3/chatpdb/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)    10988 2024-04-17 20:47:59.000000 chatpdb-0.1.3/chatpdb/__main__.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 05:41:06.300648 chatpdb-0.1.3/chatpdb/chat/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      126 2024-04-17 20:46:43.000000 chatpdb-0.1.3/chatpdb/chat/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1206 2024-04-18 02:40:12.000000 chatpdb-0.1.3/chatpdb/chat/interface.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 05:41:06.301507 chatpdb-0.1.3/chatpdb/chat/llm/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      132 2024-04-17 20:46:43.000000 chatpdb-0.1.3/chatpdb/chat/llm/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1233 2024-04-17 22:36:33.000000 chatpdb-0.1.3/chatpdb/chat/llm/interface.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1678 2024-04-18 02:40:12.000000 chatpdb-0.1.3/chatpdb/chat/llm/openai.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 05:41:06.302543 chatpdb-0.1.3/chatpdb/chat/prompts/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      243 2024-04-17 20:46:43.000000 chatpdb-0.1.3/chatpdb/chat/prompts/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1753 2024-04-18 02:40:12.000000 chatpdb-0.1.3/chatpdb/chat/prompts/ask.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1901 2024-04-18 02:40:12.000000 chatpdb-0.1.3/chatpdb/chat/prompts/explain.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      546 2024-04-18 02:40:12.000000 chatpdb-0.1.3/chatpdb/chat/prompts/system.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1625 2024-04-18 02:40:12.000000 chatpdb-0.1.3/chatpdb/debugger.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1431 2024-04-18 02:40:12.000000 chatpdb-0.1.3/chatpdb/frame.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1041 2024-04-17 21:33:19.000000 chatpdb-0.1.3/chatpdb/stdout.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 05:41:06.303345 chatpdb-0.1.3/chatpdb.egg-info/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     4287 2024-04-18 05:41:06.000000 chatpdb-0.1.3/chatpdb.egg-info/PKG-INFO
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      608 2024-04-18 05:41:06.000000 chatpdb-0.1.3/chatpdb.egg-info/SOURCES.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-18 05:41:06.000000 chatpdb-0.1.3/chatpdb.egg-info/dependency_links.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       74 2024-04-18 05:41:06.000000 chatpdb-0.1.3/chatpdb.egg-info/requires.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        8 2024-04-18 05:41:06.000000 chatpdb-0.1.3/chatpdb.egg-info/top_level.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1626 2024-04-18 05:40:41.000000 chatpdb-0.1.3/pyproject.toml
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       38 2024-04-18 05:41:06.303907 chatpdb-0.1.3/setup.cfg
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 05:41:06.303115 chatpdb-0.1.3/tests/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      452 2024-04-18 02:40:12.000000 chatpdb-0.1.3/tests/test_debugger.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      432 2024-04-18 02:40:12.000000 chatpdb-0.1.3/tests/test_fixtures.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      454 2024-04-18 02:40:12.000000 chatpdb-0.1.3/tests/test_frame.py
```

### Comparing `chatpdb-0.1.2/LICENSE` & `chatpdb-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.2/PKG-INFO` & `chatpdb-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatpdb
-Version: 0.1.2
+Version: 0.1.3
 Summary: A chatgpt enabled python debugger
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/chatpdb
 Project-URL: Issues, https://github.com/never-over/chatpdb/issues
 Keywords: python,chatgpt,pdb,ai,chat,debugger
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `chatpdb-0.1.2/README.md` & `chatpdb-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.2/chatpdb/__init__.py` & `chatpdb-0.1.3/chatpdb/__init__.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.2/chatpdb/__main__.py` & `chatpdb-0.1.3/chatpdb/__main__.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.2/chatpdb/chat/interface.py` & `chatpdb-0.1.3/chatpdb/chat/interface.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.2/chatpdb/chat/llm/interface.py` & `chatpdb-0.1.3/chatpdb/chat/llm/interface.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.2/chatpdb/chat/llm/openai.py` & `chatpdb-0.1.3/chatpdb/chat/llm/openai.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.2/chatpdb/chat/prompts/ask.py` & `chatpdb-0.1.3/chatpdb/chat/prompts/ask.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.2/chatpdb/chat/prompts/explain.py` & `chatpdb-0.1.3/chatpdb/chat/prompts/explain.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.2/chatpdb/chat/prompts/system.py` & `chatpdb-0.1.3/chatpdb/chat/prompts/system.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.2/chatpdb/debugger.py` & `chatpdb-0.1.3/chatpdb/debugger.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.2/chatpdb/frame.py` & `chatpdb-0.1.3/chatpdb/frame.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.2/chatpdb/stdout.py` & `chatpdb-0.1.3/chatpdb/stdout.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.2/chatpdb.egg-info/PKG-INFO` & `chatpdb-0.1.3/chatpdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatpdb
-Version: 0.1.2
+Version: 0.1.3
 Summary: A chatgpt enabled python debugger
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/chatpdb
 Project-URL: Issues, https://github.com/never-over/chatpdb/issues
 Keywords: python,chatgpt,pdb,ai,chat,debugger
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `chatpdb-0.1.2/chatpdb.egg-info/SOURCES.txt` & `chatpdb-0.1.3/chatpdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.2/pyproject.toml` & `chatpdb-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "chatpdb"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Caelean Barnes", email="caeleanb@gmail.com" },
   { name="Evan Doyle", email="evanmdoyle@gmail.com" },
 ]
 description = "A chatgpt enabled python debugger"
 readme = "README.md"
 requires-python = ">=3.7"
```

