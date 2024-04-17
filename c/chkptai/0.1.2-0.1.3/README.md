# Comparing `tmp/chkptai-0.1.2.tar.gz` & `tmp/chkptai-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chkptai-0.1.2.tar", last modified: Wed Apr 17 17:14:00 2024, max compression
+gzip compressed data, was "chkptai-0.1.3.tar", last modified: Wed Apr 17 21:59:43 2024, max compression
```

## Comparing `chkptai-0.1.2.tar` & `chkptai-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jp         (501) staff       (20)        0 2024-04-17 17:14:00.190981 chkptai-0.1.2/
--rw-r--r--   0 jp         (501) staff       (20)       97 2024-04-11 22:46:48.000000 chkptai-0.1.2/MANIFEST.in
--rw-r--r--   0 jp         (501) staff       (20)      639 2024-04-17 17:14:00.190751 chkptai-0.1.2/PKG-INFO
--rw-r--r--   0 jp         (501) staff       (20)      103 2024-04-16 18:49:54.000000 chkptai-0.1.2/README.md
--rw-r--r--   0 jp         (501) staff       (20)      733 2024-04-17 16:58:22.000000 chkptai-0.1.2/pyproject.toml
--rw-r--r--   0 jp         (501) staff       (20)       38 2024-04-17 17:14:00.191034 chkptai-0.1.2/setup.cfg
--rw-r--r--   0 jp         (501) staff       (20)      164 2024-04-17 17:13:30.000000 chkptai-0.1.2/setup.py
-drwxr-xr-x   0 jp         (501) staff       (20)        0 2024-04-17 17:14:00.187726 chkptai-0.1.2/src/
-drwxr-xr-x   0 jp         (501) staff       (20)        0 2024-04-17 17:14:00.188645 chkptai-0.1.2/src/chkptai/
--rw-r--r--   0 jp         (501) staff       (20)     6170 2024-04-17 17:12:55.000000 chkptai-0.1.2/src/chkptai/ChkptAI.py
--rw-r--r--   0 jp         (501) staff       (20)       92 2024-04-17 17:13:42.000000 chkptai-0.1.2/src/chkptai/__init__.py
--rw-r--r--   0 jp         (501) staff       (20)     4719 2024-04-13 21:24:58.000000 chkptai-0.1.2/src/chkptai/chkpt_types.py
-drwxr-xr-x   0 jp         (501) staff       (20)        0 2024-04-17 17:14:00.190088 chkptai-0.1.2/src/chkptai.egg-info/
--rw-r--r--   0 jp         (501) staff       (20)      639 2024-04-17 17:14:00.000000 chkptai-0.1.2/src/chkptai.egg-info/PKG-INFO
--rw-r--r--   0 jp         (501) staff       (20)      364 2024-04-17 17:14:00.000000 chkptai-0.1.2/src/chkptai.egg-info/SOURCES.txt
--rw-r--r--   0 jp         (501) staff       (20)        1 2024-04-17 17:14:00.000000 chkptai-0.1.2/src/chkptai.egg-info/dependency_links.txt
--rw-r--r--   0 jp         (501) staff       (20)        1 2024-04-12 22:51:28.000000 chkptai-0.1.2/src/chkptai.egg-info/not-zip-safe
--rw-r--r--   0 jp         (501) staff       (20)       64 2024-04-17 17:14:00.000000 chkptai-0.1.2/src/chkptai.egg-info/requires.txt
--rw-r--r--   0 jp         (501) staff       (20)        8 2024-04-17 17:14:00.000000 chkptai-0.1.2/src/chkptai.egg-info/top_level.txt
-drwxr-xr-x   0 jp         (501) staff       (20)        0 2024-04-17 17:14:00.189845 chkptai-0.1.2/tests/
--rw-r--r--   0 jp         (501) staff       (20)     5063 2024-04-15 21:30:22.000000 chkptai-0.1.2/tests/test_chkptai.py
--rw-r--r--   0 jp         (501) staff       (20)      440 2024-04-15 21:28:38.000000 chkptai-0.1.2/tests/tests.py
+drwxr-xr-x   0 jp         (501) staff       (20)        0 2024-04-17 21:59:43.563193 chkptai-0.1.3/
+-rw-r--r--   0 jp         (501) staff       (20)       97 2024-04-11 22:46:48.000000 chkptai-0.1.3/MANIFEST.in
+-rw-r--r--   0 jp         (501) staff       (20)     2211 2024-04-17 21:59:43.562987 chkptai-0.1.3/PKG-INFO
+-rw-r--r--   0 jp         (501) staff       (20)     1676 2024-04-17 21:56:50.000000 chkptai-0.1.3/README.md
+-rw-r--r--   0 jp         (501) staff       (20)      733 2024-04-17 16:58:22.000000 chkptai-0.1.3/pyproject.toml
+-rw-r--r--   0 jp         (501) staff       (20)       38 2024-04-17 21:59:43.563233 chkptai-0.1.3/setup.cfg
+-rw-r--r--   0 jp         (501) staff       (20)      310 2024-04-17 21:59:18.000000 chkptai-0.1.3/setup.py
+drwxr-xr-x   0 jp         (501) staff       (20)        0 2024-04-17 21:59:43.560365 chkptai-0.1.3/src/
+drwxr-xr-x   0 jp         (501) staff       (20)        0 2024-04-17 21:59:43.561252 chkptai-0.1.3/src/chkptai/
+-rw-r--r--   0 jp         (501) staff       (20)     6156 2024-04-17 20:52:10.000000 chkptai-0.1.3/src/chkptai/ChkptAI.py
+-rw-r--r--   0 jp         (501) staff       (20)       92 2024-04-17 21:59:32.000000 chkptai-0.1.3/src/chkptai/__init__.py
+-rw-r--r--   0 jp         (501) staff       (20)     4719 2024-04-17 20:49:39.000000 chkptai-0.1.3/src/chkptai/chkpt_types.py
+drwxr-xr-x   0 jp         (501) staff       (20)        0 2024-04-17 21:59:43.562535 chkptai-0.1.3/src/chkptai.egg-info/
+-rw-r--r--   0 jp         (501) staff       (20)     2211 2024-04-17 21:59:43.000000 chkptai-0.1.3/src/chkptai.egg-info/PKG-INFO
+-rw-r--r--   0 jp         (501) staff       (20)      364 2024-04-17 21:59:43.000000 chkptai-0.1.3/src/chkptai.egg-info/SOURCES.txt
+-rw-r--r--   0 jp         (501) staff       (20)        1 2024-04-17 21:59:43.000000 chkptai-0.1.3/src/chkptai.egg-info/dependency_links.txt
+-rw-r--r--   0 jp         (501) staff       (20)        1 2024-04-12 22:51:28.000000 chkptai-0.1.3/src/chkptai.egg-info/not-zip-safe
+-rw-r--r--   0 jp         (501) staff       (20)       64 2024-04-17 21:59:43.000000 chkptai-0.1.3/src/chkptai.egg-info/requires.txt
+-rw-r--r--   0 jp         (501) staff       (20)        8 2024-04-17 21:59:43.000000 chkptai-0.1.3/src/chkptai.egg-info/top_level.txt
+drwxr-xr-x   0 jp         (501) staff       (20)        0 2024-04-17 21:59:43.562345 chkptai-0.1.3/tests/
+-rw-r--r--   0 jp         (501) staff       (20)     5063 2024-04-15 21:30:22.000000 chkptai-0.1.3/tests/test_chkptai.py
+-rw-r--r--   0 jp         (501) staff       (20)      440 2024-04-15 21:28:38.000000 chkptai-0.1.3/tests/tests.py
```

### Comparing `chkptai-0.1.2/pyproject.toml` & `chkptai-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chkptai-0.1.2/src/chkptai/ChkptAI.py` & `chkptai-0.1.3/src/chkptai/ChkptAI.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         index: int,
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ):
         """
-        Sends feedback directly using the non-proxied raw client. This method bypasses
+        Sends feedback to Checkpoint-AI's platform. This method bypasses
         the proxy to ensure feedback is sent without interception.
 
         Args:
             response (str | ChkptChatCompletion | ChkptChatCompletionChunk): The response ID or
                 the response object to which feedback is being sent.
             name (str): The name of the feedback parameter.
             value (float): The value of the feedback.
```

### Comparing `chkptai-0.1.2/src/chkptai/chkpt_types.py` & `chkptai-0.1.3/src/chkptai/chkpt_types.py`

 * *Files identical despite different names*

### Comparing `chkptai-0.1.2/tests/test_chkptai.py` & `chkptai-0.1.3/tests/test_chkptai.py`

 * *Files identical despite different names*

