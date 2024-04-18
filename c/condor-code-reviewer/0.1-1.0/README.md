# Comparing `tmp/condor_code_reviewer-0.1.tar.gz` & `tmp/condor_code_reviewer-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "condor_code_reviewer-0.1.tar", last modified: Wed Mar 27 01:20:09 2024, max compression
+gzip compressed data, was "condor_code_reviewer-1.0.tar", last modified: Thu Apr 18 03:41:40 2024, max compression
```

## Comparing `condor_code_reviewer-0.1.tar` & `condor_code_reviewer-1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-03-27 01:20:09.636166 condor_code_reviewer-0.1/
--rw-r--r--   0 cparedesr   (501) staff       (20)      108 2024-03-27 01:20:09.635901 condor_code_reviewer-0.1/PKG-INFO
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-03-27 01:20:09.635584 condor_code_reviewer-0.1/condor_code_reviewer.egg-info/
--rw-r--r--   0 cparedesr   (501) staff       (20)      108 2024-03-27 01:20:09.000000 condor_code_reviewer-0.1/condor_code_reviewer.egg-info/PKG-INFO
--rw-r--r--   0 cparedesr   (501) staff       (20)      386 2024-03-27 01:20:09.000000 condor_code_reviewer-0.1/condor_code_reviewer.egg-info/SOURCES.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)        1 2024-03-27 01:20:09.000000 condor_code_reviewer-0.1/condor_code_reviewer.egg-info/dependency_links.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)       40 2024-03-27 01:20:09.000000 condor_code_reviewer-0.1/condor_code_reviewer.egg-info/entry_points.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)       16 2024-03-27 01:20:09.000000 condor_code_reviewer-0.1/condor_code_reviewer.egg-info/requires.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)        4 2024-03-27 01:20:09.000000 condor_code_reviewer-0.1/condor_code_reviewer.egg-info/top_level.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)       38 2024-03-27 01:20:09.636207 condor_code_reviewer-0.1/setup.cfg
--rw-r--r--   0 cparedesr   (501) staff       (20)      305 2024-03-27 01:19:23.000000 condor_code_reviewer-0.1/setup.py
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-03-27 01:20:09.635035 condor_code_reviewer-0.1/src/
--rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-26 23:26:52.000000 condor_code_reviewer-0.1/src/__init__.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     1948 2024-03-27 00:51:27.000000 condor_code_reviewer-0.1/src/cli.py
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-03-27 01:20:09.635381 condor_code_reviewer-0.1/src/lib/
--rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-19 00:32:11.000000 condor_code_reviewer-0.1/src/lib/__init__.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     2902 2024-03-19 12:49:30.000000 condor_code_reviewer-0.1/src/lib/github_pr.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     1688 2024-03-19 00:32:11.000000 condor_code_reviewer-0.1/src/lib/openai_assistant.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     2058 2024-03-26 23:27:28.000000 condor_code_reviewer-0.1/src/reviewer.py
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:41:40.818978 condor_code_reviewer-1.0/
+-rw-r--r--   0 cparedesr   (501) staff       (20)      108 2024-04-18 03:41:40.818736 condor_code_reviewer-1.0/PKG-INFO
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:41:40.818494 condor_code_reviewer-1.0/condor_code_reviewer.egg-info/
+-rw-r--r--   0 cparedesr   (501) staff       (20)      108 2024-04-18 03:41:40.000000 condor_code_reviewer-1.0/condor_code_reviewer.egg-info/PKG-INFO
+-rw-r--r--   0 cparedesr   (501) staff       (20)      386 2024-04-18 03:41:40.000000 condor_code_reviewer-1.0/condor_code_reviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)        1 2024-04-18 03:41:40.000000 condor_code_reviewer-1.0/condor_code_reviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)       40 2024-04-18 03:41:40.000000 condor_code_reviewer-1.0/condor_code_reviewer.egg-info/entry_points.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)       16 2024-04-18 03:41:40.000000 condor_code_reviewer-1.0/condor_code_reviewer.egg-info/requires.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)        4 2024-04-18 03:41:40.000000 condor_code_reviewer-1.0/condor_code_reviewer.egg-info/top_level.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)       38 2024-04-18 03:41:40.819025 condor_code_reviewer-1.0/setup.cfg
+-rw-r--r--   0 cparedesr   (501) staff       (20)      305 2024-04-18 03:41:12.000000 condor_code_reviewer-1.0/setup.py
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:41:40.817440 condor_code_reviewer-1.0/src/
+-rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-26 23:26:52.000000 condor_code_reviewer-1.0/src/__init__.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     1948 2024-03-27 00:51:27.000000 condor_code_reviewer-1.0/src/cli.py
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 03:41:40.818133 condor_code_reviewer-1.0/src/lib/
+-rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-19 00:32:11.000000 condor_code_reviewer-1.0/src/lib/__init__.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     2902 2024-03-19 12:49:30.000000 condor_code_reviewer-1.0/src/lib/github_pr.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     1688 2024-03-19 00:32:11.000000 condor_code_reviewer-1.0/src/lib/openai_assistant.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     2120 2024-04-18 03:38:52.000000 condor_code_reviewer-1.0/src/reviewer.py
```

### Comparing `condor_code_reviewer-0.1/src/cli.py` & `condor_code_reviewer-1.0/src/cli.py`

 * *Files identical despite different names*

### Comparing `condor_code_reviewer-0.1/src/lib/github_pr.py` & `condor_code_reviewer-1.0/src/lib/github_pr.py`

 * *Files identical despite different names*

### Comparing `condor_code_reviewer-0.1/src/lib/openai_assistant.py` & `condor_code_reviewer-1.0/src/lib/openai_assistant.py`

 * *Files identical despite different names*

### Comparing `condor_code_reviewer-0.1/src/reviewer.py` & `condor_code_reviewer-1.0/src/reviewer.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
     def __run_steps(self):
         for step in self.steps:
             step()
 
     def add_pr_description(self):
         message = f"Pull Request Description: {self.gh.pr.title}\n\n{self.gh.pr.body}"
+        message += f"\n\nPR Author: @{self.gh.pr.user.login}"
         self.assistant.add_message(message, "user")
 
     def add_commit_messages(self):
         messages = "\n".join(self.gh.get_commit_messages())
         self.assistant.add_and_retrieve_message(messages, "user")
 
     def review_files(self):
```

