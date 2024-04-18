# Comparing `tmp/pytest_hot_reloading-0.1.0a8.tar.gz` & `tmp/pytest_hot_reloading-0.1.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_hot_reloading-0.1.0a8.tar", max compression
+gzip compressed data, was "pytest_hot_reloading-0.1.0a9.tar", max compression
```

## Comparing `pytest_hot_reloading-0.1.0a8.tar` & `pytest_hot_reloading-0.1.0a9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2023-06-23 00:51:16.873262 pytest_hot_reloading-0.1.0a8/LICENSE
--rw-r--r--   0        0        0     5736 2023-06-23 00:51:16.873262 pytest_hot_reloading-0.1.0a8/README.md
--rw-r--r--   0        0        0     1037 2023-06-23 00:51:16.893262 pytest_hot_reloading-0.1.0a8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-23 00:51:16.893262 pytest_hot_reloading-0.1.0a8/pytest_hot_reloading/__init__.py
--rw-r--r--   0        0        0     2450 2023-06-23 00:51:16.893262 pytest_hot_reloading-0.1.0a8/pytest_hot_reloading/client.py
--rw-r--r--   0        0        0    10754 2023-06-23 00:51:16.893262 pytest_hot_reloading-0.1.0a8/pytest_hot_reloading/daemon.py
--rw-r--r--   0        0        0     9705 2023-06-23 00:51:16.893262 pytest_hot_reloading-0.1.0a8/pytest_hot_reloading/plugin.py
--rw-r--r--   0        0        0        1 2023-06-23 00:51:16.893262 pytest_hot_reloading-0.1.0a8/pytest_hot_reloading/py.typed
--rw-r--r--   0        0        0     2305 2023-06-23 00:51:16.893262 pytest_hot_reloading-0.1.0a8/pytest_hot_reloading/workarounds.py
--rw-r--r--   0        0        0     6234 1970-01-01 00:00:00.000000 pytest_hot_reloading-0.1.0a8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-11-30 03:42:44.812736 pytest_hot_reloading-0.1.0a9/LICENSE
+-rw-r--r--   0        0        0     6867 2023-11-30 03:42:44.812736 pytest_hot_reloading-0.1.0a9/README.md
+-rw-r--r--   0        0        0     1067 2023-11-30 03:42:44.828736 pytest_hot_reloading-0.1.0a9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-11-30 03:42:44.828736 pytest_hot_reloading-0.1.0a9/pytest_hot_reloading/__init__.py
+-rw-r--r--   0        0        0     3091 2023-11-30 03:42:44.832736 pytest_hot_reloading-0.1.0a9/pytest_hot_reloading/client.py
+-rw-r--r--   0        0        0    11288 2023-11-30 03:42:44.832736 pytest_hot_reloading-0.1.0a9/pytest_hot_reloading/daemon.py
+-rw-r--r--   0        0        0     9663 2023-11-30 03:42:44.832736 pytest_hot_reloading-0.1.0a9/pytest_hot_reloading/plugin.py
+-rw-r--r--   0        0        0        1 2023-11-30 03:42:44.832736 pytest_hot_reloading-0.1.0a9/pytest_hot_reloading/py.typed
+-rw-r--r--   0        0        0     2305 2023-11-30 03:42:44.832736 pytest_hot_reloading-0.1.0a9/pytest_hot_reloading/workarounds.py
+-rw-r--r--   0        0        0     7459 1970-01-01 00:00:00.000000 pytest_hot_reloading-0.1.0a9/PKG-INFO
```

### Comparing `pytest_hot_reloading-0.1.0a8/LICENSE` & `pytest_hot_reloading-0.1.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_hot_reloading-0.1.0a8/README.md` & `pytest_hot_reloading-0.1.0a9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ![versions](https://img.shields.io/pypi/pyversions/pytest-hot-reloading)
 
 A hot reloading pytest daemon, implemented as a plugin.
 
 ## Features
 - Uses the [jurigged](https://github.com/breuleux/jurigged) library to watch and hot reload files
 - Caches test discovery in many situations
-- Improved performance by not having to import libraries again and again and skipping initializtion logic
+- Improved performance by not having to import libraries again and again and skipping initialization logic
 - System for registering workarounds in case something doesn't work out of the box
 
 ## Trade-offs
 - First run is slower
 - May not work with some libraries
 - Sometimes gets in a bad state and needs to be restarted
 
@@ -44,25 +44,32 @@
 
 Example using pyproject.toml:
 ```toml
 [tool.pytest.ini_options]
 addopts = "-p pytest_hot_reloading.plugin"
 ```
 
-When running pytest, the plugin will detect whether the daemon is running, and start it if is not.
+When running pytest, the plugin will detect whether the daemon is running.
+If the daemon is not running, it will error unless the `--daemon-start-if-needed` argument is passed.
+
+The current version of the VS Code Python extension is not, by default, compatible with automatically starting the daemon. The
+test runner will hang. However, you can revert to legacy behavior which will allow for using the automatic starting. 
+See the VS Code section below for more information.
+
 Note that a pid file is created to track the pid.
 
 Imports and in many cases initialization logic are not reran on subsequent runs, which can be a huge time saver.
 
 Currently, if you want to debug, you will want to run the daemon manually with debugging.
 
 ### JetBrains (IDEA, PyCharm, etc)
 
 Create a REGULAR Python run configuration, with pytest as the *module*. For parameters, add `--daemon`. Strongly consider storing
-in the project so it is shared with other developers.
+in the project so it is shared with other developers. Note that you most likely also need to set the working directory to the
+project root where the pytest configuration is located so that it knows to use the plugin you configured earlier.
 
 ![JetBrains Example](docs/jetbrains-hot-reloading-example.png)
 
 For more information on parameters, see the VS Code section below.
 
 ### VS Code
 
@@ -98,31 +105,52 @@
 
 If the daemon is already running and you run pytest with `--daemon`, then the old one will be stopped
 and a new one will be started. Note that `pytest --daemon` is NOT how you run tests. It is only used to start
 the daemon.
 
 The daemon can be stopped with `pytest --stop-daemon`. This can be used if it gets into a bad state.
 
+To enable automatically starting the server, you have to, currently, disable the new Python Test Adapter:
+
+In your devcontainer.json or user settings:
+```json
+"python.experiments.optOutFrom": [
+    "pythonTestAdapter"
+],
+```
+
+Then enable automatically starting the daemon in your settings:
+```json
+"python.testing.pytestArgs": [
+    "--daemon-start-if-needed",
+    "tests"
+],
+```
+
 ## Arguments and Env Variables
 - `PYTEST_DAEMON_PORT`
     - The port the daemon listens on.
     - Default: `4852`.
     - Command line: `--daemon-port`
 - `PYTEST_DAEMON_PYTEST_NAME`
-    - The name of the pytest executable.
+    - The name of the pytest executable. Used for spawning the daemon.
     - Default: `pytest`.
     - Command line: `--pytest-name`
 - `PYTEST_DAEMON_WATCH_GLOBS`
     - The colon separated globs to watch.
     - Default: `./**/*.py`.
     - Command line: `--daemon-watch-globs`
 - `PYTEST_DAEMON_IGNORE_WATCH_GLOBS`
     - The colon separated globs to ignore.
     - Default: `./.venv/*`.
     - Command line: `--daemon-ignore-watch-globs`
+- `PYTEST_DAEMON_START_IF_NEEDED`
+    - Start the pytest daemon if it is not running.
+    - Default: `False`
+    - Command line: `--daemon-start-if-needed`
 
 ## Workarounds
 Libraries that use mutated globals may need a workaround to work with this plugin. The preferred
 route is to have the library update its code to not mutate globals in a test environment, or to
 restore them after a test suite has ran. In some cases, that isn't possible, usually because
 the person with the problem doesn't own the library and can't wait around for a fix.
```

### Comparing `pytest_hot_reloading-0.1.0a8/pyproject.toml` & `pytest_hot_reloading-0.1.0a9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 [tool.ruff]
-line-length = 120
+line-length = 98
+
+[tool.ruff.lint.pycodestyle]
+max-line-length = 120
 
 [tool.black]
 line-length = 98
 
 [tool.poetry]
 name = "pytest-hot-reloading"
-version = "0.1.0-alpha.8"
+version = "0.1.0-alpha.9"
 description = ""
 authors = ["James Hutchison <jamesghutchison@proton.me>"]
 readme = "README.md"
 packages = [{ include = "pytest_hot_reloading" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 jurigged = "^0.5.5"
 cachetools = "^5.3.0"
 types-cachetools = "^5.3.0.5"
+megamock = "^0.1.0b9"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.2.0"
-ruff = "^0.0.261"
-black = "^23.3.0"
+ruff = "^0.1.6"
 pytest = "^7.2.2"
-megamock = "^0.1.0b6"
 pytest-django = "^4.5.2"
-django = "^4.2.2"
+django = "4.2.2"
 psycopg2-binary = "^2.9.6"
 pytest-env = "^0.8.1"
 pytest-xdist = "^3.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pytest_hot_reloading-0.1.0a8/pytest_hot_reloading/client.py` & `pytest_hot_reloading-0.1.0a9/pytest_hot_reloading/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,58 @@
+import json
+import os
 import socket
 import sys
 import time
 import xmlrpc.client
+from pathlib import Path
 from typing import cast
 
 
 class PytestClient:
     _socket: socket.socket | None
     _daemon_host: str
     _daemon_port: int
     _pytest_name: str
+    _will_start_daemon_if_needed: bool
 
     def __init__(
-        self, daemon_host: str = "localhost", daemon_port: int = 4852, pytest_name: str = "pytest"
+        self,
+        daemon_host: str = "localhost",
+        daemon_port: int = 4852,
+        pytest_name: str = "pytest",
+        start_daemon_if_needed: bool = False,
     ) -> None:
         self._socket = None
         self._daemon_host = daemon_host
         self._daemon_port = daemon_port
         self._pytest_name = pytest_name
+        self._will_start_daemon_if_needed = start_daemon_if_needed
 
     def _get_server(self) -> xmlrpc.client.ServerProxy:
         server_url = f"http://{self._daemon_host}:{self._daemon_port}"
         server = xmlrpc.client.ServerProxy(server_url)
 
         return server
 
-    def run(self, cwd: str, args: list[str]) -> int:
-        self._start_daemon_if_needed()
+    def run(self, cwd: Path, args: list[str]) -> int:
+        if self._will_start_daemon_if_needed:
+            self._start_daemon_if_needed()
+        elif not self._daemon_running():
+            raise Exception(
+                "Daemon is not running and must be started, or add --daemon-start-if-needed"
+            )
 
         server = self._get_server()
 
+        env = os.environ.copy()
+        sys_path = sys.path
+
         start = time.time()
-        result: dict = cast(dict, server.run_pytest(cwd, args))
+        result: dict = cast(dict, server.run_pytest(str(cwd), json.dumps(env), sys_path, args))
         print(f"Daemon took {(time.time() - start):.3f} seconds to reply")
 
         stdout = result["stdout"].data.decode("utf-8")
         stderr = result["stderr"].data.decode("utf-8")
 
         print(stdout, file=sys.stdout)
         print(stderr, file=sys.stderr)
@@ -56,28 +73,31 @@
             print("Daemon stopped")
 
     def abort(self) -> None:
         # Close the socket
         if self._socket:
             self._socket.close()
 
-    def _start_daemon_if_needed(self) -> None:
-        # check if the daemon is running on the expected host and port
-        # if not, start the daemon
-
+    def _daemon_running(self) -> bool:
         # first, try to connect
         try:
             self._socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self._socket.connect((self._daemon_host, self._daemon_port))
             # the daemon is running
             # close the socket
             self._socket.close()
+            return True
         except ConnectionRefusedError:
             # the daemon is not running
-            # start the daemon
+            return False
+
+    def _start_daemon_if_needed(self) -> None:
+        # check if the daemon is running on the expected host and port
+        # if not, start the daemon
+        if not self._daemon_running():
             self._start_daemon()
 
     def _start_daemon(self) -> None:
         from pytest_hot_reloading.daemon import PytestDaemon
 
         # start the daemon
         PytestDaemon.start(
```

### Comparing `pytest_hot_reloading-0.1.0a8/pytest_hot_reloading/daemon.py` & `pytest_hot_reloading-0.1.0a9/pytest_hot_reloading/daemon.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import copy
+import json
 import os
 import re
 import socket
 import subprocess
 import sys
 import tempfile
 import time
@@ -69,15 +70,15 @@
 
         return {"shutdown": "ok"}
 
     @staticmethod
     def wait_to_be_ready(host: str = "localhost", port: int = 4852) -> None:
         # poll the connection to the daemon using sockets
         # and return when it is ready
-        for _ in range(100):
+        for _ in range(1000):
             try:
                 sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
                 sock.connect((host, port))
             except ConnectionRefusedError:
                 time.sleep(0.1)
                 continue
             else:
@@ -115,15 +116,15 @@
         try:
             with open(self.pid_file, "r") as f:
                 pid = int(f.read())
             os.kill(pid, 9)
         except FileNotFoundError:
             raise Exception(f"Port {self._daemon_port} is already in use")
 
-    def run_pytest(self, cwd: str, args: list[str]) -> dict:
+    def run_pytest(self, cwd: str, env_json: str, sys_path: list[str], args: list[str]) -> dict:
         # run pytest using command line args
         # run the pytest main logic
 
         in_progress_workarounds = self._workaround_library_issues_pre()
 
         import pytest_hot_reloading.plugin as plugin
 
@@ -148,23 +149,41 @@
 
         # monkeypatch in the main that does test collection caching
         orig_main = _pytest.main._main
         _pytest.main._main = _pytest_main
 
         # store current working directory
         prev_cwd = os.getcwd()
+        # switch to client working directory
         os.chdir(cwd)
 
+        # copy the environment
+        env_old = os.environ.copy()
+        # switch to client environment
+        new_env = json.loads(env_json)
+        os.environ.update(new_env)
+
+        # copy sys.path
+        sys_path_old = sys.path
+        # switch to client path
+        sys.path = sys_path
+
         try:
             # args must omit the calling program
             status_code = pytest.main(["--color=yes"] + args)
         finally:
             os.chdir(prev_cwd)
             self._workaround_library_issues_post(in_progress_workarounds)
 
+            # restore sys.path
+            sys.path = sys_path_old
+
+            # restore environment
+            os.environ.update(env_old)
+
             # restore originals
             _pytest.main._main = orig_main
 
             sys.stdout = stdout_bak
             sys.stderr = stderr_bak
 
             stdout.seek(0)
```

### Comparing `pytest_hot_reloading-0.1.0a8/pytest_hot_reloading/plugin.py` & `pytest_hot_reloading-0.1.0a9/pytest_hot_reloading/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         default=int(os.getenv("PYTEST_DAEMON_PORT", "4852")),
         help="The port to use for the daemon. You generally shouldn't need to set this.",
     )
     group.addoption(
         "--pytest-name",
         action="store",
         default=os.getenv("PYTEST_DAEMON_PYTEST_NAME", "pytest"),
-        help="The name of the pytest executable or module",
+        help="The name of the pytest executable or module. This is used for starting the daemon.",
     )
     group.addoption(
         "--daemon-timeout",
         action="store",
         default=os.getenv("PYTEST_DAEMON_TIMEOUT", (5 * 60)),
         help="The timeout in seconds to wait on a test suite to finish. This is not yet implemented.",
     )
@@ -59,14 +59,23 @@
     )
     group.addoption(
         "--stop-daemon",
         action="store_true",
         default=False,
         help="Stop the daemon",
     )
+    group.addoption(
+        "--daemon-start-if-needed",
+        action="store_true",
+        default=os.getenv("PYTEST_DAEMON_START_IF_NEEDED", "False").lower() in ("true", "1"),
+        help=(
+            "Start the daemon if it is not running. To use this with VS Code, "
+            'you need add "python.experiments.optOutFrom": ["pythonTestAdapter"] to your config.'
+        ),
+    )
 
 
 # list of pytest hooks
 # https://docs.pytest.org/en/stable/reference.html#_pytest.hookspec.pytest_addhooks
 
 
 def pytest_cmdline_main(config: Config) -> Optional[int]:
@@ -74,14 +83,16 @@
     This hook is called by pytest and is one of the first hooks.
     """
     # early escapes
     if config.option.collectonly:
         return None
     if i_am_server:
         return None
+    if config.option.help:
+        return None
     status_code = _plugin_logic(config)
     # dont do any more work. Don't let pytest continue
     return status_code  # status code 0
 
 
 def monkey_patch_jurigged_function_definition():
     import jurigged.codetools as jurigged_codetools  # type: ignore
@@ -177,41 +188,28 @@
 
         daemon = PytestDaemon(daemon_port=daemon_port)
 
         daemon.run_forever()
         sys.exit(0)
     else:
         pytest_name = config.option.pytest_name
-        client = PytestClient(daemon_port=daemon_port, pytest_name=pytest_name)
+        client = PytestClient(
+            daemon_port=daemon_port,
+            pytest_name=pytest_name,
+            start_daemon_if_needed=config.option.daemon_start_if_needed,
+        )
 
         if config.option.stop_daemon:
             client.stop()
             return 0
 
-        # find the index of the first value that is not None
-        for idx, val in enumerate(
-            [
-                x.endswith(pytest_name) or x.endswith(f"{pytest_name}/__main__.py")
-                for x in sys.argv
-            ]
-        ):
-            if val:
-                pytest_name_index = idx
-                break
-        else:
-            if "pytest_runner" in sys.argv[0]:
-                pytest_name_index = 0
-            else:
-                print(sys.argv)
-                raise Exception(
-                    "Could not find pytest name in args. "
-                    "Check the configured name versus the actual name."
-                )
-        cwd = os.getcwd()
-        status_code = client.run(cwd, sys.argv[pytest_name_index + 1 :])
+        cwd = config.invocation_params.dir
+        args = list(config.invocation_params.args)
+
+        status_code = client.run(cwd, args)
         return status_code
 
 
 def _get_pattern_filters(config: Config) -> str | Callable[[str], bool]:
     """
     Jurigged takes in a pattern argument. The argument is either a glob string
     or a function that returns True if the path passed into it should be watched.
```

### Comparing `pytest_hot_reloading-0.1.0a8/pytest_hot_reloading/workarounds.py` & `pytest_hot_reloading-0.1.0a9/pytest_hot_reloading/workarounds.py`

 * *Files identical despite different names*

### Comparing `pytest_hot_reloading-0.1.0a8/PKG-INFO` & `pytest_hot_reloading-0.1.0a9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: pytest-hot-reloading
-Version: 0.1.0a8
+Version: 0.1.0a9
 Summary: 
 Author: James Hutchison
 Author-email: jamesghutchison@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cachetools (>=5.3.0,<6.0.0)
 Requires-Dist: jurigged (>=0.5.5,<0.6.0)
+Requires-Dist: megamock (>=0.1.0b9,<0.2.0)
 Requires-Dist: types-cachetools (>=5.3.0.5,<6.0.0.0)
 Description-Content-Type: text/markdown
 
 # A PyTest Hot Reloading Plugin
 ![versions](https://img.shields.io/pypi/pyversions/pytest-hot-reloading)
 
 A hot reloading pytest daemon, implemented as a plugin.
 
 ## Features
 - Uses the [jurigged](https://github.com/breuleux/jurigged) library to watch and hot reload files
 - Caches test discovery in many situations
-- Improved performance by not having to import libraries again and again and skipping initializtion logic
+- Improved performance by not having to import libraries again and again and skipping initialization logic
 - System for registering workarounds in case something doesn't work out of the box
 
 ## Trade-offs
 - First run is slower
 - May not work with some libraries
 - Sometimes gets in a bad state and needs to be restarted
 
@@ -59,25 +61,32 @@
 
 Example using pyproject.toml:
 ```toml
 [tool.pytest.ini_options]
 addopts = "-p pytest_hot_reloading.plugin"
 ```
 
-When running pytest, the plugin will detect whether the daemon is running, and start it if is not.
+When running pytest, the plugin will detect whether the daemon is running.
+If the daemon is not running, it will error unless the `--daemon-start-if-needed` argument is passed.
+
+The current version of the VS Code Python extension is not, by default, compatible with automatically starting the daemon. The
+test runner will hang. However, you can revert to legacy behavior which will allow for using the automatic starting. 
+See the VS Code section below for more information.
+
 Note that a pid file is created to track the pid.
 
 Imports and in many cases initialization logic are not reran on subsequent runs, which can be a huge time saver.
 
 Currently, if you want to debug, you will want to run the daemon manually with debugging.
 
 ### JetBrains (IDEA, PyCharm, etc)
 
 Create a REGULAR Python run configuration, with pytest as the *module*. For parameters, add `--daemon`. Strongly consider storing
-in the project so it is shared with other developers.
+in the project so it is shared with other developers. Note that you most likely also need to set the working directory to the
+project root where the pytest configuration is located so that it knows to use the plugin you configured earlier.
 
 ![JetBrains Example](docs/jetbrains-hot-reloading-example.png)
 
 For more information on parameters, see the VS Code section below.
 
 ### VS Code
 
@@ -113,31 +122,52 @@
 
 If the daemon is already running and you run pytest with `--daemon`, then the old one will be stopped
 and a new one will be started. Note that `pytest --daemon` is NOT how you run tests. It is only used to start
 the daemon.
 
 The daemon can be stopped with `pytest --stop-daemon`. This can be used if it gets into a bad state.
 
+To enable automatically starting the server, you have to, currently, disable the new Python Test Adapter:
+
+In your devcontainer.json or user settings:
+```json
+"python.experiments.optOutFrom": [
+    "pythonTestAdapter"
+],
+```
+
+Then enable automatically starting the daemon in your settings:
+```json
+"python.testing.pytestArgs": [
+    "--daemon-start-if-needed",
+    "tests"
+],
+```
+
 ## Arguments and Env Variables
 - `PYTEST_DAEMON_PORT`
     - The port the daemon listens on.
     - Default: `4852`.
     - Command line: `--daemon-port`
 - `PYTEST_DAEMON_PYTEST_NAME`
-    - The name of the pytest executable.
+    - The name of the pytest executable. Used for spawning the daemon.
     - Default: `pytest`.
     - Command line: `--pytest-name`
 - `PYTEST_DAEMON_WATCH_GLOBS`
     - The colon separated globs to watch.
     - Default: `./**/*.py`.
     - Command line: `--daemon-watch-globs`
 - `PYTEST_DAEMON_IGNORE_WATCH_GLOBS`
     - The colon separated globs to ignore.
     - Default: `./.venv/*`.
     - Command line: `--daemon-ignore-watch-globs`
+- `PYTEST_DAEMON_START_IF_NEEDED`
+    - Start the pytest daemon if it is not running.
+    - Default: `False`
+    - Command line: `--daemon-start-if-needed`
 
 ## Workarounds
 Libraries that use mutated globals may need a workaround to work with this plugin. The preferred
 route is to have the library update its code to not mutate globals in a test environment, or to
 restore them after a test suite has ran. In some cases, that isn't possible, usually because
 the person with the problem doesn't own the library and can't wait around for a fix.
```

