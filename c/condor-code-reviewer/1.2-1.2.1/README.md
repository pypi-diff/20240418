# Comparing `tmp/condor_code_reviewer-1.2.tar.gz` & `tmp/condor_code_reviewer-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "condor_code_reviewer-1.2.tar", last modified: Thu Apr 18 03:49:49 2024, max compression
+gzip compressed data, was "condor_code_reviewer-1.2.1.tar", last modified: Thu Apr 18 03:54:52 2024, max compression
```

## Comparing `condor_code_reviewer-1.2.tar` & `condor_code_reviewer-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:49:49.163848 condor_code_reviewer-1.2/
--rw-r--r--   0 cparedesr   (501) staff       (20)      108 2024-04-18 03:49:49.163597 condor_code_reviewer-1.2/PKG-INFO
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:49:49.163393 condor_code_reviewer-1.2/condor_code_reviewer.egg-info/
--rw-r--r--   0 cparedesr   (501) staff       (20)      108 2024-04-18 03:49:49.000000 condor_code_reviewer-1.2/condor_code_reviewer.egg-info/PKG-INFO
--rw-r--r--   0 cparedesr   (501) staff       (20)      386 2024-04-18 03:49:49.000000 condor_code_reviewer-1.2/condor_code_reviewer.egg-info/SOURCES.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)        1 2024-04-18 03:49:49.000000 condor_code_reviewer-1.2/condor_code_reviewer.egg-info/dependency_links.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)       40 2024-04-18 03:49:49.000000 condor_code_reviewer-1.2/condor_code_reviewer.egg-info/entry_points.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)       16 2024-04-18 03:49:49.000000 condor_code_reviewer-1.2/condor_code_reviewer.egg-info/requires.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)        4 2024-04-18 03:49:49.000000 condor_code_reviewer-1.2/condor_code_reviewer.egg-info/top_level.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)       38 2024-04-18 03:49:49.163904 condor_code_reviewer-1.2/setup.cfg
--rw-r--r--   0 cparedesr   (501) staff       (20)      305 2024-04-18 03:49:41.000000 condor_code_reviewer-1.2/setup.py
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:49:49.162833 condor_code_reviewer-1.2/src/
--rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-26 23:26:52.000000 condor_code_reviewer-1.2/src/__init__.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     1948 2024-03-27 00:51:27.000000 condor_code_reviewer-1.2/src/cli.py
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:49:49.163193 condor_code_reviewer-1.2/src/lib/
--rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-19 00:32:11.000000 condor_code_reviewer-1.2/src/lib/__init__.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     2902 2024-03-19 12:49:30.000000 condor_code_reviewer-1.2/src/lib/github_pr.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     1688 2024-03-19 00:32:11.000000 condor_code_reviewer-1.2/src/lib/openai_assistant.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     2176 2024-04-18 03:48:59.000000 condor_code_reviewer-1.2/src/reviewer.py
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:54:52.702907 condor_code_reviewer-1.2.1/
+-rw-r--r--   0 cparedesr   (501) staff       (20)      110 2024-04-18 03:54:52.702691 condor_code_reviewer-1.2.1/PKG-INFO
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:54:52.702477 condor_code_reviewer-1.2.1/condor_code_reviewer.egg-info/
+-rw-r--r--   0 cparedesr   (501) staff       (20)      110 2024-04-18 03:54:52.000000 condor_code_reviewer-1.2.1/condor_code_reviewer.egg-info/PKG-INFO
+-rw-r--r--   0 cparedesr   (501) staff       (20)      386 2024-04-18 03:54:52.000000 condor_code_reviewer-1.2.1/condor_code_reviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)        1 2024-04-18 03:54:52.000000 condor_code_reviewer-1.2.1/condor_code_reviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)       40 2024-04-18 03:54:52.000000 condor_code_reviewer-1.2.1/condor_code_reviewer.egg-info/entry_points.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)       16 2024-04-18 03:54:52.000000 condor_code_reviewer-1.2.1/condor_code_reviewer.egg-info/requires.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)        4 2024-04-18 03:54:52.000000 condor_code_reviewer-1.2.1/condor_code_reviewer.egg-info/top_level.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)       38 2024-04-18 03:54:52.702947 condor_code_reviewer-1.2.1/setup.cfg
+-rw-r--r--   0 cparedesr   (501) staff       (20)      307 2024-04-18 03:54:51.000000 condor_code_reviewer-1.2.1/setup.py
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:54:52.701652 condor_code_reviewer-1.2.1/src/
+-rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-26 23:26:52.000000 condor_code_reviewer-1.2.1/src/__init__.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     1948 2024-03-27 00:51:27.000000 condor_code_reviewer-1.2.1/src/cli.py
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:54:52.702188 condor_code_reviewer-1.2.1/src/lib/
+-rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-19 00:32:11.000000 condor_code_reviewer-1.2.1/src/lib/__init__.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     2953 2024-04-18 03:54:26.000000 condor_code_reviewer-1.2.1/src/lib/github_pr.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     1688 2024-03-19 00:32:11.000000 condor_code_reviewer-1.2.1/src/lib/openai_assistant.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     2129 2024-04-18 03:54:37.000000 condor_code_reviewer-1.2.1/src/reviewer.py
```

### Comparing `condor_code_reviewer-1.2/src/cli.py` & `condor_code_reviewer-1.2.1/src/cli.py`

 * *Files identical despite different names*

### Comparing `condor_code_reviewer-1.2/src/lib/github_pr.py` & `condor_code_reviewer-1.2.1/src/lib/github_pr.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,17 @@
     def get_last_commit(self):
         return self.get_commits().reversed[0]
 
     def get_file_content(self, filename):
         return self.get_repo().get_contents(filename).decoded_content.decode('utf-8')
     
     def get_file_diff(self, filename):
-        return self.get_modified_files()[filename].patch
+        file_diff = self.get_modified_files()[filename]
+
+        return file_diff.patch, file_diff.position
     
     def comment_on_file(self, filename, comment, line=1):
         self.pr.create_review_comment(
             comment,
             self.get_last_commit(),
             filename,
             line
```

### Comparing `condor_code_reviewer-1.2/src/lib/openai_assistant.py` & `condor_code_reviewer-1.2.1/src/lib/openai_assistant.py`

 * *Files identical despite different names*

### Comparing `condor_code_reviewer-1.2/src/reviewer.py` & `condor_code_reviewer-1.2.1/src/reviewer.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,22 +27,21 @@
 
     def add_commit_messages(self):
         messages = "\n".join(self.gh.get_commit_messages())
         self.assistant.add_and_retrieve_message(messages, "user")
 
     def review_files(self):
         for filename in self.gh.get_modified_files():
-            diff = self.gh.get_file_diff(filename)
+            diff, pos = self.gh.get_file_diff(filename)
             message = f"Reviewing file: {filename}.\nDiff:\n\n{diff}"
 
             response = self.assistant.add_and_retrieve_message(message, "user")
-            first_line = diff.split("\n")[0]
 
             if response and response != 'APIError: No response':
-                self.gh.comment_on_file(filename, response, first_line)
+                self.gh.comment_on_file(filename, response, pos)
 
     def summary_review(self):
         summary = self.assistant.add_and_retrieve_message("Summary Review", "user")
         self.gh.comment_on_pr(summary)
 
     def add_step(self, func, system_message=None):
         def wrapper(*args, **kwargs):
```

