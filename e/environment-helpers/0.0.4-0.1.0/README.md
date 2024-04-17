# Comparing `tmp/environment_helpers-0.0.4.tar.gz` & `tmp/environment_helpers-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "environment_helpers-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "environment_helpers-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `environment_helpers-0.0.4.tar` & `environment_helpers-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1078 2024-03-26 01:01:19.504125 environment_helpers-0.0.4/LICENSE
--rw-r--r--   0        0        0      195 2024-03-27 18:15:42.865584 environment_helpers-0.0.4/README.md
--rw-r--r--   0        0        0     3775 2024-03-28 20:09:35.259942 environment_helpers-0.0.4/environment_helpers/__init__.py
--rw-r--r--   0        0        0      348 2024-03-26 03:25:02.457553 environment_helpers-0.0.4/environment_helpers/_scripts/launcher-kind.py
--rw-r--r--   0        0        0      188 2024-03-26 01:03:58.624127 environment_helpers-0.0.4/environment_helpers/_scripts/scheme.py
--rw-r--r--   0        0        0     2033 2024-03-26 03:23:13.784219 environment_helpers-0.0.4/environment_helpers/_scripts/system-scheme.py
--rw-r--r--   0        0        0      197 2024-03-25 22:17:38.794017 environment_helpers-0.0.4/environment_helpers/_scripts/version.py
--rw-r--r--   0        0        0     2112 2024-03-28 17:29:08.173170 environment_helpers-0.0.4/environment_helpers/build.py
--rw-r--r--   0        0        0      989 2024-03-26 03:36:32.970894 environment_helpers-0.0.4/environment_helpers/install.py
--rw-r--r--   0        0        0     3639 2024-03-27 18:20:19.818920 environment_helpers-0.0.4/environment_helpers/introspect.py
--rw-r--r--   0        0        0     1780 2024-03-28 20:09:40.243276 environment_helpers-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 environment_helpers-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-03-26 01:01:19.504125 environment_helpers-0.1.0/LICENSE
+-rw-r--r--   0        0        0      195 2024-03-27 18:15:42.865584 environment_helpers-0.1.0/README.md
+-rw-r--r--   0        0        0     4020 2024-04-17 23:24:04.423141 environment_helpers-0.1.0/environment_helpers/__init__.py
+-rw-r--r--   0        0        0      408 2024-04-17 22:49:36.176876 environment_helpers-0.1.0/environment_helpers/_scripts/call.py
+-rw-r--r--   0        0        0      348 2024-03-26 03:25:02.457553 environment_helpers-0.1.0/environment_helpers/_scripts/launcher-kind.py
+-rw-r--r--   0        0        0      188 2024-03-26 01:03:58.624127 environment_helpers-0.1.0/environment_helpers/_scripts/scheme.py
+-rw-r--r--   0        0        0     2033 2024-03-26 03:23:13.784219 environment_helpers-0.1.0/environment_helpers/_scripts/system-scheme.py
+-rw-r--r--   0        0        0      197 2024-03-25 22:17:38.794017 environment_helpers-0.1.0/environment_helpers/_scripts/version.py
+-rw-r--r--   0        0        0     2112 2024-03-28 17:29:08.173170 environment_helpers-0.1.0/environment_helpers/build.py
+-rw-r--r--   0        0        0      989 2024-03-26 03:36:32.970894 environment_helpers-0.1.0/environment_helpers/install.py
+-rw-r--r--   0        0        0     5097 2024-04-17 23:22:58.890812 environment_helpers-0.1.0/environment_helpers/introspect.py
+-rw-r--r--   0        0        0     1780 2024-04-17 23:25:09.065445 environment_helpers-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 environment_helpers-0.1.0/PKG-INFO
```

### Comparing `environment_helpers-0.0.4/LICENSE` & `environment_helpers-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `environment_helpers-0.0.4/environment_helpers/__init__.py` & `environment_helpers-0.1.0/environment_helpers/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from typing import Any, Collection, Literal, Optional, Protocol
 
 import environment_helpers.build
 import environment_helpers.install
 import environment_helpers.introspect
 
 
-__version__ = '0.0.4'
+__version__ = '0.1.0'
 
 
 class Environment(Protocol):
     """Object representing a Python environment."""
 
     @property
     def base(self) -> pathlib.Path: ...
@@ -30,14 +30,19 @@
     @property
     def scripts(self) -> pathlib.Path: ...
 
     @property
     def scheme(self) -> environment_helpers.introspect.SchemeDict:
         """Default install scheme for the environment."""
 
+    @property
+    def introspectable(self) -> environment_helpers.introspect.Introspectable:
+        """Introspectable object for the environment."""
+        return environment_helpers.introspect.Introspectable(self.interpreter)
+
     def run_interpreter(self, *args: Sequence[str], **kwargs: Any) -> bytes:
         return subprocess.check_output([os.fspath(self.interpreter), *args], **kwargs)
 
     def run_script(self, name: str, *args: Sequence[str]) -> bytes:
         return subprocess.check_output([os.fspath(self.scripts / name), *args])
 
     def install_wheel(self, path: os.PathLike[str], scheme: Optional[str] = None) -> None:
@@ -86,16 +91,16 @@
 
         subprocess.check_call([*cmd, *requirements])
 
 
 class VirtualEnvironment(Environment):
     """Object representing a virtual environment (using the ``venv`` scheme)."""
 
-    def __init__(self, path: pathlib.Path) -> None:
-        self._base = path
+    def __init__(self, path: os.PathLike[str]) -> None:
+        self._base = os.fspath(path)
         self._scheme = environment_helpers.introspect.get_virtual_environment_scheme(path)
         assert self.interpreter.is_file()
 
     @property
     def base(self) -> pathlib.Path:
         return self._base
```

### Comparing `environment_helpers-0.0.4/environment_helpers/_scripts/system-scheme.py` & `environment_helpers-0.1.0/environment_helpers/_scripts/system-scheme.py`

 * *Files identical despite different names*

### Comparing `environment_helpers-0.0.4/environment_helpers/build.py` & `environment_helpers-0.1.0/environment_helpers/build.py`

 * *Files identical despite different names*

### Comparing `environment_helpers-0.0.4/environment_helpers/install.py` & `environment_helpers-0.1.0/environment_helpers/install.py`

 * *Files identical despite different names*

### Comparing `environment_helpers-0.0.4/environment_helpers/introspect.py` & `environment_helpers-0.1.0/environment_helpers/introspect.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import functools
 import json
 import os
+import pickle
 import subprocess
 import sys
 import sysconfig
 import warnings
 
-from typing import Any, Literal, NamedTuple, Optional, TypedDict
+from collections.abc import Sequence
+from typing import Any, Callable, Dict, Literal, NamedTuple, Optional, TypedDict, TypeVar
 
 
 if sys.version_info >= (3, 9):
     import importlib.resources as importlib_resources
 else:
     import importlib_resources
 
 
 LauncherKind = Literal['posix', 'win-ia32', 'win-amd64', 'win-arm', 'win-arm64']
 
+T = TypeVar('T')
+
 
 class SchemeDict(TypedDict):
     stdlib: str
     platstdlib: str
     purelib: str
     platlib: str
     include: str
@@ -33,26 +37,14 @@
     major: int
     minor: int
     micro: int
     releaselevel: str
     serial: int
 
 
-def _run_script(name: str, interpreter: os.PathLike[str], **kwargs: Any) -> Any:
-    script = importlib_resources.files('environment_helpers._scripts') / f'{name}.py'
-    with importlib_resources.as_file(script) as script_path:
-        data = subprocess.check_output([os.fspath(interpreter), os.fspath(script_path)])
-    return json.loads(data)
-
-
-def get_version(interpreter: os.PathLike[str]) -> PythonVersion:
-    data = _run_script('version', interpreter)
-    return PythonVersion(**data)
-
-
 def get_virtual_environment_scheme(path: os.PathLike[str]) -> SchemeDict:
     """Calculates the installation paths for the scheme used by a certain virtual environment.
 
     :param path: Path of the target virtual environment.
     """
     config_vars = sysconfig.get_config_vars().copy()
     config_vars['base'] = config_vars['platbase'] = os.fspath(path)
@@ -70,44 +62,84 @@
         warnings.warn(
             f"Unknown platform '{os.name}', using the default install scheme.", stacklevel=2
         )
         return sysconfig.get_paths(vars=config_vars)
     return sysconfig.get_paths(scheme=scheme, vars=config_vars)
 
 
-@functools.lru_cache
-def get_scheme(interpreter: os.PathLike[str], scheme: Optional[str] = None) -> SchemeDict:
-    """Finds the installation paths for a certain Python install scheme.
-
-    This helper needs to run the Python interpreter for the target environment.
-
-    :param interpreter: Path to the Python interpreter to introspect.
-    :param scheme: Name of the target scheme name. If None, it uses the default scheme.
-    """
-    return _run_script('scheme', interpreter)
-
-
-@functools.lru_cache
-def get_system_scheme(interpreter: os.PathLike[str]) -> SchemeDict:
-    """Finds the installation paths for the system Python install scheme.
-
-    Certain vendors, such as Debian, have a different scheme for system packages.
-    This function finds the install scheme for system packages.
-
-    This helper needs to run the Python interpreter for the target environment.
-
-    :param interpreter: Path to the Python interpreter to introspect.
-    """
-    # Fedora automatically changes the default scheme unless RPM_BUILD_ROOT is set
-    environment = os.environ.copy()
-    environment['RPM_BUILD_ROOT'] = None
-    return _run_script('system-scheme', interpreter, env=environment)
+class Introspectable:
+    def __init__(self, interpreter: os.PathLike[str]) -> None:
+        self._interpreter = interpreter
+
+    def _run_script(self, name: str, **kwargs: Any) -> Any:
+        script = importlib_resources.files('environment_helpers._scripts') / f'{name}.py'
+        with importlib_resources.as_file(script) as script_path:
+            data = subprocess.check_output(
+                [os.fspath(self._interpreter), os.fspath(script_path)], **kwargs
+            )
+        return json.loads(data)
+
+    def get_version(self, interpreter: os.PathLike[str]) -> PythonVersion:
+        data = self._run_script('version', interpreter)
+        return PythonVersion(**data)
+
+    @functools.lru_cache
+    def get_scheme(self, interpreter: os.PathLike[str], scheme: Optional[str] = None) -> SchemeDict:
+        """Finds the installation paths for a certain Python install scheme.
+
+        This helper needs to run the Python interpreter for the target environment.
+
+        :param interpreter: Path to the Python interpreter to introspect.
+        :param scheme: Name of the target scheme name. If None, it uses the default scheme.
+        """
+        return self._run_script('scheme', interpreter)
+
+    @functools.lru_cache
+    def get_system_scheme(self, interpreter: os.PathLike[str]) -> SchemeDict:
+        """Finds the installation paths for the system Python install scheme.
+
+        Certain vendors, such as Debian, have a different scheme for system packages.
+        This function finds the install scheme for system packages.
+
+        This helper needs to run the Python interpreter for the target environment.
+
+        :param interpreter: Path to the Python interpreter to introspect.
+        """
+        # Fedora automatically changes the default scheme unless RPM_BUILD_ROOT is set
+        environment = os.environ.copy()
+        environment['RPM_BUILD_ROOT'] = None
+        return self._run_script('system-scheme', interpreter, env=environment)
+
+    @functools.lru_cache
+    def get_launcher_kind(self, interpreter: os.PathLike[str]) -> Optional[LauncherKind]:
+        """Find the launcher kind.
+
+        This helper needs to run the Python interpreter for the target environment.
+
+        :param interpreter: Path to the Python interpreter to introspect.
+        """
+        return self._run_script('launcher-kind', interpreter)
+
+    def call(self, func: Callable[[Any], T], *args: Sequence[Any], **kwargs: Dict[str, Any]) -> T:
+        """Call the a function in the target environment.
+
+        :param interpreter: Path to the Python interpreter to introspect.
+        :param func: Function to call.
+        :param args: Positional arguments to pass to the function.
+        :param kwargs: Keyword arguments to pass to the function.
+        """
+        args_dict = {'args': args, 'kwargs': kwargs}
+        pickled_args_dict = pickle.dumps(args_dict)
+
+        script = importlib_resources.files('environment_helpers._scripts') / 'call.py'
+        with importlib_resources.as_file(script) as script_path:
+            data = subprocess.check_output(
+                [
+                    os.fspath(self._interpreter),
+                    os.fspath(script_path),
+                    func.__module__,
+                    func.__qualname__,
+                ],
+                input=pickled_args_dict,
+            )
 
-
-def get_launcher_kind(interpreter: os.PathLike[str]) -> Optional[LauncherKind]:
-    """Find the launcher kind.
-
-    This helper needs to run the Python interpreter for the target environment.
-
-    :param interpreter: Path to the Python interpreter to introspect.
-    """
-    return _run_script('launcher-kind', interpreter)
+        return pickle.loads(data)
```

### Comparing `environment_helpers-0.0.4/pyproject.toml` & `environment_helpers-0.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['flit-core >= 3.4']
 build-backend = 'flit_core.buildapi'
 
 [project]
 name = 'environment-helpers'
-version = '0.0.4'
+version = '0.1.0'
 description = 'Collection of helpers for managing Python environments'
 readme = 'README.md'
 requires-python = '>= 3.8'
 license.file = 'LICENSE'
 authors = [
   { name = 'Filipe Laíns', email = 'lains@riseup.net' },
 ]
```

### Comparing `environment_helpers-0.0.4/PKG-INFO` & `environment_helpers-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: environment-helpers
-Version: 0.0.4
+Version: 0.1.0
 Summary: Collection of helpers for managing Python environments
 Author-email: Filipe Laíns <lains@riseup.net>
 Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

