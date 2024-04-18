# Comparing `tmp/codedepot_depot-0.0.1.tar.gz` & `tmp/codedepot_depot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedepot_depot-0.0.1.tar", last modified: Thu Apr 18 09:35:11 2024, max compression
+gzip compressed data, was "codedepot_depot-0.0.2.tar", last modified: Thu Apr 18 11:30:56 2024, max compression
```

## Comparing `codedepot_depot-0.0.1.tar` & `codedepot_depot-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       54 2024-04-15 07:13:36.336177 codedepot_depot-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-04-15 13:02:27.184638 codedepot_depot-0.0.1/depot/__init__.py
--rw-r--r--   0        0        0     5825 2024-04-18 09:14:30.404632 codedepot_depot-0.0.1/depot/api.py
--rw-r--r--   0        0        0      624 2024-04-18 08:11:02.116570 codedepot_depot-0.0.1/depot/cluster_spec.py
--rw-r--r--   0        0        0     2829 2024-04-18 08:05:17.371127 codedepot_depot-0.0.1/depot/config.py
--rw-r--r--   0        0        0      507 2024-04-18 06:56:25.799963 codedepot_depot-0.0.1/depot/jobfile.py
--rw-r--r--   0        0        0     4323 2024-04-18 09:11:33.534727 codedepot_depot-0.0.1/depot/main.py
--rw-r--r--   0        0        0      616 2024-04-16 05:00:55.267184 codedepot_depot-0.0.1/depot/provider_spec.py
--rw-r--r--   0        0        0      720 2024-04-18 09:35:11.109670 codedepot_depot-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-15 20:33:04.196404 codedepot_depot-0.0.1/test/__init__.py
--rw-r--r--   0        0        0       86 2024-04-16 05:02:59.830823 codedepot_depot-0.0.1/test/resources/cluster_test.yaml
--rw-r--r--   0        0        0       87 2024-04-15 20:48:31.758568 codedepot_depot-0.0.1/test/resources/config.json
--rw-r--r--   0        0        0       80 2024-04-15 20:35:06.454038 codedepot_depot-0.0.1/test/resources/local_cred.json
--rw-r--r--   0        0        0       96 2024-04-16 04:58:41.947831 codedepot_depot-0.0.1/test/resources/provider_test.yaml
--rw-r--r--   0        0        0        0 2024-04-16 04:06:38.432329 codedepot_depot-0.0.1/test/test_client.py
--rw-r--r--   0        0        0      408 2024-04-16 05:35:56.755146 codedepot_depot-0.0.1/test/test_provider.py
--rw-r--r--   0        0        0      666 2024-04-16 05:28:37.442814 codedepot_depot-0.0.1/test/utils.py
--rw-r--r--   0        0        0      662 1970-01-01 00:00:00.000000 codedepot_depot-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       54 2024-04-15 07:13:36.336177 codedepot_depot-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 13:02:27.184638 codedepot_depot-0.0.2/depot/__init__.py
+-rw-r--r--   0        0        0     5825 2024-04-18 09:14:30.404632 codedepot_depot-0.0.2/depot/api.py
+-rw-r--r--   0        0        0      624 2024-04-18 08:11:02.116570 codedepot_depot-0.0.2/depot/cluster_spec.py
+-rw-r--r--   0        0        0     2847 2024-04-18 10:44:40.563189 codedepot_depot-0.0.2/depot/config.py
+-rw-r--r--   0        0        0      507 2024-04-18 06:56:25.799963 codedepot_depot-0.0.2/depot/jobfile.py
+-rw-r--r--   0        0        0     4323 2024-04-18 11:30:13.752393 codedepot_depot-0.0.2/depot/main.py
+-rw-r--r--   0        0        0      616 2024-04-16 05:00:55.267184 codedepot_depot-0.0.2/depot/provider_spec.py
+-rw-r--r--   0        0        0      737 2024-04-18 11:30:56.586275 codedepot_depot-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-15 20:33:04.196404 codedepot_depot-0.0.2/test/__init__.py
+-rw-r--r--   0        0        0       86 2024-04-16 05:02:59.830823 codedepot_depot-0.0.2/test/resources/cluster_test.yaml
+-rw-r--r--   0        0        0       87 2024-04-15 20:48:31.758568 codedepot_depot-0.0.2/test/resources/config.json
+-rw-r--r--   0        0        0       80 2024-04-15 20:35:06.454038 codedepot_depot-0.0.2/test/resources/local_cred.json
+-rw-r--r--   0        0        0       96 2024-04-16 04:58:41.947831 codedepot_depot-0.0.2/test/resources/provider_test.yaml
+-rw-r--r--   0        0        0        0 2024-04-16 04:06:38.432329 codedepot_depot-0.0.2/test/test_client.py
+-rw-r--r--   0        0        0      408 2024-04-16 05:35:56.755146 codedepot_depot-0.0.2/test/test_provider.py
+-rw-r--r--   0        0        0      666 2024-04-16 05:28:37.442814 codedepot_depot-0.0.2/test/utils.py
+-rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 codedepot_depot-0.0.2/PKG-INFO
```

### Comparing `codedepot_depot-0.0.1/depot/api.py` & `codedepot_depot-0.0.2/depot/api.py`

 * *Files identical despite different names*

### Comparing `codedepot_depot-0.0.1/depot/cluster_spec.py` & `codedepot_depot-0.0.2/depot/cluster_spec.py`

 * *Files identical despite different names*

### Comparing `codedepot_depot-0.0.1/depot/config.py` & `codedepot_depot-0.0.2/depot/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,17 +55,17 @@
             DepotConfig.DEFAULT_CONFIG_FILE)
 
         return cls.from_file(config_path)
 
     @staticmethod
     def create():
         endpoint = prompt(
-            'Enter your API endpoint [https//depot.codedepot.ai]: ')
+            'Enter your API endpoint [https://depot.staging.codedepot.ai]: ')
         if not endpoint:
-            endpoint = 'https//depot.codedepot.ai'
+            endpoint = 'https://depot.stating.codedepot.ai'
         username = prompt('Enter your login: ')
         # Check if the username is empty TODO: check if the username is valid
         if not username:
             print('Username is required')
             return None
 
         email = prompt('Enter your email: ')
```

### Comparing `codedepot_depot-0.0.1/depot/main.py` & `codedepot_depot-0.0.2/depot/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     # Parse the arguments
     return parser.parse_args()
 
 
 def main():
     args = parse_args()
     if args.version:
-        print("0.0.1")
+        print("0.0.2")
         return
 
     if args.command == 'login':
         DepotConfig.create()
         return
 
     config = DepotConfig.default()
```

### Comparing `codedepot_depot-0.0.1/depot/provider_spec.py` & `codedepot_depot-0.0.2/depot/provider_spec.py`

 * *Files identical despite different names*

### Comparing `codedepot_depot-0.0.1/pyproject.toml` & `codedepot_depot-0.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm]
 
 [project]
 name = "codedepot-depot"
-version = "0.0.1"
+version = "0.0.2"
 description = "Job launch support for Git AI"
 readme = "README.md"
 authors = [
     { name = "CodeDepot", email = "contact@codedepot.ai" },
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -19,14 +19,15 @@
     "prettytable",
     "prompt-toolkit",
     "py",
     "pyaml",
     "pydantic",
     "pygit2",
     "requests",
+    "depot_api",
 ]
 
 [project.urls]
 Homepage = "https://github.com/codedepotai/git-ai"
 
 [project.scripts]
 depot = "depot.main:main"
```

### Comparing `codedepot_depot-0.0.1/test/utils.py` & `codedepot_depot-0.0.2/test/utils.py`

 * *Files identical despite different names*

### Comparing `codedepot_depot-0.0.1/PKG-INFO` & `codedepot_depot-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedepot-depot
-Version: 0.0.1
+Version: 0.0.2
 Summary: Job launch support for Git AI
 Author-Email: CodeDepot <contact@codedepot.ai>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/codedepotai/git-ai
 Requires-Python: >=3.10
@@ -12,12 +12,13 @@
 Requires-Dist: prettytable
 Requires-Dist: prompt-toolkit
 Requires-Dist: py
 Requires-Dist: pyaml
 Requires-Dist: pydantic
 Requires-Dist: pygit2
 Requires-Dist: requests
+Requires-Dist: depot_api
 Description-Content-Type: text/markdown
 
 # Depot
 
 This is the depot client. More docs to come.
```

