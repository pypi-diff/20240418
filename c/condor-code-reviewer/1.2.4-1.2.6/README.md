# Comparing `tmp/condor_code_reviewer-1.2.4.tar.gz` & `tmp/condor_code_reviewer-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "condor_code_reviewer-1.2.4.tar", last modified: Thu Apr 18 04:08:31 2024, max compression
+gzip compressed data, was "condor_code_reviewer-1.2.6.tar", last modified: Thu Apr 18 04:14:45 2024, max compression
```

## Comparing `condor_code_reviewer-1.2.4.tar` & `condor_code_reviewer-1.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:08:31.738992 condor_code_reviewer-1.2.4/
--rw-r--r--   0 cparedesr   (501) staff       (20)      110 2024-04-18 04:08:31.738758 condor_code_reviewer-1.2.4/PKG-INFO
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:08:31.738529 condor_code_reviewer-1.2.4/condor_code_reviewer.egg-info/
--rw-r--r--   0 cparedesr   (501) staff       (20)      110 2024-04-18 04:08:31.000000 condor_code_reviewer-1.2.4/condor_code_reviewer.egg-info/PKG-INFO
--rw-r--r--   0 cparedesr   (501) staff       (20)      386 2024-04-18 04:08:31.000000 condor_code_reviewer-1.2.4/condor_code_reviewer.egg-info/SOURCES.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)        1 2024-04-18 04:08:31.000000 condor_code_reviewer-1.2.4/condor_code_reviewer.egg-info/dependency_links.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)       40 2024-04-18 04:08:31.000000 condor_code_reviewer-1.2.4/condor_code_reviewer.egg-info/entry_points.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)       16 2024-04-18 04:08:31.000000 condor_code_reviewer-1.2.4/condor_code_reviewer.egg-info/requires.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)        4 2024-04-18 04:08:31.000000 condor_code_reviewer-1.2.4/condor_code_reviewer.egg-info/top_level.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)       38 2024-04-18 04:08:31.739034 condor_code_reviewer-1.2.4/setup.cfg
--rw-r--r--   0 cparedesr   (501) staff       (20)      307 2024-04-18 04:08:28.000000 condor_code_reviewer-1.2.4/setup.py
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:08:31.737593 condor_code_reviewer-1.2.4/src/
--rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-26 23:26:52.000000 condor_code_reviewer-1.2.4/src/__init__.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     1948 2024-03-27 00:51:27.000000 condor_code_reviewer-1.2.4/src/cli.py
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:08:31.738165 condor_code_reviewer-1.2.4/src/lib/
--rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-19 00:32:11.000000 condor_code_reviewer-1.2.4/src/lib/__init__.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     2876 2024-04-18 03:57:06.000000 condor_code_reviewer-1.2.4/src/lib/github_pr.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     1688 2024-03-19 00:32:11.000000 condor_code_reviewer-1.2.4/src/lib/openai_assistant.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     2119 2024-04-18 04:08:13.000000 condor_code_reviewer-1.2.4/src/reviewer.py
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:14:45.052969 condor_code_reviewer-1.2.6/
+-rw-r--r--   0 cparedesr   (501) staff       (20)      110 2024-04-18 04:14:45.052755 condor_code_reviewer-1.2.6/PKG-INFO
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:14:45.052552 condor_code_reviewer-1.2.6/condor_code_reviewer.egg-info/
+-rw-r--r--   0 cparedesr   (501) staff       (20)      110 2024-04-18 04:14:45.000000 condor_code_reviewer-1.2.6/condor_code_reviewer.egg-info/PKG-INFO
+-rw-r--r--   0 cparedesr   (501) staff       (20)      386 2024-04-18 04:14:45.000000 condor_code_reviewer-1.2.6/condor_code_reviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)        1 2024-04-18 04:14:45.000000 condor_code_reviewer-1.2.6/condor_code_reviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)       40 2024-04-18 04:14:45.000000 condor_code_reviewer-1.2.6/condor_code_reviewer.egg-info/entry_points.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)       16 2024-04-18 04:14:45.000000 condor_code_reviewer-1.2.6/condor_code_reviewer.egg-info/requires.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)        4 2024-04-18 04:14:45.000000 condor_code_reviewer-1.2.6/condor_code_reviewer.egg-info/top_level.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)       38 2024-04-18 04:14:45.053009 condor_code_reviewer-1.2.6/setup.cfg
+-rw-r--r--   0 cparedesr   (501) staff       (20)      307 2024-04-18 04:14:39.000000 condor_code_reviewer-1.2.6/setup.py
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:14:45.051829 condor_code_reviewer-1.2.6/src/
+-rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-26 23:26:52.000000 condor_code_reviewer-1.2.6/src/__init__.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     1948 2024-03-27 00:51:27.000000 condor_code_reviewer-1.2.6/src/cli.py
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:14:45.052291 condor_code_reviewer-1.2.6/src/lib/
+-rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-19 00:32:11.000000 condor_code_reviewer-1.2.6/src/lib/__init__.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     2902 2024-04-18 04:10:06.000000 condor_code_reviewer-1.2.6/src/lib/github_pr.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     1688 2024-03-19 00:32:11.000000 condor_code_reviewer-1.2.6/src/lib/openai_assistant.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     2399 2024-04-18 04:14:33.000000 condor_code_reviewer-1.2.6/src/reviewer.py
```

### Comparing `condor_code_reviewer-1.2.4/src/cli.py` & `condor_code_reviewer-1.2.6/src/cli.py`

 * *Files identical despite different names*

### Comparing `condor_code_reviewer-1.2.4/src/lib/github_pr.py` & `condor_code_reviewer-1.2.6/src/lib/github_pr.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,19 +56,20 @@
 
     def get_file_content(self, filename):
         return self.get_repo().get_contents(filename).decoded_content.decode('utf-8')
     
     def get_file_diff(self, filename):
         return self.get_modified_files()[filename].patch
     
-    def comment_on_file(self, filename, comment):
+    def comment_on_file(self, filename, comment, line=1):
         self.pr.create_review_comment(
             comment,
             self.get_last_commit(),
-            filename
+            filename,
+            line
         )
 
     def comment_on_pr(self, comment):
         self.pr.create_issue_comment(comment)
     
     def _set_repository_name_and_pr_number(self):
         owner, repo, number = self.__match_pull_request_url()
```

### Comparing `condor_code_reviewer-1.2.4/src/lib/openai_assistant.py` & `condor_code_reviewer-1.2.6/src/lib/openai_assistant.py`

 * *Files identical despite different names*

### Comparing `condor_code_reviewer-1.2.4/src/reviewer.py` & `condor_code_reviewer-1.2.6/src/reviewer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 from .lib.github_pr import GithubPR 
 from .lib.openai_assistant import OpenAIAssistant
 
 class Reviewer:
     def __init__(self, openai_api_key, assistant_id, gh_api_key, pull_request_url):
         self.gh = GithubPR(gh_api_key, pull_request_url)
         self.assistant = OpenAIAssistant(openai_api_key, assistant_id)
@@ -32,16 +33,25 @@
     def review_files(self):
         for filename in self.gh.get_modified_files():
             diff = self.gh.get_file_diff(filename)
             message = f"Reviewing file: {filename}.\nDiff:\n\n{diff}"
 
             response = self.assistant.add_and_retrieve_message(message, "user")
 
+            first_change_line = self._get_first_change_line(diff)
+
             if response and response != 'APIError: No response':
-                self.gh.comment_on_file(filename, response)
+                self.gh.comment_on_file(filename, response, first_change_line)
+
+    def _get_first_change_line(self, diff):
+        match = re.search(r'@@ -(\d+),', diff)
+        if match:
+            return int(match.group(1))
+        else:
+            return 1
 
     def summary_review(self):
         summary = self.assistant.add_and_retrieve_message("Summary Review", "user")
         self.gh.comment_on_pr(summary)
 
     def add_step(self, func, system_message=None):
         def wrapper(*args, **kwargs):
```

