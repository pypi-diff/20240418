# Comparing `tmp/strudel_cli-0.0.7.tar.gz` & `tmp/strudel_cli-0.0.8.tar.gz`

## Comparing `strudel_cli-0.0.7.tar` & `strudel_cli-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 strudel_cli-0.0.7/COPYRIGHT.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 strudel_cli-0.0.7/requirements.txt
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 strudel_cli-0.0.7/src/strudel/__init__.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 strudel_cli-0.0.7/src/strudel/callbacks.py
--rw-r--r--   0        0        0    10816 2020-02-02 00:00:00.000000 strudel_cli-0.0.7/src/strudel/main.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 strudel_cli-0.0.7/src/strudel/utils.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 strudel_cli-0.0.7/tests/test_main.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 strudel_cli-0.0.7/.gitignore
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 strudel_cli-0.0.7/LICENSE
--rw-r--r--   0        0        0     6049 2020-02-02 00:00:00.000000 strudel_cli-0.0.7/README.md
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 strudel_cli-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     9701 2020-02-02 00:00:00.000000 strudel_cli-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 strudel_cli-0.0.8/COPYRIGHT.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 strudel_cli-0.0.8/requirements.txt
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 strudel_cli-0.0.8/src/strudel/__init__.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 strudel_cli-0.0.8/src/strudel/callbacks.py
+-rw-r--r--   0        0        0    10816 2020-02-02 00:00:00.000000 strudel_cli-0.0.8/src/strudel/main.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 strudel_cli-0.0.8/src/strudel/utils.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 strudel_cli-0.0.8/tests/test_main.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 strudel_cli-0.0.8/.gitignore
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 strudel_cli-0.0.8/LICENSE
+-rw-r--r--   0        0        0     6049 2020-02-02 00:00:00.000000 strudel_cli-0.0.8/README.md
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 strudel_cli-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     9701 2020-02-02 00:00:00.000000 strudel_cli-0.0.8/PKG-INFO
```

### Comparing `strudel_cli-0.0.7/COPYRIGHT.md` & `strudel_cli-0.0.8/COPYRIGHT.md`

 * *Files identical despite different names*

### Comparing `strudel_cli-0.0.7/requirements.txt` & `strudel_cli-0.0.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `strudel_cli-0.0.7/src/strudel/callbacks.py` & `strudel_cli-0.0.8/src/strudel/callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from .utils import snake_to_camel_case
 from . import __version__
 
 defaults = {
     "create-app": {
         "name": "",
         "output_dir": "",
-        "branch": "main",
+        "branch": "prod",
         "config": "",
         "verbose": 0
     },
     "add-taskflow": {
         "name": "",
         "template": "",
         "output_dir": "src/app",
-        "branch": "main",
+        "branch": "prod",
         "config": "",
         "verbose": 0
     }
 }
 
 
 def name_callback(value: str):
```

### Comparing `strudel_cli-0.0.7/src/strudel/main.py` & `strudel_cli-0.0.8/src/strudel/main.py`

 * *Files identical despite different names*

### Comparing `strudel_cli-0.0.7/src/strudel/utils.py` & `strudel_cli-0.0.8/src/strudel/utils.py`

 * *Files identical despite different names*

### Comparing `strudel_cli-0.0.7/LICENSE` & `strudel_cli-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `strudel_cli-0.0.7/README.md` & `strudel_cli-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `strudel_cli-0.0.7/pyproject.toml` & `strudel_cli-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "strudel-cli"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Cody O'Donnell", email="ctodonnell@lbl.gov" },
   { name="Dan Gunter", email="dkgunter@lbl.gov" },
 ]
 description = "A command-line tool for bootstrapping web applications based on the STRUDEL Design System"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `strudel_cli-0.0.7/PKG-INFO` & `strudel_cli-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: strudel-cli
-Version: 0.0.7
+Version: 0.0.8
 Summary: A command-line tool for bootstrapping web applications based on the STRUDEL Design System
 Project-URL: Homepage, https://github.com/strudel-science/strudel-kit
 Project-URL: Issues, https://github.com/strudel-science/strudel-kit/issues
 Author-email: Cody O'Donnell <ctodonnell@lbl.gov>, Dan Gunter <dkgunter@lbl.gov>
 License: License Agreement
         =================
```

