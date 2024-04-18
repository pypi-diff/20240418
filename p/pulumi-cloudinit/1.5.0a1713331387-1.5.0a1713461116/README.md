# Comparing `tmp/pulumi_cloudinit-1.5.0a1713331387.tar.gz` & `tmp/pulumi_cloudinit-1.5.0a1713461116.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_cloudinit-1.5.0a1713331387.tar", last modified: Wed Apr 17 05:26:15 2024, max compression
+gzip compressed data, was "pulumi_cloudinit-1.5.0a1713461116.tar", last modified: Thu Apr 18 17:27:49 2024, max compression
```

## Comparing `pulumi_cloudinit-1.5.0a1713331387.tar` & `pulumi_cloudinit-1.5.0a1713461116.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:26:15.230519 pulumi_cloudinit-1.5.0a1713331387/
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-17 05:26:15.230519 pulumi_cloudinit-1.5.0a1713331387/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-17 05:26:09.000000 pulumi_cloudinit-1.5.0a1713331387/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:26:15.230519 pulumi_cloudinit-1.5.0a1713331387/pulumi_cloudinit/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-17 05:26:09.000000 pulumi_cloudinit-1.5.0a1713331387/pulumi_cloudinit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-04-17 05:26:09.000000 pulumi_cloudinit-1.5.0a1713331387/pulumi_cloudinit/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-17 05:26:09.000000 pulumi_cloudinit-1.5.0a1713331387/pulumi_cloudinit/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    16889 2024-04-17 05:26:09.000000 pulumi_cloudinit-1.5.0a1713331387/pulumi_cloudinit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-04-17 05:26:09.000000 pulumi_cloudinit-1.5.0a1713331387/pulumi_cloudinit/get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-04-17 05:26:09.000000 pulumi_cloudinit-1.5.0a1713331387/pulumi_cloudinit/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-17 05:26:09.000000 pulumi_cloudinit-1.5.0a1713331387/pulumi_cloudinit/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-17 05:26:09.000000 pulumi_cloudinit-1.5.0a1713331387/pulumi_cloudinit/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 05:26:09.000000 pulumi_cloudinit-1.5.0a1713331387/pulumi_cloudinit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:26:15.230519 pulumi_cloudinit-1.5.0a1713331387/pulumi_cloudinit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-17 05:26:15.000000 pulumi_cloudinit-1.5.0a1713331387/pulumi_cloudinit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-17 05:26:15.000000 pulumi_cloudinit-1.5.0a1713331387/pulumi_cloudinit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 05:26:15.000000 pulumi_cloudinit-1.5.0a1713331387/pulumi_cloudinit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 05:26:15.000000 pulumi_cloudinit-1.5.0a1713331387/pulumi_cloudinit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-17 05:26:15.000000 pulumi_cloudinit-1.5.0a1713331387/pulumi_cloudinit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-17 05:26:09.000000 pulumi_cloudinit-1.5.0a1713331387/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 05:26:15.230519 pulumi_cloudinit-1.5.0a1713331387/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:27:49.560893 pulumi_cloudinit-1.5.0a1713461116/
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-18 17:27:49.560893 pulumi_cloudinit-1.5.0a1713461116/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-18 17:27:42.000000 pulumi_cloudinit-1.5.0a1713461116/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:27:49.560893 pulumi_cloudinit-1.5.0a1713461116/pulumi_cloudinit/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-18 17:27:42.000000 pulumi_cloudinit-1.5.0a1713461116/pulumi_cloudinit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-04-18 17:27:42.000000 pulumi_cloudinit-1.5.0a1713461116/pulumi_cloudinit/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-18 17:27:42.000000 pulumi_cloudinit-1.5.0a1713461116/pulumi_cloudinit/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16889 2024-04-18 17:27:42.000000 pulumi_cloudinit-1.5.0a1713461116/pulumi_cloudinit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-04-18 17:27:42.000000 pulumi_cloudinit-1.5.0a1713461116/pulumi_cloudinit/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-04-18 17:27:42.000000 pulumi_cloudinit-1.5.0a1713461116/pulumi_cloudinit/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-18 17:27:42.000000 pulumi_cloudinit-1.5.0a1713461116/pulumi_cloudinit/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-18 17:27:42.000000 pulumi_cloudinit-1.5.0a1713461116/pulumi_cloudinit/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:27:42.000000 pulumi_cloudinit-1.5.0a1713461116/pulumi_cloudinit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:27:49.560893 pulumi_cloudinit-1.5.0a1713461116/pulumi_cloudinit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-18 17:27:49.000000 pulumi_cloudinit-1.5.0a1713461116/pulumi_cloudinit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-18 17:27:49.000000 pulumi_cloudinit-1.5.0a1713461116/pulumi_cloudinit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 17:27:49.000000 pulumi_cloudinit-1.5.0a1713461116/pulumi_cloudinit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-18 17:27:49.000000 pulumi_cloudinit-1.5.0a1713461116/pulumi_cloudinit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-18 17:27:49.000000 pulumi_cloudinit-1.5.0a1713461116/pulumi_cloudinit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-18 17:27:42.000000 pulumi_cloudinit-1.5.0a1713461116/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 17:27:49.560893 pulumi_cloudinit-1.5.0a1713461116/setup.cfg
```

### Comparing `pulumi_cloudinit-1.5.0a1713331387/PKG-INFO` & `pulumi_cloudinit-1.5.0a1713461116/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_cloudinit
-Version: 1.5.0a1713331387
+Version: 1.5.0a1713461116
 Summary: A Pulumi package for creating and managing cloudinit cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-cloudinit
 Keywords: pulumi,cloudinit
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_cloudinit-1.5.0a1713331387/README.md` & `pulumi_cloudinit-1.5.0a1713461116/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1713331387/pulumi_cloudinit/__init__.py` & `pulumi_cloudinit-1.5.0a1713461116/pulumi_cloudinit/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1713331387/pulumi_cloudinit/_inputs.py` & `pulumi_cloudinit-1.5.0a1713461116/pulumi_cloudinit/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1713331387/pulumi_cloudinit/_utilities.py` & `pulumi_cloudinit-1.5.0a1713461116/pulumi_cloudinit/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1713331387/pulumi_cloudinit/config.py` & `pulumi_cloudinit-1.5.0a1713461116/pulumi_cloudinit/config.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1713331387/pulumi_cloudinit/get_config.py` & `pulumi_cloudinit-1.5.0a1713461116/pulumi_cloudinit/get_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1713331387/pulumi_cloudinit/outputs.py` & `pulumi_cloudinit-1.5.0a1713461116/pulumi_cloudinit/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1713331387/pulumi_cloudinit/provider.py` & `pulumi_cloudinit-1.5.0a1713461116/pulumi_cloudinit/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1713331387/pulumi_cloudinit.egg-info/PKG-INFO` & `pulumi_cloudinit-1.5.0a1713461116/pulumi_cloudinit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_cloudinit
-Version: 1.5.0a1713331387
+Version: 1.5.0a1713461116
 Summary: A Pulumi package for creating and managing cloudinit cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-cloudinit
 Keywords: pulumi,cloudinit
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

