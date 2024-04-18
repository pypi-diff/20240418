# Comparing `tmp/odoo_filter_addons-1.3.1.tar.gz` & `tmp/odoo_filter_addons-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo_filter_addons-1.3.1.tar", last modified: Wed Jan 31 12:30:24 2024, max compression
+gzip compressed data, was "odoo_filter_addons-1.3.2.tar", last modified: Thu Apr 18 08:57:33 2024, max compression
```

## Comparing `odoo_filter_addons-1.3.1.tar` & `odoo_filter_addons-1.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 12:30:23.996701 odoo_filter_addons-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-01-31 12:30:23.996701 odoo_filter_addons-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-01-31 12:30:04.000000 odoo_filter_addons-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 12:30:23.996701 odoo_filter_addons-1.3.1/odoo_filter_addons/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-31 12:30:04.000000 odoo_filter_addons-1.3.1/odoo_filter_addons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9124 2024-01-31 12:30:04.000000 odoo_filter_addons-1.3.1/odoo_filter_addons/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-31 12:30:04.000000 odoo_filter_addons-1.3.1/odoo_filter_addons/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 12:30:23.996701 odoo_filter_addons-1.3.1/odoo_filter_addons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-01-31 12:30:23.000000 odoo_filter_addons-1.3.1/odoo_filter_addons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-01-31 12:30:23.000000 odoo_filter_addons-1.3.1/odoo_filter_addons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 12:30:23.000000 odoo_filter_addons-1.3.1/odoo_filter_addons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-31 12:30:23.000000 odoo_filter_addons-1.3.1/odoo_filter_addons.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-01-31 12:30:23.000000 odoo_filter_addons-1.3.1/odoo_filter_addons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-31 12:30:23.000000 odoo_filter_addons-1.3.1/odoo_filter_addons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-01-31 12:30:04.000000 odoo_filter_addons-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-31 12:30:23.996701 odoo_filter_addons-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-01-31 12:30:04.000000 odoo_filter_addons-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:57:33.899129 odoo_filter_addons-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-18 08:57:33.899129 odoo_filter_addons-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-18 08:57:29.000000 odoo_filter_addons-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:57:33.899129 odoo_filter_addons-1.3.2/odoo_filter_addons/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-18 08:57:29.000000 odoo_filter_addons-1.3.2/odoo_filter_addons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-04-18 08:57:29.000000 odoo_filter_addons-1.3.2/odoo_filter_addons/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 08:57:29.000000 odoo_filter_addons-1.3.2/odoo_filter_addons/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:57:33.899129 odoo_filter_addons-1.3.2/odoo_filter_addons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-18 08:57:33.000000 odoo_filter_addons-1.3.2/odoo_filter_addons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-18 08:57:33.000000 odoo_filter_addons-1.3.2/odoo_filter_addons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 08:57:33.000000 odoo_filter_addons-1.3.2/odoo_filter_addons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-18 08:57:33.000000 odoo_filter_addons-1.3.2/odoo_filter_addons.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 08:57:33.000000 odoo_filter_addons-1.3.2/odoo_filter_addons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-18 08:57:33.000000 odoo_filter_addons-1.3.2/odoo_filter_addons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-18 08:57:29.000000 odoo_filter_addons-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 08:57:33.899129 odoo_filter_addons-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 08:57:29.000000 odoo_filter_addons-1.3.2/setup.py
```

### Comparing `odoo_filter_addons-1.3.1/PKG-INFO` & `odoo_filter_addons-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo_filter_addons
-Version: 1.3.1
+Version: 1.3.2
 Summary: Simple utlity to filter odoo addons into a single directory
 Author-email: Pablo Esteban <pablo.esteban@forgeflow.com>
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: Operating System :: POSIX
 Classifier: Framework :: Odoo
 Classifier: Programming Language :: Python :: 3
```

### Comparing `odoo_filter_addons-1.3.1/README.md` & `odoo_filter_addons-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `odoo_filter_addons-1.3.1/odoo_filter_addons/main.py` & `odoo_filter_addons-1.3.2/odoo_filter_addons/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,20 +94,20 @@
             print(f"Added module {fname}")
     # Create a message that will allow tracing the commit
     lines = [rname]
     for merge in repo["merges"]:
         merge = merge.strip()
         remote, ref = merge.split()
         if ref.startswith("refs/"):
-            commit = git("-C", rpath, "ls-remote", "--exit-code", remote, ref).split()[0]
+            commit = git("-C", rpath, "ls-remote", "--exit-code", remote, ref).strip().split()[0]
             lines.append(f"{merge} {commit}")
         elif len(ref) == 40:
             lines.append(merge)
         else:
-            commit = git("-C", rpath, "rev-parse", merge.replace(" ", "/"))
+            commit = git("-C", rpath, "rev-parse", merge.replace(" ", "/")).strip()
             lines.append(f"{merge} {commit}")
     message = "\n".join(lines)
     print(f"Partial message:\n{message}")
     return message
 
 def filter_repos(output_path, agg_path, repos, addons, release, push, gitlab_ci):
     os.chdir(output_path)
@@ -173,14 +173,15 @@
     os.chdir(agg_path)
     dump_yml("repos.yml", repos)
 
     new_argv = ["gitaggregate", "-c", "repos.yml"]
     with set_argv(new_argv):
         gitaggregate()
     print(f"gitaggregate output written to '{agg_path}'")
+
 #####################################################################
 
 # API entry point
 def api_main(input_path=None, output_path=None, clean=True, cache=False, release=False, push=False, gitlab_ci=False):
     input_path = Path(input_path).resolve() if input_path else Path.cwd()
     output_path = Path(output_path).resolve() if output_path else Path.cwd()
     if cache:
```

### Comparing `odoo_filter_addons-1.3.1/odoo_filter_addons.egg-info/PKG-INFO` & `odoo_filter_addons-1.3.2/odoo_filter_addons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo_filter_addons
-Version: 1.3.1
+Version: 1.3.2
 Summary: Simple utlity to filter odoo addons into a single directory
 Author-email: Pablo Esteban <pablo.esteban@forgeflow.com>
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: Operating System :: POSIX
 Classifier: Framework :: Odoo
 Classifier: Programming Language :: Python :: 3
```

### Comparing `odoo_filter_addons-1.3.1/pyproject.toml` & `odoo_filter_addons-1.3.2/pyproject.toml`

 * *Files identical despite different names*

