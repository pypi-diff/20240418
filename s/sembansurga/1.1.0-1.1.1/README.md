# Comparing `tmp/sembansurga-1.1.0.tar.gz` & `tmp/sembansurga-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sembansurga-1.1.0.tar", last modified: Mon Apr 15 07:13:44 2024, max compression
+gzip compressed data, was "sembansurga-1.1.1.tar", last modified: Wed Apr 17 10:38:30 2024, max compression
```

## Comparing `sembansurga-1.1.0.tar` & `sembansurga-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 07:13:44.605888 sembansurga-1.1.0/
--rw-r--r--   0 root         (0) root         (0)      405 2024-04-15 07:13:44.605888 sembansurga-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        6 2023-12-24 05:56:18.000000 sembansurga-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 07:13:44.605888 sembansurga-1.1.0/sembansurga/
--rw-r--r--   0 root         (0) root         (0)      168 2024-04-15 06:29:20.000000 sembansurga-1.1.0/sembansurga/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3498 2024-04-15 07:13:01.000000 sembansurga-1.1.0/sembansurga/sembansurga.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 07:13:44.605888 sembansurga-1.1.0/sembansurga.egg-info/
--rw-r--r--   0 root         (0) root         (0)      405 2024-04-15 07:13:44.000000 sembansurga-1.1.0/sembansurga.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      243 2024-04-15 07:13:44.000000 sembansurga-1.1.0/sembansurga.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 07:13:44.000000 sembansurga-1.1.0/sembansurga.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-15 07:13:44.000000 sembansurga-1.1.0/sembansurga.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-15 07:13:44.000000 sembansurga-1.1.0/sembansurga.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 07:13:44.605888 sembansurga-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      757 2024-04-15 07:13:16.000000 sembansurga-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 10:38:30.902079 sembansurga-1.1.1/
+-rw-r--r--   0 root         (0) root         (0)      405 2024-04-17 10:38:30.902079 sembansurga-1.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        6 2023-12-24 05:56:18.000000 sembansurga-1.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 10:38:30.902079 sembansurga-1.1.1/sembansurga/
+-rw-r--r--   0 root         (0) root         (0)      199 2024-04-17 10:29:56.000000 sembansurga-1.1.1/sembansurga/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4066 2024-04-17 10:37:27.000000 sembansurga-1.1.1/sembansurga/sembansurga.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 10:38:30.902079 sembansurga-1.1.1/sembansurga.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      405 2024-04-17 10:38:30.000000 sembansurga-1.1.1/sembansurga.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      243 2024-04-17 10:38:30.000000 sembansurga-1.1.1/sembansurga.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 10:38:30.000000 sembansurga-1.1.1/sembansurga.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-17 10:38:30.000000 sembansurga-1.1.1/sembansurga.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-17 10:38:30.000000 sembansurga-1.1.1/sembansurga.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 10:38:30.902079 sembansurga-1.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      757 2024-04-17 10:37:53.000000 sembansurga-1.1.1/setup.py
```

### Comparing `sembansurga-1.1.0/sembansurga/sembansurga.py` & `sembansurga-1.1.1/sembansurga/sembansurga.py`

 * *Files 8% similar despite different names*

```diff
@@ -113,7 +113,29 @@
     options = Options(messages=messages)
 
     # Interact with the service
     response = service.chat(options)
 
     # Print the assistant's response
     print(response.content)
+
+def re(message):
+
+    # Initialize the service
+    service = UseLLM(service_url="https://usellm.org/api/llm")
+
+    # Prepare the conversation
+    messages = [
+        Message(role="system", content="You are a helpful assistant. Your name is Semban surga, when people ask hello then gree then with Namaskaram"),
+        Message(role="user", content=message),
+    ]
+    options = Options(messages=messages)
+
+    # Interact with the service
+    response = service.chat(options)
+
+    # Print the assistant's response
+    print(response.content)
+
+
+
+
```

### Comparing `sembansurga-1.1.0/setup.py` & `sembansurga-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='sembansurga',
-    version='1.1.0',
+    version='1.1.1',
     author='sidharth',
     author_email='sidharthss2690@gmail.com',
     description='Simply superb',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

