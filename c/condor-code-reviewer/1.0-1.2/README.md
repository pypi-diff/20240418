# Comparing `tmp/condor_code_reviewer-1.0.tar.gz` & `tmp/condor_code_reviewer-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "condor_code_reviewer-1.0.tar", last modified: Thu Apr 18 03:41:40 2024, max compression
+gzip compressed data, was "condor_code_reviewer-1.2.tar", last modified: Thu Apr 18 03:49:49 2024, max compression
```

## Comparing `condor_code_reviewer-1.0.tar` & `condor_code_reviewer-1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:41:40.818978 condor_code_reviewer-1.0/
--rw-r--r--   0 cparedesr   (501) staff       (20)      108 2024-04-18 03:41:40.818736 condor_code_reviewer-1.0/PKG-INFO
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:41:40.818494 condor_code_reviewer-1.0/condor_code_reviewer.egg-info/
--rw-r--r--   0 cparedesr   (501) staff       (20)      108 2024-04-18 03:41:40.000000 condor_code_reviewer-1.0/condor_code_reviewer.egg-info/PKG-INFO
--rw-r--r--   0 cparedesr   (501) staff       (20)      386 2024-04-18 03:41:40.000000 condor_code_reviewer-1.0/condor_code_reviewer.egg-info/SOURCES.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)        1 2024-04-18 03:41:40.000000 condor_code_reviewer-1.0/condor_code_reviewer.egg-info/dependency_links.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)       40 2024-04-18 03:41:40.000000 condor_code_reviewer-1.0/condor_code_reviewer.egg-info/entry_points.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)       16 2024-04-18 03:41:40.000000 condor_code_reviewer-1.0/condor_code_reviewer.egg-info/requires.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)        4 2024-04-18 03:41:40.000000 condor_code_reviewer-1.0/condor_code_reviewer.egg-info/top_level.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)       38 2024-04-18 03:41:40.819025 condor_code_reviewer-1.0/setup.cfg
--rw-r--r--   0 cparedesr   (501) staff       (20)      305 2024-04-18 03:41:12.000000 condor_code_reviewer-1.0/setup.py
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:41:40.817440 condor_code_reviewer-1.0/src/
--rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-26 23:26:52.000000 condor_code_reviewer-1.0/src/__init__.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     1948 2024-03-27 00:51:27.000000 condor_code_reviewer-1.0/src/cli.py
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:41:40.818133 condor_code_reviewer-1.0/src/lib/
--rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-19 00:32:11.000000 condor_code_reviewer-1.0/src/lib/__init__.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     2902 2024-03-19 12:49:30.000000 condor_code_reviewer-1.0/src/lib/github_pr.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     1688 2024-03-19 00:32:11.000000 condor_code_reviewer-1.0/src/lib/openai_assistant.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     2120 2024-04-18 03:38:52.000000 condor_code_reviewer-1.0/src/reviewer.py
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:49:49.163848 condor_code_reviewer-1.2/
+-rw-r--r--   0 cparedesr   (501) staff       (20)      108 2024-04-18 03:49:49.163597 condor_code_reviewer-1.2/PKG-INFO
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:49:49.163393 condor_code_reviewer-1.2/condor_code_reviewer.egg-info/
+-rw-r--r--   0 cparedesr   (501) staff       (20)      108 2024-04-18 03:49:49.000000 condor_code_reviewer-1.2/condor_code_reviewer.egg-info/PKG-INFO
+-rw-r--r--   0 cparedesr   (501) staff       (20)      386 2024-04-18 03:49:49.000000 condor_code_reviewer-1.2/condor_code_reviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)        1 2024-04-18 03:49:49.000000 condor_code_reviewer-1.2/condor_code_reviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)       40 2024-04-18 03:49:49.000000 condor_code_reviewer-1.2/condor_code_reviewer.egg-info/entry_points.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)       16 2024-04-18 03:49:49.000000 condor_code_reviewer-1.2/condor_code_reviewer.egg-info/requires.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)        4 2024-04-18 03:49:49.000000 condor_code_reviewer-1.2/condor_code_reviewer.egg-info/top_level.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)       38 2024-04-18 03:49:49.163904 condor_code_reviewer-1.2/setup.cfg
+-rw-r--r--   0 cparedesr   (501) staff       (20)      305 2024-04-18 03:49:41.000000 condor_code_reviewer-1.2/setup.py
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:49:49.162833 condor_code_reviewer-1.2/src/
+-rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-26 23:26:52.000000 condor_code_reviewer-1.2/src/__init__.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     1948 2024-03-27 00:51:27.000000 condor_code_reviewer-1.2/src/cli.py
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:49:49.163193 condor_code_reviewer-1.2/src/lib/
+-rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-19 00:32:11.000000 condor_code_reviewer-1.2/src/lib/__init__.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     2902 2024-03-19 12:49:30.000000 condor_code_reviewer-1.2/src/lib/github_pr.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     1688 2024-03-19 00:32:11.000000 condor_code_reviewer-1.2/src/lib/openai_assistant.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     2176 2024-04-18 03:48:59.000000 condor_code_reviewer-1.2/src/reviewer.py
```

### Comparing `condor_code_reviewer-1.0/src/cli.py` & `condor_code_reviewer-1.2/src/cli.py`

 * *Files identical despite different names*

### Comparing `condor_code_reviewer-1.0/src/lib/github_pr.py` & `condor_code_reviewer-1.2/src/lib/github_pr.py`

 * *Files identical despite different names*

### Comparing `condor_code_reviewer-1.0/src/lib/openai_assistant.py` & `condor_code_reviewer-1.2/src/lib/openai_assistant.py`

 * *Files identical despite different names*

### Comparing `condor_code_reviewer-1.0/src/reviewer.py` & `condor_code_reviewer-1.2/src/reviewer.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,28 +18,31 @@
     def __run_steps(self):
         for step in self.steps:
             step()
 
     def add_pr_description(self):
         message = f"Pull Request Description: {self.gh.pr.title}\n\n{self.gh.pr.body}"
         message += f"\n\nPR Author: @{self.gh.pr.user.login}"
+
         self.assistant.add_message(message, "user")
 
     def add_commit_messages(self):
         messages = "\n".join(self.gh.get_commit_messages())
         self.assistant.add_and_retrieve_message(messages, "user")
 
     def review_files(self):
         for filename in self.gh.get_modified_files():
             diff = self.gh.get_file_diff(filename)
             message = f"Reviewing file: {filename}.\nDiff:\n\n{diff}"
 
             response = self.assistant.add_and_retrieve_message(message, "user")
+            first_line = diff.split("\n")[0]
+
             if response and response != 'APIError: No response':
-                self.gh.comment_on_file(filename, response, 1)
+                self.gh.comment_on_file(filename, response, first_line)
 
     def summary_review(self):
         summary = self.assistant.add_and_retrieve_message("Summary Review", "user")
         self.gh.comment_on_pr(summary)
 
     def add_step(self, func, system_message=None):
         def wrapper(*args, **kwargs):
```

