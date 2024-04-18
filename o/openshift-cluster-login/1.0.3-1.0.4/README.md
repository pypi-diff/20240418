# Comparing `tmp/openshift_cluster_login-1.0.3.tar.gz` & `tmp/openshift_cluster_login-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openshift_cluster_login-1.0.3.tar", max compression
+gzip compressed data, was "openshift_cluster_login-1.0.4.tar", max compression
```

## Comparing `openshift_cluster_login-1.0.3.tar` & `openshift_cluster_login-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1073 2024-04-11 09:34:54.611325 openshift_cluster_login-1.0.3/LICENSE
--rw-r--r--   0        0        0     5190 2024-04-11 09:34:54.611325 openshift_cluster_login-1.0.3/README.md
--rw-r--r--   0        0        0        0 2024-04-11 09:34:54.623324 openshift_cluster_login-1.0.3/ocl/__init__.py
--rw-r--r--   0        0        0    13422 2024-04-11 09:34:54.623324 openshift_cluster_login-1.0.3/ocl/__main__.py
--rw-r--r--   0        0        0        0 2024-04-11 09:34:54.623324 openshift_cluster_login-1.0.3/ocl/gql_definitions/__init__.py
--rw-r--r--   0        0        0       97 2024-04-11 09:34:54.623324 openshift_cluster_login-1.0.3/ocl/gql_definitions/clusters.gql
--rw-r--r--   0        0        0     1728 2024-04-11 09:34:54.623324 openshift_cluster_login-1.0.3/ocl/gql_definitions/clusters.py
--rw-r--r--   0        0        0        0 2024-04-11 09:34:54.623324 openshift_cluster_login-1.0.3/ocl/gql_definitions/fragments/__init__.py
--rw-r--r--   0        0        0      152 2024-04-11 09:34:54.623324 openshift_cluster_login-1.0.3/ocl/gql_definitions/fragments/cluster.gql
--rw-r--r--   0        0        0     1095 2024-04-11 09:34:54.623324 openshift_cluster_login-1.0.3/ocl/gql_definitions/fragments/cluster.py
--rw-r--r--   0        0        0      145 2024-04-11 09:34:54.623324 openshift_cluster_login-1.0.3/ocl/gql_definitions/namespaces.gql
--rw-r--r--   0        0        0     1982 2024-04-11 09:34:54.623324 openshift_cluster_login-1.0.3/ocl/gql_definitions/namespaces.py
--rw-r--r--   0        0        0     1745 2024-04-11 09:34:54.623324 openshift_cluster_login-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     6273 1970-01-01 00:00:00.000000 openshift_cluster_login-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-18 07:52:42.410214 openshift_cluster_login-1.0.4/LICENSE
+-rw-r--r--   0        0        0     5190 2024-04-18 07:52:42.410214 openshift_cluster_login-1.0.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-18 07:52:42.418214 openshift_cluster_login-1.0.4/ocl/__init__.py
+-rw-r--r--   0        0        0    14183 2024-04-18 07:52:42.418214 openshift_cluster_login-1.0.4/ocl/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-18 07:52:42.418214 openshift_cluster_login-1.0.4/ocl/gql_definitions/__init__.py
+-rw-r--r--   0        0        0       97 2024-04-18 07:52:42.418214 openshift_cluster_login-1.0.4/ocl/gql_definitions/clusters.gql
+-rw-r--r--   0        0        0     1728 2024-04-18 07:52:42.418214 openshift_cluster_login-1.0.4/ocl/gql_definitions/clusters.py
+-rw-r--r--   0        0        0        0 2024-04-18 07:52:42.418214 openshift_cluster_login-1.0.4/ocl/gql_definitions/fragments/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-18 07:52:42.418214 openshift_cluster_login-1.0.4/ocl/gql_definitions/fragments/cluster.gql
+-rw-r--r--   0        0        0     1095 2024-04-18 07:52:42.418214 openshift_cluster_login-1.0.4/ocl/gql_definitions/fragments/cluster.py
+-rw-r--r--   0        0        0      145 2024-04-18 07:52:42.418214 openshift_cluster_login-1.0.4/ocl/gql_definitions/namespaces.gql
+-rw-r--r--   0        0        0     1982 2024-04-18 07:52:42.418214 openshift_cluster_login-1.0.4/ocl/gql_definitions/namespaces.py
+-rw-r--r--   0        0        0     2021 2024-04-18 07:52:42.418214 openshift_cluster_login-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6273 1970-01-01 00:00:00.000000 openshift_cluster_login-1.0.4/PKG-INFO
```

### Comparing `openshift_cluster_login-1.0.3/LICENSE` & `openshift_cluster_login-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openshift_cluster_login-1.0.3/README.md` & `openshift_cluster_login-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `openshift_cluster_login-1.0.3/ocl/__main__.py` & `openshift_cluster_login-1.0.4/ocl/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os
 import re
 import shutil
 import subprocess
 import sys
 import tempfile
 import webbrowser
+from collections.abc import Generator
 from pathlib import Path
 from typing import (
     Any,
     Optional,
     Tuple,
     Union,
 )
@@ -86,15 +87,15 @@
 
     print(
         f"[bold red]Missing environment variable [bold green]{env_var}[bold green][/bold red]"
     )
     return Prompt.ask(f"Enter OCL_{var_name}", password=hidden)
 
 
-def select_cluster(cluster_name) -> Cluster:
+def select_cluster(cluster_name: str) -> Cluster:
     clusters = clusters_from_app_interface()
     # user defined clusters
     clusters += [
         Cluster(**c) for c in json.loads(get_var("USER_CLUSTERS", default="[]"))
     ]
     clusters_dict = {c.name: c for c in clusters}
     if cluster_name not in clusters_dict:
@@ -297,47 +298,72 @@
     for index in range(size):
         blend = index / size
         color = f"#{int(r1 + dr * blend):2X}{int(g1 + dg * blend):2X}{int(b1 + db * blend):2X}"
         text.stylize(color, index, index + 1)
     return text
 
 
-def bye():
+def bye() -> None:
     print(
         "Thank you for using openshift-login. :man_bowing: Have a great day ahead! :red_heart-emoji:"
     )
 
 
-def enable_requests_logging():
+def enable_requests_logging() -> None:
     from http.client import HTTPConnection  # noqa: PLC0415
 
     HTTPConnection.debuglevel = 1
     logging.getLogger().setLevel(logging.DEBUG)
     requests_log = logging.getLogger("urllib3")
     requests_log.setLevel(logging.DEBUG)
     requests_log.propagate = True
 
 
+def complete_cluster(ctx: typer.Context, incomplete: str) -> Generator[str, None, None]:
+    for cluster in clusters_from_app_interface():
+        if cluster.name.startswith(incomplete):
+            yield cluster.name
+
+
+def complete_project(ctx: typer.Context, incomplete: str) -> Generator[str, None, None]:
+    cluster = ctx.params.get("cluster_name")
+    if not cluster:
+        return
+    for ns in [
+        ns for ns in namespaces_from_app_interface() if ns.cluster.name == cluster
+    ]:
+        if ns.name.startswith(incomplete):
+            yield ns.name
+
+
 @app.command(epilog="Made with :heart: by [blue]https://github.com/chassing[/]")
 def main(  # noqa: PLR0912
-    cluster_name: str = typer.Argument(None, help="Cluster name"),
-    project: str = typer.Argument(None, help="Namespace/Project"),
+    cluster_name: str = typer.Argument(
+        None,
+        help="Cluster name",
+        autocompletion=complete_cluster,
+    ),
+    project: str = typer.Argument(
+        None,
+        help="Namespace/Project",
+        autocompletion=complete_project,
+    ),
     debug: bool = typer.Option(False, help="Enable debug mode"),
     open_in_browser: bool = typer.Option(
         False, help="Open the console in browser instead of local shell"
     ),
     display_banner: bool = typer.Option(True, help="Display shiny OCL banner"),
     refresh_login: bool = typer.Option(
         False, help="Enforce a new login to refresh the session."
     ),
     idp: list[str] = typer.Option(
         ["redhat-app-sre-auth"],
         help="Automatically login via given IDPs (use in given order, try next one if failed). Use 'manual' for manual login.",
     ),
-):
+) -> None:
     logging.basicConfig(
         level=logging.INFO if not debug else logging.DEBUG, format="%(message)s"
     )
     if debug:
         enable_requests_logging()
 
     if display_banner:
@@ -387,15 +413,15 @@
             project = ""
 
     print(
         f"""Spawn new shell, use exit or CTRL+d to leave it!
 
     URL: {console_url}
     Cluster: [bold green] {cluster.name}[/]
-    {f'Project: [bold yellow]☸ {project}[/]' if project else ''}"""
+    {f"Project: [bold yellow]☸ {project}[/]" if project else ""}"""
     )
     run(
         os.environ["SHELL"],
         check=False,
         cluster=cluster,
         capture_output=False,
         temp_kube_config=True,
```

### Comparing `openshift_cluster_login-1.0.3/ocl/gql_definitions/clusters.py` & `openshift_cluster_login-1.0.4/ocl/gql_definitions/clusters.py`

 * *Files identical despite different names*

### Comparing `openshift_cluster_login-1.0.3/ocl/gql_definitions/fragments/cluster.py` & `openshift_cluster_login-1.0.4/ocl/gql_definitions/fragments/cluster.py`

 * *Files identical despite different names*

### Comparing `openshift_cluster_login-1.0.3/ocl/gql_definitions/namespaces.py` & `openshift_cluster_login-1.0.4/ocl/gql_definitions/namespaces.py`

 * *Files identical despite different names*

### Comparing `openshift_cluster_login-1.0.3/pyproject.toml` & `openshift_cluster_login-1.0.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openshift-cluster-login"
-version = "1.0.3"
+version = "1.0.4"
 description = "Openshift cluster login on command line"
 authors = ["Christian Assing <cassing@redhat.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "http://github.com/chassing/ocl"
 packages = [{ include = "ocl" }]
 
@@ -20,30 +20,30 @@
 diskcache = "^5.4.0"
 requests-kerberos = "^0.14.0"
 pyquery = "^2.0.0"
 
 [tool.poetry.group.dev.dependencies]
 types-requests = "^2.28.7"
 pyjwt = "^2.8.0"
-ruff = "^0.1.11"
+ruff = "^0.3.7"
 mypy = "^1.8.0"
 qenerate = "^0.6.3"
 setuptools = "^69.0.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 ocl = 'ocl.__main__:app'
 
 [tool.ruff]
 line-length = 88
 target-version = 'py311'
-required-version = "0.1.11"
+required-version = "0.3.7"
 
 src = ["ocl"]
 extend-exclude = ["ocl/gql_definitions"]
 fix = true
 
 [tool.ruff.lint]
 preview = true
@@ -65,12 +65,24 @@
 ]
 [tool.ruff.format]
 preview = true
 
 [tool.ruff.lint.isort]
 known-first-party = ["ocl"]
 
+[tool.mypy]
+files = ["ocl"]
+plugins = ["pydantic.mypy"]
+enable_error_code = ["truthy-bool", "redundant-expr"]
+no_implicit_optional = true
+check_untyped_defs = true
+warn_unused_ignores = true
+show_error_codes = true
+disallow_untyped_defs = true
+disallow_incomplete_defs = true
+
+
 [[tool.mypy.overrides]]
 # Below are all of the packages that don't implement stub packages. Mypy will throw an error if we don't ignore the
 # missing imports. See: https://mypy.readthedocs.io/en/stable/running_mypy.html#missing-imports
 module = ["appdirs.*", "diskcache.*", "pyquery.*", "requests_kerberos.*"]
 ignore_missing_imports = true
```

### Comparing `openshift_cluster_login-1.0.3/PKG-INFO` & `openshift_cluster_login-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-cluster-login
-Version: 1.0.3
+Version: 1.0.4
 Summary: Openshift cluster login on command line
 Home-page: http://github.com/chassing/ocl
 License: MIT
 Author: Christian Assing
 Author-email: cassing@redhat.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

