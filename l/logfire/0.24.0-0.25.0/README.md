# Comparing `tmp/logfire-0.24.0.tar.gz` & `tmp/logfire-0.25.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logfire-0.24.0.tar", max compression
+gzip compressed data, was "logfire-0.25.0.tar", max compression
```

## Comparing `logfire-0.24.0.tar` & `logfire-0.25.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1099 2024-04-11 13:44:34.633989 logfire-0.24.0/LICENSE
--rw-r--r--   0        0        0      111 2024-04-11 13:44:34.633989 logfire-0.24.0/README.md
--rw-r--r--   0        0        0     2787 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/__init__.py
--rw-r--r--   0        0        0       88 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/__main__.py
--rw-r--r--   0        0        0      183 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/_internal/__init__.py
--rw-r--r--   0        0        0     4247 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/_internal/ast_utils.py
--rw-r--r--   0        0        0     4034 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/_internal/async_.py
--rw-r--r--   0        0        0     3534 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/_internal/auth.py
--rw-r--r--   0        0        0     2946 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/_internal/auto_trace/__init__.py
--rw-r--r--   0        0        0     4588 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/_internal/auto_trace/import_hook.py
--rw-r--r--   0        0        0     6456 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/_internal/auto_trace/rewrite_ast.py
--rw-r--r--   0        0        0     1789 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/_internal/auto_trace/types.py
--rw-r--r--   0        0        0     9110 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/_internal/backfill.py
--rw-r--r--   0        0        0    16459 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/_internal/cli.py
--rw-r--r--   0        0        0      570 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/_internal/collect_system_info.py
--rw-r--r--   0        0        0    54145 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/_internal/config.py
--rw-r--r--   0        0        0     8997 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/_internal/config_params.py
--rw-r--r--   0        0        0     4535 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/constants.py
--rw-r--r--   0        0        0       38 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/exporters/__init__.py
--rw-r--r--   0        0        0    17141 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/exporters/console.py
--rw-r--r--   0        0        0     1041 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/exporters/fallback.py
--rw-r--r--   0        0        0     7447 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/exporters/file.py
--rw-r--r--   0        0        0     4035 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/exporters/otlp.py
--rw-r--r--   0        0        0     6958 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/exporters/processor_wrapper.py
--rw-r--r--   0        0        0     1787 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/exporters/remove_pending.py
--rw-r--r--   0        0        0      691 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/exporters/wrapper.py
--rw-r--r--   0        0        0     5680 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/formatter.py
--rw-r--r--   0        0        0     5716 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/instrument.py
--rw-r--r--   0        0        0       46 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/integrations/__init__.py
--rw-r--r--   0        0        0     2634 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/integrations/executors.py
--rw-r--r--   0        0        0     9435 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/integrations/fastapi.py
--rw-r--r--   0        0        0     7732 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/json_encoder.py
--rw-r--r--   0        0        0    11646 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/json_formatter.py
--rw-r--r--   0        0        0    12089 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/json_schema.py
--rw-r--r--   0        0        0     2753 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/json_types.py
--rw-r--r--   0        0        0      313 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/limits.py
--rw-r--r--   0        0        0    47334 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/main.py
--rw-r--r--   0        0        0    12850 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/metrics.py
--rw-r--r--   0        0        0     8603 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/scrubbing.py
--rw-r--r--   0        0        0     2007 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/stack_info.py
--rw-r--r--   0        0        0    10566 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/tracer.py
--rw-r--r--   0        0        0     5852 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/utils.py
--rw-r--r--   0        0        0       53 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/cli.py
--rw-r--r--   0        0        0      145 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/exceptions.py
--rw-r--r--   0        0        0       99 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/integrations/__init__.py
--rw-r--r--   0        0        0     3718 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/integrations/logging.py
--rw-r--r--   0        0        0     3242 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/integrations/loguru.py
--rw-r--r--   0        0        0    16134 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/integrations/pydantic.py
--rw-r--r--   0        0        0     1388 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/integrations/structlog.py
--rw-r--r--   0        0        0     2327 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/propagate.py
--rw-r--r--   0        0        0        0 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/py.typed
--rw-r--r--   0        0        0    10606 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/testing.py
--rw-r--r--   0        0        0      123 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/version.py
--rw-r--r--   0        0        0     5267 2024-04-11 13:44:34.661989 logfire-0.24.0/pyproject.toml
--rw-r--r--   0        0        0     3905 1970-01-01 00:00:00.000000 logfire-0.24.0/PKG-INFO
+-rw-r--r--   0        0        0     1099 2024-04-18 17:58:08.175509 logfire-0.25.0/LICENSE
+-rw-r--r--   0        0        0      111 2024-04-18 17:58:08.175509 logfire-0.25.0/README.md
+-rw-r--r--   0        0        0     2787 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/__main__.py
+-rw-r--r--   0        0        0      183 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/__init__.py
+-rw-r--r--   0        0        0     4247 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/ast_utils.py
+-rw-r--r--   0        0        0     4034 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/async_.py
+-rw-r--r--   0        0        0     3534 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/auth.py
+-rw-r--r--   0        0        0     2946 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/auto_trace/__init__.py
+-rw-r--r--   0        0        0     4588 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/auto_trace/import_hook.py
+-rw-r--r--   0        0        0     6456 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/auto_trace/rewrite_ast.py
+-rw-r--r--   0        0        0     1789 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/auto_trace/types.py
+-rw-r--r--   0        0        0     9110 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/backfill.py
+-rw-r--r--   0        0        0    16765 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/cli.py
+-rw-r--r--   0        0        0      570 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/collect_system_info.py
+-rw-r--r--   0        0        0    52643 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/config.py
+-rw-r--r--   0        0        0     8997 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/config_params.py
+-rw-r--r--   0        0        0     4535 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/constants.py
+-rw-r--r--   0        0        0       38 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/exporters/__init__.py
+-rw-r--r--   0        0        0    17141 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/exporters/console.py
+-rw-r--r--   0        0        0     1041 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/exporters/fallback.py
+-rw-r--r--   0        0        0     7447 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/exporters/file.py
+-rw-r--r--   0        0        0     4035 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/exporters/otlp.py
+-rw-r--r--   0        0        0     8460 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/exporters/processor_wrapper.py
+-rw-r--r--   0        0        0     1787 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/exporters/remove_pending.py
+-rw-r--r--   0        0        0      691 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/exporters/wrapper.py
+-rw-r--r--   0        0        0     5680 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/formatter.py
+-rw-r--r--   0        0        0     5716 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/instrument.py
+-rw-r--r--   0        0        0       46 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/integrations/__init__.py
+-rw-r--r--   0        0        0     2634 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/integrations/executors.py
+-rw-r--r--   0        0        0     9435 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/integrations/fastapi.py
+-rw-r--r--   0        0        0     8242 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/json_encoder.py
+-rw-r--r--   0        0        0    11646 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/json_formatter.py
+-rw-r--r--   0        0        0    12255 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/json_schema.py
+-rw-r--r--   0        0        0     2753 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/json_types.py
+-rw-r--r--   0        0        0      313 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/limits.py
+-rw-r--r--   0        0        0    47334 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/main.py
+-rw-r--r--   0        0        0    12850 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/metrics.py
+-rw-r--r--   0        0        0     8603 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/scrubbing.py
+-rw-r--r--   0        0        0     2007 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/stack_info.py
+-rw-r--r--   0        0        0    10566 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/tracer.py
+-rw-r--r--   0        0        0     5852 2024-04-18 17:58:08.247509 logfire-0.25.0/logfire/_internal/utils.py
+-rw-r--r--   0        0        0       53 2024-04-18 17:58:08.251509 logfire-0.25.0/logfire/cli.py
+-rw-r--r--   0        0        0      145 2024-04-18 17:58:08.251509 logfire-0.25.0/logfire/exceptions.py
+-rw-r--r--   0        0        0       99 2024-04-18 17:58:08.251509 logfire-0.25.0/logfire/integrations/__init__.py
+-rw-r--r--   0        0        0     3718 2024-04-18 17:58:08.251509 logfire-0.25.0/logfire/integrations/logging.py
+-rw-r--r--   0        0        0     3242 2024-04-18 17:58:08.251509 logfire-0.25.0/logfire/integrations/loguru.py
+-rw-r--r--   0        0        0    16134 2024-04-18 17:58:08.251509 logfire-0.25.0/logfire/integrations/pydantic.py
+-rw-r--r--   0        0        0     1388 2024-04-18 17:58:08.251509 logfire-0.25.0/logfire/integrations/structlog.py
+-rw-r--r--   0        0        0     2327 2024-04-18 17:58:08.251509 logfire-0.25.0/logfire/propagate.py
+-rw-r--r--   0        0        0        0 2024-04-18 17:58:08.251509 logfire-0.25.0/logfire/py.typed
+-rw-r--r--   0        0        0    10635 2024-04-18 17:58:08.251509 logfire-0.25.0/logfire/testing.py
+-rw-r--r--   0        0        0      123 2024-04-18 17:58:08.251509 logfire-0.25.0/logfire/version.py
+-rw-r--r--   0        0        0     5267 2024-04-18 17:58:08.251509 logfire-0.25.0/pyproject.toml
+-rw-r--r--   0        0        0     3905 1970-01-01 00:00:00.000000 logfire-0.25.0/PKG-INFO
```

### Comparing `logfire-0.24.0/LICENSE` & `logfire-0.25.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/__init__.py` & `logfire-0.25.0/logfire/__init__.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/ast_utils.py` & `logfire-0.25.0/logfire/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/async_.py` & `logfire-0.25.0/logfire/_internal/async_.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/auth.py` & `logfire-0.25.0/logfire/_internal/auth.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/auto_trace/__init__.py` & `logfire-0.25.0/logfire/_internal/auto_trace/__init__.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/auto_trace/import_hook.py` & `logfire-0.25.0/logfire/_internal/auto_trace/import_hook.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/auto_trace/rewrite_ast.py` & `logfire-0.25.0/logfire/_internal/auto_trace/rewrite_ast.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/auto_trace/types.py` & `logfire-0.25.0/logfire/_internal/auto_trace/types.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/backfill.py` & `logfire-0.25.0/logfire/_internal/backfill.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/cli.py` & `logfire-0.25.0/logfire/_internal/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import platform
 import shutil
 import sys
 import warnings
 import webbrowser
 from pathlib import Path
 from typing import Any, Iterator, cast
-from urllib.parse import urljoin
+from urllib.parse import urljoin, urlparse
 
 import requests
 from opentelemetry import trace
 from rich.console import Console
 from rich.progress import Progress
 from rich.table import Table
 
@@ -32,15 +32,15 @@
 from .config import LogfireCredentials
 from .constants import LOGFIRE_BASE_URL
 from .tracer import SDKTracerProvider
 from .utils import read_toml_file
 
 BASE_OTEL_INTEGRATION_URL = 'https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/'
 BASE_DOCS_URL = 'https://docs.logfire.dev'
-INTEGRATIONS_DOCS_URL = f'{BASE_DOCS_URL}/guide/integrations/'
+INTEGRATIONS_DOCS_URL = f'{BASE_DOCS_URL}/integrations/'
 
 HOME_LOGFIRE.mkdir(exist_ok=True)
 
 LOGFIRE_LOG_FILE = HOME_LOGFIRE / 'log.txt'
 file_handler = logging.FileHandler(LOGFIRE_LOG_FILE)
 file_handler.setLevel(logging.DEBUG)
 logging.basicConfig(handlers=[file_handler], level=logging.DEBUG)
@@ -56,14 +56,20 @@
     print(f'Running Logfire {VERSION} with {py_impl} {py_version} on {system}.')
 
 
 # TODO(Marcelo): Needs to be updated to reflect `logfire auth`.
 def parse_whoami(args: argparse.Namespace) -> None:
     """Get your dashboard url and project name."""
     data_dir = Path(args.data_dir)
+    current_user = LogfireCredentials.get_current_user(session=args._session, logfire_api_url=args.logfire_url)
+    if current_user is None:
+        sys.stderr.write('Not logged in. Run `logfire auth` to log in.\n')
+    else:
+        username = current_user['name']
+        sys.stderr.write(f'Logged in as: {username}\n')
     credentials = LogfireCredentials.load_creds_file(data_dir)
     if credentials is None:
         sys.stderr.write(f'No Logfire credentials found in {data_dir.resolve()}\n')
         sys.exit(1)
     else:
         sys.stderr.write(f'Credentials loaded from data dir: {data_dir.resolve()}\n\n')
         credentials.print_token_summary()
@@ -220,15 +226,15 @@
         console.print('\n[bold blue]For further information, visit[/bold blue]', end=' ')
         console.print(f'[link={INTEGRATIONS_DOCS_URL}]{INTEGRATIONS_DOCS_URL}[/link]')
 
 
 def parse_auth(args: argparse.Namespace) -> None:
     """Authenticate with Logfire.
 
-    This command will authenticate you with Logfire, and store the credentials.
+    It will authenticate you with Logfire, and store the credentials.
     """
     console = Console(file=sys.stderr)
     logfire_url = cast(str, args.logfire_url)
 
     if DEFAULT_FILE.is_file():
         data = cast(DefaultFile, read_toml_file(DEFAULT_FILE))
         if is_logged_in(data, logfire_url):  # pragma: no branch
@@ -239,15 +245,16 @@
 
     console.print()
     console.print('Welcome to Logfire! :fire:')
     console.print('Before you can send data to Logfire, we need to authenticate you.')
     console.print()
 
     device_code, frontend_auth_url = request_device_code(args._session, logfire_url)
-    console.input('Press [bold]Enter[/] to open logfire.dev in your browser...')
+    frontend_host = urlparse(frontend_auth_url).netloc
+    console.input(f'Press [bold]Enter[/] to open {frontend_host} in your browser...')
     try:
         webbrowser.open(frontend_auth_url, new=2)
     except webbrowser.Error:
         pass
     console.print(f"Please open [bold]{frontend_auth_url}[/] in your browser to authenticate if it hasn't already.")
     console.print('Waiting for you to authenticate with Logfire...')
 
@@ -328,74 +335,70 @@
         project_name=project_name,
     )
     if project_info:
         credentials = _write_credentials(project_info, data_dir, logfire_url)
         console.print(f'Project configured successfully. You will be able to view it at: {credentials.project_url}')
 
 
-def main(args: list[str] | None = None) -> None:
-    """Run the CLI."""
+def _main(args: list[str] | None = None) -> None:
     parser = argparse.ArgumentParser(
         prog='logfire',
         description='The CLI for Pydantic Logfire.',
-        add_help=True,
         epilog='See https://docs.logfire.dev/guide/cli/ for more detailed documentation.',
     )
 
     parser.add_argument('--version', action='store_true', help='show the version and exit')
+    global_opts = parser.add_argument_group(title='global options')
+    global_opts.add_argument('--logfire-url', default=LOGFIRE_BASE_URL, help=argparse.SUPPRESS)
     parser.set_defaults(func=lambda _: parser.print_help())  # type: ignore
     subparsers = parser.add_subparsers(title='commands', metavar='')
 
     # Note(DavidM): Let's try to keep the commands listed in alphabetical order if we can
-    cmd_auth = subparsers.add_parser('auth', help='Authenticate with Logfire')
-    cmd_auth.add_argument('--logfire-url', default=LOGFIRE_BASE_URL, help=argparse.SUPPRESS)
+    cmd_auth = subparsers.add_parser('auth', help='authenticate with Logfire', description=parse_auth.__doc__)
     cmd_auth.set_defaults(func=parse_auth)
 
-    cmd_backfill = subparsers.add_parser('backfill', help='Bulk ingest backfill data')
+    cmd_backfill = subparsers.add_parser('backfill', help='bulk ingest backfill data')
     cmd_backfill.add_argument('--data-dir', default='.logfire')
     cmd_backfill.add_argument('--file', default='logfire_spans.bin')
-    cmd_backfill.add_argument('--logfire-url', default=LOGFIRE_BASE_URL, help=argparse.SUPPRESS)
     cmd_backfill.set_defaults(func=parse_backfill)
 
-    cmd_clean = subparsers.add_parser('clean', help='Remove the contents of the Logfire data directory')
+    cmd_clean = subparsers.add_parser('clean', help='remove the contents of the Logfire data directory')
     cmd_clean.add_argument('--data-dir', default='.logfire')
-    cmd_clean.add_argument('--logs', action='store_true', default=False, help='Remove the Logfire logs.')
+    cmd_clean.add_argument('--logs', action='store_true', default=False, help='remove the Logfire logs')
     cmd_clean.set_defaults(func=parse_clean)
 
     cmd_inspect = subparsers.add_parser(
         'inspect',
-        help="Suggest opentelemetry instrumentations based on your environment's installed packages",
+        help="suggest OpenTelemetry instrumentations based on your environment's installed packages",
     )
     cmd_inspect.set_defaults(func=parse_inspect)
 
-    cmd_whoami = subparsers.add_parser('whoami', help='Display the URL to your Logfire project')
+    cmd_whoami = subparsers.add_parser('whoami', help='display the URL to your Logfire project')
     cmd_whoami.add_argument('--data-dir', default='.logfire')
     cmd_whoami.set_defaults(func=parse_whoami)
 
-    cmd_projects = subparsers.add_parser('projects', help='Project management with Logfire.')
+    cmd_projects = subparsers.add_parser('projects', help='project management for Logfire')
+    cmd_projects.set_defaults(func=lambda _: cmd_projects.print_help())  # type: ignore
     projects_subparsers = cmd_projects.add_subparsers()
-    cmd_projects_list = projects_subparsers.add_parser('list', help='List projects.')
-    cmd_projects_list.add_argument('--logfire-url', default=LOGFIRE_BASE_URL, help='Logfire API URL.')
+    cmd_projects_list = projects_subparsers.add_parser('list', help='list projects')
     cmd_projects_list.set_defaults(func=parse_list_projects)
 
-    cmd_projects_new = projects_subparsers.add_parser('new', help='Create a new project.')
-    cmd_projects_new.add_argument('project_name', nargs='?', help='Project name.')
+    cmd_projects_new = projects_subparsers.add_parser('new', help='create a new project')
+    cmd_projects_new.add_argument('project_name', nargs='?', help='project name')
     cmd_projects_new.add_argument('--data-dir', default='.logfire')
-    cmd_projects_new.add_argument('--logfire-url', default=LOGFIRE_BASE_URL, help='Logfire API URL.')
-    cmd_projects_new.add_argument('--org', help='Project organization.')
+    cmd_projects_new.add_argument('--org', help='project organization')
     cmd_projects_new.add_argument(
-        '--default-org', action='store_true', help='Whether to create project under user default organization.'
+        '--default-org', action='store_true', help='whether to create project under user default organization'
     )
     cmd_projects_new.set_defaults(func=parse_create_new_project)
 
-    cmd_projects_use = projects_subparsers.add_parser('use', help='Use a project.')
-    cmd_projects_use.add_argument('project_name', help='Project name.')
-    cmd_projects_use.add_argument('--org', help='Project organization.')
+    cmd_projects_use = projects_subparsers.add_parser('use', help='use a project')
+    cmd_projects_use.add_argument('project_name', help='project name')
+    cmd_projects_use.add_argument('--org', help='project organization')
     cmd_projects_use.add_argument('--data-dir', default='.logfire')
-    cmd_projects_use.add_argument('--logfire-url', default=LOGFIRE_BASE_URL, help='Logfire API URL.')
     cmd_projects_use.set_defaults(func=parse_use_project)
 
     namespace = parser.parse_args(args)
 
     trace.set_tracer_provider(tracer_provider=SDKTracerProvider())
     tracer = trace.get_tracer(__name__)
 
@@ -409,7 +412,16 @@
             session.headers.update(context)
             namespace._session = session
 
             if namespace.version:
                 version_callback()
             else:
                 namespace.func(namespace)
+
+
+def main(args: list[str] | None = None) -> None:
+    """Run the CLI."""
+    try:
+        _main(args)
+    except KeyboardInterrupt:
+        sys.stderr.write('User cancelled.\n')
+        sys.exit(1)
```

### Comparing `logfire-0.24.0/logfire/_internal/collect_system_info.py` & `logfire-0.25.0/logfire/_internal/collect_system_info.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/config.py` & `logfire-0.25.0/logfire/_internal/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -598,53 +598,39 @@
                             colors=self.console.colors,
                             include_timestamp=self.console.include_timestamps,
                             verbose=self.console.verbose,
                         ),
                     )
                 )
 
-            credentials_from_local_file = None
-
             metric_readers = self.metric_readers
 
             if (self.send_to_logfire == 'if-token-present' and self.token is not None) or self.send_to_logfire is True:
-                new_credentials: LogfireCredentials | None = None
+                credentials: LogfireCredentials | None = None
                 if self.token is None:
-                    credentials_from_local_file = LogfireCredentials.load_creds_file(self.data_dir)
-                    credentials_to_save = credentials_from_local_file
-                    if not credentials_from_local_file:  # pragma: no branch
-                        if os.getenv('LOGFIRE_ANONYMOUS_PROJECT_ENABLED') == 'true':  # pragma: no cover
-                            new_credentials = LogfireCredentials.create_anonymous_project(
-                                logfire_api_url=self.base_url,
-                                requested_project_name=self.project_name or default_project_name(),
-                                session=self.logfire_api_session,
-                            )
-                        else:
-                            new_credentials = LogfireCredentials.initialize_project(
-                                logfire_api_url=self.base_url,
-                                project_name=self.project_name,
-                                session=self.logfire_api_session,
-                            )
-                        new_credentials.write_creds_file(self.data_dir)
-                        if self.show_summary:  # pragma: no branch
-                            new_credentials.print_token_summary()
-                        credentials_to_save = new_credentials
-                        # to avoid printing another summary
-                        credentials_from_local_file = None
-
-                    assert credentials_to_save is not None
-                    self.token = self.token or credentials_to_save.token
-                    self.project_name = self.project_name or credentials_to_save.project_name
-                    self.base_url = self.base_url or credentials_to_save.logfire_api_url
+                    if (credentials := LogfireCredentials.load_creds_file(self.data_dir)) is None:  # pragma: no branch
+                        credentials = LogfireCredentials.initialize_project(
+                            logfire_api_url=self.base_url,
+                            project_name=self.project_name,
+                            session=self.logfire_api_session,
+                        )
+                        credentials.write_creds_file(self.data_dir)
+                    self.token = credentials.token
+                    self.project_name = credentials.project_name
+                    self.base_url = self.base_url or credentials.logfire_api_url
+                else:
+                    credentials = self._initialize_credentials_from_token(self.token)
+                    if credentials is not None:
+                        self.project_name = credentials.project_name
+
+                if self.show_summary and credentials is not None:  # pragma: no cover
+                    credentials.print_token_summary()
 
                 headers = {'User-Agent': f'logfire/{VERSION}', 'Authorization': self.token}
-                # NOTE: Only check the backend if we didn't call it already.
-                if new_credentials is None:
-                    self.logfire_api_session.headers.update(headers)
-                    self.check_logfire_backend()
+                self.logfire_api_session.headers.update(headers)
 
                 session = OTLPExporterHttpSession(max_body_size=OTLP_MAX_BODY_SIZE)
                 session.headers.update(headers)
                 otel_traces_exporter_env = os.getenv(OTEL_TRACES_EXPORTER)
                 otel_traces_exporter_env = otel_traces_exporter_env.lower() if otel_traces_exporter_env else None
                 if otel_traces_exporter_env is None or otel_traces_exporter_env == 'otlp':
                     span_exporter = OTLPSpanExporter(endpoint=self.traces_endpoint, session=session)
@@ -673,17 +659,14 @@
                         )
                     ]
 
             tracer_provider.add_span_processor(PendingSpanProcessor(self.id_generator, tuple(processors)))
 
             metric_readers = metric_readers or []
 
-            if self.show_summary and credentials_from_local_file:  # pragma: no cover
-                credentials_from_local_file.print_token_summary()
-
             meter_provider = MeterProvider(metric_readers=metric_readers, resource=resource)
             if self.collect_system_metrics:
                 configure_metrics(meter_provider)
 
             # we need to shut down any existing providers to avoid leaking resources (like threads)
             # but if this takes longer than 100ms you should call `logfire.shutdown` before reconfiguring
             self._meter_provider.shutdown(
@@ -734,36 +717,50 @@
         This is used internally and should not be called by users of the SDK.
 
         Returns:
             The meter.
         """
         return self.get_meter_provider().get_meter('logfire', VERSION)
 
-    def check_logfire_backend(self) -> None:
+    def _initialize_credentials_from_token(self, token: str) -> LogfireCredentials | None:
         """Check that the token is valid.
 
         Issue a warning if the Logfire API is unreachable, or we get a response other than 200 or 401.
 
         We continue unless we get a 401 and allow OTel to take of storing data locally for back-fill.
 
         Raises:
             LogfireConfigError: If the token is invalid.
         """
         try:
-            response = self.logfire_api_session.get(urljoin(self.base_url, '/v1/health'), timeout=10)
+            response = self.logfire_api_session.get(
+                urljoin(self.base_url, '/v1/info'),
+                timeout=10,
+                headers={**COMMON_REQUEST_HEADERS, 'Authorization': token},
+            )
         except requests.RequestException as e:
             warnings.warn(f'Logfire API is unreachable, you may have trouble sending data. Error: {e}')
-        else:
-            if response.status_code == 401:
-                raise LogfireConfigError('Invalid Logfire token.')
-            elif response.status_code != 200:
-                # any other status code is considered unhealthy
-                warnings.warn(
-                    f'Logfire API is unhealthy, you may have trouble sending data. Status code: {response.status_code}'
-                )
+            return None
+
+        if response.status_code == 401:
+            raise LogfireConfigError('Invalid Logfire token.')
+        elif response.status_code != 200:
+            # any other status code is considered unhealthy
+            warnings.warn(
+                f'Logfire API is unhealthy, you may have trouble sending data. Status code: {response.status_code}'
+            )
+            return None
+
+        data = response.json()
+        return LogfireCredentials(
+            token=token,
+            project_name=data['project_name'],
+            project_url=data['project_url'],
+            logfire_api_url=self.base_url,
+        )
 
 
 def _get_default_span_processor(exporter: SpanExporter) -> SpanProcessor:
     schedule_delay_millis = _get_int_from_env(OTEL_BSP_SCHEDULE_DELAY) or 500
     return BatchSpanProcessor(exporter, schedule_delay_millis=schedule_delay_millis)
 
 
@@ -822,14 +819,33 @@
         if DEFAULT_FILE.is_file():  # pragma: no branch
             data = cast(DefaultFile, read_toml_file(DEFAULT_FILE))
             if is_logged_in(data, logfire_api_url):  # pragma: no branch
                 return data['tokens'][logfire_api_url]['token']
         raise LogfireConfigError('You are not authenticated. Please run `logfire auth` to authenticate.')
 
     @classmethod
+    def get_current_user(cls, session: requests.Session, logfire_api_url: str) -> dict[str, Any] | None:
+        try:
+            user_token = cls._get_user_token(logfire_api_url=logfire_api_url)
+        except LogfireConfigError:
+            return None
+        return cls._get_user_for_token(user_token, session, logfire_api_url)
+
+    @classmethod
+    def _get_user_for_token(cls, user_token: str, session: requests.Session, logfire_api_url: str) -> dict[str, Any]:
+        headers = {**COMMON_REQUEST_HEADERS, 'Authorization': user_token}
+        account_info_url = urljoin(logfire_api_url, '/v1/account/me')
+        try:
+            response = session.get(account_info_url, headers=headers)
+            UnexpectedResponse.raise_for_status(response)
+        except requests.RequestException as e:
+            raise LogfireConfigError('Error retrieving user information.') from e
+        return response.json()
+
+    @classmethod
     def get_user_projects(cls, session: requests.Session, logfire_api_url: str) -> list[dict[str, Any]]:
         """Get list of projects that user has access to them.
 
         Args:
             session: HTTP client session used to communicate with the Logfire API.
             logfire_api_url: The Logfire API base URL.
 
@@ -950,22 +966,17 @@
         except requests.RequestException as e:
             raise LogfireConfigError('Error retrieving list of organizations.') from e
         organizations = [item['organization_name'] for item in response.json()]
 
         if organization not in organizations:
             if len(organizations) > 1:
                 # Get user default organization
-                account_info_url = urljoin(logfire_api_url, '/v1/account/me')
-                try:
-                    response = session.get(account_info_url, headers=headers)
-                    UnexpectedResponse.raise_for_status(response)
-                except requests.RequestException as e:
-                    raise LogfireConfigError('Error retrieving user information.') from e
-                json_response = response.json()
-                user_default_organization_name = json_response.get('default_organization', {}).get('organization_name')
+                user_details = cls._get_user_for_token(user_token, session, logfire_api_url)
+                assert user_details is not None
+                user_default_organization_name = user_details.get('default_organization', {}).get('organization_name')
 
                 if default_organization and user_default_organization_name:
                     organization = user_default_organization_name
                 else:
                     organization = Prompt.ask(
                         '\nTo create and use a new project, please provide the following information:\n'
                         'Select the organization to create the project in',
@@ -1074,50 +1085,14 @@
                 f'Project initialized successfully. You will be able to view it at: {result.project_url}\n'
                 'Press Enter to continue'
             )
             return result
         except TypeError as e:  # pragma: no cover
             raise LogfireConfigError(f'Invalid credentials, when initializing project: {e}') from e
 
-    @classmethod
-    def create_anonymous_project(
-        cls,
-        *,
-        logfire_api_url: str,
-        requested_project_name: str,
-        session: requests.Session,
-    ) -> Self:  # pragma: no cover
-        """Create a new project on logfire.dev requesting the given project name.
-
-        Args:
-            logfire_api_url: The Logfire API base URL.
-            requested_project_name: Name to request for the project, the actual returned name may include a random
-                suffix to make it unique.
-            session: HTTP client session used to communicate with the Logfire API.
-
-        Returns:
-            The new credentials.
-
-        Raises:
-            LogfireConfigError: If there was an error creating the new project.
-        """
-        url = urljoin(logfire_api_url, '/v1/projects/')
-        try:
-            params = {'requested_project_name': requested_project_name}
-            response = session.post(url, params=params, headers=COMMON_REQUEST_HEADERS)
-            UnexpectedResponse.raise_for_status(response)
-        except requests.RequestException as e:
-            raise LogfireConfigError('Error creating new project.') from e
-        else:
-            json_data = response.json()
-            try:
-                return cls(**json_data, logfire_api_url=logfire_api_url)
-            except TypeError as e:
-                raise LogfireConfigError(f'Invalid credentials, when creating project at {url}: {e}') from e
-
     def write_creds_file(self, creds_dir: Path) -> None:
         """Write a credentials file to the given path."""
         ensure_data_dir_exists(creds_dir)
         data = dataclasses.asdict(self)
         path = _get_creds_file(creds_dir)
         path.write_text(json.dumps(data, indent=2) + '\n')
```

### Comparing `logfire-0.24.0/logfire/_internal/config_params.py` & `logfire-0.25.0/logfire/_internal/config_params.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/constants.py` & `logfire-0.25.0/logfire/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/exporters/console.py` & `logfire-0.25.0/logfire/_internal/exporters/console.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/exporters/fallback.py` & `logfire-0.25.0/logfire/_internal/exporters/fallback.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/exporters/file.py` & `logfire-0.25.0/logfire/_internal/exporters/file.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/exporters/otlp.py` & `logfire-0.25.0/logfire/_internal/exporters/otlp.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/exporters/processor_wrapper.py` & `logfire-0.25.0/logfire/_internal/exporters/processor_wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
 
-from urllib.parse import urlparse
+from urllib.parse import parse_qs, urlparse
 
 from opentelemetry import context
 from opentelemetry.sdk.trace import ReadableSpan, Span, SpanProcessor
 from opentelemetry.semconv.trace import SpanAttributes
 
 from ..constants import (
     ATTRIBUTES_MESSAGE_KEY,
     ATTRIBUTES_MESSAGE_TEMPLATE_KEY,
     ATTRIBUTES_SPAN_TYPE_KEY,
     PENDING_SPAN_NAME_SUFFIX,
     log_level_attributes,
 )
 from ..scrubbing import Scrubber
-from ..utils import ReadableSpanDict, span_to_dict
+from ..utils import ReadableSpanDict, span_to_dict, truncate_string
 
 
 class SpanProcessorWrapper(SpanProcessor):
     """Wrapper around other processors to intercept starting and ending spans with our own global logic.
 
     Suppresses starting/ending if the current context has a `suppress_instrumentation` value.
     Tweaks the send/receive span names generated by the ASGI middleware.
@@ -171,8 +171,33 @@
     # Minor optimization: only do this if there's a change.
     if names and (new_name := names[-1]) != name:
         if is_pending:
             new_name += PENDING_SPAN_NAME_SUFFIX
         span['name'] = new_name
 
     if messages and (message := messages[-1]) != name:
+        # Add query params to the message if:
+        # 1. The message currently ends with the target
+        # 2. We have a URL to parse query params from
+        # 3. Some query params exist
+        # 4. The target doesn't already end with the query string
+        #       (it's supposed to according to the spec, but the OTEL libraries don't include it)
+        if (
+            url and target and isinstance(url, str) and isinstance(target, str) and message.endswith(target)
+        ):  # pragma: no branch
+            query_string = urlparse(url).query
+            query_params = parse_qs(query_string)
+            if query_params and not target.endswith(query_string):
+                pairs = [(k, v) for k, vs in query_params.items() for v in vs]
+                # Put shorter query params first so that they'll be visible in the UI even if the whole message isn't.
+                pairs.sort(key=lambda pair: (len(pair[0]) + len(pair[1]), pair))
+                # Limit keys and values to 20 chars each.
+                truncated_pairs = [[truncate_string(s, max_length=20, middle='…') for s in pair] for pair in pairs]
+                # Show
+                #   /path?foo=1&bar=2%203
+                # as:
+                #   /path ? foo='1' & bar='2 3'
+                # to make things nice and readable.
+                # Note that we show decoded values, e.g. %20 -> ' '.
+                message += ' ? ' + ' & '.join(f'{k}={v!r}' for k, v in truncated_pairs)
+
         span['attributes'] = {**attributes, ATTRIBUTES_MESSAGE_KEY: message}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `logfire-0.24.0/logfire/_internal/exporters/remove_pending.py` & `logfire-0.25.0/logfire/_internal/exporters/remove_pending.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/exporters/wrapper.py` & `logfire-0.25.0/logfire/_internal/exporters/wrapper.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/formatter.py` & `logfire-0.25.0/logfire/_internal/formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/instrument.py` & `logfire-0.25.0/logfire/_internal/instrument.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/integrations/executors.py` & `logfire-0.25.0/logfire/_internal/integrations/executors.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/integrations/fastapi.py` & `logfire-0.25.0/logfire/_internal/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/json_encoder.py` & `logfire-0.25.0/logfire/_internal/json_encoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,17 +38,17 @@
 
 def _bytearray_encoder(o: bytearray) -> str:
     return _bytes_encoder(bytes(o))
 
 
 def _set_encoder(o: set[Any]) -> JsonValue:
     try:
-        return to_json_value(sorted(o))
+        return [to_json_value(item) for item in sorted(o)]
     except TypeError:
-        return to_json_value(list(o))
+        return [to_json_value(item) for item in o]
 
 
 def _to_isoformat(o: Any) -> str:
     return o.isoformat()
 
 
 def _pandas_data_frame_encoder(o: Any) -> JsonValue:
@@ -215,14 +215,17 @@
     return lookup
 
 
 def to_json_value(o: Any) -> JsonValue:
     try:
         if isinstance(o, (int, float, str, bool, type(None))):
             return o
+        if isinstance(o, (list, tuple)):
+            # we do list & tuple before Mapping as it's > twice as fast and just as common
+            return [to_json_value(item) for item in o]  # type: ignore
         elif isinstance(o, Mapping):
             return {key if isinstance(key, str) else safe_repr(key): to_json_value(value) for key, value in o.items()}  # type: ignore
         elif dataclasses.is_dataclass(o):
             return {f.name: to_json_value(getattr(o, f.name)) for f in dataclasses.fields(o)}
         elif is_attrs(o):
             return _get_attrs_data(o)
         elif is_sqlalchemy(o):
@@ -243,15 +246,20 @@
         pass
 
     # In case we don't know how to encode, use `repr()`.
     return safe_repr(o)
 
 
 def logfire_json_dumps(obj: Any) -> str:
-    return json.dumps(to_json_value(obj), separators=(',', ':'))
+    try:
+        return json.dumps(obj, default=to_json_value, separators=(',', ':'))
+    except TypeError:
+        # fallback to eagerly calling to_json_value to take care of object keys which are not strings
+        # see https://github.com/pydantic/platform/pull/2045
+        return json.dumps(to_json_value(obj), separators=(',', ':'))
 
 
 def is_sqlalchemy(obj: Any) -> bool:
     try:
         from sqlalchemy.orm import DeclarativeBase, DeclarativeMeta
 
         if isinstance(obj, DeclarativeBase):
```

### Comparing `logfire-0.24.0/logfire/_internal/json_formatter.py` & `logfire-0.25.0/logfire/_internal/json_formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/json_schema.py` & `logfire-0.25.0/logfire/_internal/json_schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,19 +42,14 @@
         bytearray: _bytearray_schema,
         Enum: _enum_schema,
         Decimal: {'type': 'string', 'format': 'decimal'},
         datetime.datetime: {'type': 'string', 'format': 'date-time'},
         datetime.date: {'type': 'string', 'format': 'date'},
         datetime.time: {'type': 'string', 'format': 'time'},
         datetime.timedelta: {'type': 'string', 'x-python-datatype': 'timedelta'},
-        list: _array_schema,
-        tuple: _array_schema,
-        set: _array_schema,
-        frozenset: _array_schema,
-        deque: _array_schema,
         GeneratorType: _generator_schema,
         IPv4Address: {'type': 'string', 'format': 'ipv4'},
         IPv6Address: {'type': 'string', 'format': 'ipv6'},
         IPv4Interface: {'type': 'string', 'format': 'ipv4interface'},
         IPv6Interface: {'type': 'string', 'format': 'ipv6interface'},
         IPv4Network: {'type': 'string', 'format': 'ipv4network'},
         IPv6Network: {'type': 'string', 'format': 'ipv6network'},
@@ -101,38 +96,46 @@
 
     Args:
         obj: The object to create the JSON Schema from.
 
     Returns:
         The JSON Schema.
     """
-    if dataclasses.is_dataclass(obj):
-        return _dataclass_schema(obj)
+    if obj is None:
+        return {}
+    # cover common types first before calling `type_to_schema` to avoid the overhead of imports if not necessary
+    obj_type = obj.__class__
+    if obj_type in {str, int, bool, float}:
+        return {}
+    elif obj_type in {list, tuple, set, frozenset, deque}:
+        return _array_schema(obj)
     elif isinstance(obj, Mapping):
         return _mapping_schema(obj)
+    elif dataclasses.is_dataclass(obj):
+        return _dataclass_schema(obj)
     elif is_attrs(obj):
         return _attrs_schema(obj)
     elif is_sqlalchemy(obj):
         return _sqlalchemy_schema(obj)
 
     global _type_to_schema
     _type_to_schema = _type_to_schema or type_to_schema()
-    for base in obj.__class__.__mro__[:-1]:
+    for base in obj_type.__mro__[:-1]:
         try:
             schema = _type_to_schema[base]
         except KeyError:
             continue
         else:
             return schema(obj) if callable(schema) else schema
 
-    if obj is None or isinstance(obj, (str, int, bool, float)):
+    # cover subclasses of common types, can't come earlier due to conflicts with IntEnum and StrEnum
+    if isinstance(obj, (str, int, float)):
         return {}
-    elif isinstance(obj, Sequence) and not isinstance(obj, str):
-        name = obj.__class__.__name__  # type: ignore[reportUnknownMemberType]
-        return {'type': 'array', 'title': name, 'x-python-datatype': 'Sequence'}
+    elif isinstance(obj, Sequence):
+        return {'type': 'array', 'title': obj_type.__name__, 'x-python-datatype': 'Sequence'}
 
     return {'type': 'object', 'x-python-datatype': 'unknown'}
 
 
 JsonSchemaProperties = NewType('JsonSchemaProperties', JsonDict)
```

### Comparing `logfire-0.24.0/logfire/_internal/json_types.py` & `logfire-0.25.0/logfire/_internal/json_types.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/main.py` & `logfire-0.25.0/logfire/_internal/main.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/metrics.py` & `logfire-0.25.0/logfire/_internal/metrics.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/scrubbing.py` & `logfire-0.25.0/logfire/_internal/scrubbing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/stack_info.py` & `logfire-0.25.0/logfire/_internal/stack_info.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/tracer.py` & `logfire-0.25.0/logfire/_internal/tracer.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/_internal/utils.py` & `logfire-0.25.0/logfire/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/integrations/logging.py` & `logfire-0.25.0/logfire/integrations/logging.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/integrations/loguru.py` & `logfire-0.25.0/logfire/integrations/loguru.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/integrations/pydantic.py` & `logfire-0.25.0/logfire/integrations/pydantic.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/integrations/structlog.py` & `logfire-0.25.0/logfire/integrations/structlog.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/propagate.py` & `logfire-0.25.0/logfire/propagate.py`

 * *Files identical despite different names*

### Comparing `logfire-0.24.0/logfire/testing.py` & `logfire-0.25.0/logfire/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,18 +158,18 @@
         self,
         fixed_line_number: int | None = 123,
         strip_filepaths: bool = True,
         include_resources: bool = False,
         include_package_versions: bool = False,
         _include_pending_spans: bool = False,
         _strip_function_qualname: bool = True,
-    ):
+    ) -> list[ReadableSpanModel]:
         """Same as exported_spans_as_dict but converts the dicts to pydantic models.
 
-        This allows using the result in exporters that expect ReadableSpans, not dicts.
+        This allows using the result in exporters that expect `ReadableSpan`s, not dicts.
         """
         return [
             ReadableSpanModel(**span)
             for span in self.exported_spans_as_dict(
                 fixed_line_number=fixed_line_number,
                 strip_filepaths=strip_filepaths,
                 include_resources=include_resources,
```

### Comparing `logfire-0.24.0/pyproject.toml` & `logfire-0.25.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # TODO revert this file to hatchling using https://github.com/pydantic/platform/pull/264/commits/01e4d2258776f98284d019d5040eceeb5e9af42f
 # when we move it to a new repo
 
 [tool.poetry]
 name = "logfire"
-version = "0.24.0"
+version = "0.25.0"
 description = "Coming soon..."
 authors = [
     "Pydantic Team <engineering@pydantic.dev>",
     "Samuel Colvin <samuel@pydantic.dev>",
     "Hasan Ramezani <hasan@pydantic.dev>",
     "Adrian Garcia Badaracco <adrian@pydantic.dev>",
     "David Montague <david@pydantic.dev>",
```

### Comparing `logfire-0.24.0/PKG-INFO` & `logfire-0.25.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logfire
-Version: 0.24.0
+Version: 0.25.0
 Summary: Coming soon...
 License: MIT
 Author: Pydantic Team
 Author-email: engineering@pydantic.dev
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

