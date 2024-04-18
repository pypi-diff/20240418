# Comparing `tmp/digdaglog2sql-0.0.3rc1.tar.gz` & `tmp/digdaglog2sql-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digdaglog2sql-0.0.3rc1.tar", max compression
+gzip compressed data, was "digdaglog2sql-0.1.0.tar", max compression
```

## Comparing `digdaglog2sql-0.0.3rc1.tar` & `digdaglog2sql-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0    11340 2022-05-10 19:42:24.385811 digdaglog2sql-0.0.3rc1/LICENSE
--rw-r--r--   0        0        0     1483 2022-05-10 19:42:24.385811 digdaglog2sql-0.0.3rc1/README.md
--rw-r--r--   0        0        0       22 2022-05-10 19:42:24.385811 digdaglog2sql-0.0.3rc1/digdaglog2sql/__init__.py
--rw-r--r--   0        0        0     3069 2022-05-10 19:42:24.385811 digdaglog2sql-0.0.3rc1/digdaglog2sql/cli.py
--rw-r--r--   0        0        0      318 2022-05-10 19:42:24.389811 digdaglog2sql-0.0.3rc1/digdaglog2sql/extractor.py
--rw-r--r--   0        0        0     1191 2022-05-10 19:42:24.389811 digdaglog2sql-0.0.3rc1/digdaglog2sql/td_op.py
--rw-r--r--   0        0        0     1398 2022-05-10 19:42:36.085770 digdaglog2sql-0.0.3rc1/pyproject.toml
--rw-r--r--   0        0        0     2348 2022-05-10 19:42:37.199669 digdaglog2sql-0.0.3rc1/setup.py
--rw-r--r--   0        0        0     2211 2022-05-10 19:42:37.199980 digdaglog2sql-0.0.3rc1/PKG-INFO
+-rw-r--r--   0        0        0    11340 2024-04-18 00:00:23.709936 digdaglog2sql-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1384 2024-04-18 00:00:23.709936 digdaglog2sql-0.1.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-18 00:00:23.709936 digdaglog2sql-0.1.0/digdaglog2sql/__init__.py
+-rw-r--r--   0        0        0     2477 2024-04-18 00:00:23.709936 digdaglog2sql-0.1.0/digdaglog2sql/cli.py
+-rw-r--r--   0        0        0      318 2024-04-18 00:00:23.709936 digdaglog2sql-0.1.0/digdaglog2sql/extractor.py
+-rw-r--r--   0        0        0     1191 2024-04-18 00:00:23.709936 digdaglog2sql-0.1.0/digdaglog2sql/td_op.py
+-rw-r--r--   0        0        0     1276 2024-04-18 00:00:32.746046 digdaglog2sql-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2155 1970-01-01 00:00:00.000000 digdaglog2sql-0.1.0/PKG-INFO
```

### Comparing `digdaglog2sql-0.0.3rc1/LICENSE` & `digdaglog2sql-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `digdaglog2sql-0.0.3rc1/README.md` & `digdaglog2sql-0.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -16,23 +16,35 @@
 
 ## Usage
 
 ```sh
 $ digdaglog2sql --help
 Usage: digdaglog2sql [OPTIONS]
 
-Options:
-  --input FILENAME               Option is mutually exclusive with session_id,
-                                 site.
-  --session-id INTEGER           Session ID of workflow. Option is mutually
-                                 exclusive with input.
-  --site [us|jp|eu01|ap02|ap03]  Option is mutually exclusive with input.
-  --output FILENAME              [required]
+Input log by file:
+  --input FILENAME               Input file name of a workflow log. Use - for
+                                 STDIN.
+
+Download log by Session ID:
+  --session-id INTEGER           Session ID of the target workflow.
+  --site [us|jp|eu01|ap02|ap03]  Treasure Workflow site name.  [default: us]
+  --endpoint TEXT                Digdag server endpoint.
+  --http                         Enforce to use http schema.
+
+Output:
+  --output FILENAME              Output file name. Use - for STDOUT.  [required]
+
+Other options:
   --drop-cdp-db                  If true, drop cdp_audience_xxx DB name.
   --help                         Show this message and exit.
+
+Constraints:
+  {--input, --session-id}  exactly 1 required
+  {--site, --endpoint}     exactly 1 required if --session-id is set
+  {--site, --http}         mutually exclusive
 ```
 
 You can use log file on local environment.
 
 ```sh
 digdaglog2sql --input workflow-log.txt --output output.sql
 ```
@@ -40,19 +52,7 @@
 Or, you can use Session ID of Treasure Workflow.
 
 ```sh
 digdaglog2sql --session-id 12345 --site us --output output.sql
 ```
 
 Ensure set `TD_API_KEY` into environment variable.
-
-## Note
-
-As of May 5 2022, if you want to use sqllineage for Trino and Hive logs from Treasure Data,
-recommend to install sqlparse and sqllineage as the following:
-
-```sh
-pip install git+https://github.com/chezou/sqlparse.git@trino#egg=sqlparse==0.4.3.dev0
-pip install git+https://github.com/chezou/sqllineage.git@trino#egg=sqllineage==1.3.4
-```
-
-You have to ensure to have node environment for sqllineage installation from source.
```

### Comparing `digdaglog2sql-0.0.3rc1/digdaglog2sql/cli.py` & `digdaglog2sql-0.1.0/digdaglog2sql/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,93 +1,76 @@
 import os
-import typing
+from typing import IO, Iterable, Optional, cast
 
 import click
+import cloup
 import tdworkflow
+from cloup import constraint, option, option_group
+from cloup.constraints import If, RequireExactly, mutually_exclusive
 
 from .extractor import extract_sql
 
 
-class Mutex(click.Option):
-    def __init__(self, *args, **kwargs):
-        self.not_required_if: list = kwargs.pop("not_required_if")
-
-        assert self.not_required_if, "'not_required_if' parameter required"
-        kwargs["help"] = (
-            kwargs.get("help", "")
-            + "Option is mutually exclusive with "
-            + ", ".join(self.not_required_if)
-            + "."
-        ).strip()
-        super(Mutex, self).__init__(*args, **kwargs)
-
-    def handle_parse_result(self, ctx, opts, args):
-        current_opt: bool = self.name in opts
-        for mutex_opt in self.not_required_if:
-            if mutex_opt in opts:
-                if current_opt:
-                    raise click.UsageError(
-                        f"Illegal usage: '{str(self.name)}' is mutually exclusive with "
-                        + str(mutex_opt)
-                        + "."
-                    )
-                else:
-                    self.prompt = None
-        return super(Mutex, self).handle_parse_result(ctx, opts, args)
-
-
-@click.command()
-@click.option(
-    "--input",
-    type=click.File("r"),
-    prompt=True,
-    cls=Mutex,
-    not_required_if=["session_id", "site", "endpoint", "http"],
-)
-@click.option(
-    "--session-id",
-    type=int,
-    help="Session ID of workflow. ",
-    cls=Mutex,
-    not_required_if=["input"],
-)
-@click.option(
-    "--site",
-    type=click.Choice(["us", "jp", "eu01", "ap02", "ap03"]),
-    default="us",
-    cls=Mutex,
-    not_required_if=["input", "endpoint", "http"],
-)
-@click.option("--output", type=click.File("wt"), required=True)
-@click.option(
-    "--drop-cdp-db", help="If true, drop cdp_audience_xxx DB name. ", is_flag=True
-)
-@click.option(
-    "--endpoint",
-    type=str,
-    help="Digdag server endpoint.",
-    cls=Mutex,
-    not_required_if=["site", "input"],
-)
-@click.option(
-    "--http",
-    help="Use http schema.",
+@cloup.command(show_constraints=True)
+@option_group(
+    "Input log by file",
+    option(
+        "--input",
+        help="Input file name of a workflow log. Use - for STDIN.",
+        type=click.File("r"),
+    ),
+)
+@option_group(
+    "Download log by Session ID",
+    option("--session-id", help="Session ID of the target workflow.", type=int),
+    option(
+        "--site",
+        type=click.Choice(["us", "jp", "eu01", "ap02", "ap03"]),
+        help="Treasure Workflow site name.",
+        default="us",
+        show_default=True,
+    ),
+    option(
+        "--endpoint",
+        type=str,
+        help="Digdag server endpoint.",
+    ),
+    option(
+        "--http",
+        help="Enforce to use http schema.",
+        is_flag=True,
+        default=False,
+    ),
+)
+@option_group(
+    "Output",
+    option(
+        "--output",
+        help="Output file name. Use - for STDOUT.",
+        type=click.File("wt"),
+        required=True,
+    ),
+)
+@option(
+    "--drop-cdp-db",
+    help="If true, drop cdp_audience_xxx DB name. ",
     is_flag=True,
     default=False,
-    cls=Mutex,
-    not_required_if=["input", "side"],
 )
+@constraint(RequireExactly(1), ["input", "session_id"])
+@constraint(If("session_id", then=RequireExactly(1)), ["site", "endpoint"])
+@constraint(mutually_exclusive, ["site", "http"])
 def run(
-    input: typing.IO,
-    output: typing.IO,
-    session_id: str,
+    input: Optional[IO],
+    output: IO,
+    session_id: Optional[int],
     site: str,
     drop_cdp_db: bool,
-    endpoint: str,
-    http: bool,
+    endpoint: Optional[str],
+    http: Optional[bool],
 ):
 
     log = ""
     if input:
         log = input.read()
     elif session_id:
         tdwf_opts = {}
@@ -95,23 +78,21 @@
             tdwf_opts["endpoint"] = endpoint
             if http:
                 tdwf_opts["schema"] = "http"
         else:
             apikey = os.getenv("TD_API_KEY")
             if not apikey:
                 raise ValueError("TD_API_KEY should be set in environment variable.")
-            if not site:
-                raise ValueError("site option should be set.")
 
             tdwf_opts["site"] = site
             tdwf_opts["apikey"] = apikey
 
         client = tdworkflow.client.Client(**tdwf_opts)
         attempt = client.session_attempts(session=session_id)[0]
-        log = "".join(client.logs(attempt=attempt))
+        log = "".join(cast(Iterable[str], client.logs(attempt=attempt)))
 
     sql = extract_sql(log, drop_cdp_db=drop_cdp_db)
     output.write(sql)
 
 
 if __file__ == "__main__":
     run()
```

### Comparing `digdaglog2sql-0.0.3rc1/digdaglog2sql/td_op.py` & `digdaglog2sql-0.1.0/digdaglog2sql/td_op.py`

 * *Files identical despite different names*

### Comparing `digdaglog2sql-0.0.3rc1/pyproject.toml` & `digdaglog2sql-0.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "digdaglog2sql"
-version = "v0.0.3rc1" # Use poetry-dynamic-versioning
+version = "v0.1.0" # Use poetry-dynamic-versioning
 description = "Extract SQLs from digdag log"
 license = "Apache-2.0"
 readme = "README.md"
 authors = ["Aki Ariga <chezou@gmail.com>"]
 maintainers = ["Aki Ariga <chezou@gmail.com>"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8.1"
 taskipy = "^1.10.1"
 click = "^8.1.3"
-tdworkflow = "^0.6.0"
+tdworkflow = "^0.8.3"
+cloup = "~0.14.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2"
 mypy = "^0.950"
 black = "^22.3.0"
-flake8 = "^4.0.1"
+flake8 = "^7.0.0"
 isort = "^5.10.1"
-importlib-metadata = {version = ">=1.6.0", python = "<3.8"}
 
 [tool.poetry.scripts]
 digdaglog2sql = "digdaglog2sql.cli:run"
 
 [tool.poetry-dynamic-versioning]
 enable = true
 style = "pep440"
@@ -34,14 +34,10 @@
 fmt = { cmd = "black tests digdaglog2sql && isort digdaglog2sql tests", help = "format code" }
 lint = { cmd = "task lint_black && task lint_flake8 && task lint_isort && task lint_mypy", help = "exec lint" }
 lint_flake8 = "flake8 --max-line-length=88 tests digdaglog2sql"
 lint_mypy = "mypy tests digdaglog2sql"
 lint_black = "black --check tests digdaglog2sql"
 lint_isort = "isort digdaglog2sql tests --check-only"
 
-[[tool.mypy.overrides]]
-module = ["tdworkflow"]
-ignore_missing_imports = true
-
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `digdaglog2sql-0.0.3rc1/PKG-INFO` & `digdaglog2sql-0.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: digdaglog2sql
-Version: 0.0.3rc1
+Version: 0.1.0
 Summary: Extract SQLs from digdag log
 License: Apache-2.0
 Author: Aki Ariga
 Author-email: chezou@gmail.com
 Maintainer: Aki Ariga
 Maintainer-email: chezou@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: cloup (>=0.14.0,<0.15.0)
 Requires-Dist: taskipy (>=1.10.1,<2.0.0)
-Requires-Dist: tdworkflow (>=0.6.0,<0.7.0)
+Requires-Dist: tdworkflow (>=0.8.3,<0.9.0)
 Description-Content-Type: text/markdown
 
 # digdaglog2sql
 
 ## Install
 
 ```sh
@@ -37,23 +38,35 @@
 
 ## Usage
 
 ```sh
 $ digdaglog2sql --help
 Usage: digdaglog2sql [OPTIONS]
 
-Options:
-  --input FILENAME               Option is mutually exclusive with session_id,
-                                 site.
-  --session-id INTEGER           Session ID of workflow. Option is mutually
-                                 exclusive with input.
-  --site [us|jp|eu01|ap02|ap03]  Option is mutually exclusive with input.
-  --output FILENAME              [required]
+Input log by file:
+  --input FILENAME               Input file name of a workflow log. Use - for
+                                 STDIN.
+
+Download log by Session ID:
+  --session-id INTEGER           Session ID of the target workflow.
+  --site [us|jp|eu01|ap02|ap03]  Treasure Workflow site name.  [default: us]
+  --endpoint TEXT                Digdag server endpoint.
+  --http                         Enforce to use http schema.
+
+Output:
+  --output FILENAME              Output file name. Use - for STDOUT.  [required]
+
+Other options:
   --drop-cdp-db                  If true, drop cdp_audience_xxx DB name.
   --help                         Show this message and exit.
+
+Constraints:
+  {--input, --session-id}  exactly 1 required
+  {--site, --endpoint}     exactly 1 required if --session-id is set
+  {--site, --http}         mutually exclusive
 ```
 
 You can use log file on local environment.
 
 ```sh
 digdaglog2sql --input workflow-log.txt --output output.sql
 ```
@@ -62,19 +75,7 @@
 
 ```sh
 digdaglog2sql --session-id 12345 --site us --output output.sql
 ```
 
 Ensure set `TD_API_KEY` into environment variable.
 
-## Note
-
-As of May 5 2022, if you want to use sqllineage for Trino and Hive logs from Treasure Data,
-recommend to install sqlparse and sqllineage as the following:
-
-```sh
-pip install git+https://github.com/chezou/sqlparse.git@trino#egg=sqlparse==0.4.3.dev0
-pip install git+https://github.com/chezou/sqllineage.git@trino#egg=sqllineage==1.3.4
-```
-
-You have to ensure to have node environment for sqllineage installation from source.
-
```

