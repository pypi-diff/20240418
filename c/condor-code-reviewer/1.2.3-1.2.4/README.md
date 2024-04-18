# Comparing `tmp/condor_code_reviewer-1.2.3.tar.gz` & `tmp/condor_code_reviewer-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "condor_code_reviewer-1.2.3.tar", last modified: Thu Apr 18 04:06:11 2024, max compression
+gzip compressed data, was "condor_code_reviewer-1.2.4.tar", last modified: Thu Apr 18 04:08:31 2024, max compression
```

## Comparing `condor_code_reviewer-1.2.3.tar` & `condor_code_reviewer-1.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:06:11.428070 condor_code_reviewer-1.2.3/
--rw-r--r--   0 cparedesr   (501) staff       (20)      110 2024-04-18 04:06:11.427871 condor_code_reviewer-1.2.3/PKG-INFO
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:06:11.427684 condor_code_reviewer-1.2.3/condor_code_reviewer.egg-info/
--rw-r--r--   0 cparedesr   (501) staff       (20)      110 2024-04-18 04:06:11.000000 condor_code_reviewer-1.2.3/condor_code_reviewer.egg-info/PKG-INFO
--rw-r--r--   0 cparedesr   (501) staff       (20)      386 2024-04-18 04:06:11.000000 condor_code_reviewer-1.2.3/condor_code_reviewer.egg-info/SOURCES.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)        1 2024-04-18 04:06:11.000000 condor_code_reviewer-1.2.3/condor_code_reviewer.egg-info/dependency_links.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)       40 2024-04-18 04:06:11.000000 condor_code_reviewer-1.2.3/condor_code_reviewer.egg-info/entry_points.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)       16 2024-04-18 04:06:11.000000 condor_code_reviewer-1.2.3/condor_code_reviewer.egg-info/requires.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)        4 2024-04-18 04:06:11.000000 condor_code_reviewer-1.2.3/condor_code_reviewer.egg-info/top_level.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)       38 2024-04-18 04:06:11.428110 condor_code_reviewer-1.2.3/setup.cfg
--rw-r--r--   0 cparedesr   (501) staff       (20)      307 2024-04-18 04:06:07.000000 condor_code_reviewer-1.2.3/setup.py
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:06:11.426750 condor_code_reviewer-1.2.3/src/
--rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-26 23:26:52.000000 condor_code_reviewer-1.2.3/src/__init__.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     1948 2024-03-27 00:51:27.000000 condor_code_reviewer-1.2.3/src/cli.py
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:06:11.427383 condor_code_reviewer-1.2.3/src/lib/
--rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-19 00:32:11.000000 condor_code_reviewer-1.2.3/src/lib/__init__.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     2876 2024-04-18 03:57:06.000000 condor_code_reviewer-1.2.3/src/lib/github_pr.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     1688 2024-03-19 00:32:11.000000 condor_code_reviewer-1.2.3/src/lib/openai_assistant.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     2119 2024-04-18 04:05:31.000000 condor_code_reviewer-1.2.3/src/reviewer.py
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:08:31.738992 condor_code_reviewer-1.2.4/
+-rw-r--r--   0 cparedesr   (501) staff       (20)      110 2024-04-18 04:08:31.738758 condor_code_reviewer-1.2.4/PKG-INFO
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:08:31.738529 condor_code_reviewer-1.2.4/condor_code_reviewer.egg-info/
+-rw-r--r--   0 cparedesr   (501) staff       (20)      110 2024-04-18 04:08:31.000000 condor_code_reviewer-1.2.4/condor_code_reviewer.egg-info/PKG-INFO
+-rw-r--r--   0 cparedesr   (501) staff       (20)      386 2024-04-18 04:08:31.000000 condor_code_reviewer-1.2.4/condor_code_reviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)        1 2024-04-18 04:08:31.000000 condor_code_reviewer-1.2.4/condor_code_reviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)       40 2024-04-18 04:08:31.000000 condor_code_reviewer-1.2.4/condor_code_reviewer.egg-info/entry_points.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)       16 2024-04-18 04:08:31.000000 condor_code_reviewer-1.2.4/condor_code_reviewer.egg-info/requires.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)        4 2024-04-18 04:08:31.000000 condor_code_reviewer-1.2.4/condor_code_reviewer.egg-info/top_level.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)       38 2024-04-18 04:08:31.739034 condor_code_reviewer-1.2.4/setup.cfg
+-rw-r--r--   0 cparedesr   (501) staff       (20)      307 2024-04-18 04:08:28.000000 condor_code_reviewer-1.2.4/setup.py
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:08:31.737593 condor_code_reviewer-1.2.4/src/
+-rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-26 23:26:52.000000 condor_code_reviewer-1.2.4/src/__init__.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     1948 2024-03-27 00:51:27.000000 condor_code_reviewer-1.2.4/src/cli.py
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:08:31.738165 condor_code_reviewer-1.2.4/src/lib/
+-rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-19 00:32:11.000000 condor_code_reviewer-1.2.4/src/lib/__init__.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     2876 2024-04-18 03:57:06.000000 condor_code_reviewer-1.2.4/src/lib/github_pr.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     1688 2024-03-19 00:32:11.000000 condor_code_reviewer-1.2.4/src/lib/openai_assistant.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     2119 2024-04-18 04:08:13.000000 condor_code_reviewer-1.2.4/src/reviewer.py
```

### Comparing `condor_code_reviewer-1.2.3/src/cli.py` & `condor_code_reviewer-1.2.4/src/cli.py`

 * *Files identical despite different names*

### Comparing `condor_code_reviewer-1.2.3/src/lib/github_pr.py` & `condor_code_reviewer-1.2.4/src/lib/github_pr.py`

 * *Files identical despite different names*

### Comparing `condor_code_reviewer-1.2.3/src/lib/openai_assistant.py` & `condor_code_reviewer-1.2.4/src/lib/openai_assistant.py`

 * *Files identical despite different names*

### Comparing `condor_code_reviewer-1.2.3/src/reviewer.py` & `condor_code_reviewer-1.2.4/src/reviewer.py`

 * *Files identical despite different names*

