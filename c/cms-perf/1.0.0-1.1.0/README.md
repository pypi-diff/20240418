# Comparing `tmp/cms_perf-1.0.0.tar.gz` & `tmp/cms_perf-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cms_perf-1.0.0.tar", last modified: Wed Sep  2 10:25:01 2020, max compression
+gzip compressed data, was "cms_perf-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cms_perf-1.0.0.tar` & `cms_perf-1.1.0.tar`

### file list

```diff
@@ -1,35 +1,13 @@
--rw-r--r--   0        0        0      325 2020-08-24 15:28:50.149502 cms_perf-1.0.0/.coveragerc
--rw-r--r--   0        0        0      169 2019-11-20 21:22:45.358000 cms_perf-1.0.0/.flake8
--rw-r--r--   0        0        0     3403 2020-08-22 11:57:37.663264 cms_perf-1.0.0/.gitignore
--rw-r--r--   0        0        0      171 2020-08-22 11:57:37.664172 cms_perf-1.0.0/.readthedocs.yml
--rw-r--r--   0        0        0      562 2020-07-15 12:10:10.743471 cms_perf-1.0.0/.travis.yml
--rw-r--r--   0        0        0     1078 2020-06-26 16:29:00.544473 cms_perf-1.0.0/LICENSE
--rw-r--r--   0        0        0     1532 2020-08-24 15:42:31.481816 cms_perf-1.0.0/README.rst
--rw-r--r--   0        0        0       70 2020-09-02 10:00:49.233499 cms_perf-1.0.0/cms_perf/__init__.py
--rw-r--r--   0        0        0       92 2020-07-15 12:10:10.745258 cms_perf-1.0.0/cms_perf/__main__.py
--rw-r--r--   0        0        0     3343 2020-08-24 15:28:50.150471 cms_perf-1.0.0/cms_perf/report.py
--rw-r--r--   0        0        0        0 2020-08-24 15:28:50.150659 cms_perf-1.0.0/cms_perf/sensors/__init__.py
--rw-r--r--   0        0        0      860 2020-08-24 15:28:50.152100 cms_perf-1.0.0/cms_perf/sensors/net_load.py
--rw-r--r--   0        0        0     2565 2020-08-24 15:28:50.152727 cms_perf-1.0.0/cms_perf/sensors/sensor.py
--rw-r--r--   0        0        0     2348 2020-08-24 15:28:50.153019 cms_perf-1.0.0/cms_perf/sensors/xrd_load.py
--rw-r--r--   0        0        0        0 2020-08-24 15:28:50.153127 cms_perf-1.0.0/cms_perf/setup/__init__.py
--rw-r--r--   0        0        0     3308 2020-09-01 09:27:10.618377 cms_perf-1.0.0/cms_perf/setup/cli.py
--rw-r--r--   0        0        0     9042 2020-08-24 15:28:50.154308 cms_perf-1.0.0/cms_perf/setup/cli_parser.py
--rw-r--r--   0        0        0      634 2020-08-22 11:57:37.671300 cms_perf-1.0.0/docs/Makefile
--rw-r--r--   0        0        0     2482 2020-08-22 11:57:37.672053 cms_perf-1.0.0/docs/conf.py
--rw-r--r--   0        0        0     2204 2020-08-24 15:28:50.154857 cms_perf-1.0.0/docs/generate_docs.py
--rw-r--r--   0        0        0     1820 2020-08-22 11:57:37.673067 cms_perf-1.0.0/docs/index.rst
--rw-r--r--   0        0        0      795 2020-08-22 11:57:37.673576 cms_perf-1.0.0/docs/make.bat
--rw-r--r--   0        0        0     2309 2020-08-22 11:57:37.674279 cms_perf-1.0.0/docs/source/cli_lang.rst
--rw-r--r--   0        0        0     1829 2020-08-22 11:57:37.674775 cms_perf-1.0.0/docs/source/sched.rst
--rw-r--r--   0        0        0     3311 2020-09-01 08:52:32.740087 cms_perf-1.0.0/docs/source/setup.rst
--rw-r--r--   0        0        0      886 2020-08-23 05:57:54.728966 cms_perf-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2020-07-13 14:26:36.266696 cms_perf-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     2479 2020-07-21 07:34:36.467931 cms_perf-1.0.0/tests/mimicry.py
--rw-r--r--   0        0        0     4139 2020-09-01 09:27:10.671697 cms_perf-1.0.0/tests/test_cli.py
--rw-r--r--   0        0        0     2897 2020-08-24 15:28:50.156515 cms_perf-1.0.0/tests/test_cli_parser.py
--rw-r--r--   0        0        0      362 2020-08-24 15:28:50.157039 cms_perf-1.0.0/tests/test_sensors.py
--rw-r--r--   0        0        0     1101 2020-08-24 15:28:50.157608 cms_perf-1.0.0/tests/test_xrd_load.py
--rw-r--r--   0        0        0      704 2020-09-01 09:27:10.597924 cms_perf-1.0.0/tests/utility.py
--rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 cms_perf-1.0.0/setup.py
--rw-r--r--   0        0        0      215 1970-01-01 00:00:00.000000 cms_perf-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1651 2024-04-18 13:00:23.381007 cms_perf-1.1.0/README.rst
+-rw-r--r--   0        0        0       70 2024-04-18 13:00:23.381007 cms_perf-1.1.0/cms_perf/__init__.py
+-rw-r--r--   0        0        0       93 2024-04-18 13:00:23.381007 cms_perf-1.1.0/cms_perf/__main__.py
+-rw-r--r--   0        0        0     4291 2024-04-18 13:00:23.381007 cms_perf-1.1.0/cms_perf/report.py
+-rw-r--r--   0        0        0        0 2024-04-18 13:00:23.381007 cms_perf-1.1.0/cms_perf/sensors/__init__.py
+-rw-r--r--   0        0        0      861 2024-04-18 13:00:23.381007 cms_perf-1.1.0/cms_perf/sensors/net_load.py
+-rw-r--r--   0        0        0     2566 2024-04-18 13:00:23.381007 cms_perf-1.1.0/cms_perf/sensors/sensor.py
+-rw-r--r--   0        0        0     2544 2024-04-18 13:00:23.381007 cms_perf-1.1.0/cms_perf/sensors/xrd_load.py
+-rw-r--r--   0        0        0        0 2024-04-18 13:00:23.381007 cms_perf-1.1.0/cms_perf/setup/__init__.py
+-rw-r--r--   0        0        0     3586 2024-04-18 13:00:23.381007 cms_perf-1.1.0/cms_perf/setup/cli.py
+-rw-r--r--   0        0        0     9934 2024-04-18 13:00:23.381007 cms_perf-1.1.0/cms_perf/setup/cli_parser.py
+-rw-r--r--   0        0        0      901 2024-04-18 13:00:23.385007 cms_perf-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 cms_perf-1.1.0/PKG-INFO
```

### Comparing `cms_perf-1.0.0/README.rst` & `cms_perf-1.1.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 =================================
 ``cms_perf`` - XRootD load sensor
 =================================
 
-.. image:: https://readthedocs.org/projects/cms_perf/badge/?version=latest
-    :target: http://cms_perf.readthedocs.io/en/latest/?badge=latest
+.. image:: https://readthedocs.org/projects/cms-perf/badge/?version=latest
+    :target: http://cms-perf.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/pypi/v/cms_perf.svg
     :alt: Available on PyPI
     :target: https://pypi.python.org/pypi/cms_perf/
 
 .. image:: https://img.shields.io/github/license/maxfischer2781/cms_perf.svg
     :alt: License
     :target: https://github.com/maxfischer2781/cms_perf/blob/master/LICENSE
 
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4011821.svg
+   :target: https://doi.org/10.5281/zenodo.4011821
+
 Sensor for use in the XRootD ``cms.perf`` directive.
 Measures system load, as well as cpu, memory, and network utilization,
 to enable load-balancing in a cluster of multiple XRootD servers.
 
 With its support for individual re-configuration of each sensor reading,
 ``cms_perf`` allows to fine-tune or even re-define load reporting to your needs.
 No need to hack any scripts, just install, configure, run.
```

### Comparing `cms_perf-1.0.0/cms_perf/report.py` & `cms_perf-1.1.0/cms_perf/report.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 """
 The main loop collecting and reporting values
 """
+
 from typing import Callable
 import sys
 import time
 
 from .setup.cli import CLI
 from .setup import cli_parser
 
 
 class PseudoSched:
     """Imitation of the ``cms.sched`` directive to compute total load"""
 
-    def __init__(self, cpu=0, io=0, mem=0, pag=0, runq=0, maxload=100):
+    def __init__(
+        self,
+        cpu: int = 0,
+        io: int = 0,
+        mem: int = 0,
+        pag: int = 0,
+        runq: int = 0,
+        maxload: int = 100,
+    ):
         self.cpu = cpu
         self.io = io
         self.mem = mem
         self.pag = pag
         self.runq = runq
         self.maxload = maxload
 
@@ -51,67 +60,98 @@
     """
     Iterable that wakes up roughly every ``interval`` seconds
 
     The iterable pauses so that the time spent between iterations
     plus the pause time equals ``interval`` as closely as possible.
     """
     while True:
-        suspended = time.time()
+        suspended = time.monotonic()
         yield
-        duration = time.time() - suspended
+        duration = time.monotonic() - suspended
         time.sleep(max(0.1, interval - duration))
 
 
 def clamp_percentages(value: float) -> int:
     """Restrict a percentage ``value`` to an integer between 0 and 100"""
     return 0 if value < 0.0 else 100 if value > 100.0 else int(value)
 
 
 def run_forever(
     interval: float,
+    rampup: float,
     prunq: Callable[[], float],
     pmem: Callable[[], float],
     pcpu: Callable[[], float],
     ppag: Callable[[], float],
     pio: Callable[[], float],
-    sched: PseudoSched = None,
+    sched: "PseudoSched | None" = None,
 ):
     """Write sensor information to stdout every ``interval`` seconds"""
     sensors = (prunq, pcpu, pmem, ppag, pio)
     try:
-        for _ in every(interval):
-            values = [clamp_percentages(sensor()) for sensor in sensors]
-            print(*values, end="", flush=True)
-            if sched is not None:
-                load, rejected = sched.weight(*values)
-                print(
-                    f" {load}{'!' if rejected else ''}",
-                    end="",
-                    file=sys.stderr,
-                    flush=True,
-                )
-            print(flush=True)
+        if rampup > 1.0:
+            report_rampup(interval, rampup, sched, *sensors)
+        report_forever(interval, sched, *sensors)
     except KeyboardInterrupt:
         pass
 
 
+def report_rampup(
+    interval: float,
+    rampup: float,
+    sched: "PseudoSched | None",
+    *sensors: Callable[[], float],
+) -> None:
+    start_time = time.monotonic()
+    for _ in every(interval):
+        values = [clamp_percentages(sensor()) for sensor in sensors]
+        weight = min((time.monotonic() - start_time) / rampup, 1.0)
+        report_one(
+            [int(value * weight + (1 - weight) * 100) for value in values], sched
+        )
+        if weight >= 1:
+            break
+
+
+def report_forever(
+    interval: float, sched: "PseudoSched | None", *sensors: Callable[[], float]
+) -> None:
+    for _ in every(interval):
+        values = [clamp_percentages(sensor()) for sensor in sensors]
+        report_one(values, sched)
+
+
+def report_one(values: "list[int]", sched: "PseudoSched | None" = None) -> None:
+    print(*values, end="", flush=True)
+    if sched is not None:
+        load, rejected = sched.weight(*values)
+        print(
+            f" {load}{'!' if rejected else ''}",
+            end="",
+            file=sys.stderr,
+            flush=True,
+        )
+    print(flush=True)
+
+
 def main():
     """Run the sensor based on CLI arguments"""
     options = CLI.parse_args()
     prunq, pcpu, pmem, ppag, pio = cli_parser.compile_sensors(
         options.interval,
         options.prunq,
         options.pcpu,
         options.pmem,
         options.ppag,
         options.pio,
     )
     sched = PseudoSched.from_directive(options.sched) if options.sched else None
     run_forever(
         interval=options.interval,
+        rampup=options.rampup,
         prunq=prunq,
         pcpu=pcpu,
         pmem=pmem,
         ppag=ppag,
         pio=pio,
         sched=sched,
     )
```

### Comparing `cms_perf-1.0.0/cms_perf/sensors/net_load.py` & `cms_perf-1.1.0/cms_perf/sensors/net_load.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Sensor for network load
 """
+
 import enum
 
 import psutil
 
 from ..setup.cli_parser import cli_domain, cli_call
```

### Comparing `cms_perf-1.0.0/cms_perf/sensors/sensor.py` & `cms_perf-1.1.0/cms_perf/sensors/sensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Sensors for the canonical cms.perf measurements
 
 .. note::
 
     The paging load has no canonical meaning anymore.
     It exists for backwards compatibility but is assumed 0.
 """
+
 import time
 import enum
 
 import psutil
 
 from ..setup.cli_parser import cli_call, cli_domain
```

### Comparing `cms_perf-1.0.0/cms_perf/sensors/xrd_load.py` & `cms_perf-1.1.0/cms_perf/sensors/xrd_load.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 """
 Sensors for resources used by XRootD processes
 """
+
 from typing import List
 import time
 
 import psutil
 
 from ..setup.cli_parser import cli_call
 
 
-def rescan(interval):
-    return min(interval * 10, 3600)
-
-
 @cli_call(name="xrd.piowait")
 def xrd_piowait(interval: float) -> float:
     """Percentage of time waiting for IO by all XRootD processes"""
     tracker = cached_tracker(interval)
     return 100.0 * tracker.io_wait()
 
 
@@ -31,23 +28,28 @@
 def xrd_threads(interval: float) -> float:
     """Number of threads by all XRootD processes"""
     tracker = cached_tracker(interval)
     return tracker.num_threads()
 
 
 def cached_tracker(interval: float):
+    # how often the tracker scans for processes
+    rescan_interval = max(
+        60,
+        int(min(interval * 10, 3600)) // 10 * 10,
+    )
     try:
-        return TRACKER_CACHE[interval]
+        return TRACKER_CACHE[rescan_interval]
     except KeyError:
-        tracker = XrootdTracker(rescan_interval=rescan(interval))
-        TRACKER_CACHE[interval] = tracker
+        tracker = XrootdTracker(rescan_interval=rescan_interval)
+        TRACKER_CACHE[rescan_interval] = tracker
         return tracker
 
 
-TRACKER_CACHE = {}
+TRACKER_CACHE: "dict[float, XrootdTracker]" = {}
 
 
 def is_alive(proc: psutil.Process) -> bool:
     """Test that `proc` is running but not a zombie"""
     return proc.is_running() and proc.status() != psutil.STATUS_ZOMBIE
 
 
@@ -61,25 +63,28 @@
     def xrootds(self) -> List[psutil.Process]:
         if self._refresh_xrootds():
             self._xrootd_procs = [
                 proc
                 for proc in psutil.process_iter()
                 if proc.name() == "xrootd" and is_alive(proc)
             ]
-            self._next_scan = time.time() + self.rescan_interval
+            self._next_scan = time.monotonic() + self.rescan_interval
         return self._xrootd_procs
 
-    def _refresh_xrootds(self):
+    def _refresh_xrootds(self) -> bool:
         return (
             not self._xrootd_procs
-            or time.time() > self._next_scan
+            or time.monotonic() > self._next_scan
             or not all(is_alive(proc) for proc in self._xrootd_procs)
         )
 
     def io_wait(self) -> float:
-        return max((xrd.cpu_times().iowait for xrd in self.xrootds), default=0)
+        return max(
+            (xrd.cpu_times().iowait for xrd in self.xrootds),  # type: ignore
+            default=0,
+        )
 
     def num_fds(self) -> int:
         return sum(xrd.num_fds() for xrd in self.xrootds)
 
     def num_threads(self) -> int:
         return sum(xrd.num_threads() for xrd in self.xrootds)
```

### Comparing `cms_perf-1.0.0/cms_perf/setup/cli.py` & `cms_perf-1.1.0/cms_perf/setup/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,83 +1,97 @@
 import argparse
 
 from ..setup import cli_parser
 from .. import __version__ as lib_version
 
 # ensure sensors are loaded
-from ..sensors import sensor, xrd_load, net_load  # noqa
+from ..sensors import sensor, xrd_load, net_load  # noqa  # pyright: ignore
 
 
 class ConfigArgumentParser(argparse.ArgumentParser):
     """
     Custom parser for ini-style config files, provided as ``@/path/to/config``
 
     Allows comments and the use of key value notation, as in::
 
         # Set the --prunq option
         prunq = 100.0*loadq/40/ncores
     """
 
-    def convert_arg_line_to_args(self, arg_line):
+    def convert_arg_line_to_args(self, arg_line: str) -> "list[str]":
         arg_line, *_ = arg_line.split("#", 1)
         if not arg_line.strip():
             return []
         key, _, value = [elem.strip() for elem in arg_line.partition("=")]
         key = key if key.startswith("--") else ("--" + key)
         return [key, value] if value else [key]
 
 
-INTERVAL_UNITS = {"": 1, "s": 1, "m": 60, "h": 60 * 60}
+INTERVAL_UNITS = {
+    "": 1,
+    "s": 1,
+    "m": 60,
+    "h": 60 * 60,
+    "d": 60 * 60 * 24,
+    "w": 60 * 60 * 24 * 7,
+}
 
 
 def duration(literal: str) -> float:
     """
     Parse an XRootD duration literal as a float representing seconds
 
     A literal consists of a float literal, e.g. ``12`` or ``17.5``,
     and an optional unit ``s`` (for seconds), ``m`` (for minutes),
-    or ``h`` (for hours). If no unit is given, ``s`` is assumed.
+    and so on. If no unit is given, ``s`` is assumed.
     """
     literal = literal.strip()
     value, unit = (
         (literal, "") if literal[-1].isdigit() else (literal[:-1], literal[-1])
     )
     try:
         scale = INTERVAL_UNITS[unit]
     except KeyError:
         expected = ", ".join(map(repr, INTERVAL_UNITS))
         raise argparse.ArgumentTypeError(
-            f"{unit!r} is not a valid time unit – expected one of {expected}"
-        )
+            f"{unit!r} is not a valid time unit - expected one of {expected}"
+        ) from None
     return float(value) * scale
 
 
 CLI = ConfigArgumentParser(
     description="Performance Sensor for XRootD cms.perf directive",
     epilog=(
         "In regular intervals, outputs a single line with percentages of: "
         "system load, "
         "cpu utilization, "
         "memory utilizaion, "
         "paging load, and "
         "network utilization. "
         "The paging load exists for historical reasons; "
         "it cannot be reliably computed."
+        "Time can be suffixed with s, m, h, d or w."
     ),
     fromfile_prefix_chars="@",
 )
 CLI.add_argument(
     "--version",
     action="version",
     version=lib_version,
 )
 CLI.add_argument(
     "--interval",
     default="60s",
-    help="Interval between output; suffixed by s, m, or h [default: %(default)s]",
+    help="Interval between output [default: %(default)s]",
+    type=duration,
+)
+CLI.add_argument(
+    "--rampup",
+    default="0s",
+    help="Duration in which usage is dampened [default: %(default)s]",
     type=duration,
 )
 CLI.add_argument(
     "--prunq",
     default="100.0*loadq/ncores",
     type=cli_parser.parse_sensor,
     help="Expression to compute system load percentage [default: %(default)s]",
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cms_perf-1.0.0/cms_perf/setup/cli_parser.py` & `cms_perf-1.1.0/cms_perf/setup/cli_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,43 +3,45 @@
 
 The syntax is loosely speaking:
 * float math including ``*``, ``/``, ``+``, ``-`` and parentheses
 * calls with and without arguments
 * constants such as enums
 and everything compiles down to Python source code.
 
-The math part is an explicitly defined.
-Both calls and constants are automatically generated from Python objects.
+The math part is an explicitly defined infix parser rule.
+The parts for both calls and constants are automatically generated from Python objects.
 """
+
 from typing import TypeVar, Optional, Dict, NamedTuple, List, Callable, Type
-from typing_extensions import Protocol
 import inspect
 import enum
 
 import pyparsing as pp
 
 pp.ParserElement.enablePackrat()
 
 
 # Auto-generated expressions
-GENERATED = pp.Forward().setName("TERM")
+GENERATED: pp.Forward = pp.Forward().setName("TERM")  # type: ignore
 
 
 # Number literals – float should be precise enough for everything
 NUMBER = pp.Regex(r"-?\d+\.?\d*").setName("NUMBER")
 
 
-@NUMBER.setParseAction
+@NUMBER.setParseAction  # type: ignore
 def transpile(result: pp.ParseResults) -> str:
-    return result[0]
+    """Capture float literals directly"""
+    return result[0]  # type: ignore
 
 
 # Mathematical Operators
-def transpile_binop(result: pp.ParseResults):
-    (*terms,) = result[0]
+def transpile_binop(result: pp.ParseResults) -> str:
+    """Capture binary operations such as ``12 * b`` and add precedence via ``()``"""
+    terms = list(result[0])  # type: ignore
     return f"({' '.join(terms)})"
 
 
 EXPRESSION = pp.infixNotation(
     (NUMBER | GENERATED),
     [
         (pp.oneOf(operators), 2, pp.opAssoc.LEFT, transpile_binop)
@@ -47,60 +49,55 @@
     ],
 ).setName('(NUMBER | TERM), [ ("*" | "/" | "+" | "-"), (NUMBER | TERM | EXPRESSION)]')
 
 
 def parse(code: str) -> str:
     """Parse a CLI code string to Python source code"""
     try:
-        return EXPRESSION.parseString(code, parseAll=True)[0]
+        return EXPRESSION.parseString(code, parseAll=True)[0]  # type: ignore
     except pp.ParseException as pe:
         raise SyntaxError(
             str(pe), ("<cms_perf.cli_parser code>", pe.col, pe.loc, code)
         ) from None
 
 
 # Sensor Plugins
-class CLICall(Protocol):
-    """A callable that can be registered for the CLI to provide values"""
-
-    def __call__(self, *args, **kwargs) -> float:
-        ...
-
-
-class Transform(Protocol):
-    """A callable that can be registered for the CLI to transform values"""
-
-    def __call__(self, *args: float) -> float:
-        ...
+CLICall = Callable[..., float]
 
 
 S = TypeVar("S", bound=CLICall)
 
 
 class CallInfo(NamedTuple):
+    """Information for running `cli_name(...)` via `call`"""
+
     call: Callable[..., float]
     cli_name: str
 
 
 class DomainInfo(NamedTuple):
+    """Information for translating literal of `cli_name` in a type `domain`"""
+
     domain: type
     cli_name: str
     parser: pp.ParserElement
 
 
 # transpiled_name => CallInfo
 KNOWN_CALLABLES: Dict[str, CallInfo] = {}
 KNOWN_DOMAINS: Dict[str, DomainInfo] = {}
 
 KNOWN_DOMAINS_MAP: Dict[type, DomainInfo] = {}
 
 
 # automatic parser generation
-def _extend_generated(*rules, base=GENERATED):
-    base << pp.MatchFirst((*(base.expr.exprs if base.expr else ()), *rules))
+def _extend_generated(*rules: pp.ParserElement, base: pp.Forward = GENERATED):
+    base <<= pp.MatchFirst(
+        (*(base.expr.exprs if base.expr else ()), *rules)  # type:ignore
+    )
 
 
 _COMPILEABLE_PARAMETERS = (
     inspect.Parameter.POSITIONAL_OR_KEYWORD,
     inspect.Parameter.VAR_POSITIONAL,
 )
 
@@ -115,80 +112,89 @@
         domain_info = KNOWN_DOMAINS_MAP[annotation]
         return domain_info.parser.copy().setName(
             f"{parameter.name}={domain_info.cli_name}"
         )
     return EXPRESSION.copy().setName(f"{parameter.name}=TERM")
 
 
-def _compile_cli_call(call_name: str, transpiled_name: str, call: Callable):
+def _compile_cli_call(
+    call_name: str, transpiled_name: str, call: CLICall
+) -> "list[pp.ParserElement]":
     """Compile a call with a given argument arity to a transpile expression"""
-    transpilers = []
+    transpilers: "list[pp.ParserElement]" = []
     parameters = inspect.signature(call).parameters
     implicit_interval = "interval" in parameters
     if implicit_interval:
-        assert next(iter(parameters)) == "interval", "interval must be first"
+        assert (
+            next(iter(parameters)) == "interval"
+        ), "interval must be the first parameter"
         parameters = {k: v for k, v in parameters.items() if k != "interval"}
     for parameter in parameters.values():
         assert parameter.kind in _COMPILEABLE_PARAMETERS, f"Cannot compile {parameter}"
+    # if all parameters are optional, allow call without arguments
     if all(
         param.default is not inspect.Parameter.empty
         or param.kind == inspect.Parameter.VAR_POSITIONAL
         for param in parameters.values()
     ):
         default_call = pp.Suppress(call_name).setName(f'"{call_name}"')
 
-        @default_call.setParseAction
-        def transpile_default(result: pp.ParseResults) -> str:
+        @default_call.setParseAction  # type: ignore
+        def transpile_default(result: pp.ParseResults) -> str:  # type: ignore[reportUnusedFunction]
             arguments = "interval" if implicit_interval else ""
             return f"{transpiled_name}({arguments})"
 
         transpilers.append(default_call)
+    # if parameters may be passed, allow call with parametrised arguments
     if len(parameters):
-        argument_parsers = []
+        argument_parsers: "list[pp.ParserElement]" = []
         for parameter in parameters.values():
+            # individual parameter
             if parameter.kind != inspect.Parameter.VAR_POSITIONAL:
                 if argument_parsers:
                     argument_parsers.append(pp.Suppress(","))
                 argument_parsers.append(_compile_parameter(parameter))
+            # variadic parameter, compile to a list of parameters
             else:
                 param_parser = pp.delimitedList(_compile_parameter(parameter))
                 if argument_parsers:
                     argument_parsers.append(
                         pp.Optional(pp.Suppress(",") - param_parser)
                     )
                 else:
                     argument_parsers.append(pp.Optional(param_parser))
         signature = pp.And((LEFT_PAR, *argument_parsers, RIGHT_PAR))
         parameter_call = pp.Suppress(call_name).setName(f'"{call_name}"') + signature
 
-        @parameter_call.setParseAction
-        def transpile_with_args(result: pp.ParseResults) -> str:
+        @parameter_call.setParseAction  # type: ignore
+        def transpile_with_args(result: pp.ParseResults) -> str:  # type: ignore[reportUnusedFunction]
             arguments = ("interval, " if implicit_interval else "") + ", ".join(result)
             return f"{transpiled_name}({arguments})"
 
         transpilers.append(parameter_call)
     return transpilers[::-1]
 
 
 # registration decorators
-def cli_call(name: Optional[str] = None):
+def cli_call(name: Optional[str] = None) -> Callable[[S], S]:
     """
     Register a sensor or transformation for the CLI with its own name or ``name``
     """
     assert not callable(name), "cli_call must be called before decorating"
 
     def register(call: S) -> S:
         _register_cli_callable(call, name)
         return call
 
     return register
 
 
 def _register_cli_callable(call: S, cli_name: Optional[str]) -> S:
-    cli_name = cli_name if cli_name is not None else call.__name__
+    cli_name = cli_name if cli_name is not None else call.__name__  # type: ignore
+    assert isinstance(cli_name, str)
     source_name = cli_name.replace(".", "_")
     assert (
         source_name not in KNOWN_CALLABLES
     ), f"cannot re-register CLI callable {source_name}"
     KNOWN_CALLABLES[source_name] = CallInfo(call, cli_name)
     _extend_generated(*_compile_cli_call(cli_name, source_name, call))
     return call
@@ -202,16 +208,16 @@
     Register a value domain for the CLI displayed with its own name or ``name``
     """
 
     def register(domain: TP) -> TP:
         if issubclass(domain, enum.Enum):
             _register_enum(domain, name)
         else:
-            raise TypeError(f"Cannot register CLI domain: {domain}")
-        return domain
+            raise TypeError(f"Can only register Enum domain, not {domain}")
+        return domain  # type: ignore
 
     return register
 
 
 def _register_enum(domain: Type[enum.Enum], cli_name: Optional[str]):
     cli_name = cli_name if cli_name is not None else domain.__name__
     source_name = cli_name.replace(".", "_")
@@ -219,17 +225,17 @@
         source_name not in KNOWN_DOMAINS
     ), f"cannot re-register CLI domain {source_name}"
     cases = sorted(domain.__members__, reverse=True)
     match_case = pp.MatchFirst(tuple(map(pp.Keyword, cases))).setName(
         " | ".join(f'"{case}"' for case in cases)
     )
 
-    @match_case.setParseAction
-    def transpile_enum_case(result: pp.ParseResults):
-        (case,) = result
+    @match_case.setParseAction  # type: ignore
+    def transpile_enum_case(result: pp.ParseResults) -> str:  # type: ignore[reportUnusedFunction]
+        case: str = result[0]  # type: ignore
         return f"{source_name}['{case}']"
 
     KNOWN_DOMAINS_MAP[domain] = KNOWN_DOMAINS[source_name] = DomainInfo(
         domain, cli_name, match_case
     )
 
 
@@ -253,35 +259,35 @@
     return eval(code, {}, {})
 
 
 def compile_sensors(
     interval: float, *sensors: Callable[..., Callable[[], float]]
 ) -> List[Callable[[], float]]:
     raw_sensors = {name: sf_info.call for name, sf_info in KNOWN_CALLABLES.items()}
-    raw_domains = {name: dm_info.domain for name, dm_info in KNOWN_DOMAINS.items()}
+    raw_domains = {name: dm_info.domain for name, dm_info in KNOWN_DOMAINS.items()}  # type: ignore[reportUnknownMemberType]
     return [
         factory(interval=interval, **raw_sensors, **raw_domains) for factory in sensors
     ]
 
 
 # CLI transformations
 @cli_call(name="max")
-def maximum(a, b, *others):
+def maximum(a: float, b: float, *others: float) -> float:
     """The maximum value of all arguments"""
     return max(a, b, *others)
 
 
 @cli_call(name="min")
-def minimum(a, b, *others):
+def minimum(a: float, b: float, *others: float):
     """The minimum value of all arguments"""
     return min(a, b, *others)
 
 
 if __name__ == "__main__":
     # provide debug information on the parser
-    from ..sensors import sensor, net_load, xrd_load  # noqa
+    from ..sensors import sensor, net_load, xrd_load  # noqa  # pyright: ignore
     from . import cli_parser  # noqa
 
     print("EXPRESSION:", cli_parser.EXPRESSION)
     print("TERM:", cli_parser.GENERATED.expr)
     for domain in cli_parser.KNOWN_DOMAINS.values():
         print(f"{domain.cli_name}: {domain.parser}")
```

### Comparing `cms_perf-1.0.0/pyproject.toml` & `cms_perf-1.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -11,25 +11,27 @@
 keywords = "xrootd cms.perf"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
 ]
-requires = ["psutil >=5.6.2", "pyparsing", "typing-extensions"]
+requires = ["psutil >=5.6.2", "pyparsing"]
 
 [tool.flit.scripts]
 cms_perf = "cms_perf.report:main"
 
 [tool.flit.metadata.requires-extra]
 test = [
-    "pytest >=4.3.0",
+    "pytest",
+    "coverage",
+    "pytest-cov",
     "codecov",
     "flake8",
     "flake8-bugbear",
-    "black",
+    "black >= 24.4.0",
     "setproctitle",
 ]
 doc = ["sphinx", "sphinx-tabs"]
 
 [tool.black]
 target-version = ['py36', 'py37', 'py38']
```

