# Comparing `tmp/exceptiongroup-1.1.3.tar.gz` & `tmp/exceptiongroup-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exceptiongroup-1.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "exceptiongroup-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `exceptiongroup-1.1.3.tar` & `exceptiongroup-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
--rw-r--r--   0        0        0     3704 2023-08-14 12:26:13.095081 exceptiongroup-1.1.3/LICENSE
--rw-r--r--   0        0        0     5276 2023-08-14 12:26:13.095081 exceptiongroup-1.1.3/README.rst
--rw-r--r--   0        0        0     2064 2023-08-14 12:26:13.095081 exceptiongroup-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      920 2023-08-14 12:26:13.095081 exceptiongroup-1.1.3/src/exceptiongroup/__init__.py
--rw-r--r--   0        0        0     4541 2023-08-14 12:26:13.095081 exceptiongroup-1.1.3/src/exceptiongroup/_catch.py
--rw-r--r--   0        0        0    11009 2023-08-14 12:26:13.095081 exceptiongroup-1.1.3/src/exceptiongroup/_exceptions.py
--rw-r--r--   0        0        0    19475 2023-08-14 12:26:13.095081 exceptiongroup-1.1.3/src/exceptiongroup/_formatting.py
--rw-r--r--   0        0        0      160 2023-08-14 12:26:22.119340 exceptiongroup-1.1.3/src/exceptiongroup/_version.py
--rw-r--r--   0        0        0        0 2023-08-14 12:26:13.095081 exceptiongroup-1.1.3/src/exceptiongroup/py.typed
--rw-r--r--   0        0        0        0 2023-08-14 12:26:13.095081 exceptiongroup-1.1.3/tests/__init__.py
--rw-r--r--   0        0        0       84 2023-08-14 12:26:13.095081 exceptiongroup-1.1.3/tests/conftest.py
--rw-r--r--   0        0        0     6810 2023-08-14 12:26:13.095081 exceptiongroup-1.1.3/tests/test_catch.py
--rw-r--r--   0        0        0     5609 2023-08-14 12:26:13.095081 exceptiongroup-1.1.3/tests/test_catch_py311.py
--rw-r--r--   0        0        0    30667 2023-08-14 12:26:13.095081 exceptiongroup-1.1.3/tests/test_exceptions.py
--rw-r--r--   0        0        0    18256 2023-08-14 12:26:13.095081 exceptiongroup-1.1.3/tests/test_formatting.py
--rw-r--r--   0        0        0     6083 1970-01-01 00:00:00.000000 exceptiongroup-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3704 2023-11-21 08:41:28.130623 exceptiongroup-1.2.0/LICENSE
+-rw-r--r--   0        0        0     5796 2023-11-21 08:41:28.130623 exceptiongroup-1.2.0/README.rst
+-rw-r--r--   0        0        0     2184 2023-11-21 08:41:28.130623 exceptiongroup-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1049 2023-11-21 08:41:28.130623 exceptiongroup-1.2.0/src/exceptiongroup/__init__.py
+-rw-r--r--   0        0        0     4669 2023-11-21 08:41:28.130623 exceptiongroup-1.2.0/src/exceptiongroup/_catch.py
+-rw-r--r--   0        0        0    11010 2023-11-21 08:41:28.130623 exceptiongroup-1.2.0/src/exceptiongroup/_exceptions.py
+-rw-r--r--   0        0        0    21005 2023-11-21 08:41:28.130623 exceptiongroup-1.2.0/src/exceptiongroup/_formatting.py
+-rw-r--r--   0        0        0     1338 2023-11-21 08:41:28.130623 exceptiongroup-1.2.0/src/exceptiongroup/_suppress.py
+-rw-r--r--   0        0        0      411 2023-11-21 08:41:35.778687 exceptiongroup-1.2.0/src/exceptiongroup/_version.py
+-rw-r--r--   0        0        0        0 2023-11-21 08:41:28.130623 exceptiongroup-1.2.0/src/exceptiongroup/py.typed
+-rw-r--r--   0        0        0        0 2023-11-21 08:41:28.130623 exceptiongroup-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      479 2023-11-21 08:41:28.130623 exceptiongroup-1.2.0/tests/apport_excepthook.py
+-rw-r--r--   0        0        0       84 2023-11-21 08:41:28.130623 exceptiongroup-1.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     1925 2023-11-21 08:41:28.130623 exceptiongroup-1.2.0/tests/test_apport_monkeypatching.py
+-rw-r--r--   0        0        0     7163 2023-11-21 08:41:28.130623 exceptiongroup-1.2.0/tests/test_catch.py
+-rw-r--r--   0        0        0     5958 2023-11-21 08:41:28.130623 exceptiongroup-1.2.0/tests/test_catch_py311.py
+-rw-r--r--   0        0        0    30667 2023-11-21 08:41:28.130623 exceptiongroup-1.2.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0    18256 2023-11-21 08:41:28.130623 exceptiongroup-1.2.0/tests/test_formatting.py
+-rw-r--r--   0        0        0      442 2023-11-21 08:41:28.130623 exceptiongroup-1.2.0/tests/test_suppress.py
+-rw-r--r--   0        0        0     6603 1970-01-01 00:00:00.000000 exceptiongroup-1.2.0/PKG-INFO
```

### Comparing `exceptiongroup-1.1.3/LICENSE` & `exceptiongroup-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exceptiongroup-1.1.3/README.rst` & `exceptiongroup-1.2.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,16 @@
   correctly handle exception groups even when monkey patching is disabled, or blocked by
   another custom exception hook:
 
   * ``traceback.format_exception()``
   * ``traceback.format_exception_only()``
   * ``traceback.print_exception()``
   * ``traceback.print_exc()``
+* A backported version of ``contextlib.suppress()`` from Python 3.12.1 which also
+  handles suppressing exceptions inside exception groups
 
 If this package is imported on Python 3.11 or later, the built-in implementations of the
 exception group classes are used instead, ``TracebackException`` is not monkey patched
 and the exception hook won't be installed.
 
 See the `standard library documentation`_ for more information on exception groups.
 
@@ -80,14 +82,26 @@
         RuntimeError: runtime_err_handler
     }):
         ...
 
 **NOTE**: Just like with ``except*``, you cannot handle ``BaseExceptionGroup`` or
 ``ExceptionGroup`` with ``catch()``.
 
+Suppressing exceptions
+======================
+
+This library contains a backport of the ``contextlib.suppress()`` context manager from
+Python 3.12.1. It allows you to selectively ignore certain exceptions, even when they're
+inside exception groups::
+
+    from exceptiongroup import suppress
+
+    with suppress(RuntimeError):
+        raise ExceptionGroup("", [RuntimeError("boo")])
+
 Notes on monkey patching
 ========================
 
 To make exception groups render properly when an unhandled exception group is being
 printed out, this package does two things when it is imported on any Python version
 earlier than 3.11:
```

### Comparing `exceptiongroup-1.1.3/pyproject.toml` & `exceptiongroup-1.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -41,23 +41,26 @@
 
 [tool.setuptools_scm]
 version_scheme = "post-release"
 local_scheme = "dirty-tag"
 write_to = "src/exceptiongroup/_version.py"
 
 [tool.ruff]
-line-length = 88
 select = [
     "E", "F", "W",  # default flake-8
     "I",            # isort
     "ISC",          # flake8-implicit-str-concat
     "PGH",          # pygrep-hooks
     "RUF100",       # unused noqa (yesqa)
+    "UP",           # pyupgrade
 ]
-target-version = "py37"
+
+[tool.ruff.pyupgrade]
+# Preserve types, even if a file imports `from __future__ import annotations`.
+keep-runtime-typing = true
 
 [tool.ruff.isort]
 known-first-party = ["exceptiongroup"]
 
 [tool.pytest.ini_options]
 addopts = "-rsx --tb=short --strict-config --strict-markers"
 testpaths = ["tests"]
```

### Comparing `exceptiongroup-1.1.3/src/exceptiongroup/__init__.py` & `exceptiongroup-1.2.0/src/exceptiongroup/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,15 @@
     "BaseExceptionGroup",
     "ExceptionGroup",
     "catch",
     "format_exception",
     "format_exception_only",
     "print_exception",
     "print_exc",
+    "suppress",
 ]
 
 import os
 import sys
 
 from ._catch import catch
 from ._version import version as __version__  # noqa: F401
@@ -34,7 +35,12 @@
         format_exception_only,
         print_exc,
         print_exception,
     )
 
     BaseExceptionGroup = BaseExceptionGroup
     ExceptionGroup = ExceptionGroup
+
+if sys.version_info < (3, 12, 1):
+    from ._suppress import suppress
+else:
+    from contextlib import suppress
```

### Comparing `exceptiongroup-1.1.3/src/exceptiongroup/_catch.py` & `exceptiongroup-1.2.0/src/exceptiongroup/_catch.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,18 @@
             if matched:
                 try:
                     try:
                         raise matched
                     except BaseExceptionGroup:
                         result = handler(matched)
                 except BaseExceptionGroup as new_exc:
-                    new_exceptions.extend(new_exc.exceptions)
+                    if new_exc is matched:
+                        new_exceptions.append(new_exc)
+                    else:
+                        new_exceptions.extend(new_exc.exceptions)
                 except BaseException as new_exc:
                     new_exceptions.append(new_exc)
                 else:
                     if inspect.iscoroutine(result):
                         raise TypeError(
                             f"Error trying to handle {matched!r} with {handler!r}. "
                             "Exception handler must be a sync function."
```

### Comparing `exceptiongroup-1.1.3/src/exceptiongroup/_exceptions.py` & `exceptiongroup-1.2.0/src/exceptiongroup/_exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     return False
 
 
 def get_condition_filter(
     condition: type[_BaseExceptionT]
     | tuple[type[_BaseExceptionT], ...]
-    | Callable[[_BaseExceptionT_co], bool]
+    | Callable[[_BaseExceptionT_co], bool],
 ) -> Callable[[_BaseExceptionT_co], bool]:
     if isclass(condition) and issubclass(
         cast(Type[BaseException], condition), BaseException
     ):
         return partial(check_direct_subclass, parents=(condition,))
     elif isinstance(condition, tuple):
         if all(isclass(x) and issubclass(x, BaseException) for x in condition):
```

### Comparing `exceptiongroup-1.1.3/src/exceptiongroup/_formatting.py` & `exceptiongroup-1.2.0/src/exceptiongroup/_formatting.py`

 * *Files 8% similar despite different names*

```diff
@@ -355,14 +355,54 @@
         PatchedTracebackException.format
     )
     traceback.TracebackException.format_exception_only = (  # type: ignore[assignment]
         PatchedTracebackException.format_exception_only
     )
     sys.excepthook = exceptiongroup_excepthook
 
+# Ubuntu's system Python has a sitecustomize.py file that imports
+# apport_python_hook and replaces sys.excepthook.
+#
+# The custom hook captures the error for crash reporting, and then calls
+# sys.__excepthook__ to actually print the error.
+#
+# We don't mind it capturing the error for crash reporting, but we want to
+# take over printing the error. So we monkeypatch the apport_python_hook
+# module so that instead of calling sys.__excepthook__, it calls our custom
+# hook.
+#
+# More details: https://github.com/python-trio/trio/issues/1065
+if getattr(sys.excepthook, "__name__", None) in (
+    "apport_excepthook",
+    # on ubuntu 22.10 the hook was renamed to partial_apport_excepthook
+    "partial_apport_excepthook",
+):
+    # patch traceback like above
+    traceback.TracebackException.__init__ = (  # type: ignore[assignment]
+        PatchedTracebackException.__init__
+    )
+    traceback.TracebackException.format = (  # type: ignore[assignment]
+        PatchedTracebackException.format
+    )
+    traceback.TracebackException.format_exception_only = (  # type: ignore[assignment]
+        PatchedTracebackException.format_exception_only
+    )
+
+    from types import ModuleType
+
+    import apport_python_hook
+
+    assert sys.excepthook is apport_python_hook.apport_excepthook
+
+    # monkeypatch the sys module that apport has imported
+    fake_sys = ModuleType("exceptiongroup_fake_sys")
+    fake_sys.__dict__.update(sys.__dict__)
+    fake_sys.__excepthook__ = exceptiongroup_excepthook
+    apport_python_hook.sys = fake_sys
+
 
 @singledispatch
 def format_exception_only(__exc: BaseException) -> List[str]:
     return list(
         PatchedTracebackException(
             type(__exc), __exc, None, compact=True
         ).format_exception_only()
```

### Comparing `exceptiongroup-1.1.3/tests/test_catch.py` & `exceptiongroup-1.2.0/tests/test_catch.py`

 * *Files 6% similar despite different names*

```diff
@@ -204,7 +204,19 @@
         coro = handler(eg)
         request.addfinalizer(coro.close)
         return coro
 
     with pytest.raises(TypeError, match="Exception handler must be a sync function."):
         with catch({TypeError: delegate}):
             raise ExceptionGroup("message", [TypeError("uh-oh")])
+
+
+def test_bare_reraise_from_naked_exception():
+    def handler(eg):
+        raise
+
+    with pytest.raises(ExceptionGroup) as excgrp, catch({Exception: handler}):
+        raise KeyError("foo")
+
+    assert len(excgrp.value.exceptions) == 1
+    assert isinstance(excgrp.value.exceptions[0], KeyError)
+    assert str(excgrp.value.exceptions[0]) == "'foo'"
```

### Comparing `exceptiongroup-1.1.3/tests/test_catch_py311.py` & `exceptiongroup-1.2.0/tests/test_catch_py311.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,7 +172,19 @@
             raise
         except* TypeError:
             pass
 
     assert excgrp.value is not middle_exc
     assert excgrp.value.__cause__ is first_exc
     assert excgrp.value.__context__ is first_exc
+
+
+def test_bare_reraise_from_naked_exception():
+    with pytest.raises(ExceptionGroup) as excgrp:
+        try:
+            raise KeyError("foo")
+        except* KeyError:
+            raise
+
+    assert len(excgrp.value.exceptions) == 1
+    assert isinstance(excgrp.value.exceptions[0], KeyError)
+    assert str(excgrp.value.exceptions[0]) == "'foo'"
```

### Comparing `exceptiongroup-1.1.3/tests/test_exceptions.py` & `exceptiongroup-1.2.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `exceptiongroup-1.1.3/tests/test_formatting.py` & `exceptiongroup-1.2.0/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `exceptiongroup-1.1.3/PKG-INFO` & `exceptiongroup-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exceptiongroup
-Version: 1.1.3
+Version: 1.2.0
 Summary: Backport of PEP 654 (exception groups)
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -41,14 +41,16 @@
   correctly handle exception groups even when monkey patching is disabled, or blocked by
   another custom exception hook:
 
   * ``traceback.format_exception()``
   * ``traceback.format_exception_only()``
   * ``traceback.print_exception()``
   * ``traceback.print_exc()``
+* A backported version of ``contextlib.suppress()`` from Python 3.12.1 which also
+  handles suppressing exceptions inside exception groups
 
 If this package is imported on Python 3.11 or later, the built-in implementations of the
 exception group classes are used instead, ``TracebackException`` is not monkey patched
 and the exception hook won't be installed.
 
 See the `standard library documentation`_ for more information on exception groups.
 
@@ -99,14 +101,26 @@
         RuntimeError: runtime_err_handler
     }):
         ...
 
 **NOTE**: Just like with ``except*``, you cannot handle ``BaseExceptionGroup`` or
 ``ExceptionGroup`` with ``catch()``.
 
+Suppressing exceptions
+======================
+
+This library contains a backport of the ``contextlib.suppress()`` context manager from
+Python 3.12.1. It allows you to selectively ignore certain exceptions, even when they're
+inside exception groups::
+
+    from exceptiongroup import suppress
+
+    with suppress(RuntimeError):
+        raise ExceptionGroup("", [RuntimeError("boo")])
+
 Notes on monkey patching
 ========================
 
 To make exception groups render properly when an unhandled exception group is being
 printed out, this package does two things when it is imported on any Python version
 earlier than 3.11:
```

