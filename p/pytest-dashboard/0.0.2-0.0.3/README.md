# Comparing `tmp/pytest_dashboard-0.0.2.tar.gz` & `tmp/pytest_dashboard-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_dashboard-0.0.2.tar", max compression
+gzip compressed data, was "pytest_dashboard-0.0.3.tar", max compression
```

## Comparing `pytest_dashboard-0.0.2.tar` & `pytest_dashboard-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1495 2024-04-18 05:32:26.612604 pytest_dashboard-0.0.2/LICENSE
--rw-r--r--   0        0        0       18 2024-04-18 05:32:26.612604 pytest_dashboard-0.0.2/README.md
--rw-r--r--   0        0        0     1187 2024-04-18 05:32:39.016659 pytest_dashboard-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-18 05:32:26.612604 pytest_dashboard-0.0.2/pytest_dashboard/__init__.py
--rw-r--r--   0        0        0     1113 2024-04-18 05:32:26.612604 pytest_dashboard-0.0.2/pytest_dashboard/commands.py
--rw-r--r--   0        0        0     1810 2024-04-18 05:32:26.612604 pytest_dashboard-0.0.2/pytest_dashboard/conftest.py
--rw-r--r--   0        0        0     1359 1970-01-01 00:00:00.000000 pytest_dashboard-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1495 2024-04-18 07:33:10.969513 pytest_dashboard-0.0.3/LICENSE
+-rw-r--r--   0        0        0       18 2024-04-18 07:33:10.969513 pytest_dashboard-0.0.3/README.md
+-rw-r--r--   0        0        0      742 2024-04-18 07:33:23.693717 pytest_dashboard-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-18 07:33:10.969513 pytest_dashboard-0.0.3/pytest_dashboard/__init__.py
+-rw-r--r--   0        0        0      818 2024-04-18 07:33:10.969513 pytest_dashboard-0.0.3/pytest_dashboard/_commands.py
+-rw-r--r--   0        0        0     1821 2024-04-18 07:33:10.969513 pytest_dashboard-0.0.3/pytest_dashboard/conftest.py
+-rw-r--r--   0        0        0      121 2024-04-18 07:33:10.969513 pytest_dashboard-0.0.3/pytest_dashboard/launch_pytest_dashboard.py
+-rw-r--r--   0        0        0       95 2024-04-18 07:33:10.969513 pytest_dashboard-0.0.3/pytest_dashboard/run_pytest.py
+-rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 pytest_dashboard-0.0.3/PKG-INFO
```

### Comparing `pytest_dashboard-0.0.2/LICENSE` & `pytest_dashboard-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_dashboard-0.0.2/pyproject.toml` & `pytest_dashboard-0.0.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,22 @@
 [tool.poetry]
 name = "pytest-dashboard"
-version = "0.0.2"  # ignored by versioning plugin
+version = "0.0.3"  # ignored by versioning plugin
 description = ""
 authors = ["kazuma.naito <kazuma.naito@murata.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/pyfemtet/pytest-dashboard"
 
 [tool.poetry.dependencies]
 python = " >= 3.9.3, < 3.13"
-numpy = "^1.26.2"
-pandas = "^2.1.3"
-openpyxl = "^3.1.2"
-scipy = "^1.11.4"
-tqdm = "^4.66.1"
-psutil = "^5.9.6"
 dash = "^2.14.2"
 plotly = "^5.18.0"
 dash-bootstrap-components = "^1.5.0"
-pip-licenses = "^4.3.3"
-sphinx = "==7.2.6"
-myst-parser = "==2.0.0"
-sphinx-rtd-theme = "==2.0.0"
-sphinx-autobuild = "==2021.3.14"
-sphinx-design = "^0.5.0"
 pytest = "^7.4.3"
-junitparser = "^3.1.2"
-lxml = "^5.2.1"
-
-[tool.poetry.scripts]
-run_pytest = "pytest_dashboard.commands:run_pytest"
-run_dashboard = "pytest_dashboard.commands:launch_pytest_dashboard"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `pytest_dashboard-0.0.2/pytest_dashboard/conftest.py` & `pytest_dashboard-0.0.3/pytest_dashboard/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,10 +67,9 @@
                 f'    {report.when}: {report.outcome}{BR}'
             )
     if report.when == 'teardown':
         during_test = False
 
 
 def pytest_runtest_teardown(item):
-    # global during_test
-    # during_test = False
+    # this function is called before pytest_report_teststatus
     pass
```

