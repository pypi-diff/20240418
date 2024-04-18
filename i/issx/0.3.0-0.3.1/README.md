# Comparing `tmp/issx-0.3.0.tar.gz` & `tmp/issx-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "issx-0.3.0.tar", max compression
+gzip compressed data, was "issx-0.3.1.tar", max compression
```

## Comparing `issx-0.3.0.tar` & `issx-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1101 2024-04-17 19:21:35.947322 issx-0.3.0/LICENCE
--rw-r--r--   0        0        0     4935 2024-04-17 19:21:35.955323 issx-0.3.0/README.md
--rw-r--r--   0        0        0     3190 2024-04-17 19:21:35.955323 issx-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-17 19:21:35.955323 issx-0.3.0/src/issx/__init__.py
--rw-r--r--   0        0        0     4462 2024-04-17 19:21:35.955323 issx-0.3.0/src/issx/cli.py
--rw-r--r--   0        0        0      200 2024-04-17 19:21:35.955323 issx-0.3.0/src/issx/clients/__init__.py
--rw-r--r--   0        0        0      317 2024-04-17 19:21:35.955323 issx-0.3.0/src/issx/clients/exceptions.py
--rw-r--r--   0        0        0     3604 2024-04-17 19:21:35.955323 issx-0.3.0/src/issx/clients/gitlab.py
--rw-r--r--   0        0        0     2082 2024-04-17 19:21:35.955323 issx-0.3.0/src/issx/clients/interfaces.py
--rw-r--r--   0        0        0     3453 2024-04-17 19:21:35.955323 issx-0.3.0/src/issx/clients/redmine.py
--rw-r--r--   0        0        0        0 2024-04-17 19:21:35.955323 issx-0.3.0/src/issx/domain/__init__.py
--rw-r--r--   0        0        0      205 2024-04-17 19:21:35.955323 issx-0.3.0/src/issx/domain/issues.py
--rw-r--r--   0        0        0     2441 2024-04-17 19:21:35.955323 issx-0.3.0/src/issx/instance_managers.py
--rw-r--r--   0        0        0        0 2024-04-17 19:21:35.955323 issx-0.3.0/src/issx/py.typed
--rw-r--r--   0        0        0     2356 2024-04-17 19:21:35.955323 issx-0.3.0/src/issx/services.py
--rw-r--r--   0        0        0     5995 1970-01-01 00:00:00.000000 issx-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1101 2024-04-17 19:33:27.429475 issx-0.3.1/LICENCE
+-rw-r--r--   0        0        0     5032 2024-04-17 19:33:27.429475 issx-0.3.1/README.md
+-rw-r--r--   0        0        0     3190 2024-04-17 19:33:27.433475 issx-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-17 19:33:27.433475 issx-0.3.1/src/issx/__init__.py
+-rw-r--r--   0        0        0     4600 2024-04-17 19:33:27.433475 issx-0.3.1/src/issx/cli.py
+-rw-r--r--   0        0        0      200 2024-04-17 19:33:27.433475 issx-0.3.1/src/issx/clients/__init__.py
+-rw-r--r--   0        0        0      317 2024-04-17 19:33:27.433475 issx-0.3.1/src/issx/clients/exceptions.py
+-rw-r--r--   0        0        0     3604 2024-04-17 19:33:27.433475 issx-0.3.1/src/issx/clients/gitlab.py
+-rw-r--r--   0        0        0     2082 2024-04-17 19:33:27.433475 issx-0.3.1/src/issx/clients/interfaces.py
+-rw-r--r--   0        0        0     3453 2024-04-17 19:33:27.433475 issx-0.3.1/src/issx/clients/redmine.py
+-rw-r--r--   0        0        0        0 2024-04-17 19:33:27.433475 issx-0.3.1/src/issx/domain/__init__.py
+-rw-r--r--   0        0        0      205 2024-04-17 19:33:27.433475 issx-0.3.1/src/issx/domain/issues.py
+-rw-r--r--   0        0        0     2441 2024-04-17 19:33:27.433475 issx-0.3.1/src/issx/instance_managers.py
+-rw-r--r--   0        0        0        0 2024-04-17 19:33:27.433475 issx-0.3.1/src/issx/py.typed
+-rw-r--r--   0        0        0     2356 2024-04-17 19:33:27.433475 issx-0.3.1/src/issx/services.py
+-rw-r--r--   0        0        0     6092 1970-01-01 00:00:00.000000 issx-0.3.1/PKG-INFO
```

### Comparing `issx-0.3.0/LICENCE` & `issx-0.3.1/LICENCE`

 * *Files identical despite different names*

### Comparing `issx-0.3.0/README.md` & `issx-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,16 @@
 ```
 
 where `source` and `target` are the names of the projects configured in the configuration file.
 
 Optionally you can customize the issue title and description by providing `--title-format/-T` and `--description-format/-D` flags.
 The format should be a string with placeholders for the issue fields (e.g. `{title}`, `{description}`, `{id}` etc.).
 
+Assigning the issue to the current user is also possible by providing `--assign-to-me/-M` flag.
+
 ### Configuration file
 
 The configuration file can be either in the working directory (`issx.toml`) or in `~/.config/issx.toml`.
 
 It should have the following structure:
 
 ```toml
```

### Comparing `issx-0.3.0/pyproject.toml` & `issx-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "issx"
-version = "0.3.0"
+version = "0.3.1"
 description = "Tool for synchronizing issues between different services"
 authors = [
     "nekeal <szymon.sc.cader@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `issx-0.3.0/src/issx/cli.py` & `issx-0.3.1/src/issx/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,15 +67,22 @@
             "--allow-duplicates",
             "-A",
             help="Allow for duplicate issues. If set, the command will return the first"
             " issue found with the same title. If no issues are found,"
             " a new issue will be created.",
         ),
     ] = False,
-    assign_to_me: Annotated[bool, typer.Option("--assign-to-me", "-M")] = False,
+    assign_to_me: Annotated[
+        bool,
+        typer.Option(
+            "--assign-to-me",
+            "-M",
+            help="Whether to assign a newly created issue to the current user",
+        ),
+    ] = False,
 ) -> int:
     console.print(
         Text.assemble(
             f"Copying issue {issue_id} from project ",
             (source_project_name, "bold magenta"),
             " to project ",
             (target_project_name, "bold magenta"),
```

### Comparing `issx-0.3.0/src/issx/clients/gitlab.py` & `issx-0.3.1/src/issx/clients/gitlab.py`

 * *Files identical despite different names*

### Comparing `issx-0.3.0/src/issx/clients/interfaces.py` & `issx-0.3.1/src/issx/clients/interfaces.py`

 * *Files identical despite different names*

### Comparing `issx-0.3.0/src/issx/clients/redmine.py` & `issx-0.3.1/src/issx/clients/redmine.py`

 * *Files identical despite different names*

### Comparing `issx-0.3.0/src/issx/instance_managers.py` & `issx-0.3.1/src/issx/instance_managers.py`

 * *Files identical despite different names*

### Comparing `issx-0.3.0/src/issx/services.py` & `issx-0.3.1/src/issx/services.py`

 * *Files identical despite different names*

### Comparing `issx-0.3.0/PKG-INFO` & `issx-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issx
-Version: 0.3.0
+Version: 0.3.1
 Summary: Tool for synchronizing issues between different services
 Home-page: https://nekeal.github.io/issx
 License: MIT
 Author: nekeal
 Author-email: szymon.sc.cader@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -76,14 +76,16 @@
 ```
 
 where `source` and `target` are the names of the projects configured in the configuration file.
 
 Optionally you can customize the issue title and description by providing `--title-format/-T` and `--description-format/-D` flags.
 The format should be a string with placeholders for the issue fields (e.g. `{title}`, `{description}`, `{id}` etc.).
 
+Assigning the issue to the current user is also possible by providing `--assign-to-me/-M` flag.
+
 ### Configuration file
 
 The configuration file can be either in the working directory (`issx.toml`) or in `~/.config/issx.toml`.
 
 It should have the following structure:
 
 ```toml
```

