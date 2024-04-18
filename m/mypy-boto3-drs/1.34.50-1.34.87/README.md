# Comparing `tmp/mypy-boto3-drs-1.34.50.tar.gz` & `tmp/mypy_boto3_drs-1.34.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-drs-1.34.50.tar", last modified: Mon Feb 26 20:23:14 2024, max compression
+gzip compressed data, was "mypy_boto3_drs-1.34.87.tar", last modified: Thu Apr 18 19:34:21 2024, max compression
```

## Comparing `mypy-boto3-drs-1.34.50.tar` & `mypy_boto3_drs-1.34.87.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 20:23:14.084718 mypy-boto3-drs-1.34.50/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-26 20:22:48.000000 mypy-boto3-drs-1.34.50/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14201 2024-02-26 20:23:14.084718 mypy-boto3-drs-1.34.50/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12662 2024-02-26 20:22:48.000000 mypy-boto3-drs-1.34.50/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 20:23:14.084718 mypy-boto3-drs-1.34.50/mypy_boto3_drs/
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-02-26 20:22:48.000000 mypy-boto3-drs-1.34.50/mypy_boto3_drs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-02-26 20:22:48.000000 mypy-boto3-drs-1.34.50/mypy_boto3_drs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-02-26 20:22:48.000000 mypy-boto3-drs-1.34.50/mypy_boto3_drs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42476 2024-02-26 20:22:49.000000 mypy-boto3-drs-1.34.50/mypy_boto3_drs/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    42473 2024-02-26 20:22:49.000000 mypy-boto3-drs-1.34.50/mypy_boto3_drs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18654 2024-02-26 20:22:50.000000 mypy-boto3-drs-1.34.50/mypy_boto3_drs/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    18654 2024-02-26 20:22:50.000000 mypy-boto3-drs-1.34.50/mypy_boto3_drs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14153 2024-02-26 20:22:49.000000 mypy-boto3-drs-1.34.50/mypy_boto3_drs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14141 2024-02-26 20:22:49.000000 mypy-boto3-drs-1.34.50/mypy_boto3_drs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 20:22:48.000000 mypy-boto3-drs-1.34.50/mypy_boto3_drs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    56948 2024-02-26 20:22:50.000000 mypy-boto3-drs-1.34.50/mypy_boto3_drs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    56948 2024-02-26 20:22:50.000000 mypy-boto3-drs-1.34.50/mypy_boto3_drs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-26 20:22:48.000000 mypy-boto3-drs-1.34.50/mypy_boto3_drs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 20:23:14.084718 mypy-boto3-drs-1.34.50/mypy_boto3_drs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14201 2024-02-26 20:23:14.000000 mypy-boto3-drs-1.34.50/mypy_boto3_drs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-26 20:23:14.000000 mypy-boto3-drs-1.34.50/mypy_boto3_drs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 20:23:14.000000 mypy-boto3-drs-1.34.50/mypy_boto3_drs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 20:23:14.000000 mypy-boto3-drs-1.34.50/mypy_boto3_drs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-26 20:23:14.000000 mypy-boto3-drs-1.34.50/mypy_boto3_drs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-26 20:23:14.000000 mypy-boto3-drs-1.34.50/mypy_boto3_drs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 20:23:14.084718 mypy-boto3-drs-1.34.50/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-02-26 20:22:48.000000 mypy-boto3-drs-1.34.50/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:34:21.120631 mypy_boto3_drs-1.34.87/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-18 19:31:56.000000 mypy_boto3_drs-1.34.87/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14201 2024-04-18 19:34:21.120631 mypy_boto3_drs-1.34.87/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12662 2024-04-18 19:31:56.000000 mypy_boto3_drs-1.34.87/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:34:21.116630 mypy_boto3_drs-1.34.87/mypy_boto3_drs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-18 19:31:56.000000 mypy_boto3_drs-1.34.87/mypy_boto3_drs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-18 19:31:56.000000 mypy_boto3_drs-1.34.87/mypy_boto3_drs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-18 19:31:56.000000 mypy_boto3_drs-1.34.87/mypy_boto3_drs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42476 2024-04-18 19:31:56.000000 mypy_boto3_drs-1.34.87/mypy_boto3_drs/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42473 2024-04-18 19:31:56.000000 mypy_boto3_drs-1.34.87/mypy_boto3_drs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18735 2024-04-18 19:31:57.000000 mypy_boto3_drs-1.34.87/mypy_boto3_drs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18735 2024-04-18 19:31:57.000000 mypy_boto3_drs-1.34.87/mypy_boto3_drs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14153 2024-04-18 19:31:57.000000 mypy_boto3_drs-1.34.87/mypy_boto3_drs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14141 2024-04-18 19:31:57.000000 mypy_boto3_drs-1.34.87/mypy_boto3_drs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:31:56.000000 mypy_boto3_drs-1.34.87/mypy_boto3_drs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    57147 2024-04-18 19:31:58.000000 mypy_boto3_drs-1.34.87/mypy_boto3_drs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57147 2024-04-18 19:31:57.000000 mypy_boto3_drs-1.34.87/mypy_boto3_drs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-18 19:31:56.000000 mypy_boto3_drs-1.34.87/mypy_boto3_drs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:34:21.120631 mypy_boto3_drs-1.34.87/mypy_boto3_drs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14201 2024-04-18 19:34:21.000000 mypy_boto3_drs-1.34.87/mypy_boto3_drs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-18 19:34:21.000000 mypy_boto3_drs-1.34.87/mypy_boto3_drs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:34:21.000000 mypy_boto3_drs-1.34.87/mypy_boto3_drs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:34:21.000000 mypy_boto3_drs-1.34.87/mypy_boto3_drs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-18 19:34:21.000000 mypy_boto3_drs-1.34.87/mypy_boto3_drs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 19:34:21.000000 mypy_boto3_drs-1.34.87/mypy_boto3_drs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 19:34:21.120631 mypy_boto3_drs-1.34.87/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-18 19:31:56.000000 mypy_boto3_drs-1.34.87/setup.py
```

### Comparing `mypy-boto3-drs-1.34.50/LICENSE` & `mypy_boto3_drs-1.34.87/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.34.50/PKG-INFO` & `mypy_boto3_drs-1.34.87/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-drs
-Version: 1.34.50
-Summary: Type annotations for boto3.drs 1.34.50 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.87
+Summary: Type annotations for boto3.drs 1.34.87 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-drs.svg?color=blue)](https://pypi.org/project/mypy-boto3-drs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-drs)](https://pepy.tech/project/mypy-boto3-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.drs 1.34.50](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[boto3.drs 1.34.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-drs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-drs-1.34.50/README.md` & `mypy_boto3_drs-1.34.87/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-drs.svg?color=blue)](https://pypi.org/project/mypy-boto3-drs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-drs)](https://pepy.tech/project/mypy-boto3-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.drs 1.34.50](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[boto3.drs 1.34.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-drs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-drs-1.34.50/mypy_boto3_drs/__init__.py` & `mypy_boto3_drs-1.34.87/mypy_boto3_drs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.34.50/mypy_boto3_drs/__init__.pyi` & `mypy_boto3_drs-1.34.87/mypy_boto3_drs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.34.50/mypy_boto3_drs/__main__.py` & `mypy_boto3_drs-1.34.87/mypy_boto3_drs/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.drs 1.34.50\n"
-        "Version:         1.34.50\n"
-        "Builder version: 7.23.1\n"
+        "Type annotations for boto3.drs 1.34.87\n"
+        "Version:         1.34.87\n"
+        "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.50")
+    print("1.34.87")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-drs-1.34.50/mypy_boto3_drs/client.py` & `mypy_boto3_drs-1.34.87/mypy_boto3_drs/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.34.50/mypy_boto3_drs/client.pyi` & `mypy_boto3_drs-1.34.87/mypy_boto3_drs/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.34.50/mypy_boto3_drs/literals.py` & `mypy_boto3_drs-1.34.87/mypy_boto3_drs/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,14 +280,15 @@
 ReplicationDirectionType = Literal["FAILBACK", "FAILOVER"]
 ReplicationStatusType = Literal["ERROR", "IN_PROGRESS", "PROTECTED", "STOPPED"]
 TargetInstanceTypeRightSizingMethodType = Literal["BASIC", "IN_AWS", "NONE"]
 VolumeStatusType = Literal[
     "CONTAINS_MARKETPLACE_PRODUCT_CODES",
     "MISSING_VOLUME_ATTRIBUTES",
     "MISSING_VOLUME_ATTRIBUTES_AND_PRECHECK_UNAVAILABLE",
+    "PENDING",
     "REGULAR",
 ]
 drsServiceName = Literal["drs"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -354,14 +355,15 @@
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
@@ -374,24 +376,26 @@
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
@@ -452,15 +456,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -640,14 +643,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-drs-1.34.50/mypy_boto3_drs/literals.pyi` & `mypy_boto3_drs-1.34.87/mypy_boto3_drs/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -280,14 +280,15 @@
 ReplicationDirectionType = Literal["FAILBACK", "FAILOVER"]
 ReplicationStatusType = Literal["ERROR", "IN_PROGRESS", "PROTECTED", "STOPPED"]
 TargetInstanceTypeRightSizingMethodType = Literal["BASIC", "IN_AWS", "NONE"]
 VolumeStatusType = Literal[
     "CONTAINS_MARKETPLACE_PRODUCT_CODES",
     "MISSING_VOLUME_ATTRIBUTES",
     "MISSING_VOLUME_ATTRIBUTES_AND_PRECHECK_UNAVAILABLE",
+    "PENDING",
     "REGULAR",
 ]
 drsServiceName = Literal["drs"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -354,14 +355,15 @@
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
@@ -374,24 +376,26 @@
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
@@ -452,15 +456,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -640,14 +643,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-drs-1.34.50/mypy_boto3_drs/paginator.py` & `mypy_boto3_drs-1.34.87/mypy_boto3_drs/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.34.50/mypy_boto3_drs/paginator.pyi` & `mypy_boto3_drs-1.34.87/mypy_boto3_drs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.34.50/mypy_boto3_drs/type_defs.py` & `mypy_boto3_drs-1.34.87/mypy_boto3_drs/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,18 +236,18 @@
         "sourceNetworkID": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 CPUTypeDef = TypedDict(
     "CPUTypeDef",
     {
         "cores": NotRequired[int],
         "modelName": NotRequired[str],
@@ -659,14 +659,15 @@
 )
 SourceCloudPropertiesTypeDef = TypedDict(
     "SourceCloudPropertiesTypeDef",
     {
         "originAccountID": NotRequired[str],
         "originAvailabilityZone": NotRequired[str],
         "originRegion": NotRequired[str],
+        "sourceOutpostArn": NotRequired[str],
     },
 )
 StagingAreaTypeDef = TypedDict(
     "StagingAreaTypeDef",
     {
         "errorMessage": NotRequired[str],
         "stagingAccountID": NotRequired[str],
@@ -1353,14 +1354,15 @@
         "dataReplicationError": NotRequired[DataReplicationErrorTypeDef],
         "dataReplicationInitiation": NotRequired[DataReplicationInitiationTypeDef],
         "dataReplicationState": NotRequired[DataReplicationStateType],
         "etaDateTime": NotRequired[str],
         "lagDuration": NotRequired[str],
         "replicatedDisks": NotRequired[List[DataReplicationInfoReplicatedDiskTypeDef]],
         "stagingAvailabilityZone": NotRequired[str],
+        "stagingOutpostArn": NotRequired[str],
     },
 )
 JobLogEventDataTypeDef = TypedDict(
     "JobLogEventDataTypeDef",
     {
         "conversionProperties": NotRequired[ConversionPropertiesTypeDef],
         "conversionServerID": NotRequired[str],
@@ -1405,14 +1407,15 @@
         "dataReplicationState": NotRequired[RecoveryInstanceDataReplicationStateType],
         "etaDateTime": NotRequired[str],
         "lagDuration": NotRequired[str],
         "replicatedDisks": NotRequired[
             List[RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef]
         ],
         "stagingAvailabilityZone": NotRequired[str],
+        "stagingOutpostArn": NotRequired[str],
     },
 )
 DescribeSourceNetworksResponseTypeDef = TypedDict(
     "DescribeSourceNetworksResponseTypeDef",
     {
         "items": List[SourceNetworkTypeDef],
         "nextToken": str,
@@ -1499,14 +1502,15 @@
         "isDrill": NotRequired[bool],
         "jobID": NotRequired[str],
         "originAvailabilityZone": NotRequired[str],
         "originEnvironment": NotRequired[OriginEnvironmentType],
         "pointInTimeSnapshotDateTime": NotRequired[str],
         "recoveryInstanceID": NotRequired[str],
         "recoveryInstanceProperties": NotRequired[RecoveryInstancePropertiesTypeDef],
+        "sourceOutpostArn": NotRequired[str],
         "sourceServerID": NotRequired[str],
         "tags": NotRequired[Dict[str, str]],
     },
 )
 DescribeJobLogItemsResponseTypeDef = TypedDict(
     "DescribeJobLogItemsResponseTypeDef",
     {
```

### Comparing `mypy-boto3-drs-1.34.50/mypy_boto3_drs/type_defs.pyi` & `mypy_boto3_drs-1.34.87/mypy_boto3_drs/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -236,18 +236,18 @@
         "sourceNetworkID": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 CPUTypeDef = TypedDict(
     "CPUTypeDef",
     {
         "cores": NotRequired[int],
         "modelName": NotRequired[str],
@@ -659,14 +659,15 @@
 )
 SourceCloudPropertiesTypeDef = TypedDict(
     "SourceCloudPropertiesTypeDef",
     {
         "originAccountID": NotRequired[str],
         "originAvailabilityZone": NotRequired[str],
         "originRegion": NotRequired[str],
+        "sourceOutpostArn": NotRequired[str],
     },
 )
 StagingAreaTypeDef = TypedDict(
     "StagingAreaTypeDef",
     {
         "errorMessage": NotRequired[str],
         "stagingAccountID": NotRequired[str],
@@ -1353,14 +1354,15 @@
         "dataReplicationError": NotRequired[DataReplicationErrorTypeDef],
         "dataReplicationInitiation": NotRequired[DataReplicationInitiationTypeDef],
         "dataReplicationState": NotRequired[DataReplicationStateType],
         "etaDateTime": NotRequired[str],
         "lagDuration": NotRequired[str],
         "replicatedDisks": NotRequired[List[DataReplicationInfoReplicatedDiskTypeDef]],
         "stagingAvailabilityZone": NotRequired[str],
+        "stagingOutpostArn": NotRequired[str],
     },
 )
 JobLogEventDataTypeDef = TypedDict(
     "JobLogEventDataTypeDef",
     {
         "conversionProperties": NotRequired[ConversionPropertiesTypeDef],
         "conversionServerID": NotRequired[str],
@@ -1405,14 +1407,15 @@
         "dataReplicationState": NotRequired[RecoveryInstanceDataReplicationStateType],
         "etaDateTime": NotRequired[str],
         "lagDuration": NotRequired[str],
         "replicatedDisks": NotRequired[
             List[RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef]
         ],
         "stagingAvailabilityZone": NotRequired[str],
+        "stagingOutpostArn": NotRequired[str],
     },
 )
 DescribeSourceNetworksResponseTypeDef = TypedDict(
     "DescribeSourceNetworksResponseTypeDef",
     {
         "items": List[SourceNetworkTypeDef],
         "nextToken": str,
@@ -1499,14 +1502,15 @@
         "isDrill": NotRequired[bool],
         "jobID": NotRequired[str],
         "originAvailabilityZone": NotRequired[str],
         "originEnvironment": NotRequired[OriginEnvironmentType],
         "pointInTimeSnapshotDateTime": NotRequired[str],
         "recoveryInstanceID": NotRequired[str],
         "recoveryInstanceProperties": NotRequired[RecoveryInstancePropertiesTypeDef],
+        "sourceOutpostArn": NotRequired[str],
         "sourceServerID": NotRequired[str],
         "tags": NotRequired[Dict[str, str]],
     },
 )
 DescribeJobLogItemsResponseTypeDef = TypedDict(
     "DescribeJobLogItemsResponseTypeDef",
     {
```

### Comparing `mypy-boto3-drs-1.34.50/mypy_boto3_drs.egg-info/PKG-INFO` & `mypy_boto3_drs-1.34.87/mypy_boto3_drs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-drs
-Version: 1.34.50
-Summary: Type annotations for boto3.drs 1.34.50 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.87
+Summary: Type annotations for boto3.drs 1.34.87 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-drs.svg?color=blue)](https://pypi.org/project/mypy-boto3-drs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-drs)](https://pepy.tech/project/mypy-boto3-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.drs 1.34.50](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[boto3.drs 1.34.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-drs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-drs-1.34.50/mypy_boto3_drs.egg-info/SOURCES.txt` & `mypy_boto3_drs-1.34.87/mypy_boto3_drs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.34.50/setup.py` & `mypy_boto3_drs-1.34.87/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-drs",
-    version="1.34.50",
+    version="1.34.87",
     packages=["mypy_boto3_drs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.drs 1.34.50 service generated with mypy-boto3-builder 7.23.1",
+    description="Type annotations for boto3.drs 1.34.87 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

