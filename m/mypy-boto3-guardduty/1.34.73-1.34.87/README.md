# Comparing `tmp/mypy-boto3-guardduty-1.34.73.tar.gz` & `tmp/mypy_boto3_guardduty-1.34.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-guardduty-1.34.73.tar", last modified: Thu Mar 28 19:34:42 2024, max compression
+gzip compressed data, was "mypy_boto3_guardduty-1.34.87.tar", last modified: Thu Apr 18 19:34:21 2024, max compression
```

## Comparing `mypy-boto3-guardduty-1.34.73.tar` & `mypy_boto3_guardduty-1.34.87.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:34:42.032071 mypy-boto3-guardduty-1.34.73/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-28 19:32:46.000000 mypy-boto3-guardduty-1.34.73/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14027 2024-03-28 19:34:42.032071 mypy-boto3-guardduty-1.34.73/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12464 2024-03-28 19:32:46.000000 mypy-boto3-guardduty-1.34.73/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:34:42.028071 mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty/
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-03-28 19:32:46.000000 mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-03-28 19:32:46.000000 mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-28 19:32:46.000000 mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50390 2024-03-28 19:32:46.000000 mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    50387 2024-03-28 19:32:46.000000 mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15659 2024-03-28 19:32:47.000000 mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    15659 2024-03-28 19:32:47.000000 mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11966 2024-03-28 19:32:46.000000 mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11955 2024-03-28 19:32:46.000000 mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 19:32:46.000000 mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    90770 2024-03-28 19:32:49.000000 mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    90770 2024-03-28 19:32:48.000000 mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-28 19:32:46.000000 mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:34:42.032071 mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14027 2024-03-28 19:34:41.000000 mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-28 19:34:42.000000 mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:34:41.000000 mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:34:41.000000 mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-28 19:34:42.000000 mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-28 19:34:42.000000 mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 19:34:42.032071 mypy-boto3-guardduty-1.34.73/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-03-28 19:32:46.000000 mypy-boto3-guardduty-1.34.73/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:34:21.808632 mypy_boto3_guardduty-1.34.87/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-18 19:31:59.000000 mypy_boto3_guardduty-1.34.87/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14027 2024-04-18 19:34:21.808632 mypy_boto3_guardduty-1.34.87/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12464 2024-04-18 19:31:59.000000 mypy_boto3_guardduty-1.34.87/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:34:21.804632 mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty/
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-18 19:31:59.000000 mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-18 19:31:59.000000 mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-18 19:31:59.000000 mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50390 2024-04-18 19:32:00.000000 mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50387 2024-04-18 19:32:00.000000 mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15720 2024-04-18 19:32:00.000000 mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15720 2024-04-18 19:32:00.000000 mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11966 2024-04-18 19:32:00.000000 mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11955 2024-04-18 19:32:00.000000 mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:31:59.000000 mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    90852 2024-04-18 19:32:02.000000 mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90852 2024-04-18 19:32:02.000000 mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-18 19:31:59.000000 mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:34:21.808632 mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14027 2024-04-18 19:34:21.000000 mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-18 19:34:21.000000 mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:34:21.000000 mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:34:21.000000 mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-18 19:34:21.000000 mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 19:34:21.000000 mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 19:34:21.808632 mypy_boto3_guardduty-1.34.87/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-18 19:31:59.000000 mypy_boto3_guardduty-1.34.87/setup.py
```

### Comparing `mypy-boto3-guardduty-1.34.73/LICENSE` & `mypy_boto3_guardduty-1.34.87/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.34.73/PKG-INFO` & `mypy_boto3_guardduty-1.34.87/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-guardduty
-Version: 1.34.73
-Summary: Type annotations for boto3.GuardDuty 1.34.73 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.87
+Summary: Type annotations for boto3.GuardDuty 1.34.87 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-guardduty.svg?color=blue)](https://pypi.org/project/mypy-boto3-guardduty)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-guardduty)](https://pepy.tech/project/mypy-boto3-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GuardDuty 1.34.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
+[boto3.GuardDuty 1.34.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-guardduty-1.34.73/README.md` & `mypy_boto3_guardduty-1.34.87/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-guardduty.svg?color=blue)](https://pypi.org/project/mypy-boto3-guardduty)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-guardduty)](https://pepy.tech/project/mypy-boto3-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GuardDuty 1.34.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
+[boto3.GuardDuty 1.34.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty/__init__.py` & `mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty/__init__.pyi` & `mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty/__main__.py` & `mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GuardDuty 1.34.73\n"
-        "Version:         1.34.73\n"
+        "Type annotations for boto3.GuardDuty 1.34.87\n"
+        "Version:         1.34.87\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.73")
+    print("1.34.87")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty/client.py` & `mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty/client.pyi` & `mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty/literals.py` & `mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,14 +299,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -319,24 +320,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
```

### Comparing `mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty/literals.pyi` & `mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -299,14 +299,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -319,24 +320,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
```

### Comparing `mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty/paginator.py` & `mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty/paginator.pyi` & `mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty/type_defs.py` & `mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1143,14 +1143,15 @@
         "NextToken": NotRequired[str],
     },
 )
 LocalIpDetailsTypeDef = TypedDict(
     "LocalIpDetailsTypeDef",
     {
         "IpAddressV4": NotRequired[str],
+        "IpAddressV6": NotRequired[str],
     },
 )
 LocalPortDetailsTypeDef = TypedDict(
     "LocalPortDetailsTypeDef",
     {
         "Port": NotRequired[int],
         "PortName": NotRequired[str],
@@ -2074,14 +2075,15 @@
 RemoteIpDetailsTypeDef = TypedDict(
     "RemoteIpDetailsTypeDef",
     {
         "City": NotRequired[CityTypeDef],
         "Country": NotRequired[CountryTypeDef],
         "GeoLocation": NotRequired[GeoLocationTypeDef],
         "IpAddressV4": NotRequired[str],
+        "IpAddressV6": NotRequired[str],
         "Organization": NotRequired[OrganizationTypeDef],
     },
 )
 ScanConditionTypeDef = TypedDict(
     "ScanConditionTypeDef",
     {
         "MapEquals": List[ScanConditionPairTypeDef],
```

### Comparing `mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty/type_defs.pyi` & `mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1143,14 +1143,15 @@
         "NextToken": NotRequired[str],
     },
 )
 LocalIpDetailsTypeDef = TypedDict(
     "LocalIpDetailsTypeDef",
     {
         "IpAddressV4": NotRequired[str],
+        "IpAddressV6": NotRequired[str],
     },
 )
 LocalPortDetailsTypeDef = TypedDict(
     "LocalPortDetailsTypeDef",
     {
         "Port": NotRequired[int],
         "PortName": NotRequired[str],
@@ -2074,14 +2075,15 @@
 RemoteIpDetailsTypeDef = TypedDict(
     "RemoteIpDetailsTypeDef",
     {
         "City": NotRequired[CityTypeDef],
         "Country": NotRequired[CountryTypeDef],
         "GeoLocation": NotRequired[GeoLocationTypeDef],
         "IpAddressV4": NotRequired[str],
+        "IpAddressV6": NotRequired[str],
         "Organization": NotRequired[OrganizationTypeDef],
     },
 )
 ScanConditionTypeDef = TypedDict(
     "ScanConditionTypeDef",
     {
         "MapEquals": List[ScanConditionPairTypeDef],
```

### Comparing `mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty.egg-info/PKG-INFO` & `mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-guardduty
-Version: 1.34.73
-Summary: Type annotations for boto3.GuardDuty 1.34.73 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.87
+Summary: Type annotations for boto3.GuardDuty 1.34.87 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-guardduty.svg?color=blue)](https://pypi.org/project/mypy-boto3-guardduty)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-guardduty)](https://pepy.tech/project/mypy-boto3-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GuardDuty 1.34.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
+[boto3.GuardDuty 1.34.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-guardduty-1.34.73/mypy_boto3_guardduty.egg-info/SOURCES.txt` & `mypy_boto3_guardduty-1.34.87/mypy_boto3_guardduty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.34.73/setup.py` & `mypy_boto3_guardduty-1.34.87/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-guardduty",
-    version="1.34.73",
+    version="1.34.87",
     packages=["mypy_boto3_guardduty"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.GuardDuty 1.34.73 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.GuardDuty 1.34.87 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

