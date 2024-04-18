# Comparing `tmp/msfabricpysdkcore-0.0.6.tar.gz` & `tmp/msfabricpysdkcore-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msfabricpysdkcore-0.0.6.tar", last modified: Wed Apr 17 12:38:20 2024, max compression
+gzip compressed data, was "msfabricpysdkcore-0.0.7.tar", last modified: Wed Apr 17 15:03:31 2024, max compression
```

## Comparing `msfabricpysdkcore-0.0.6.tar` & `msfabricpysdkcore-0.0.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 12:38:20.846543 msfabricpysdkcore-0.0.6/
--rw-rw-rw-   0        0        0     1156 2024-04-10 07:49:21.000000 msfabricpysdkcore-0.0.6/LICENSE
--rw-rw-rw-   0        0        0    16383 2024-04-17 12:38:20.843721 msfabricpysdkcore-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0    15865 2024-04-17 08:55:42.000000 msfabricpysdkcore-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 12:38:20.690564 msfabricpysdkcore-0.0.6/msfabricpysdkcore/
--rw-rw-rw-   0        0        0       78 2024-04-10 09:59:59.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/__init__.py
--rw-rw-rw-   0        0        0     3778 2024-04-11 09:28:32.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/admin_item.py
--rw-rw-rw-   0        0        0     4248 2024-04-11 07:13:04.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/admin_workspace.py
--rw-rw-rw-   0        0        0    21039 2024-04-11 09:11:00.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/adminapi.py
--rw-rw-rw-   0        0        0     1929 2024-04-12 14:12:32.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/auth.py
--rw-rw-rw-   0        0        0     1761 2024-04-10 09:00:53.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/capacity.py
--rw-rw-rw-   0        0        0     1060 2024-04-10 09:50:03.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/client.py
--rw-rw-rw-   0        0        0    32048 2024-04-16 15:03:12.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/coreapi.py
--rw-rw-rw-   0        0        0    14722 2024-04-10 15:15:40.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/domain.py
--rw-rw-rw-   0        0        0    11570 2024-04-16 14:02:36.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/item.py
--rw-rw-rw-   0        0        0     2745 2024-04-11 11:55:54.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/job_instance.py
--rw-rw-rw-   0        0        0     3928 2024-04-11 11:55:24.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/lakehouse.py
--rw-rw-rw-   0        0        0     2848 2024-04-11 16:24:05.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/long_running_operation.py
--rw-rw-rw-   0        0        0     2102 2024-04-10 09:00:15.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/onelakeshortcut.py
--rw-rw-rw-   0        0        0     3834 2024-04-15 14:15:34.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/otheritems.py
-drwxrwxrwx   0        0        0        0 2024-04-17 12:38:20.834665 msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/
--rw-rw-rw-   0        0        0        0 2024-03-22 16:16:45.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/__init__.py
--rw-rw-rw-   0        0        0     2062 2024-04-11 09:34:12.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_admin_apis.py
--rw-rw-rw-   0        0        0     4649 2024-04-10 15:12:58.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_domains.py
--rw-rw-rw-   0        0        0     2398 2024-04-10 09:53:02.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_git.py
--rw-rw-rw-   0        0        0    21116 2024-04-17 07:45:33.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_items_incl_lakehouse.py
--rw-rw-rw-   0        0        0     1581 2024-04-10 09:53:00.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_jobs.py
--rw-rw-rw-   0        0        0     2390 2024-04-10 09:53:04.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_shortcuts.py
--rw-rw-rw-   0        0        0     6563 2024-04-10 09:53:06.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_workspaces_capacities.py
--rw-rw-rw-   0        0        0    48660 2024-04-16 15:03:00.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/workspace.py
-drwxrwxrwx   0        0        0        0 2024-04-17 12:38:20.840708 msfabricpysdkcore-0.0.6/msfabricpysdkcore.egg-info/
--rw-rw-rw-   0        0        0    16383 2024-04-17 12:38:20.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1091 2024-04-17 12:38:20.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 12:38:20.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-17 12:38:20.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-17 12:38:20.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      564 2024-04-15 14:48:54.000000 msfabricpysdkcore-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-17 12:38:20.846543 msfabricpysdkcore-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      235 2024-04-15 14:48:59.000000 msfabricpysdkcore-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 15:03:31.693594 msfabricpysdkcore-0.0.7/
+-rw-rw-rw-   0        0        0     1156 2024-04-10 07:49:21.000000 msfabricpysdkcore-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0    16383 2024-04-17 15:03:31.690585 msfabricpysdkcore-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0    15865 2024-04-17 08:55:42.000000 msfabricpysdkcore-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 15:03:31.590930 msfabricpysdkcore-0.0.7/msfabricpysdkcore/
+-rw-rw-rw-   0        0        0       78 2024-04-10 09:59:59.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/__init__.py
+-rw-rw-rw-   0        0        0     3778 2024-04-11 09:28:32.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/admin_item.py
+-rw-rw-rw-   0        0        0     4248 2024-04-11 07:13:04.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/admin_workspace.py
+-rw-rw-rw-   0        0        0    21039 2024-04-11 09:11:00.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/adminapi.py
+-rw-rw-rw-   0        0        0     1929 2024-04-12 14:12:32.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/auth.py
+-rw-rw-rw-   0        0        0     1761 2024-04-10 09:00:53.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/capacity.py
+-rw-rw-rw-   0        0        0     1060 2024-04-10 09:50:03.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/client.py
+-rw-rw-rw-   0        0        0    32048 2024-04-16 15:03:12.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/coreapi.py
+-rw-rw-rw-   0        0        0    14722 2024-04-10 15:15:40.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/domain.py
+-rw-rw-rw-   0        0        0    11570 2024-04-16 14:02:36.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/item.py
+-rw-rw-rw-   0        0        0     2745 2024-04-11 11:55:54.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/job_instance.py
+-rw-rw-rw-   0        0        0     3928 2024-04-11 11:55:24.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/lakehouse.py
+-rw-rw-rw-   0        0        0     2848 2024-04-11 16:24:05.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/long_running_operation.py
+-rw-rw-rw-   0        0        0     2102 2024-04-10 09:00:15.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/onelakeshortcut.py
+-rw-rw-rw-   0        0        0     3834 2024-04-15 14:15:34.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/otheritems.py
+drwxrwxrwx   0        0        0        0 2024-04-17 15:03:31.680446 msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-22 16:16:45.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/__init__.py
+-rw-rw-rw-   0        0        0     2048 2024-04-17 14:16:01.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_admin_apis.py
+-rw-rw-rw-   0        0        0     4635 2024-04-17 14:16:20.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_domains.py
+-rw-rw-rw-   0        0        0     2399 2024-04-17 14:16:25.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_git.py
+-rw-rw-rw-   0        0        0    21117 2024-04-17 14:15:50.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_items_incl_lakehouse.py
+-rw-rw-rw-   0        0        0     1581 2024-04-10 09:53:00.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_jobs.py
+-rw-rw-rw-   0        0        0     2391 2024-04-17 14:16:33.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_shortcuts.py
+-rw-rw-rw-   0        0        0     6549 2024-04-17 14:16:38.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_workspaces_capacities.py
+-rw-rw-rw-   0        0        0    48660 2024-04-16 15:03:00.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore/workspace.py
+drwxrwxrwx   0        0        0        0 2024-04-17 15:03:31.686224 msfabricpysdkcore-0.0.7/msfabricpysdkcore.egg-info/
+-rw-rw-rw-   0        0        0    16383 2024-04-17 15:03:31.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1091 2024-04-17 15:03:31.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 15:03:31.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-17 15:03:31.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-17 15:03:31.000000 msfabricpysdkcore-0.0.7/msfabricpysdkcore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      564 2024-04-17 14:22:06.000000 msfabricpysdkcore-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 15:03:31.694608 msfabricpysdkcore-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      235 2024-04-17 14:22:14.000000 msfabricpysdkcore-0.0.7/setup.py
```

### Comparing `msfabricpysdkcore-0.0.6/LICENSE` & `msfabricpysdkcore-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.6/PKG-INFO` & `msfabricpysdkcore-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: msfabricpysdkcore
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python SDK for Microsoft Fabric
 Author: Andreas Rederer
 Project-URL: Homepage, https://github.com/DaSenf1860/ms-fabric-sdk-core
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.30.0
 Requires-Dist: azure-identity>=1.15.0
 
 # Python SDK for Microsoft Fabric
```

### Comparing `msfabricpysdkcore-0.0.6/README.md` & `msfabricpysdkcore-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.6/msfabricpysdkcore/admin_item.py` & `msfabricpysdkcore-0.0.7/msfabricpysdkcore/admin_item.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.6/msfabricpysdkcore/admin_workspace.py` & `msfabricpysdkcore-0.0.7/msfabricpysdkcore/admin_workspace.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.6/msfabricpysdkcore/adminapi.py` & `msfabricpysdkcore-0.0.7/msfabricpysdkcore/adminapi.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.6/msfabricpysdkcore/auth.py` & `msfabricpysdkcore-0.0.7/msfabricpysdkcore/auth.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.6/msfabricpysdkcore/capacity.py` & `msfabricpysdkcore-0.0.7/msfabricpysdkcore/capacity.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.6/msfabricpysdkcore/client.py` & `msfabricpysdkcore-0.0.7/msfabricpysdkcore/client.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.6/msfabricpysdkcore/coreapi.py` & `msfabricpysdkcore-0.0.7/msfabricpysdkcore/coreapi.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.6/msfabricpysdkcore/domain.py` & `msfabricpysdkcore-0.0.7/msfabricpysdkcore/domain.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.6/msfabricpysdkcore/item.py` & `msfabricpysdkcore-0.0.7/msfabricpysdkcore/item.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.6/msfabricpysdkcore/job_instance.py` & `msfabricpysdkcore-0.0.7/msfabricpysdkcore/job_instance.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.6/msfabricpysdkcore/lakehouse.py` & `msfabricpysdkcore-0.0.7/msfabricpysdkcore/lakehouse.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.6/msfabricpysdkcore/long_running_operation.py` & `msfabricpysdkcore-0.0.7/msfabricpysdkcore/long_running_operation.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.6/msfabricpysdkcore/onelakeshortcut.py` & `msfabricpysdkcore-0.0.7/msfabricpysdkcore/onelakeshortcut.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.6/msfabricpysdkcore/otheritems.py` & `msfabricpysdkcore-0.0.7/msfabricpysdkcore/otheritems.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_admin_apis.py` & `msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_admin_apis.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import unittest
-from dotenv import load_dotenv
+#from dotenv import load_dotenv
 from msfabricpysdkcore import FabricClientAdmin
 
-load_dotenv()
 
 class TestFabricClientCore(unittest.TestCase):
 
     def __init__(self, *args, **kwargs):
         super(TestFabricClientCore, self).__init__(*args, **kwargs)
```

### Comparing `msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_domains.py` & `msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_domains.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import unittest
-from dotenv import load_dotenv
+#from dotenv import load_dotenv
 from datetime import datetime
 from msfabricpysdkcore import FabricClientCore, FabricClientAdmin
 
-load_dotenv()
 
 class TestFabricClientCore(unittest.TestCase):
 
     def __init__(self, *args, **kwargs):
         super(TestFabricClientCore, self).__init__(*args, **kwargs)
```

### Comparing `msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_git.py` & `msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_git.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from msfabricpysdkcore.coreapi import FabricClientCore
 from datetime import datetime
-from dotenv import load_dotenv
+#from dotenv import load_dotenv
 
 class TestFabricClientCore(unittest.TestCase):
 
     def __init__(self, *args, **kwargs):
         super(TestFabricClientCore, self).__init__(*args, **kwargs)
         #load_dotenv()
         self.fc = FabricClientCore()
```

### Comparing `msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_items_incl_lakehouse.py` & `msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_items_incl_lakehouse.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 from datetime import datetime
-from dotenv import load_dotenv
+#from dotenv import load_dotenv
 from time import sleep
 from msfabricpysdkcore.coreapi import FabricClientCore
 
 class TestFabricClientCore(unittest.TestCase):
 
     def __init__(self, *args, **kwargs):
         super(TestFabricClientCore, self).__init__(*args, **kwargs)
```

### Comparing `msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_jobs.py` & `msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_shortcuts.py` & `msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_shortcuts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from msfabricpysdkcore.coreapi import FabricClientCore
 from datetime import datetime
-from dotenv import load_dotenv
+#from dotenv import load_dotenv
 
 class TestFabricClientCore(unittest.TestCase):
 
     def __init__(self, *args, **kwargs):
         super(TestFabricClientCore, self).__init__(*args, **kwargs)
         #load_dotenv()
         self.fc = FabricClientCore()
```

### Comparing `msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_workspaces_capacities.py` & `msfabricpysdkcore-0.0.7/msfabricpysdkcore/tests/test_workspaces_capacities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import unittest
-from dotenv import load_dotenv
+#from dotenv import load_dotenv
 from datetime import datetime
 from msfabricpysdkcore.coreapi import FabricClientCore
 
-load_dotenv()
 
 class TestFabricClientCore(unittest.TestCase):
 
     def __init__(self, *args, **kwargs):
         super(TestFabricClientCore, self).__init__(*args, **kwargs)
         self.fc = FabricClientCore()
         datetime_str = datetime.now().strftime("%Y%m%d%H%M%S")
```

### Comparing `msfabricpysdkcore-0.0.6/msfabricpysdkcore/workspace.py` & `msfabricpysdkcore-0.0.7/msfabricpysdkcore/workspace.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.6/msfabricpysdkcore.egg-info/PKG-INFO` & `msfabricpysdkcore-0.0.7/msfabricpysdkcore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: msfabricpysdkcore
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python SDK for Microsoft Fabric
 Author: Andreas Rederer
 Project-URL: Homepage, https://github.com/DaSenf1860/ms-fabric-sdk-core
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.30.0
 Requires-Dist: azure-identity>=1.15.0
 
 # Python SDK for Microsoft Fabric
```

### Comparing `msfabricpysdkcore-0.0.6/msfabricpysdkcore.egg-info/SOURCES.txt` & `msfabricpysdkcore-0.0.7/msfabricpysdkcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.6/pyproject.toml` & `msfabricpysdkcore-0.0.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools >= 65.5.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msfabricpysdkcore"
-version = "0.0.6"
+version = "0.0.7"
 dynamic = ["dependencies"]
 authors = [
   { name="Andreas Rederer"},
 ]
 description = "A Python SDK for Microsoft Fabric"
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

