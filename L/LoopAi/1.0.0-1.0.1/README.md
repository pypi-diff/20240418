# Comparing `tmp/loopai-1.0.0.tar.gz` & `tmp/LoopAi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loopai-1.0.0.tar", last modified: Thu Apr 18 19:13:37 2024, max compression
+gzip compressed data, was "LoopAi-1.0.1.tar", last modified: Thu Apr 18 19:56:59 2024, max compression
```

## Comparing `loopai-1.0.0.tar` & `LoopAi-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2024-04-18 19:13:37.661989 loopai-1.0.0/
-drwxrwx---   0 root         (0) everybody  (9997)        0 2024-04-18 19:13:37.429989 loopai-1.0.0/LoopAi/
--rw-rw----   0 root         (0) everybody  (9997)     1127 2024-04-18 19:09:58.000000 loopai-1.0.0/LoopAi/LoopAi.py
--rw-rw----   0 root         (0) everybody  (9997)       21 2024-04-18 19:09:58.000000 loopai-1.0.0/LoopAi/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2024-04-18 19:13:37.581989 loopai-1.0.0/LoopAi.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      596 2024-04-18 19:13:37.000000 loopai-1.0.0/LoopAi.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      193 2024-04-18 19:13:37.000000 loopai-1.0.0/LoopAi.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2024-04-18 19:13:37.000000 loopai-1.0.0/LoopAi.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)        9 2024-04-18 19:13:37.000000 loopai-1.0.0/LoopAi.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        7 2024-04-18 19:13:37.000000 loopai-1.0.0/LoopAi.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)      596 2024-04-18 19:13:37.589989 loopai-1.0.0/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)       38 2024-04-18 19:13:37.661989 loopai-1.0.0/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      794 2024-04-18 19:09:58.000000 loopai-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:56:59.828822 LoopAi-1.0.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:56:59.824823 LoopAi-1.0.1/LoopAi/
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-04-18 19:17:58.000000 LoopAi-1.0.1/LoopAi/LoopAi.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-18 19:53:35.000000 LoopAi-1.0.1/LoopAi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:56:59.828822 LoopAi-1.0.1/LoopAi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      636 2024-04-18 19:56:59.000000 LoopAi-1.0.1/LoopAi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      193 2024-04-18 19:56:59.000000 LoopAi-1.0.1/LoopAi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 19:56:59.000000 LoopAi-1.0.1/LoopAi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-18 19:56:59.000000 LoopAi-1.0.1/LoopAi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-18 19:56:59.000000 LoopAi-1.0.1/LoopAi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      636 2024-04-18 19:56:59.828822 LoopAi-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 19:56:59.828822 LoopAi-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      795 2024-04-18 19:55:58.000000 LoopAi-1.0.1/setup.py
```

### Comparing `loopai-1.0.0/LoopAi/LoopAi.py` & `LoopAi-1.0.1/LoopAi/LoopAi.py`

 * *Files identical despite different names*

### Comparing `loopai-1.0.0/setup.py` & `LoopAi-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'A python libary that gives you access to a set of Ai models including WormGpt , Gemini , blackbox and more'
 
 # Setting up
 setup(
     name="LoopAi",
     version=VERSION,
     author="DarkLoop (Organisation)",
@@ -18,8 +18,8 @@
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
-)
+)
```

