# Comparing `tmp/pytest_memray-1.5.0.tar.gz` & `tmp/pytest_memray-1.6.0.tar.gz`

## Comparing `pytest_memray-1.5.0.tar` & `pytest_memray-1.6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 pytest_memray-1.5.0/Makefile
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 pytest_memray-1.5.0/tox.ini
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pytest_memray-1.5.0/docs/api.rst
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 pytest_memray-1.5.0/docs/conf.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 pytest_memray-1.5.0/docs/configuration.rst
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pytest_memray-1.5.0/docs/index.rst
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 pytest_memray-1.5.0/docs/news.rst
--rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 pytest_memray-1.5.0/docs/usage.rst
--rw-r--r--   0        0        0   254627 2020-02-02 00:00:00.000000 pytest_memray-1.5.0/docs/_static/images/logo.png
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pytest_memray-1.5.0/docs/demo/test_ok.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 pytest_memray-1.5.0/docs/news/template.jinja2
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 pytest_memray-1.5.0/src/pytest_memray/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pytest_memray-1.5.0/src/pytest_memray/_version.py
--rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 pytest_memray-1.5.0/src/pytest_memray/marks.py
--rw-r--r--   0        0        0    14778 2020-02-02 00:00:00.000000 pytest_memray-1.5.0/src/pytest_memray/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_memray-1.5.0/src/pytest_memray/py.typed
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 pytest_memray-1.5.0/src/pytest_memray/utils.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pytest_memray-1.5.0/tests/conftest.py
--rw-r--r--   0        0        0    19852 2020-02-02 00:00:00.000000 pytest_memray-1.5.0/tests/test_pytest_memray.py
--rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 pytest_memray-1.5.0/tests/test_utils.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 pytest_memray-1.5.0/.gitignore
--rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 pytest_memray-1.5.0/LICENSE
--rw-r--r--   0        0        0     7938 2020-02-02 00:00:00.000000 pytest_memray-1.5.0/README.md
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 pytest_memray-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     9837 2020-02-02 00:00:00.000000 pytest_memray-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 pytest_memray-1.6.0/Makefile
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 pytest_memray-1.6.0/tox.ini
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pytest_memray-1.6.0/docs/api.rst
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 pytest_memray-1.6.0/docs/conf.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 pytest_memray-1.6.0/docs/configuration.rst
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pytest_memray-1.6.0/docs/index.rst
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 pytest_memray-1.6.0/docs/news.rst
+-rw-r--r--   0        0        0     6549 2020-02-02 00:00:00.000000 pytest_memray-1.6.0/docs/usage.rst
+-rw-r--r--   0        0        0   254627 2020-02-02 00:00:00.000000 pytest_memray-1.6.0/docs/_static/images/logo.png
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pytest_memray-1.6.0/docs/demo/test_ok.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 pytest_memray-1.6.0/docs/news/template.jinja2
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 pytest_memray-1.6.0/src/pytest_memray/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pytest_memray-1.6.0/src/pytest_memray/_version.py
+-rw-r--r--   0        0        0     8075 2020-02-02 00:00:00.000000 pytest_memray-1.6.0/src/pytest_memray/marks.py
+-rw-r--r--   0        0        0    15144 2020-02-02 00:00:00.000000 pytest_memray-1.6.0/src/pytest_memray/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_memray-1.6.0/src/pytest_memray/py.typed
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 pytest_memray-1.6.0/src/pytest_memray/utils.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pytest_memray-1.6.0/tests/conftest.py
+-rw-r--r--   0        0        0    24949 2020-02-02 00:00:00.000000 pytest_memray-1.6.0/tests/test_pytest_memray.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 pytest_memray-1.6.0/tests/test_utils.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 pytest_memray-1.6.0/.gitignore
+-rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 pytest_memray-1.6.0/LICENSE
+-rw-r--r--   0        0        0     8193 2020-02-02 00:00:00.000000 pytest_memray-1.6.0/README.md
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 pytest_memray-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0    10093 2020-02-02 00:00:00.000000 pytest_memray-1.6.0/PKG-INFO
```

### Comparing `pytest_memray-1.5.0/Makefile` & `pytest_memray-1.6.0/Makefile`

 * *Files identical despite different names*

### Comparing `pytest_memray-1.5.0/tox.ini` & `pytest_memray-1.6.0/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 [tox]
 envlist =
-    py310-cov
+    py312-cov
+    py312
+    py311
     py310
     py39
     py38
     docs
     lint
 requires = tox>=4.2
 
 [testenv]
 description =
     Run tests under {basepython}
     cov: with coverage
 passenv =
     CI
-    PYTEST_
-    VIRTUALENV_
+    PYTEST_*
+    VIRTUALENV_*
 setenv =
     COVERAGE_FILE = {toxworkdir}/.coverage.{envname}
     VIRTUALENV_NO_SETUPTOOLS = true
     VIRTUALENV_NO_WHEEL = true
 extras =
     test
 commands =
     make check
 allowlist_externals =
     make
 package = wheel
 wheel_build_env = .pkg
 
-[testenv:py310-cov]
+[testenv:py312-cov]
 commands =
     make coverage
 
 [testenv:docs]
 description = invoke sphinx-build to build the HTML docs
 setenv =
     VIRTUALENV_NO_SETUPTOOLS = false
```

### Comparing `pytest_memray-1.5.0/docs/conf.py` & `pytest_memray-1.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytest_memray-1.5.0/docs/configuration.rst` & `pytest_memray-1.6.0/docs/configuration.rst`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,17 @@
     Show the N most recent stack entries when showing tracebacks of memory allocations
 
   ``--native``
     Include native frames when showing tracebacks of memory allocations (will be slower)
 
   ``--trace-python-allocators``
     Record allocations made by the Pymalloc allocator (will be slower)
+  
+  ``--fail-on-increase``
+    Fail a test with the limit_memory marker if it uses more memory than its last successful run
 
 .. tab:: Config file options
 
   ``memray(bool)``
     Activate memray tracking.
 
   ``most-allocations(string)``
@@ -45,7 +48,10 @@
     Show the N most recent stack entries when showing tracebacks of memory allocations
 
   ``native(bool)``
     Include native frames when showing tracebacks of memory allocations (will be slower)
 
   ``trace_python_allocators(bool)``
     Record allocations made by the Pymalloc allocator (will be slower)
+
+  ``--fail-on-increase(bool)``
+    Fail a test with the limit_memory marker if it uses more memory than its last successful run
```

### Comparing `pytest_memray-1.5.0/docs/usage.rst` & `pytest_memray-1.6.0/docs/usage.rst`

 * *Files 9% similar despite different names*

```diff
@@ -31,25 +31,30 @@
 Markers
 ~~~~~~~
 
 This plugin provides `markers <https://docs.pytest.org/en/latest/example/markers.html>`__
 that can be used to enforce additional checks and validations on tests.
 
 
-.. py:function:: pytest.mark.limit_memory(memory_limit: str)
+.. py:function:: pytest.mark.limit_memory(memory_limit: str, current_thread_only: bool = False)
 
-    Fail the execution of the test if the test allocates more memory than allowed.
+    Fail the execution of the test if the test allocates more peak memory than allowed.
 
     When this marker is applied to a test, it will cause the test to fail if the
-    execution of the test allocates more memory than allowed. It takes a single argument
-    with a string indicating the maximum memory that the test can allocate.
+    execution of the test allocates more memory (at the peak/high watermark) than allowed.
+    It takes a single argument with a string indicating the maximum memory that the test
+    can allocate.
 
     The format for the string is ``<NUMBER> ([KMGTP]B|B)``. The marker will raise
     ``ValueError`` if the string format cannot be parsed correctly.
 
+    If the optional keyword-only argument ``current_thread_only`` is set to *True*, the
+    plugin will only track memory allocations made by the current thread and all other
+    allocations will be ignored.
+
     .. warning::
 
         As the Python interpreter has its own
         `object allocator <https://docs.python.org/3/c-api/memory.html>`__ it's possible
         that memory is not immediately released to the system when objects are deleted,
         so tests using this marker may need to give some room to account for this.
 
@@ -58,15 +63,15 @@
     .. code-block:: python
 
         @pytest.mark.limit_memory("24 MB")
         def test_foobar():
             pass  # do some stuff that allocates memory
 
 
-.. py:function:: pytest.mark.limit_leaks(location_limit: str, filter_fn: LeaksFilterFunction | None = None)
+.. py:function:: pytest.mark.limit_leaks(location_limit: str, filter_fn: LeaksFilterFunction | None = None, current_thread_only: bool = False)
 
     Fail the execution of the test if any call stack in the test leaks more memory than
     allowed.
 
     .. important::
        To detect leaks, Memray needs to intercept calls to the Python allocators and
        report native call frames. This is adds significant overhead, and will slow your
@@ -91,14 +96,18 @@
     represents a filtering function that will be called once for each distinct call
     stack that leaked more memory than allowed. If it returns *True*, leaks from that
     location will be included in the final report. If it returns *False*, leaks
     associated with the stack it was called with will be ignored. If all leaks are
     ignored, the test will not fail. This can be used to discard any known false
     positives.
 
+    If the optional keyword-only argument ``current_thread_only`` is set to *True*, the
+    plugin will only track memory allocations made by the current thread and all other
+    allocations will be ignored.
+
     .. tip::
 
        You can pass the ``--memray-bin-path`` argument to ``pytest`` to specify
        a directory where Memray will store the binary files with the results. You
        can then use the ``memray`` CLI to further investigate the allocations and the
        leaks using any Memray reporters you'd like. Check `the memray docs
        <https://bloomberg.github.io/memray/getting_started.html>`_ for more
```

### Comparing `pytest_memray-1.5.0/docs/_static/images/logo.png` & `pytest_memray-1.6.0/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `pytest_memray-1.5.0/docs/news/template.jinja2` & `pytest_memray-1.6.0/docs/news/template.jinja2`

 * *Files identical despite different names*

### Comparing `pytest_memray-1.5.0/src/pytest_memray/marks.py` & `pytest_memray-1.6.0/src/pytest_memray/marks.py`

 * *Files 23% similar despite different names*

```diff
@@ -123,14 +123,36 @@
         """Generate a longrepr user-facing error message."""
         return (
             f"Test was allowed to leak {sizeof_fmt(self.max_memory)} "
             "per location but at least one location leaked more"
         )
 
 
+@dataclass
+class _MoreMemoryInfo:
+    previous_memory: float
+    new_memory: float
+
+    @property
+    def section(self) -> PytestSection:
+        """Return a tuple in the format expected by section reporters."""
+        return (
+            "memray-max-memory",
+            "Test uses more memory than previous run",
+        )
+
+    @property
+    def long_repr(self) -> str:
+        """Generate a longrepr user-facing error message."""
+        return (
+            f"Test previously used {sizeof_fmt(self.previous_memory)} "
+            f"but now uses {sizeof_fmt(self.new_memory)}"
+        )
+
+
 def _generate_section_text(
     allocations: list[AllocationRecord], native_stacks: bool, num_stacks: int
 ) -> str:
     text_lines = []
     for record in allocations:
         size = record.size
         stack_trace = (
@@ -158,23 +180,43 @@
         return True
 
     frames = tuple(StackFrame(*frame) for frame in stack)
     return filter_fn(Stack(frames))
 
 
 def limit_memory(
-    limit: str, *, _result_file: Path, _config: Config
-) -> _MemoryInfo | None:
+    limit: str,
+    *,
+    current_thread_only: bool = False,
+    _result_file: Path,
+    _config: Config,
+    _test_id: str,
+) -> _MemoryInfo | _MoreMemoryInfo | None:
     """Limit memory used by the test."""
     reader = FileReader(_result_file)
-    allocations: list[AllocationRecord] = list(
-        reader.get_high_watermark_allocation_records(merge_threads=True)
-    )
+    allocations: list[AllocationRecord] = [
+        record
+        for record in reader.get_high_watermark_allocation_records(
+            merge_threads=not current_thread_only
+        )
+        if not current_thread_only or record.tid == reader.metadata.main_thread_id
+    ]
     max_memory = parse_memory_string(limit)
     total_allocated_memory = sum(record.size for record in allocations)
+
+    if _config.cache is not None:
+        cache = _config.cache.get(f"memray/{_test_id}", {})
+        previous = cache.get("total_allocated_memory", float("inf"))
+        fail_on_increase = cast(bool, value_or_ini(_config, "fail_on_increase"))
+        if fail_on_increase and total_allocated_memory > previous:
+            return _MoreMemoryInfo(previous, total_allocated_memory)
+
+        cache["total_allocated_memory"] = total_allocated_memory
+        _config.cache.set(f"memray/{_test_id}", cache)
+
     if total_allocated_memory < max_memory:
         return None
     num_stacks: int = cast(int, value_or_ini(_config, "stacks"))
     native_stacks: bool = cast(bool, value_or_ini(_config, "native"))
     return _MemoryInfo(
         max_memory=max_memory,
         allocations=allocations,
@@ -184,21 +226,27 @@
     )
 
 
 def limit_leaks(
     location_limit: str,
     *,
     filter_fn: Optional[LeaksFilterFunction] = None,
+    current_thread_only: bool = False,
     _result_file: Path,
     _config: Config,
+    _test_id: str,
 ) -> _LeakedInfo | None:
     reader = FileReader(_result_file)
-    allocations: list[AllocationRecord] = list(
-        reader.get_leaked_allocation_records(merge_threads=True)
-    )
+    allocations: list[AllocationRecord] = [
+        record
+        for record in reader.get_leaked_allocation_records(
+            merge_threads=not current_thread_only
+        )
+        if not current_thread_only or record.tid == reader.metadata.main_thread_id
+    ]
 
     memory_limit = parse_memory_string(location_limit)
 
     leaked_allocations = list(
         allocation
         for allocation in allocations
         if (
```

### Comparing `pytest_memray-1.5.0/src/pytest_memray/plugin.py` & `pytest_memray-1.6.0/src/pytest_memray/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from typing import List
 from typing import Tuple
 from typing import cast
 from typing import Protocol
 
 from _pytest.terminal import TerminalReporter
 from memray import AllocationRecord
+from memray import FileFormat
 from memray import FileReader
 from memray import Metadata
 from memray import Tracker
 from pytest import CallInfo
 from pytest import CollectReport
 from pytest import Config
 from pytest import ExitCode
@@ -48,14 +49,15 @@
 
 
 class PluginFn(Protocol):
     def __call__(
         *args: Any,
         _result_file: Path,
         _config: Config,
+        _test_id: str,
         **kwargs: Any,
     ) -> SectionMetadata | None:
         ...
 
 
 MARKERS = {
     "limit_memory": limit_memory,
@@ -72,30 +74,28 @@
     """Count elements from the iterable into evenly spaced bins
 
     >>> scores = [82, 85, 90, 91, 70, 87, 45]
     >>> histogram(scores, 0, 100, 10)
     [0, 0, 0, 0, 1, 0, 0, 1, 3, 2]
 
     """
-    step = ((high - low) / bins) or low
+    step = ((high - low) / bins) or low or 1
     dist = collections.Counter((x - low) // step for x in iterable)
     return [dist[b] for b in range(bins)]
 
 
 def cli_hist(data: Iterable[float], bins: int, *, log_scale: bool = True) -> str:
     bars = " ▁▂▃▄▅▆▇█"
+    if log_scale:
+        data = [math.log(number if number else 1) for number in data]
     low = min(data)
     high = max(data)
-    if log_scale:
-        data = map(math.log, filter(lambda number: number != 0, data))
-        low = math.log(low)
-        high = math.log(high)
     data_bins = histogram(data, low=low, high=high, bins=bins)
     bar_indexes = (int(elem * (len(bars) - 1) / max(data_bins)) for elem in data_bins)
-    result = " ".join(bars[bar_index] for bar_index in bar_indexes)
+    result = "".join(bars[bar_index] for bar_index in bar_indexes)
     return result
 
 
 ResultElement = List[Tuple[object, int]]
 
 
 @dataclass
@@ -129,23 +129,23 @@
         else:
             self._tmp_dir = None
             self.result_path = path
         self._bin_prefix = config.getvalue("memray_bin_prefix") or uuid.uuid4().hex
         self.result_metadata_path = self.result_path / "metadata"
         self.result_metadata_path.mkdir(exist_ok=True, parents=True)
 
-    @hookimpl(hookwrapper=True)  # type: ignore[misc] # Untyped decorator
+    @hookimpl(hookwrapper=True)
     def pytest_unconfigure(self, config: Config) -> Generator[None, None, None]:
         yield
         if self._tmp_dir is not None:
             self._tmp_dir.cleanup()
         if os.environ.get("MEMRAY_RESULT_PATH"):
             del os.environ["MEMRAY_RESULT_PATH"]
 
-    @hookimpl(hookwrapper=True)  # type: ignore[misc] # Untyped decorator
+    @hookimpl(hookwrapper=True)
     def pytest_pyfunc_call(self, pyfuncitem: Function) -> object | None:
         func = pyfuncitem.obj
 
         markers = {
             marker.name
             for marker in pyfuncitem.iter_markers()
             if marker.name in MARKERS
@@ -183,14 +183,15 @@
             test_result: object | Any = None
             try:
                 result_file = _build_bin_path()
                 with Tracker(
                     result_file,
                     native_traces=native,
                     trace_python_allocators=trace_python_allocators,
+                    file_format=FileFormat.AGGREGATED_ALLOCATIONS,
                 ):
                     test_result = func(*args, **kwargs)
                 try:
                     metadata = FileReader(result_file).metadata
                 except OSError:
                     return None
                 result = Result(pyfuncitem.nodeid, metadata, result_file)
@@ -208,15 +209,15 @@
                 # to be wrapped again.
                 pyfuncitem.obj = func
             return test_result
 
         pyfuncitem.obj = wrapper
         yield
 
-    @hookimpl(hookwrapper=True)  # type: ignore[misc] # Untyped decorator
+    @hookimpl(hookwrapper=True)
     def pytest_runtest_makereport(
         self, item: Item, call: CallInfo[None]
     ) -> Generator[None, TestReport | None, TestReport | None]:
         outcome = yield
         if call.when != "call" or outcome is None:
             return None
 
@@ -233,35 +234,36 @@
             if not result:
                 continue
             res = marker_fn(
                 *marker.args,
                 **marker.kwargs,
                 _result_file=result.result_file,
                 _config=self.config,
+                _test_id=item.nodeid,
             )
             if res:
                 report.outcome = "failed"
                 report.longrepr = res.long_repr
                 report.sections.append(res.section)
                 outcome.force_result(report)
         return None
 
-    @hookimpl(hookwrapper=True, trylast=True)  # type: ignore[misc] # Untyped decorator
+    @hookimpl(hookwrapper=True, trylast=True)
     def pytest_report_teststatus(
         self, report: CollectReport | TestReport
     ) -> Generator[None, TestReport, None]:
         outcome = yield
         if report.when != "call" or report.outcome != "failed":
             return None
 
         if any("memray" in section for section, _ in report.sections):
             outcome.force_result(("failed", "M", "MEMORY PROBLEMS"))
         return None
 
-    @hookimpl  # type: ignore[misc] # Untyped decorator
+    @hookimpl
     def pytest_terminal_summary(
         self, terminalreporter: TerminalReporter, exitstatus: ExitCode
     ) -> None:
         if value_or_ini(self.config, "hide_memray_summary") or not value_or_ini(
             self.config, "memray"
         ):
             return
@@ -283,14 +285,16 @@
                 node_id: result.metadata.peak_memory
                 for node_id, result in self.results.items()
                 if result.result_file.exists()
             }
         )
 
         max_results = cast(int, value_or_ini(self.config, "most_allocations"))
+        if max_results == 0:
+            max_results = len(total_sizes)
 
         for test_id, total_size in total_sizes.most_common(max_results):
             result = self.results[test_id]
             reader = FileReader(result.result_file)
             func = reader.get_high_watermark_allocation_records
             records = list(func(merge_threads=True))
             if not records:
@@ -378,14 +382,20 @@
     )
     group.addoption(
         "--trace-python-allocators",
         action="store_true",
         default=False,
         help="Record allocations made by the Pymalloc allocator (will be slower)",
     )
+    group.addoption(
+        "--fail-on-increase",
+        action="store_true",
+        default=False,
+        help="Fail a test with the limit_memory marker if it uses more memory than its last successful run",
+    )
 
     parser.addini("memray", "Activate pytest.ini setting", type="bool")
     parser.addini(
         "hide_memray_summary",
         "Hide the memray summary at the end of the execution",
         type="bool",
     )
@@ -401,14 +411,19 @@
         type="bool",
     )
     parser.addini(
         "trace_python_allocators",
         help="Record allocations made by the Pymalloc allocator (will be slower)",
         type="bool",
     )
+    parser.addini(
+        "fail-on-increase",
+        help="Fail a test with the limit_memory marker if it uses more memory than its last successful run",
+        type="bool",
+    )
     help_msg = "Show the N tests that allocate most memory (N=0 for all)"
     parser.addini("most_allocations", help_msg)
 
 
 def pytest_configure(config: Config) -> None:
     pytest_memray = Manager(config)
     config.pluginmanager.register(pytest_memray, "memray_manager")
```

### Comparing `pytest_memray-1.5.0/src/pytest_memray/utils.py` & `pytest_memray-1.6.0/src/pytest_memray/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         raise ValueError(f"Invalid memory size format: {mem_str}")
     quantity, unit = match.groups()
     return float(quantity) * UNIT_TO_MULTIPLIER[unit.upper()]
 
 
 def value_or_ini(config: Config, key: str) -> object:
     value = config.getvalue(key)
-    if value:
+    if value is not None:
         return value
     try:
         return config.getini(key)
     except (KeyError, ValueError):
         return value
```

### Comparing `pytest_memray-1.5.0/tests/test_pytest_memray.py` & `pytest_memray-1.6.0/tests/test_pytest_memray.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,40 @@
 from __future__ import annotations
 
+import re
 import xml.etree.ElementTree as ET
 from types import SimpleNamespace
 from unittest.mock import ANY
 from unittest.mock import patch
 
 import pytest
+from memray import FileFormat
 from memray import Tracker
 from pytest import ExitCode
 from pytest import Pytester
 
+from pytest_memray.marks import StackFrame
+
+
+def extract_stacks(test_output: str) -> list[list[StackFrame]]:
+    ret: list[list[StackFrame]] = []
+    before_start = True
+    for line in test_output.splitlines():
+        if before_start:
+            if "List of allocations:" in line:
+                before_start = False
+        elif "allocated here" in line:
+            ret.append([])
+        elif (match := re.match(r"^ {8}([^:]+):(.*):(\d+)$", line)) is not None:
+            ret[-1].append(
+                StackFrame(function=match[1], filename=match[2], lineno=int(match[3]))
+            )
+
+    return ret
+
 
 def test_help_message(pytester: Pytester) -> None:
     result = pytester.runpytest("--help")
     # fnmatch_lines does an assertion internally
     result.stdout.fnmatch_lines(
         [
             "memray:",
@@ -172,18 +193,19 @@
     """
     )
 
     result = pytester.runpytest("--memray", f"--stacks={num_stacks}")
 
     assert result.ret == ExitCode.TESTS_FAILED
 
-    output = result.stdout.str()
-
-    assert "valloc:" in output
-    assert output.count("rec:") == min(num_stacks - 1, 10)
+    stacks = extract_stacks(result.stdout.str())
+    valloc_stacks = [stack for stack in stacks if stack[0].function == "valloc"]
+    (valloc_stack,) = valloc_stacks
+    num_rec_frames = sum(1 for frame in valloc_stack if frame.function == "rec")
+    assert num_rec_frames == min(num_stacks - 1, 10)
 
 
 @pytest.mark.parametrize("native", [True, False])
 def test_memray_report_native(native: bool, pytester: Pytester) -> None:
     pytester.makepyfile(
         """
         import pytest
@@ -200,15 +222,18 @@
     with patch("pytest_memray.plugin.Tracker", wraps=Tracker) as mock:
         result = pytester.runpytest("--memray", *(["--native"] if native else []))
 
     assert result.ret == ExitCode.TESTS_FAILED
 
     output = result.stdout.str()
     mock.assert_called_once_with(
-        ANY, native_traces=native, trace_python_allocators=False
+        ANY,
+        native_traces=native,
+        trace_python_allocators=False,
+        file_format=FileFormat.AGGREGATED_ALLOCATIONS,
     )
 
     if native:
         assert "MemoryAllocator_1" in output
     else:
         assert "MemoryAllocator_1" not in output
 
@@ -243,15 +268,18 @@
 
     assert result.ret == (
         ExitCode.TESTS_FAILED if trace_python_allocators else ExitCode.OK
     )
 
     output = result.stdout.str()
     mock.assert_called_once_with(
-        ANY, native_traces=False, trace_python_allocators=trace_python_allocators
+        ANY,
+        native_traces=False,
+        trace_python_allocators=trace_python_allocators,
+        file_format=FileFormat.AGGREGATED_ALLOCATIONS,
     )
 
     if trace_python_allocators:
         assert "allocate_with_pymalloc" in output
     else:
         assert "allocate_with_pymalloc" not in output
 
@@ -344,19 +372,19 @@
     pytester.makepyfile(
         """
         import pytest
         from memray._test import MemoryAllocator
         allocator = MemoryAllocator()
 
         def allocating_func1():
-            allocator.valloc(1024)
+            allocator.valloc(1024*1024)
             allocator.free()
 
         def allocating_func2():
-            allocator.valloc(1024*2)
+            allocator.valloc(1024*1024*2)
             allocator.free()
 
         def test_foo():
             allocating_func1()
 
         def test_bar():
             allocating_func2()
@@ -369,14 +397,47 @@
 
     output = result.stdout.str()
 
     assert "results for test_memray_report_limit.py::test_foo" not in output
     assert "results for test_memray_report_limit.py::test_bar" in output
 
 
+def test_memray_report_limit_without_limit(pytester: Pytester) -> None:
+    pytester.makepyfile(
+        """
+        import pytest
+        from memray._test import MemoryAllocator
+        allocator = MemoryAllocator()
+
+        def allocating_func1():
+            allocator.valloc(1024)
+            allocator.free()
+
+        def allocating_func2():
+            allocator.valloc(1024*2)
+            allocator.free()
+
+        def test_foo():
+            allocating_func1()
+
+        def test_bar():
+            allocating_func2()
+    """
+    )
+
+    result = pytester.runpytest("--memray", "--most-allocations=0")
+
+    assert result.ret == ExitCode.OK
+
+    output = result.stdout.str()
+
+    assert "results for test_memray_report_limit_without_limit.py::test_foo" in output
+    assert "results for test_memray_report_limit_without_limit.py::test_bar" in output
+
+
 def test_failing_tests_are_not_reported(pytester: Pytester) -> None:
     pytester.makepyfile(
         """
         import pytest
         from memray._test import MemoryAllocator
         allocator = MemoryAllocator()
 
@@ -595,14 +656,15 @@
     result = pytester.runpytest("-Werror", "--memray")
     assert result.ret == ExitCode.OK
 
 
 @pytest.mark.parametrize(
     "size, outcome",
     [
+        (0, ExitCode.OK),
         (1, ExitCode.OK),
         (1024 * 1 / 10, ExitCode.OK),
         (1024 * 1, ExitCode.TESTS_FAILED),
         (1024 * 10, ExitCode.TESTS_FAILED),
     ],
 )
 def test_leak_marker(pytester: Pytester, size: int, outcome: ExitCode) -> None:
@@ -623,18 +685,17 @@
 
     assert result.ret == outcome
 
 
 @pytest.mark.parametrize(
     "size, outcome",
     [
-        (1, ExitCode.OK),
-        (1024 * 1 / 10, ExitCode.OK),
-        (1024 * 1, ExitCode.TESTS_FAILED),
-        (1024 * 10, ExitCode.TESTS_FAILED),
+        (4 * 1024, ExitCode.OK),
+        (0.4 * 1024 * 1024, ExitCode.OK),
+        (4 * 1024 * 1024, ExitCode.TESTS_FAILED),
     ],
 )
 def test_leak_marker_in_a_thread(
     pytester: Pytester, size: int, outcome: ExitCode
 ) -> None:
     pytester.makepyfile(
         f"""
@@ -642,15 +703,15 @@
         from memray._test import MemoryAllocator
         allocator = MemoryAllocator()
         import threading
         def allocating_func():
             for _ in range(10):
                 allocator.valloc({size})
                 # No free call here
-        @pytest.mark.limit_leaks("5KB")
+        @pytest.mark.limit_leaks("20MB")
         def test_memory_alloc_fails():
             t = threading.Thread(target=allocating_func)
             t.start()
             t.join()
         """
     )
 
@@ -738,7 +799,122 @@
     )
 
     result = pytester.runpytest("--memray")
     assert result.ret == ExitCode.TESTS_FAILED
 
     output = result.stdout.str()
     assert "Only one Memray marker can be applied to each test" in output
+
+
+def test_fail_on_increase(pytester: Pytester):
+    pytester.makepyfile(
+        """
+        import pytest
+        from memray._test import MemoryAllocator
+        allocator = MemoryAllocator()
+
+        @pytest.mark.limit_memory("100MB")
+        def test_memory_alloc_fails():
+            allocator.valloc(1024)
+            allocator.free()
+        """
+    )
+    result = pytester.runpytest("--memray")
+    assert result.ret == ExitCode.OK
+    pytester.makepyfile(
+        """
+        import pytest
+        from memray._test import MemoryAllocator
+        allocator = MemoryAllocator()
+
+        @pytest.mark.limit_memory("100MB")
+        def test_memory_alloc_fails():
+            allocator.valloc(1024 * 10)
+            allocator.free()
+        """
+    )
+    result = pytester.runpytest("--memray", "--fail-on-increase")
+    assert result.ret == ExitCode.TESTS_FAILED
+    output = result.stdout.str()
+    assert "Test uses more memory than previous run" in output
+    assert "Test previously used 1.0KiB but now uses 10.0KiB" in output
+
+
+def test_fail_on_increase_unset(pytester: Pytester):
+    pytester.makepyfile(
+        """
+        import pytest
+        from memray._test import MemoryAllocator
+        allocator = MemoryAllocator()
+
+        @pytest.mark.limit_memory("100MB")
+        def test_memory_alloc_fails():
+            allocator.valloc(1024)
+            allocator.free()
+        """
+    )
+    result = pytester.runpytest("--memray")
+    assert result.ret == ExitCode.OK
+    pytester.makepyfile(
+        """
+        import pytest
+        from memray._test import MemoryAllocator
+        allocator = MemoryAllocator()
+
+        @pytest.mark.limit_memory("100MB")
+        def test_memory_alloc_fails():
+            allocator.valloc(1024 * 10)
+            allocator.free()
+        """
+    )
+    result = pytester.runpytest("--memray")
+    assert result.ret == ExitCode.OK
+
+
+def test_limit_memory_in_current_thread(pytester: Pytester) -> None:
+    pytester.makepyfile(
+        """
+        import pytest
+        from memray._test import MemoryAllocator
+        allocator = MemoryAllocator()
+        import threading
+        def allocating_func():
+            for _ in range(10):
+                allocator.valloc(1024*5)
+                # No free call here
+
+        @pytest.mark.limit_memory("5KB", current_thread_only=True)
+        def test_memory_alloc_fails():
+            t = threading.Thread(target=allocating_func)
+            t.start()
+            t.join()
+        """
+    )
+
+    result = pytester.runpytest("--memray")
+
+    assert result.ret == ExitCode.OK
+
+
+def test_leaks_in_current_thread(pytester: Pytester) -> None:
+    pytester.makepyfile(
+        """
+        import pytest
+        from memray._test import MemoryAllocator
+        allocator = MemoryAllocator()
+        import threading
+        def allocating_func():
+            for _ in range(10):
+                allocator.valloc(1024*5)
+                # No free call here
+
+        @pytest.mark.limit_leaks("5KB", current_thread_only=True)
+        def test_memory_alloc_fails():
+            t = threading.Thread(target=allocating_func)
+            t.start()
+            t.join()
+        """
+    )
+
+    result = pytester.runpytest("--memray")
+
+    assert result.ret == ExitCode.OK
```

### Comparing `pytest_memray-1.5.0/tests/test_utils.py` & `pytest_memray-1.6.0/tests/test_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from typing import NoReturn
 from unittest.mock import create_autospec
 
 import pytest
 
 from pytest_memray.utils import WriteEnabledDirectoryAction
 from pytest_memray.utils import parse_memory_string
+from pytest_memray.plugin import cli_hist
 
 
 @pytest.mark.parametrize(
     "the_str, expected",
     [
         ("100 B", 100),
         ("100B", 100),
@@ -119,7 +120,29 @@
     tmp_path.chmod(tmp_path.stat().st_mode & ~write)
     exp = f"cannot create directory {path} due to [Errno 13] Permission denied:"
     try:
         with pytest.raises(ValueError, match=re.escape(exp)):
             w_dir_check(path)
     finally:
         tmp_path.chmod(tmp_path.stat().st_mode | write)
+
+
+def test_histogram_with_zero_byte_allocations():
+    # GIVEN
+    allocations = [0, 100, 990, 1000, 50000]
+
+    # WHEN
+    histogram = cli_hist(allocations, bins=5)
+
+    # THEN
+    assert histogram == "▄ ▄█▄"
+
+
+def test_histogram_with_only_zero_byte_allocations():
+    # GIVEN
+    allocations = [0, 0, 0, 0]
+
+    # WHEN
+    histogram = cli_hist(allocations, bins=5)
+
+    # THEN
+    assert histogram == "█    "
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytest_memray-1.5.0/.gitignore` & `pytest_memray-1.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_memray-1.5.0/LICENSE` & `pytest_memray-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_memray-1.5.0/README.md` & `pytest_memray-1.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -93,23 +93,27 @@
 - `--memray-bin-path` - path where to write the memray binary dumps (by default a
   temporary folder)
 - `--memray-bin-prefix` - prefix to use for the binary dump (by default a random UUID4
   hex)
 - `--stacks=STACKS` - Show the N stack entries when showing tracebacks of memory allocations
 - `--native` - Show native frames when showing tracebacks of memory allocations (will be slower)
 - `--trace-python-allocators` - Record allocations made by the Pymalloc allocator (will be slower)
+- `--fail-on-increase` - Fail a test with the `limit_memory`` marker if it uses
+  more memory than its last successful run
 
 ## Configuration - INI
 
 - `memray(bool)` - activate memray tracking
 - `most-allocations(string)` - show the N tests that allocate most memory (N=0 for all)
 - `hide_memray_summary(bool)` - hide the memray summary at the end of the execution
 - `stacks(int)` - Show the N stack entries when showing tracebacks of memory allocations
 - `native(bool)`- Show native frames when showing tracebacks of memory allocations (will be slower)
-- `trace_python_allocators` - Record allocations made by the Pymalloc allocator (will be slower)
+- `trace_python_allocators(bool)` - Record allocations made by the Pymalloc allocator (will be slower)
+- `fail-on-increase(bool)` - Fail a test with the `limit_memory` marker if it
+  uses more memory than its last successful run
 
 ## License
 
 pytest-memray is Apache-2.0 licensed, as found in the [LICENSE](LICENSE) file.
 
 ## Code of Conduct
```

### Comparing `pytest_memray-1.5.0/pyproject.toml` & `pytest_memray-1.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ]
 maintainers = [
   { name = "Pablo Galindo Salgado", email = "pgalindo3@bloomberg.net" },
 ]
 requires-python = ">=3.8"
 dependencies = [
   "pytest>=7.2",
-  "memray>=1.5",
+  "memray>=1.12",
 ]
 optional-dependencies.docs = [
   "furo>=2022.12.7",
   "sphinx>=6.1.3",
   "sphinx-argparse>=0.4",
   "sphinx-inline-tabs>=2022.1.2b11",
   "sphinxcontrib-programoutput>=0.17",
```

### Comparing `pytest_memray-1.5.0/PKG-INFO` & `pytest_memray-1.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pytest-memray
-Version: 1.5.0
+Version: 1.6.0
 Summary: A simple plugin to use with pytest
 Project-URL: Bug Tracker, https://github.com/bloomberg/pytest-memray/issues
 Project-URL: Documentation, https://pytest-memray.readthedocs.io
 Project-URL: Source Code, https://github.com/bloomberg/pytest-memray
 Author-email: Pablo Galindo Salgado <pgalindo3@bloomberg.net>
 Maintainer-email: Pablo Galindo Salgado <pgalindo3@bloomberg.net>
 License-Expression: Apache-2.0
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Debuggers
 Requires-Python: >=3.8
-Requires-Dist: memray>=1.5
+Requires-Dist: memray>=1.12
 Requires-Dist: pytest>=7.2
 Provides-Extra: docs
 Requires-Dist: furo>=2022.12.7; extra == 'docs'
 Requires-Dist: sphinx-argparse>=0.4; extra == 'docs'
 Requires-Dist: sphinx-inline-tabs>=2022.1.2b11; extra == 'docs'
 Requires-Dist: sphinx>=6.1.3; extra == 'docs'
 Requires-Dist: sphinxcontrib-programoutput>=0.17; extra == 'docs'
@@ -136,23 +136,27 @@
 - `--memray-bin-path` - path where to write the memray binary dumps (by default a
   temporary folder)
 - `--memray-bin-prefix` - prefix to use for the binary dump (by default a random UUID4
   hex)
 - `--stacks=STACKS` - Show the N stack entries when showing tracebacks of memory allocations
 - `--native` - Show native frames when showing tracebacks of memory allocations (will be slower)
 - `--trace-python-allocators` - Record allocations made by the Pymalloc allocator (will be slower)
+- `--fail-on-increase` - Fail a test with the `limit_memory`` marker if it uses
+  more memory than its last successful run
 
 ## Configuration - INI
 
 - `memray(bool)` - activate memray tracking
 - `most-allocations(string)` - show the N tests that allocate most memory (N=0 for all)
 - `hide_memray_summary(bool)` - hide the memray summary at the end of the execution
 - `stacks(int)` - Show the N stack entries when showing tracebacks of memory allocations
 - `native(bool)`- Show native frames when showing tracebacks of memory allocations (will be slower)
-- `trace_python_allocators` - Record allocations made by the Pymalloc allocator (will be slower)
+- `trace_python_allocators(bool)` - Record allocations made by the Pymalloc allocator (will be slower)
+- `fail-on-increase(bool)` - Fail a test with the `limit_memory` marker if it
+  uses more memory than its last successful run
 
 ## License
 
 pytest-memray is Apache-2.0 licensed, as found in the [LICENSE](LICENSE) file.
 
 ## Code of Conduct
```

