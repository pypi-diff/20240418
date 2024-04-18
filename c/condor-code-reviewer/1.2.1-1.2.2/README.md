# Comparing `tmp/condor_code_reviewer-1.2.1.tar.gz` & `tmp/condor_code_reviewer-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "condor_code_reviewer-1.2.1.tar", last modified: Thu Apr 18 03:54:52 2024, max compression
+gzip compressed data, was "condor_code_reviewer-1.2.2.tar", last modified: Thu Apr 18 03:57:21 2024, max compression
```

## Comparing `condor_code_reviewer-1.2.1.tar` & `condor_code_reviewer-1.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:54:52.702907 condor_code_reviewer-1.2.1/
--rw-r--r--   0 cparedesr   (501) staff       (20)      110 2024-04-18 03:54:52.702691 condor_code_reviewer-1.2.1/PKG-INFO
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:54:52.702477 condor_code_reviewer-1.2.1/condor_code_reviewer.egg-info/
--rw-r--r--   0 cparedesr   (501) staff       (20)      110 2024-04-18 03:54:52.000000 condor_code_reviewer-1.2.1/condor_code_reviewer.egg-info/PKG-INFO
--rw-r--r--   0 cparedesr   (501) staff       (20)      386 2024-04-18 03:54:52.000000 condor_code_reviewer-1.2.1/condor_code_reviewer.egg-info/SOURCES.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)        1 2024-04-18 03:54:52.000000 condor_code_reviewer-1.2.1/condor_code_reviewer.egg-info/dependency_links.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)       40 2024-04-18 03:54:52.000000 condor_code_reviewer-1.2.1/condor_code_reviewer.egg-info/entry_points.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)       16 2024-04-18 03:54:52.000000 condor_code_reviewer-1.2.1/condor_code_reviewer.egg-info/requires.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)        4 2024-04-18 03:54:52.000000 condor_code_reviewer-1.2.1/condor_code_reviewer.egg-info/top_level.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)       38 2024-04-18 03:54:52.702947 condor_code_reviewer-1.2.1/setup.cfg
--rw-r--r--   0 cparedesr   (501) staff       (20)      307 2024-04-18 03:54:51.000000 condor_code_reviewer-1.2.1/setup.py
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:54:52.701652 condor_code_reviewer-1.2.1/src/
--rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-26 23:26:52.000000 condor_code_reviewer-1.2.1/src/__init__.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     1948 2024-03-27 00:51:27.000000 condor_code_reviewer-1.2.1/src/cli.py
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:54:52.702188 condor_code_reviewer-1.2.1/src/lib/
--rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-19 00:32:11.000000 condor_code_reviewer-1.2.1/src/lib/__init__.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     2953 2024-04-18 03:54:26.000000 condor_code_reviewer-1.2.1/src/lib/github_pr.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     1688 2024-03-19 00:32:11.000000 condor_code_reviewer-1.2.1/src/lib/openai_assistant.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     2129 2024-04-18 03:54:37.000000 condor_code_reviewer-1.2.1/src/reviewer.py
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:57:21.232640 condor_code_reviewer-1.2.2/
+-rw-r--r--   0 cparedesr   (501) staff       (20)      110 2024-04-18 03:57:21.232386 condor_code_reviewer-1.2.2/PKG-INFO
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:57:21.232075 condor_code_reviewer-1.2.2/condor_code_reviewer.egg-info/
+-rw-r--r--   0 cparedesr   (501) staff       (20)      110 2024-04-18 03:57:21.000000 condor_code_reviewer-1.2.2/condor_code_reviewer.egg-info/PKG-INFO
+-rw-r--r--   0 cparedesr   (501) staff       (20)      386 2024-04-18 03:57:21.000000 condor_code_reviewer-1.2.2/condor_code_reviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)        1 2024-04-18 03:57:21.000000 condor_code_reviewer-1.2.2/condor_code_reviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)       40 2024-04-18 03:57:21.000000 condor_code_reviewer-1.2.2/condor_code_reviewer.egg-info/entry_points.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)       16 2024-04-18 03:57:21.000000 condor_code_reviewer-1.2.2/condor_code_reviewer.egg-info/requires.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)        4 2024-04-18 03:57:21.000000 condor_code_reviewer-1.2.2/condor_code_reviewer.egg-info/top_level.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)       38 2024-04-18 03:57:21.232715 condor_code_reviewer-1.2.2/setup.cfg
+-rw-r--r--   0 cparedesr   (501) staff       (20)      307 2024-04-18 03:57:20.000000 condor_code_reviewer-1.2.2/setup.py
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:57:21.230735 condor_code_reviewer-1.2.2/src/
+-rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-26 23:26:52.000000 condor_code_reviewer-1.2.2/src/__init__.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     1948 2024-03-27 00:51:27.000000 condor_code_reviewer-1.2.2/src/cli.py
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:57:21.231739 condor_code_reviewer-1.2.2/src/lib/
+-rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-19 00:32:11.000000 condor_code_reviewer-1.2.2/src/lib/__init__.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     2876 2024-04-18 03:57:06.000000 condor_code_reviewer-1.2.2/src/lib/github_pr.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     1688 2024-03-19 00:32:11.000000 condor_code_reviewer-1.2.2/src/lib/openai_assistant.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     2124 2024-04-18 03:57:10.000000 condor_code_reviewer-1.2.2/src/reviewer.py
```

### Comparing `condor_code_reviewer-1.2.1/src/cli.py` & `condor_code_reviewer-1.2.2/src/cli.py`

 * *Files identical despite different names*

### Comparing `condor_code_reviewer-1.2.1/src/lib/github_pr.py` & `condor_code_reviewer-1.2.2/src/lib/github_pr.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,24 +54,21 @@
     def get_last_commit(self):
         return self.get_commits().reversed[0]
 
     def get_file_content(self, filename):
         return self.get_repo().get_contents(filename).decoded_content.decode('utf-8')
     
     def get_file_diff(self, filename):
-        file_diff = self.get_modified_files()[filename]
-
-        return file_diff.patch, file_diff.position
+        return self.get_modified_files()[filename].patch
     
-    def comment_on_file(self, filename, comment, line=1):
+    def comment_on_file(self, filename, comment):
         self.pr.create_review_comment(
             comment,
             self.get_last_commit(),
-            filename,
-            line
+            filename
         )
 
     def comment_on_pr(self, comment):
         self.pr.create_issue_comment(comment)
     
     def _set_repository_name_and_pr_number(self):
         owner, repo, number = self.__match_pull_request_url()
```

### Comparing `condor_code_reviewer-1.2.1/src/lib/openai_assistant.py` & `condor_code_reviewer-1.2.2/src/lib/openai_assistant.py`

 * *Files identical despite different names*

### Comparing `condor_code_reviewer-1.2.1/src/reviewer.py` & `condor_code_reviewer-1.2.2/src/reviewer.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         for filename in self.gh.get_modified_files():
             diff, pos = self.gh.get_file_diff(filename)
             message = f"Reviewing file: {filename}.\nDiff:\n\n{diff}"
 
             response = self.assistant.add_and_retrieve_message(message, "user")
 
             if response and response != 'APIError: No response':
-                self.gh.comment_on_file(filename, response, pos)
+                self.gh.comment_on_file(filename, response)
 
     def summary_review(self):
         summary = self.assistant.add_and_retrieve_message("Summary Review", "user")
         self.gh.comment_on_pr(summary)
 
     def add_step(self, func, system_message=None):
         def wrapper(*args, **kwargs):
```

