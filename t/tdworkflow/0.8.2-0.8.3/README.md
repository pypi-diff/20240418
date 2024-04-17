# Comparing `tmp/tdworkflow-0.8.2.tar.gz` & `tmp/tdworkflow-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdworkflow-0.8.2.tar", last modified: Sun Jan 14 16:41:41 2024, max compression
+gzip compressed data, was "tdworkflow-0.8.3.tar", last modified: Wed Apr 17 23:16:22 2024, max compression
```

## Comparing `tdworkflow-0.8.2.tar` & `tdworkflow-0.8.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 16:41:41.051535 tdworkflow-0.8.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 16:41:41.043535 tdworkflow-0.8.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 16:41:41.043535 tdworkflow-0.8.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/.github/workflows/pythonapp.yml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18112 2024-01-14 16:41:41.051535 tdworkflow-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 16:41:41.047536 tdworkflow-0.8.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 16:41:41.047536 tdworkflow-0.8.2/docs/references/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/docs/references/client.rst
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/docs/references/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/docs/references/misc.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/docs/references/model.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-14 16:41:41.051535 tdworkflow-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 16:41:41.047536 tdworkflow-0.8.2/tdworkflow/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/tdworkflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/tdworkflow/attempt.py
--rw-r--r--   0 runner    (1001) docker     (127)    39160 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/tdworkflow/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/tdworkflow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/tdworkflow/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/tdworkflow/project.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/tdworkflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/tdworkflow/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/tdworkflow/revision.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/tdworkflow/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/tdworkflow/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/tdworkflow/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/tdworkflow/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/tdworkflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 16:41:41.051535 tdworkflow-0.8.2/tdworkflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18112 2024-01-14 16:41:41.000000 tdworkflow-0.8.2/tdworkflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-01-14 16:41:41.000000 tdworkflow-0.8.2/tdworkflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-14 16:41:41.000000 tdworkflow-0.8.2/tdworkflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-14 16:41:41.000000 tdworkflow-0.8.2/tdworkflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-14 16:41:41.000000 tdworkflow-0.8.2/tdworkflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 16:41:41.051535 tdworkflow-0.8.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 16:41:41.043535 tdworkflow-0.8.2/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 16:41:41.051535 tdworkflow-0.8.2/tests/resources/sample_project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/tests/resources/sample_project/.digdag
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 16:41:41.051535 tdworkflow-0.8.2/tests/resources/sample_project/ignore_dir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/tests/resources/sample_project/ignore_dir/dummy
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/tests/resources/sample_project/main.dig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 16:41:41.051535 tdworkflow-0.8.2/tests/resources/sample_project/py_scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 16:41:41.051535 tdworkflow-0.8.2/tests/resources/sample_project/py_scripts/__ignoredir__/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/tests/resources/sample_project/py_scripts/__ignoredir__/dummy
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/tests/resources/sample_project/py_scripts/exec.py
--rw-r--r--   0 runner    (1001) docker     (127)    24529 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-01-14 16:41:27.000000 tdworkflow-0.8.2/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:22.682745 tdworkflow-0.8.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:22.674745 tdworkflow-0.8.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:22.674745 tdworkflow-0.8.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/.github/workflows/pythonapp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18112 2024-04-17 23:16:22.682745 tdworkflow-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:22.674745 tdworkflow-0.8.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:22.678745 tdworkflow-0.8.3/docs/references/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/docs/references/client.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/docs/references/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/docs/references/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/docs/references/model.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 23:16:22.682745 tdworkflow-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:22.678745 tdworkflow-0.8.3/tdworkflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/attempt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39160 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/revision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:22.682745 tdworkflow-0.8.3/tdworkflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18112 2024-04-17 23:16:22.000000 tdworkflow-0.8.3/tdworkflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-17 23:16:22.000000 tdworkflow-0.8.3/tdworkflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 23:16:22.000000 tdworkflow-0.8.3/tdworkflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-17 23:16:22.000000 tdworkflow-0.8.3/tdworkflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-17 23:16:22.000000 tdworkflow-0.8.3/tdworkflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:22.678745 tdworkflow-0.8.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:22.674745 tdworkflow-0.8.3/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:22.678745 tdworkflow-0.8.3/tests/resources/sample_project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tests/resources/sample_project/.digdag
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:22.678745 tdworkflow-0.8.3/tests/resources/sample_project/ignore_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tests/resources/sample_project/ignore_dir/dummy
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tests/resources/sample_project/main.dig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:22.682745 tdworkflow-0.8.3/tests/resources/sample_project/py_scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:22.682745 tdworkflow-0.8.3/tests/resources/sample_project/py_scripts/__ignoredir__/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tests/resources/sample_project/py_scripts/__ignoredir__/dummy
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tests/resources/sample_project/py_scripts/exec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24529 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tests/test_util.py
```

### Comparing `tdworkflow-0.8.2/.github/workflows/pythonapp.yml` & `tdworkflow-0.8.3/.github/workflows/pythonapp.yml`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.2/.github/workflows/pythonpublish.yml` & `tdworkflow-0.8.3/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.2/.gitignore` & `tdworkflow-0.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.2/.readthedocs.yml` & `tdworkflow-0.8.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.2/CHANGES.rst` & `tdworkflow-0.8.3/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.2/LICENSE` & `tdworkflow-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.2/PKG-INFO` & `tdworkflow-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdworkflow
-Version: 0.8.2
+Version: 0.8.3
 Summary: Unofficial Treasure Workflow API client
 Author-email: Aki Ariga <chezou@gmail.com>
 Maintainer-email: Aki Ariga <chezou@gmail.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `tdworkflow-0.8.2/README.rst` & `tdworkflow-0.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.2/docs/Makefile` & `tdworkflow-0.8.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.2/docs/conf.py` & `tdworkflow-0.8.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.2/docs/make.bat` & `tdworkflow-0.8.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.2/docs/references/model.rst` & `tdworkflow-0.8.3/docs/references/model.rst`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.2/pyproject.toml` & `tdworkflow-0.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.2/tdworkflow/attempt.py` & `tdworkflow-0.8.3/tdworkflow/attempt.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.2/tdworkflow/client.py` & `tdworkflow-0.8.3/tdworkflow/client.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.2/tdworkflow/log.py` & `tdworkflow-0.8.3/tdworkflow/log.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.2/tdworkflow/project.py` & `tdworkflow-0.8.3/tdworkflow/project.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.2/tdworkflow/resource.py` & `tdworkflow-0.8.3/tdworkflow/resource.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.2/tdworkflow/revision.py` & `tdworkflow-0.8.3/tdworkflow/revision.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.2/tdworkflow/schedule.py` & `tdworkflow-0.8.3/tdworkflow/schedule.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.2/tdworkflow/session.py` & `tdworkflow-0.8.3/tdworkflow/session.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.2/tdworkflow/task.py` & `tdworkflow-0.8.3/tdworkflow/task.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.2/tdworkflow/util.py` & `tdworkflow-0.8.3/tdworkflow/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 def archive_files(target_dir: str, exclude_patterns: List[str]) -> io.BytesIO:
     _partial = r")|(".join(exclude_patterns)
     pattern = rf"({_partial})"
 
     target_dir_path = Path(target_dir)
     _bytes = io.BytesIO()
-    with tarfile.open(mode="w:gz", fileobj=_bytes) as tar:
+    with tarfile.open(mode="w:gz", fileobj=_bytes, format=tarfile.GNU_FORMAT) as tar:
         for current_dir, directories, files in os.walk(target_dir_path):
             for file_or_dir in [*directories, *files]:
                 file_path = Path(os.path.join(current_dir, file_or_dir))
                 if re.search(pattern, str(file_path)) or file_or_dir.startswith("."):
                     continue
                 relative_path = file_path.relative_to(target_dir_path)
                 logger.info(f"Added {file_path} as {relative_path}")
```

### Comparing `tdworkflow-0.8.2/tdworkflow/workflow.py` & `tdworkflow-0.8.3/tdworkflow/workflow.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.2/tdworkflow.egg-info/PKG-INFO` & `tdworkflow-0.8.3/tdworkflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdworkflow
-Version: 0.8.2
+Version: 0.8.3
 Summary: Unofficial Treasure Workflow API client
 Author-email: Aki Ariga <chezou@gmail.com>
 Maintainer-email: Aki Ariga <chezou@gmail.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `tdworkflow-0.8.2/tdworkflow.egg-info/SOURCES.txt` & `tdworkflow-0.8.3/tdworkflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.2/tests/test_client.py` & `tdworkflow-0.8.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.2/tests/test_util.py` & `tdworkflow-0.8.3/tests/test_util.py`

 * *Files identical despite different names*

