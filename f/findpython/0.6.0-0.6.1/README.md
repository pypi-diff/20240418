# Comparing `tmp/findpython-0.6.0.tar.gz` & `tmp/findpython-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findpython-0.6.0.tar", last modified: Tue Mar 26 03:59:08 2024, max compression
+gzip compressed data, was "findpython-0.6.1.tar", last modified: Thu Apr 18 11:15:58 2024, max compression
```

## Comparing `findpython-0.6.0.tar` & `findpython-0.6.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1075 2024-03-26 03:58:57.046483 findpython-0.6.0/LICENSE
--rw-r--r--   0        0        0     4646 2024-03-26 03:58:57.046483 findpython-0.6.0/README.md
--rw-r--r--   0        0        0     1576 2024-03-26 03:59:08.018398 findpython-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1928 2024-03-26 03:58:57.046483 findpython-0.6.0/src/findpython/__init__.py
--rw-r--r--   0        0        0     2735 2024-03-26 03:58:57.046483 findpython-0.6.0/src/findpython/__main__.py
--rw-r--r--   0        0        0       22 2024-03-26 03:59:08.018398 findpython-0.6.0/src/findpython/__version__.py
--rw-r--r--   0        0        0     7665 2024-03-26 03:58:57.046483 findpython-0.6.0/src/findpython/finder.py
--rw-r--r--   0        0        0      442 2024-03-26 03:58:57.046483 findpython-0.6.0/src/findpython/pep514tools/__init__.py
--rw-r--r--   0        0        0      254 2024-03-26 03:58:57.046483 findpython-0.6.0/src/findpython/pep514tools/__main__.py
--rw-r--r--   0        0        0     6567 2024-03-26 03:58:57.046483 findpython-0.6.0/src/findpython/pep514tools/_registry.py
--rw-r--r--   0        0        0     4638 2024-03-26 03:58:57.046483 findpython-0.6.0/src/findpython/pep514tools/environment.py
--rw-r--r--   0        0        0      846 2024-03-26 03:58:57.046483 findpython-0.6.0/src/findpython/providers/__init__.py
--rw-r--r--   0        0        0     1058 2024-03-26 03:58:57.046483 findpython-0.6.0/src/findpython/providers/asdf.py
--rw-r--r--   0        0        0     1823 2024-03-26 03:58:57.046483 findpython-0.6.0/src/findpython/providers/base.py
--rw-r--r--   0        0        0      759 2024-03-26 03:58:57.046483 findpython-0.6.0/src/findpython/providers/macos.py
--rw-r--r--   0        0        0      662 2024-03-26 03:58:57.046483 findpython-0.6.0/src/findpython/providers/path.py
--rw-r--r--   0        0        0     1072 2024-03-26 03:58:57.050483 findpython-0.6.0/src/findpython/providers/pyenv.py
--rw-r--r--   0        0        0     1138 2024-03-26 03:58:57.050483 findpython-0.6.0/src/findpython/providers/rye.py
--rw-r--r--   0        0        0     1395 2024-03-26 03:58:57.050483 findpython-0.6.0/src/findpython/providers/winreg.py
--rw-r--r--   0        0        0     7104 2024-03-26 03:58:57.050483 findpython-0.6.0/src/findpython/python.py
--rw-r--r--   0        0        0     4424 2024-03-26 03:58:57.050483 findpython-0.6.0/src/findpython/utils.py
--rw-r--r--   0        0        0        0 2024-03-26 03:58:57.050483 findpython-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0     1919 2024-03-26 03:58:57.050483 findpython-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0      612 2024-03-26 03:58:57.050483 findpython-0.6.0/tests/test_cli.py
--rw-r--r--   0        0        0     4780 2024-03-26 03:58:57.050483 findpython-0.6.0/tests/test_finder.py
--rw-r--r--   0        0        0     3321 2024-03-26 03:58:57.050483 findpython-0.6.0/tests/test_posix.py
--rw-r--r--   0        0        0      681 2024-03-26 03:58:57.050483 findpython-0.6.0/tests/test_utils.py
--rw-r--r--   0        0        0     5275 1970-01-01 00:00:00.000000 findpython-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-04-18 11:15:49.651351 findpython-0.6.1/LICENSE
+-rw-r--r--   0        0        0     4646 2024-04-18 11:15:49.651351 findpython-0.6.1/README.md
+-rw-r--r--   0        0        0     1576 2024-04-18 11:15:58.019341 findpython-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1928 2024-04-18 11:15:49.651351 findpython-0.6.1/src/findpython/__init__.py
+-rw-r--r--   0        0        0     2735 2024-04-18 11:15:49.651351 findpython-0.6.1/src/findpython/__main__.py
+-rw-r--r--   0        0        0       22 2024-04-18 11:15:58.015341 findpython-0.6.1/src/findpython/__version__.py
+-rw-r--r--   0        0        0     7665 2024-04-18 11:15:49.651351 findpython-0.6.1/src/findpython/finder.py
+-rw-r--r--   0        0        0      442 2024-04-18 11:15:49.651351 findpython-0.6.1/src/findpython/pep514tools/__init__.py
+-rw-r--r--   0        0        0      254 2024-04-18 11:15:49.651351 findpython-0.6.1/src/findpython/pep514tools/__main__.py
+-rw-r--r--   0        0        0     6567 2024-04-18 11:15:49.651351 findpython-0.6.1/src/findpython/pep514tools/_registry.py
+-rw-r--r--   0        0        0     4638 2024-04-18 11:15:49.651351 findpython-0.6.1/src/findpython/pep514tools/environment.py
+-rw-r--r--   0        0        0      846 2024-04-18 11:15:49.651351 findpython-0.6.1/src/findpython/providers/__init__.py
+-rw-r--r--   0        0        0     1058 2024-04-18 11:15:49.651351 findpython-0.6.1/src/findpython/providers/asdf.py
+-rw-r--r--   0        0        0     1823 2024-04-18 11:15:49.651351 findpython-0.6.1/src/findpython/providers/base.py
+-rw-r--r--   0        0        0      759 2024-04-18 11:15:49.651351 findpython-0.6.1/src/findpython/providers/macos.py
+-rw-r--r--   0        0        0      662 2024-04-18 11:15:49.651351 findpython-0.6.1/src/findpython/providers/path.py
+-rw-r--r--   0        0        0     1072 2024-04-18 11:15:49.651351 findpython-0.6.1/src/findpython/providers/pyenv.py
+-rw-r--r--   0        0        0     1138 2024-04-18 11:15:49.651351 findpython-0.6.1/src/findpython/providers/rye.py
+-rw-r--r--   0        0        0     1602 2024-04-18 11:15:49.651351 findpython-0.6.1/src/findpython/providers/winreg.py
+-rw-r--r--   0        0        0     7104 2024-04-18 11:15:49.651351 findpython-0.6.1/src/findpython/python.py
+-rw-r--r--   0        0        0     4424 2024-04-18 11:15:49.651351 findpython-0.6.1/src/findpython/utils.py
+-rw-r--r--   0        0        0        0 2024-04-18 11:15:49.651351 findpython-0.6.1/tests/__init__.py
+-rw-r--r--   0        0        0     1919 2024-04-18 11:15:49.651351 findpython-0.6.1/tests/conftest.py
+-rw-r--r--   0        0        0      612 2024-04-18 11:15:49.651351 findpython-0.6.1/tests/test_cli.py
+-rw-r--r--   0        0        0     4780 2024-04-18 11:15:49.651351 findpython-0.6.1/tests/test_finder.py
+-rw-r--r--   0        0        0     3321 2024-04-18 11:15:49.651351 findpython-0.6.1/tests/test_posix.py
+-rw-r--r--   0        0        0      681 2024-04-18 11:15:49.651351 findpython-0.6.1/tests/test_utils.py
+-rw-r--r--   0        0        0     5275 1970-01-01 00:00:00.000000 findpython-0.6.1/PKG-INFO
```

### Comparing `findpython-0.6.0/LICENSE` & `findpython-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `findpython-0.6.0/README.md` & `findpython-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `findpython-0.6.0/pyproject.toml` & `findpython-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
-version = "0.6.0"
+version = "0.6.1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/frostming/findpython"
```

### Comparing `findpython-0.6.0/src/findpython/__init__.py` & `findpython-0.6.1/src/findpython/__init__.py`

 * *Files identical despite different names*

### Comparing `findpython-0.6.0/src/findpython/__main__.py` & `findpython-0.6.1/src/findpython/__main__.py`

 * *Files identical despite different names*

### Comparing `findpython-0.6.0/src/findpython/finder.py` & `findpython-0.6.1/src/findpython/finder.py`

 * *Files identical despite different names*

### Comparing `findpython-0.6.0/src/findpython/pep514tools/_registry.py` & `findpython-0.6.1/src/findpython/pep514tools/_registry.py`

 * *Files identical despite different names*

### Comparing `findpython-0.6.0/src/findpython/pep514tools/environment.py` & `findpython-0.6.1/src/findpython/pep514tools/environment.py`

 * *Files identical despite different names*

### Comparing `findpython-0.6.0/src/findpython/providers/__init__.py` & `findpython-0.6.1/src/findpython/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `findpython-0.6.0/src/findpython/providers/asdf.py` & `findpython-0.6.1/src/findpython/providers/asdf.py`

 * *Files identical despite different names*

### Comparing `findpython-0.6.0/src/findpython/providers/base.py` & `findpython-0.6.1/src/findpython/providers/base.py`

 * *Files identical despite different names*

### Comparing `findpython-0.6.0/src/findpython/providers/macos.py` & `findpython-0.6.1/src/findpython/providers/macos.py`

 * *Files identical despite different names*

### Comparing `findpython-0.6.0/src/findpython/providers/path.py` & `findpython-0.6.1/src/findpython/providers/path.py`

 * *Files identical despite different names*

### Comparing `findpython-0.6.0/src/findpython/providers/pyenv.py` & `findpython-0.6.1/src/findpython/providers/pyenv.py`

 * *Files identical despite different names*

### Comparing `findpython-0.6.0/src/findpython/providers/rye.py` & `findpython-0.6.1/src/findpython/providers/rye.py`

 * *Files identical despite different names*

### Comparing `findpython-0.6.0/src/findpython/providers/winreg.py` & `findpython-0.6.1/src/findpython/providers/winreg.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,14 +32,20 @@
                 continue
             try:
                 path = Path(install_path.executable_path)
             except AttributeError:
                 continue
             if path.exists():
                 py_version = getattr(version.info, "version", None)
+                parse_version: Version | None = None
+                if py_version:
+                    try:
+                        parse_version = Version(py_version)
+                    except ValueError:
+                        pass
                 py_ver = self.version_maker(
                     path,
-                    Version(py_version) if py_version else None,
+                    parse_version,
                     getattr(version.info, "sys_architecture", SYS_ARCHITECTURE),
                     path,
                 )
                 yield py_ver
```

### Comparing `findpython-0.6.0/src/findpython/python.py` & `findpython-0.6.1/src/findpython/python.py`

 * *Files identical despite different names*

### Comparing `findpython-0.6.0/src/findpython/utils.py` & `findpython-0.6.1/src/findpython/utils.py`

 * *Files identical despite different names*

### Comparing `findpython-0.6.0/tests/conftest.py` & `findpython-0.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `findpython-0.6.0/tests/test_cli.py` & `findpython-0.6.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `findpython-0.6.0/tests/test_finder.py` & `findpython-0.6.1/tests/test_finder.py`

 * *Files identical despite different names*

### Comparing `findpython-0.6.0/tests/test_posix.py` & `findpython-0.6.1/tests/test_posix.py`

 * *Files identical despite different names*

### Comparing `findpython-0.6.0/tests/test_utils.py` & `findpython-0.6.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `findpython-0.6.0/PKG-INFO` & `findpython-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findpython
-Version: 0.6.0
+Version: 0.6.1
 Summary: A utility to find python versions on your system
 Author-Email: Frost Ming <mianghong@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: findpython Version: 0.6.0 Summary: A utility to
+Metadata-Version: 2.1 Name: findpython Version: 0.6.1 Summary: A utility to
 find python versions on your system Author-Email: Frost Ming
 gmail.com> License: MIT Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Project-URL: Homepage, https://github.com/frostming/
 findpython Requires-Python: >=3.8 Requires-Dist: packaging>=20 Description-
```

