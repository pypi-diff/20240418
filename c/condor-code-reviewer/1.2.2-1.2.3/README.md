# Comparing `tmp/condor_code_reviewer-1.2.2.tar.gz` & `tmp/condor_code_reviewer-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "condor_code_reviewer-1.2.2.tar", last modified: Thu Apr 18 03:57:21 2024, max compression
+gzip compressed data, was "condor_code_reviewer-1.2.3.tar", last modified: Thu Apr 18 04:06:11 2024, max compression
```

## Comparing `condor_code_reviewer-1.2.2.tar` & `condor_code_reviewer-1.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:57:21.232640 condor_code_reviewer-1.2.2/
--rw-r--r--   0 cparedesr   (501) staff       (20)      110 2024-04-18 03:57:21.232386 condor_code_reviewer-1.2.2/PKG-INFO
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:57:21.232075 condor_code_reviewer-1.2.2/condor_code_reviewer.egg-info/
--rw-r--r--   0 cparedesr   (501) staff       (20)      110 2024-04-18 03:57:21.000000 condor_code_reviewer-1.2.2/condor_code_reviewer.egg-info/PKG-INFO
--rw-r--r--   0 cparedesr   (501) staff       (20)      386 2024-04-18 03:57:21.000000 condor_code_reviewer-1.2.2/condor_code_reviewer.egg-info/SOURCES.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)        1 2024-04-18 03:57:21.000000 condor_code_reviewer-1.2.2/condor_code_reviewer.egg-info/dependency_links.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)       40 2024-04-18 03:57:21.000000 condor_code_reviewer-1.2.2/condor_code_reviewer.egg-info/entry_points.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)       16 2024-04-18 03:57:21.000000 condor_code_reviewer-1.2.2/condor_code_reviewer.egg-info/requires.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)        4 2024-04-18 03:57:21.000000 condor_code_reviewer-1.2.2/condor_code_reviewer.egg-info/top_level.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)       38 2024-04-18 03:57:21.232715 condor_code_reviewer-1.2.2/setup.cfg
--rw-r--r--   0 cparedesr   (501) staff       (20)      307 2024-04-18 03:57:20.000000 condor_code_reviewer-1.2.2/setup.py
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:57:21.230735 condor_code_reviewer-1.2.2/src/
--rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-26 23:26:52.000000 condor_code_reviewer-1.2.2/src/__init__.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     1948 2024-03-27 00:51:27.000000 condor_code_reviewer-1.2.2/src/cli.py
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:57:21.231739 condor_code_reviewer-1.2.2/src/lib/
--rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-19 00:32:11.000000 condor_code_reviewer-1.2.2/src/lib/__init__.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     2876 2024-04-18 03:57:06.000000 condor_code_reviewer-1.2.2/src/lib/github_pr.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     1688 2024-03-19 00:32:11.000000 condor_code_reviewer-1.2.2/src/lib/openai_assistant.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     2124 2024-04-18 03:57:10.000000 condor_code_reviewer-1.2.2/src/reviewer.py
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:06:11.428070 condor_code_reviewer-1.2.3/
+-rw-r--r--   0 cparedesr   (501) staff       (20)      110 2024-04-18 04:06:11.427871 condor_code_reviewer-1.2.3/PKG-INFO
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:06:11.427684 condor_code_reviewer-1.2.3/condor_code_reviewer.egg-info/
+-rw-r--r--   0 cparedesr   (501) staff       (20)      110 2024-04-18 04:06:11.000000 condor_code_reviewer-1.2.3/condor_code_reviewer.egg-info/PKG-INFO
+-rw-r--r--   0 cparedesr   (501) staff       (20)      386 2024-04-18 04:06:11.000000 condor_code_reviewer-1.2.3/condor_code_reviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)        1 2024-04-18 04:06:11.000000 condor_code_reviewer-1.2.3/condor_code_reviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)       40 2024-04-18 04:06:11.000000 condor_code_reviewer-1.2.3/condor_code_reviewer.egg-info/entry_points.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)       16 2024-04-18 04:06:11.000000 condor_code_reviewer-1.2.3/condor_code_reviewer.egg-info/requires.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)        4 2024-04-18 04:06:11.000000 condor_code_reviewer-1.2.3/condor_code_reviewer.egg-info/top_level.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)       38 2024-04-18 04:06:11.428110 condor_code_reviewer-1.2.3/setup.cfg
+-rw-r--r--   0 cparedesr   (501) staff       (20)      307 2024-04-18 04:06:07.000000 condor_code_reviewer-1.2.3/setup.py
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:06:11.426750 condor_code_reviewer-1.2.3/src/
+-rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-26 23:26:52.000000 condor_code_reviewer-1.2.3/src/__init__.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     1948 2024-03-27 00:51:27.000000 condor_code_reviewer-1.2.3/src/cli.py
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:06:11.427383 condor_code_reviewer-1.2.3/src/lib/
+-rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-19 00:32:11.000000 condor_code_reviewer-1.2.3/src/lib/__init__.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     2876 2024-04-18 03:57:06.000000 condor_code_reviewer-1.2.3/src/lib/github_pr.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     1688 2024-03-19 00:32:11.000000 condor_code_reviewer-1.2.3/src/lib/openai_assistant.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     2119 2024-04-18 04:05:31.000000 condor_code_reviewer-1.2.3/src/reviewer.py
```

### Comparing `condor_code_reviewer-1.2.2/src/cli.py` & `condor_code_reviewer-1.2.3/src/cli.py`

 * *Files identical despite different names*

### Comparing `condor_code_reviewer-1.2.2/src/lib/github_pr.py` & `condor_code_reviewer-1.2.3/src/lib/github_pr.py`

 * *Files identical despite different names*

### Comparing `condor_code_reviewer-1.2.2/src/lib/openai_assistant.py` & `condor_code_reviewer-1.2.3/src/lib/openai_assistant.py`

 * *Files identical despite different names*

### Comparing `condor_code_reviewer-1.2.2/src/reviewer.py` & `condor_code_reviewer-1.2.3/src/reviewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     def add_commit_messages(self):
         messages = "\n".join(self.gh.get_commit_messages())
         self.assistant.add_and_retrieve_message(messages, "user")
 
     def review_files(self):
         for filename in self.gh.get_modified_files():
-            diff, pos = self.gh.get_file_diff(filename)
+            diff = self.gh.get_file_diff(filename)
             message = f"Reviewing file: {filename}.\nDiff:\n\n{diff}"
 
             response = self.assistant.add_and_retrieve_message(message, "user")
 
             if response and response != 'APIError: No response':
                 self.gh.comment_on_file(filename, response)
```

