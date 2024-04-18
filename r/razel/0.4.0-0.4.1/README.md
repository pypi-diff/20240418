# Comparing `tmp/razel-0.4.0.tar.gz` & `tmp/razel-0.4.1.tar.gz`

## Comparing `razel-0.4.0.tar` & `razel-0.4.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 razel-0.4.0/version.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 razel-0.4.0/src/razel/__init__.py
--rw-r--r--   0        0        0    17262 2020-02-02 00:00:00.000000 razel-0.4.0/src/razel/razel.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 razel-0.4.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 razel-0.4.0/LICENSE.md
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 razel-0.4.0/README.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 razel-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     9045 2020-02-02 00:00:00.000000 razel-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 razel-0.4.1/version.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 razel-0.4.1/src/razel/__init__.py
+-rw-r--r--   0        0        0    17635 2020-02-02 00:00:00.000000 razel-0.4.1/src/razel/razel.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 razel-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 razel-0.4.1/LICENSE.md
+-rw-r--r--   0        0        0     8479 2020-02-02 00:00:00.000000 razel-0.4.1/README.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 razel-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     9046 2020-02-02 00:00:00.000000 razel-0.4.1/PKG-INFO
```

### Comparing `razel-0.4.0/src/razel/razel.py` & `razel-0.4.1/src/razel/razel.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,86 +9,90 @@
 import sys
 from enum import Enum
 from typing import ClassVar, Optional, Any, Tuple, TypeVar
 from collections.abc import Mapping, Sequence
 
 
 class Razel:
-    version: ClassVar[str] = "0.4.0"
+    version: ClassVar[str] = "0.4.1"
     _instance: ClassVar[Optional[Razel]] = None
 
     class Tag(str, Enum):
         QUIET = 'razel:quiet'
         """don't be verbose if command succeeded"""
         VERBOSE = 'razel:verbose'
         """always show verbose output"""
         CONDITION = 'razel:condition'
         """keep running and don't be verbose if command failed"""
-        NO_CACHE = 'razel:no-cache',
+        NO_CACHE = 'razel:no-cache'
         """always execute a command without caching"""
-        NO_REMOTE_CACHE = 'razel:no-remote-cache',
+        NO_REMOTE_CACHE = 'razel:no-remote-cache'
         """don't use remote cache"""
-        NO_SANDBOX = 'razel:no-sandbox',
+        NO_SANDBOX = 'razel:no-sandbox'
         """disable sandbox and also cache - for commands with unspecified input/output files"""
 
     def __init__(self, workspace_dir: str) -> None:
+        workspace_dir = str(workspace_dir)
         assert os.path.isabs(workspace_dir)
         self._workspace_dir = workspace_dir
         self.razel_file = os.path.join(self._workspace_dir, "razel.jsonl")
         self._commands: list[Command] = []
 
     @staticmethod
     def init(workspace_dir: str) -> Razel:
+        workspace_dir = str(workspace_dir)
         assert Razel._instance is None
         Razel._instance = Razel(workspace_dir)
         return Razel._instance
 
     @staticmethod
     def instance() -> Razel:
         assert Razel._instance is not None
         return Razel._instance
 
     def add_data_file(self, path: str) -> File:
+        path = str(path)
         return File(self._rel_path(path), True, None)
 
     def add_output_file(self, path: str) -> File:
+        path = str(path)
         return File(self._rel_path(path), False, None)
 
     def add_command(
-        self, name: str, executable: str | File | Command, args: Sequence[str | File | Command],
-        env: Optional[Mapping[str, str]] = None
+            self, name: str, executable: str | File | Command, args: Sequence[str | File | Command],
+            env: Optional[Mapping[str, str]] = None
     ) -> CustomCommand:
         name = self._sanitize_name(name)
-        path = self._rel_path(_map_arg_to_output_path(executable))
-        command = CustomCommand(name, path, _map_args_to_output_files(args), env)
+        executable_path = _map_arg_to_output_path(executable)
+        command = CustomCommand(name, executable_path, _map_args_to_output_files(args), env)
         return self._add(command)
 
     def add_task(self, name: str, task: str, args: Sequence[str | File | Command]) -> Task:
         name = Razel._sanitize_name(name)
         command = Task(name, task, _map_args_to_output_files(args))
         return self._add(command)
 
     def ensure_equal(self, arg1: File | Command, arg2: File | Command) -> None:
         """Add a task to compare two files. In case of two commands, all output files will be compared."""
         if isinstance(arg1, Command) and isinstance(arg2, Command):
             assert len(arg1.outputs) == len(arg2.outputs), "Commands to compare have different number of output files!"
-            for i in range(len(arg1.outputs)):
-                self.ensure_equal(arg1.outputs[i], arg2.outputs[i])
+            for a, b in zip(arg1.outputs, arg2.outputs):
+                self.ensure_equal(a, b)
         else:
             file1 = _map_arg_to_output_file(arg1)
             file2 = _map_arg_to_output_file(arg2)
             name = f"{file1.basename}##shouldEqual##{file2.basename}"
             self._add(Task(name, "ensure-equal", [file1, file2]))
 
     def ensure_not_equal(self, arg1: File | Command, arg2: File | Command) -> None:
         """Add a task to compare two files. In case of two commands, all output files will be compared."""
         if isinstance(arg1, Command) and isinstance(arg2, Command):
             assert len(arg1.outputs) == len(arg2.outputs), "Commands to compare have different number of output files!"
-            for i in range(len(arg1.outputs)):
-                self.ensure_equal(arg1.outputs[i], arg2.outputs[i])
+            for a, b in zip(arg1.outputs, arg2.outputs):
+                self.ensure_equal(a, b)
         else:
             file1 = _map_arg_to_output_file(arg1)
             file2 = _map_arg_to_output_file(arg2)
             name = f"{file1.basename}##shouldNotEqual##{file2.basename}"
             self._add(Task(name, "ensure-not-equal", [file1, file2]))
 
     def run(self, args: list[str] = ["exec"]):
@@ -132,26 +136,28 @@
                 return existing
 
         self._commands.append(command)
         return command
 
     @staticmethod
     def _sanitize_name(name: str) -> str:
+        name = str(name)
         return name.replace(":", ".")  # target names may not contain ':'
 
     def _rel_path(self, file_name: str) -> str:
+        file_name = str(file_name)
         if not os.path.isabs(file_name) or not file_name.startswith(self._workspace_dir):
             return file_name
 
         return os.path.relpath(file_name, self._workspace_dir)
 
 
 class File:
     def __init__(self, file_name: str, is_data: bool, created_by: Optional[Command]) -> None:
-        self._file_name = file_name
+        self._file_name = str(file_name)
         self._is_data = is_data
         self._created_by = created_by
 
     @property
     def file_name(self) -> str:
         return self._file_name
 
@@ -172,15 +178,15 @@
 
     def ensure_not_equal(self, other: File | Command) -> None:
         Razel.instance().ensure_not_equal(self, other)
 
 
 class Command(abc.ABC):
     def __init__(self, name: str, inputs: list[File], outputs: list[File]) -> None:
-        self._name = name
+        self._name = str(name)
         self._inputs = inputs
         self._outputs = outputs
         self._stdout: File | None = None
         self._stderr: File | None = None
         self._deps: list[Command] = []
         self._tags: list[Razel.Tag | str] = []
         for out in self._outputs:
@@ -249,20 +255,20 @@
     @abc.abstractmethod
     def json_for_comparing_to_existing_command(self) -> Mapping[str, Any]:
         pass
 
 
 class CustomCommand(Command):
     def __init__(
-        self, name: str, executable: str, args: Sequence[str | File], env: Optional[Mapping[str, str]] = None
+            self, name: str, executable: str, args: Sequence[str | File], env: Optional[Mapping[str, str]] = None
     ) -> None:
         (inputs, outputs) = _split_args_in_inputs_and_outputs(args)
         super().__init__(name, inputs, outputs)
-        self._executable = executable
-        self._args = args
+        self._executable = str(executable)
+        self._args: Sequence[str | File] = [x if isinstance(x, File) else str(x) for x in args]
         self._env = env
 
     @property
     def executable(self) -> str:
         return self._executable
 
     @property
@@ -350,16 +356,16 @@
         file = Razel.instance().add_output_file(path)
         Razel.instance().add_task(path, "write-file", [file, *lines])
         return file
 
     def __init__(self, name: str, task: str, args: Sequence[str | File]) -> None:
         (inputs, outputs) = _split_args_in_inputs_and_outputs(args)
         super().__init__(name, inputs, outputs)
-        self._task = task
-        self._args = args
+        self._task = str(task)
+        self._args: Sequence[str | File] = [x if isinstance(x, File) else str(x) for x in args]
 
     @property
     def task(self) -> str:
         return self._task
 
     @property
     def args(self) -> Sequence[str | File]:
@@ -383,25 +389,25 @@
             "args": [x.file_name if isinstance(x, File) else x for x in self.args],
         }
 
 
 def _map_arg_to_output_path(arg: str | File | Command) -> str:
     if isinstance(arg, Command):
         return arg.output.file_name
-    elif isinstance(arg, File):
+    if isinstance(arg, File):
         return arg.file_name
-    return arg
+    return str(arg)
 
 
 def _map_arg_to_output_file(arg: File | Command) -> File:
     return arg.output if isinstance(arg, Command) else arg
 
 
 def _map_args_to_output_files(args: Sequence[str | File | Command]) -> Sequence[str | File]:
-    return [x.output if isinstance(x, Command) else x for x in args]
+    return [x.output if isinstance(x, Command) else x if isinstance(x, File) else str(x) for x in args]
 
 
 def _split_args_in_inputs_and_outputs(args: Sequence[str | File | Command]) -> Tuple[list[File], list[File]]:
     inputs = [x for x in args if isinstance(x, File) and (x.is_data or x.created_by)]
     outputs = [x for x in args if isinstance(x, File) and not x.is_data and x.created_by is None]
     return inputs, outputs
```

### Comparing `razel-0.4.0/LICENSE.md` & `razel-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `razel-0.4.0/README.md` & `razel-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 
 If a process is killed by the OS, the command and similar ones will be retried with less concurrency to reduce the
 total memory usage. (Doesn't work in K8s because the whole pod is killed.)
 
 ### Sandbox
 
 Commands are executed in a temporary directory which contains symlinks to the input files specific to one command.
-The allows detecting unspecified dependencies which would break caching.
+This allows detecting unspecified dependencies which would break caching.
 
 The sandbox is not meant for executing untrusted code.
 
 ### Local Caching
 
 The local cache is enabled by default and stores information about previously executed commands and output files.
 The output directory `razel-out` contains symlinks to files stored in the local cache.
```

### Comparing `razel-0.4.0/pyproject.toml` & `razel-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `razel-0.4.0/PKG-INFO` & `razel-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: razel
-Version: 0.4.0
+Version: 0.4.1
 Summary: a command executor with caching for data processing pipelines
 Project-URL: Homepage, https://github.com/reu-dev/razel
 Project-URL: Bug Tracker, https://github.com/reu-dev/razel/issues
 Author-email: Stefan Reuschl <stefan@reu-dev.de>, Kacper Sagnowski <ksagnowski@gmail.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -151,15 +151,15 @@
 
 If a process is killed by the OS, the command and similar ones will be retried with less concurrency to reduce the
 total memory usage. (Doesn't work in K8s because the whole pod is killed.)
 
 ### Sandbox
 
 Commands are executed in a temporary directory which contains symlinks to the input files specific to one command.
-The allows detecting unspecified dependencies which would break caching.
+This allows detecting unspecified dependencies which would break caching.
 
 The sandbox is not meant for executing untrusted code.
 
 ### Local Caching
 
 The local cache is enabled by default and stores information about previously executed commands and output files.
 The output directory `razel-out` contains symlinks to files stored in the local cache.
```

