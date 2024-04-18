# Comparing `tmp/pytest_dashboard-0.0.3.tar.gz` & `tmp/pytest_dashboard-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_dashboard-0.0.3.tar", max compression
+gzip compressed data, was "pytest_dashboard-0.0.4.tar", max compression
```

## Comparing `pytest_dashboard-0.0.3.tar` & `pytest_dashboard-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1495 2024-04-18 07:33:10.969513 pytest_dashboard-0.0.3/LICENSE
--rw-r--r--   0        0        0       18 2024-04-18 07:33:10.969513 pytest_dashboard-0.0.3/README.md
--rw-r--r--   0        0        0      742 2024-04-18 07:33:23.693717 pytest_dashboard-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-18 07:33:10.969513 pytest_dashboard-0.0.3/pytest_dashboard/__init__.py
--rw-r--r--   0        0        0      818 2024-04-18 07:33:10.969513 pytest_dashboard-0.0.3/pytest_dashboard/_commands.py
--rw-r--r--   0        0        0     1821 2024-04-18 07:33:10.969513 pytest_dashboard-0.0.3/pytest_dashboard/conftest.py
--rw-r--r--   0        0        0      121 2024-04-18 07:33:10.969513 pytest_dashboard-0.0.3/pytest_dashboard/launch_pytest_dashboard.py
--rw-r--r--   0        0        0       95 2024-04-18 07:33:10.969513 pytest_dashboard-0.0.3/pytest_dashboard/run_pytest.py
--rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 pytest_dashboard-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1495 2024-04-18 11:33:32.442215 pytest_dashboard-0.0.4/LICENSE
+-rw-r--r--   0        0        0      349 2024-04-18 11:33:32.442215 pytest_dashboard-0.0.4/README.md
+-rw-r--r--   0        0        0      742 2024-04-18 11:33:46.086236 pytest_dashboard-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-04-18 11:33:46.086236 pytest_dashboard-0.0.4/pytest_dashboard/__init__.py
+-rw-r--r--   0        0        0      466 2024-04-18 11:33:32.442215 pytest_dashboard-0.0.4/pytest_dashboard/_commands.py
+-rw-r--r--   0        0        0     2184 2024-04-18 11:33:32.442215 pytest_dashboard-0.0.4/pytest_dashboard/conftest.py
+-rw-r--r--   0        0        0      120 2024-04-18 11:33:32.442215 pytest_dashboard-0.0.4/pytest_dashboard/launch_pytest_dashboard.py
+-rw-r--r--   0        0        0     1126 1970-01-01 00:00:00.000000 pytest_dashboard-0.0.4/PKG-INFO
```

### Comparing `pytest_dashboard-0.0.3/LICENSE` & `pytest_dashboard-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_dashboard-0.0.3/pyproject.toml` & `pytest_dashboard-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-dashboard"
-version = "0.0.3"  # ignored by versioning plugin
+version = "0.0.4"  # ignored by versioning plugin
 description = ""
 authors = ["kazuma.naito <kazuma.naito@murata.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/pyfemtet/pytest-dashboard"
 
 [tool.poetry.dependencies]
```

### Comparing `pytest_dashboard-0.0.3/pytest_dashboard/conftest.py` & `pytest_dashboard-0.0.4/pytest_dashboard/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,24 +28,34 @@
 
 
 BR = '\n'
 during_test = False
 progress_path = None
 
 
-def set_log_path(root):
+def set_log_path(root, specified_path=None):
     global progress_path
-    progress_path = os.path.join(
-        root,
-        datetime.datetime.now().strftime('%Y%m%d-%H%M%S-progress.yaml'),
+    if specified_path is None:
+        progress_path = os.path.join(
+            root,
+            datetime.datetime.now().strftime('%Y%m%d-%H%M%S-progress.yaml'),
+        )
+    else:
+        progress_path = specified_path
+
+
+def pytest_addoption(parser):
+    parser.addoption(
+        '--progress-path', action='store', default=None, help='pytest progress file path (.yaml)'
     )
 
 
 def pytest_collection_finish(session: Session):
-    set_log_path(session.startpath)  # directory where pytest is launched
+    specified_path = session.config.getoption('progress_path')
+    set_log_path(session.startpath, specified_path)  # if None, directory where pytest is launched
     # file_or_dir: Tuple[str] or None = session.config.getoption('file_or_dir'))  # list of specified [file_or_dir]
     with open(progress_path, 'w', encoding='utf-8', newline=BR) as f:
         f.write(f'items:{BR}')
         f.writelines([f'  - {item.name}{BR}' for item in session.items])
         f.write(f'results:{BR}')
```

