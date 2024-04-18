# Comparing `tmp/pr_pilot-1.2.0.tar.gz` & `tmp/pr_pilot-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pr_pilot-1.2.0.tar", last modified: Wed Apr 17 00:43:24 2024, max compression
+gzip compressed data, was "pr_pilot-1.3.0.tar", last modified: Thu Apr 18 18:51:43 2024, max compression
```

## Comparing `pr_pilot-1.2.0.tar` & `pr_pilot-1.3.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:43:24.425831 pr_pilot-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-17 00:43:24.425831 pr_pilot-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:43:24.421831 pr_pilot-1.2.0/pr_pilot/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/pr_pilot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:43:24.421831 pr_pilot-1.2.0/pr_pilot/api/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/pr_pilot/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11037 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/pr_pilot/api/task_creation_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/pr_pilot/api/task_retrieval_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26236 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/pr_pilot/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/pr_pilot/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15420 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/pr_pilot/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/pr_pilot/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:43:24.425831 pr_pilot-1.2.0/pr_pilot/models/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/pr_pilot/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/pr_pilot/models/bad_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/pr_pilot/models/not_found.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/pr_pilot/models/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/pr_pilot/models/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     9332 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/pr_pilot/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:43:24.425831 pr_pilot-1.2.0/pr_pilot/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/pr_pilot/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/pr_pilot/test/test_bad_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/pr_pilot/test/test_not_found.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/pr_pilot/test/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/pr_pilot/test/test_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/pr_pilot/test/test_task_creation_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/pr_pilot/test/test_task_retrieval_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/pr_pilot/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:43:24.425831 pr_pilot-1.2.0/pr_pilot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-17 00:43:24.000000 pr_pilot-1.2.0/pr_pilot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-17 00:43:24.000000 pr_pilot-1.2.0/pr_pilot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 00:43:24.000000 pr_pilot-1.2.0/pr_pilot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-17 00:43:24.000000 pr_pilot-1.2.0/pr_pilot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 00:43:24.000000 pr_pilot-1.2.0/pr_pilot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 00:43:24.425831 pr_pilot-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-17 00:43:20.000000 pr_pilot-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:51:43.665241 pr_pilot-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-18 18:51:43.665241 pr_pilot-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:51:43.661241 pr_pilot-1.3.0/pr_pilot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:51:43.665241 pr_pilot-1.3.0/pr_pilot/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11037 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/api/task_creation_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/api/task_retrieval_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26236 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15420 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:51:43.665241 pr_pilot-1.3.0/pr_pilot/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/models/bad_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/models/not_found.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/models/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9332 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:51:43.665241 pr_pilot-1.3.0/pr_pilot/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/test/test_bad_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/test/test_not_found.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/test/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/test/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/test/test_task_creation_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/test/test_task_retrieval_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:51:43.665241 pr_pilot-1.3.0/pr_pilot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-18 18:51:43.000000 pr_pilot-1.3.0/pr_pilot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-18 18:51:43.000000 pr_pilot-1.3.0/pr_pilot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 18:51:43.000000 pr_pilot-1.3.0/pr_pilot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 18:51:43.000000 pr_pilot-1.3.0/pr_pilot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 18:51:43.000000 pr_pilot-1.3.0/pr_pilot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 18:51:43.665241 pr_pilot-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/setup.py
```

### Comparing `pr_pilot-1.2.0/LICENSE` & `pr_pilot-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.2.0/PKG-INFO` & `pr_pilot-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr_pilot
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python SDK for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-python
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pr_pilot Version: 1.2.0 Summary: Python SDK for PR
+Metadata-Version: 2.1 Name: pr_pilot Version: 1.3.0 Summary: Python SDK for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-python Author: Marco Lamina Author-email:
 marco@pr-pilot.ai License: GPL-3.0 Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: pydantic==2.7.0 Requires-Dist:
 urllib3==2.2.1 Requires-Dist: python-dateutil==2.9.0 Requires-Dist:
```

### Comparing `pr_pilot-1.2.0/README.md` & `pr_pilot-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.2.0/pr_pilot/__init__.py` & `pr_pilot-1.3.0/pr_pilot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     PR Pilot API
 
     API for creating PR Pilot tasks
 
-    The version of the OpenAPI document: 1.2.2
+    The version of the OpenAPI document: 1.3.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 __version__ = "1.0.0"
```

### Comparing `pr_pilot-1.2.0/pr_pilot/api/task_creation_api.py` & `pr_pilot-1.3.0/pr_pilot/api/task_creation_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PR Pilot API
 
     API for creating PR Pilot tasks
 
-    The version of the OpenAPI document: 1.2.2
+    The version of the OpenAPI document: 1.3.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
```

### Comparing `pr_pilot-1.2.0/pr_pilot/api/task_retrieval_api.py` & `pr_pilot-1.3.0/pr_pilot/api/task_retrieval_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PR Pilot API
 
     API for creating PR Pilot tasks
 
-    The version of the OpenAPI document: 1.2.2
+    The version of the OpenAPI document: 1.3.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
```

### Comparing `pr_pilot-1.2.0/pr_pilot/api_client.py` & `pr_pilot-1.3.0/pr_pilot/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PR Pilot API
 
     API for creating PR Pilot tasks
 
-    The version of the OpenAPI document: 1.2.2
+    The version of the OpenAPI document: 1.3.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import datetime
```

### Comparing `pr_pilot-1.2.0/pr_pilot/api_response.py` & `pr_pilot-1.3.0/pr_pilot/api_response.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.2.0/pr_pilot/configuration.py` & `pr_pilot-1.3.0/pr_pilot/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PR Pilot API
 
     API for creating PR Pilot tasks
 
-    The version of the OpenAPI document: 1.2.2
+    The version of the OpenAPI document: 1.3.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import copy
@@ -394,15 +394,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.2.2\n"\
+               "Version of the API: 1.3.1\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `pr_pilot-1.2.0/pr_pilot/exceptions.py` & `pr_pilot-1.3.0/pr_pilot/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PR Pilot API
 
     API for creating PR Pilot tasks
 
-    The version of the OpenAPI document: 1.2.2
+    The version of the OpenAPI document: 1.3.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from typing import Any, Optional
 from typing_extensions import Self
```

### Comparing `pr_pilot-1.2.0/pr_pilot/models/bad_request.py` & `pr_pilot-1.3.0/pr_pilot/models/bad_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PR Pilot API
 
     API for creating PR Pilot tasks
 
-    The version of the OpenAPI document: 1.2.2
+    The version of the OpenAPI document: 1.3.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `pr_pilot-1.2.0/pr_pilot/models/not_found.py` & `pr_pilot-1.3.0/pr_pilot/models/not_found.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PR Pilot API
 
     API for creating PR Pilot tasks
 
-    The version of the OpenAPI document: 1.2.2
+    The version of the OpenAPI document: 1.3.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `pr_pilot-1.2.0/pr_pilot/models/prompt.py` & `pr_pilot-1.3.0/pr_pilot/models/prompt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 # coding: utf-8
 
 """
     PR Pilot API
 
     API for creating PR Pilot tasks
 
-    The version of the OpenAPI document: 1.2.2
+    The version of the OpenAPI document: 1.3.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictStr
-from typing import Any, ClassVar, Dict, List
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
 class Prompt(BaseModel):
     """
     Prompt
     """ # noqa: E501
     prompt: StrictStr = Field(description="The prompt for the task")
     github_repo: StrictStr = Field(description="The full name of the Github repository, e.g. 'owner/repo'")
-    __properties: ClassVar[List[str]] = ["prompt", "github_repo"]
+    issue_number: Optional[StrictInt] = Field(default=None, description="Number of the issue if task is triggered in the context of an issue")
+    pr_number: Optional[StrictInt] = Field(default=None, description="Number of the PR if task is triggered in the context of a PR")
+    __properties: ClassVar[List[str]] = ["prompt", "github_repo", "issue_number", "pr_number"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -78,12 +80,14 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "prompt": obj.get("prompt"),
-            "github_repo": obj.get("github_repo")
+            "github_repo": obj.get("github_repo"),
+            "issue_number": obj.get("issue_number"),
+            "pr_number": obj.get("pr_number")
         })
         return _obj
```

### Comparing `pr_pilot-1.2.0/pr_pilot/models/task.py` & `pr_pilot-1.3.0/pr_pilot/models/task.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PR Pilot API
 
     API for creating PR Pilot tasks
 
-    The version of the OpenAPI document: 1.2.2
+    The version of the OpenAPI document: 1.3.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -32,15 +32,17 @@
     title: Annotated[str, Field(strict=True, max_length=200)]
     user_request: Optional[StrictStr] = None
     github_project: Annotated[str, Field(strict=True, max_length=200)]
     github_user: Annotated[str, Field(strict=True, max_length=200)]
     status: Annotated[str, Field(strict=True, max_length=200)]
     created: datetime
     result: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["id", "title", "user_request", "github_project", "github_user", "status", "created", "result"]
+    issue_number: Optional[Annotated[int, Field(le=2147483647, strict=True, ge=-2147483648)]] = None
+    pr_number: Optional[Annotated[int, Field(le=2147483647, strict=True, ge=-2147483648)]] = None
+    __properties: ClassVar[List[str]] = ["id", "title", "user_request", "github_project", "github_user", "status", "created", "result", "issue_number", "pr_number"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -77,14 +79,24 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # set to None if issue_number (nullable) is None
+        # and model_fields_set contains the field
+        if self.issue_number is None and "issue_number" in self.model_fields_set:
+            _dict['issue_number'] = None
+
+        # set to None if pr_number (nullable) is None
+        # and model_fields_set contains the field
+        if self.pr_number is None and "pr_number" in self.model_fields_set:
+            _dict['pr_number'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of Task from a dict"""
         if obj is None:
             return None
@@ -96,12 +108,14 @@
             "id": obj.get("id"),
             "title": obj.get("title"),
             "user_request": obj.get("user_request"),
             "github_project": obj.get("github_project"),
             "github_user": obj.get("github_user"),
             "status": obj.get("status"),
             "created": obj.get("created"),
-            "result": obj.get("result")
+            "result": obj.get("result"),
+            "issue_number": obj.get("issue_number"),
+            "pr_number": obj.get("pr_number")
         })
         return _obj
```

### Comparing `pr_pilot-1.2.0/pr_pilot/rest.py` & `pr_pilot-1.3.0/pr_pilot/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     PR Pilot API
 
     API for creating PR Pilot tasks
 
-    The version of the OpenAPI document: 1.2.2
+    The version of the OpenAPI document: 1.3.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `pr_pilot-1.2.0/pr_pilot/test/test_bad_request.py` & `pr_pilot-1.3.0/pr_pilot/test/test_bad_request.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.2.0/pr_pilot/test/test_not_found.py` & `pr_pilot-1.3.0/pr_pilot/test/test_not_found.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.2.0/pr_pilot/test/test_prompt.py` & `pr_pilot-1.3.0/pr_pilot/test/test_prompt.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.2.0/pr_pilot/test/test_task.py` & `pr_pilot-1.3.0/pr_pilot/test/test_task.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.2.0/pr_pilot/test/test_task_creation_api.py` & `pr_pilot-1.3.0/pr_pilot/test/test_task_creation_api.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.2.0/pr_pilot/test/test_task_retrieval_api.py` & `pr_pilot-1.3.0/pr_pilot/test/test_task_retrieval_api.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.2.0/pr_pilot/util.py` & `pr_pilot-1.3.0/pr_pilot/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,19 +46,23 @@
     if output_file is not None:
         with open(output_file, "a") as file:
             file.write(f"{summary}\n")
     else:
         logger.debug("GITHUB_STEP_SUMMARY environment variable is not set.")
 
 
-def create_task(repo: str, prompt: str, log=True) -> Task:
+def create_task(repo: str, prompt: str, log=True, pr_number=None, issue_number=None) -> Task:
     """Create a task for the specified repository with the given prompt."""
     with pr_pilot.ApiClient(_get_config_from_env()) as api_client:
         api_instance = pr_pilot.TaskCreationApi(api_client)
-        task = api_instance.tasks_create(Prompt(prompt=prompt, github_repo=repo))
+        if pr_number is not None:
+            pr_number = int(pr_number)
+        if issue_number is not None:
+            issue_number = int(issue_number)
+        task = api_instance.tasks_create(Prompt(prompt=prompt, github_repo=repo, issue_number=issue_number, pr_number=pr_number))
         dashboard_url = f"https://app.pr-pilot.ai/dashboard/tasks/{str(task.id)}/"
         set_github_action_output("task-id", str(task.id))
         set_github_action_output("task-url", dashboard_url)
         if log:
             logger.info(f"PR Pilot task created: {dashboard_url}")
         return task
```

### Comparing `pr_pilot-1.2.0/pr_pilot.egg-info/PKG-INFO` & `pr_pilot-1.3.0/pr_pilot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr_pilot
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python SDK for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-python
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pr_pilot Version: 1.2.0 Summary: Python SDK for PR
+Metadata-Version: 2.1 Name: pr_pilot Version: 1.3.0 Summary: Python SDK for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-python Author: Marco Lamina Author-email:
 marco@pr-pilot.ai License: GPL-3.0 Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: pydantic==2.7.0 Requires-Dist:
 urllib3==2.2.1 Requires-Dist: python-dateutil==2.9.0 Requires-Dist:
```

### Comparing `pr_pilot-1.2.0/pr_pilot.egg-info/SOURCES.txt` & `pr_pilot-1.3.0/pr_pilot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.2.0/setup.py` & `pr_pilot-1.3.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 this_dir = path.abspath(path.dirname(__file__))
 requirements_path = path.join(this_dir, 'requirements.txt')
 with open(requirements_path) as f:
     required = f.read().splitlines()
 
 setup(
     name='pr_pilot',
-    version='1.2.0',
+    version='1.3.0',
     packages=find_packages(),
     install_requires=required,
     python_requires='>=3.6',
     author='Marco Lamina',
     author_email='marco@pr-pilot.ai',
     description='Python SDK for PR Pilot, a text-to-task automation platform for Github.',
     long_description=open('README.md').read(),
```

