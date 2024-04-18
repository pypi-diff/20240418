# Comparing `tmp/rag_tool_package-0.1.1.tar.gz` & `tmp/rag_tool_package-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rag_tool_package-0.1.1.tar", last modified: Tue Apr 16 17:39:50 2024, max compression
+gzip compressed data, was "rag_tool_package-0.2.0.tar", last modified: Thu Apr 18 16:37:12 2024, max compression
```

## Comparing `rag_tool_package-0.1.1.tar` & `rag_tool_package-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 17:39:50.605835 rag_tool_package-0.1.1/
--rw-rw-rw-   0        0        0       37 2024-04-16 07:32:01.000000 rag_tool_package-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      116 2024-04-16 17:39:50.604833 rag_tool_package-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 17:39:50.547248 rag_tool_package-0.1.1/rag_tool_package/
--rw-rw-rw-   0        0        0       82 2024-04-16 07:41:11.000000 rag_tool_package-0.1.1/rag_tool_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 17:39:50.587207 rag_tool_package-0.1.1/rag_tool_package/tools/
--rw-rw-rw-   0        0        0       82 2024-04-16 07:41:11.000000 rag_tool_package-0.1.1/rag_tool_package/tools/__init__.py
--rw-rw-rw-   0        0        0     1435 2024-04-16 14:48:48.000000 rag_tool_package-0.1.1/rag_tool_package/tools/rag_tool.py
--rw-rw-rw-   0        0        0      553 2024-04-16 07:41:11.000000 rag_tool_package-0.1.1/rag_tool_package/tools/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-16 17:39:50.590046 rag_tool_package-0.1.1/rag_tool_package/yamls/
--rw-rw-rw-   0        0        0      364 2024-04-16 14:45:07.000000 rag_tool_package-0.1.1/rag_tool_package/yamls/rag_tool.yaml
-drwxrwxrwx   0        0        0        0 2024-04-16 17:39:50.603844 rag_tool_package-0.1.1/rag_tool_package.egg-info/
--rw-rw-rw-   0        0        0      116 2024-04-16 17:39:50.000000 rag_tool_package-0.1.1/rag_tool_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2024-04-16 17:39:50.000000 rag_tool_package-0.1.1/rag_tool_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 17:39:50.000000 rag_tool_package-0.1.1/rag_tool_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2024-04-16 17:39:50.000000 rag_tool_package-0.1.1/rag_tool_package.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       23 2024-04-16 17:39:50.000000 rag_tool_package-0.1.1/rag_tool_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 17:39:50.606962 rag_tool_package-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      448 2024-04-16 17:39:21.000000 rag_tool_package-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 17:39:50.602834 rag_tool_package-0.1.1/tests/
--rw-rw-rw-   0        0        0        0 2024-04-16 07:32:01.000000 rag_tool_package-0.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0      710 2024-04-16 07:32:01.000000 rag_tool_package-0.1.1/tests/test_rag_tool.py
+drwxrwxrwx   0        0        0        0 2024-04-18 16:37:12.616955 rag_tool_package-0.2.0/
+-rw-rw-rw-   0        0        0       37 2024-04-16 07:32:01.000000 rag_tool_package-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      152 2024-04-18 16:37:12.615665 rag_tool_package-0.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-18 16:37:12.568767 rag_tool_package-0.2.0/rag_tool_package/
+-rw-rw-rw-   0        0        0       82 2024-04-16 07:41:11.000000 rag_tool_package-0.2.0/rag_tool_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 16:37:12.591930 rag_tool_package-0.2.0/rag_tool_package/tools/
+-rw-rw-rw-   0        0        0       82 2024-04-16 07:41:11.000000 rag_tool_package-0.2.0/rag_tool_package/tools/__init__.py
+-rw-rw-rw-   0        0        0     2476 2024-04-18 16:33:58.000000 rag_tool_package-0.2.0/rag_tool_package/tools/rag_tool.py
+-rw-rw-rw-   0        0        0      553 2024-04-16 07:41:11.000000 rag_tool_package-0.2.0/rag_tool_package/tools/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-18 16:37:12.602021 rag_tool_package-0.2.0/rag_tool_package/yamls/
+-rw-rw-rw-   0        0        0      935 2024-04-18 16:34:21.000000 rag_tool_package-0.2.0/rag_tool_package/yamls/rag_tool.yaml
+drwxrwxrwx   0        0        0        0 2024-04-18 16:37:12.614230 rag_tool_package-0.2.0/rag_tool_package.egg-info/
+-rw-rw-rw-   0        0        0      152 2024-04-18 16:37:12.000000 rag_tool_package-0.2.0/rag_tool_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2024-04-18 16:37:12.000000 rag_tool_package-0.2.0/rag_tool_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 16:37:12.000000 rag_tool_package-0.2.0/rag_tool_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2024-04-18 16:37:12.000000 rag_tool_package-0.2.0/rag_tool_package.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       23 2024-04-18 16:37:12.000000 rag_tool_package-0.2.0/rag_tool_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 16:37:12.616955 rag_tool_package-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      484 2024-04-18 16:36:41.000000 rag_tool_package-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 16:37:12.612077 rag_tool_package-0.2.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-16 07:32:01.000000 rag_tool_package-0.2.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      710 2024-04-16 07:32:01.000000 rag_tool_package-0.2.0/tests/test_rag_tool.py
```

### Comparing `rag_tool_package-0.1.1/rag_tool_package/tools/utils.py` & `rag_tool_package-0.2.0/rag_tool_package/tools/utils.py`

 * *Files identical despite different names*

### Comparing `rag_tool_package-0.1.1/tests/test_rag_tool.py` & `rag_tool_package-0.2.0/tests/test_rag_tool.py`

 * *Files identical despite different names*

