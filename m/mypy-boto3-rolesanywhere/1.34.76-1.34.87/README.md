# Comparing `tmp/mypy-boto3-rolesanywhere-1.34.76.tar.gz` & `tmp/mypy_boto3_rolesanywhere-1.34.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rolesanywhere-1.34.76.tar", last modified: Tue Apr  2 19:32:32 2024, max compression
+gzip compressed data, was "mypy_boto3_rolesanywhere-1.34.87.tar", last modified: Thu Apr 18 19:34:22 2024, max compression
```

## Comparing `mypy-boto3-rolesanywhere-1.34.76.tar` & `mypy_boto3_rolesanywhere-1.34.87.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:32:32.171227 mypy-boto3-rolesanywhere-1.34.76/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-04-02 19:32:32.171227 mypy-boto3-rolesanywhere-1.34.76/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11815 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:32:32.171227 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20471 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20468 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13708 2024-04-02 19:32:04.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13708 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:32:32.171227 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-04-02 19:32:32.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-02 19:32:32.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:32:32.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:32:32.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 19:32:32.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 19:32:32.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:32:32.171227 mypy-boto3-rolesanywhere-1.34.76/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:34:22.616634 mypy_boto3_rolesanywhere-1.34.87/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-18 19:33:42.000000 mypy_boto3_rolesanywhere-1.34.87/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13409 2024-04-18 19:34:22.616634 mypy_boto3_rolesanywhere-1.34.87/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11827 2024-04-18 19:33:42.000000 mypy_boto3_rolesanywhere-1.34.87/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:34:22.616634 mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere/
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-18 19:33:42.000000 mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-18 19:33:42.000000 mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-18 19:33:42.000000 mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21944 2024-04-18 19:33:42.000000 mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21941 2024-04-18 19:33:42.000000 mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9735 2024-04-18 19:33:42.000000 mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9735 2024-04-18 19:33:42.000000 mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-04-18 19:33:42.000000 mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-18 19:33:42.000000 mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:33:42.000000 mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    15268 2024-04-18 19:33:42.000000 mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15268 2024-04-18 19:33:42.000000 mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-18 19:33:42.000000 mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:34:22.616634 mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13409 2024-04-18 19:34:22.000000 mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-18 19:34:22.000000 mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:34:22.000000 mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:34:22.000000 mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-18 19:34:22.000000 mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 19:34:22.000000 mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 19:34:22.616634 mypy_boto3_rolesanywhere-1.34.87/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-18 19:33:42.000000 mypy_boto3_rolesanywhere-1.34.87/setup.py
```

### Comparing `mypy-boto3-rolesanywhere-1.34.76/LICENSE` & `mypy_boto3_rolesanywhere-1.34.87/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.34.76/PKG-INFO` & `mypy_boto3_rolesanywhere-1.34.87/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rolesanywhere
-Version: 1.34.76
-Summary: Type annotations for boto3.IAMRolesAnywhere 1.34.76 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.87
+Summary: Type annotations for boto3.IAMRolesAnywhere 1.34.87 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rolesanywhere)](https://pepy.tech/project/mypy-boto3-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAMRolesAnywhere 1.34.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[boto3.IAMRolesAnywhere 1.34.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -309,35 +309,35 @@
 `mypy_boto3_rolesanywhere.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 Full list of `IAMRolesAnywhere` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/literals/).
 
 ```python
-from mypy_boto3_rolesanywhere.literals import ListCrlsPaginatorName
+from mypy_boto3_rolesanywhere.literals import CertificateFieldType
 
 
-def check_value(value: ListCrlsPaginatorName) -> bool: ...
+def check_value(value: CertificateFieldType) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_rolesanywhere.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
 Full list of `IAMRolesAnywhere` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/type_defs/).
 
 ```python
-from mypy_boto3_rolesanywhere.type_defs import BlobTypeDef
+from mypy_boto3_rolesanywhere.type_defs import MappingRuleTypeDef
 
 
-def get_value() -> BlobTypeDef:
+def get_value() -> MappingRuleTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-rolesanywhere-1.34.76/README.md` & `mypy_boto3_rolesanywhere-1.34.87/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rolesanywhere)](https://pepy.tech/project/mypy-boto3-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAMRolesAnywhere 1.34.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[boto3.IAMRolesAnywhere 1.34.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -276,35 +276,35 @@
 `mypy_boto3_rolesanywhere.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 Full list of `IAMRolesAnywhere` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/literals/).
 
 ```python
-from mypy_boto3_rolesanywhere.literals import ListCrlsPaginatorName
+from mypy_boto3_rolesanywhere.literals import CertificateFieldType
 
 
-def check_value(value: ListCrlsPaginatorName) -> bool: ...
+def check_value(value: CertificateFieldType) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_rolesanywhere.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
 Full list of `IAMRolesAnywhere` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/type_defs/).
 
 ```python
-from mypy_boto3_rolesanywhere.type_defs import BlobTypeDef
+from mypy_boto3_rolesanywhere.type_defs import MappingRuleTypeDef
 
 
-def get_value() -> BlobTypeDef:
+def get_value() -> MappingRuleTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/__init__.py` & `mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/__init__.pyi` & `mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/__main__.py` & `mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IAMRolesAnywhere 1.34.76\n"
-        "Version:         1.34.76\n"
+        "Type annotations for boto3.IAMRolesAnywhere 1.34.87\n"
+        "Version:         1.34.87\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.76")
+    print("1.34.87")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/client.py` & `mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,31 +15,35 @@
 """
 
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
+from .literals import CertificateFieldType
 from .paginator import (
     ListCrlsPaginator,
     ListProfilesPaginator,
     ListSubjectsPaginator,
     ListTrustAnchorsPaginator,
 )
 from .type_defs import (
     BlobTypeDef,
     CrlDetailResponseTypeDef,
+    DeleteAttributeMappingResponseTypeDef,
     ListCrlsResponseTypeDef,
     ListProfilesResponseTypeDef,
     ListSubjectsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTrustAnchorsResponseTypeDef,
+    MappingRuleTypeDef,
     NotificationSettingKeyTypeDef,
     NotificationSettingTypeDef,
     ProfileDetailResponseTypeDef,
+    PutAttributeMappingResponseTypeDef,
     PutNotificationSettingsResponseTypeDef,
     ResetNotificationSettingsResponseTypeDef,
     SourceTypeDef,
     SubjectDetailResponseTypeDef,
     TagTypeDef,
     TrustAnchorDetailResponseTypeDef,
 )
@@ -136,14 +140,28 @@
         certificate authority
         (CA).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.create_trust_anchor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#create_trust_anchor)
         """
 
+    def delete_attribute_mapping(
+        self,
+        *,
+        certificateField: CertificateFieldType,
+        profileId: str,
+        specifiers: Sequence[str] = ...,
+    ) -> DeleteAttributeMappingResponseTypeDef:
+        """
+        Delete an entry from the attribute mapping rules enforced by a given profile.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.delete_attribute_mapping)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#delete_attribute_mapping)
+        """
+
     def delete_crl(self, *, crlId: str) -> CrlDetailResponseTypeDef:
         """
         Deletes a certificate revocation list (CRL).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.delete_crl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#delete_crl)
         """
@@ -320,14 +338,29 @@
         Lists the trust anchors in the authenticated account and Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.list_trust_anchors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#list_trust_anchors)
         """
 
+    def put_attribute_mapping(
+        self,
+        *,
+        certificateField: CertificateFieldType,
+        mappingRules: Sequence[MappingRuleTypeDef],
+        profileId: str,
+    ) -> PutAttributeMappingResponseTypeDef:
+        """
+        Put an entry in the attribute mapping rules that will be enforced by a given
+        profile.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.put_attribute_mapping)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#put_attribute_mapping)
+        """
+
     def put_notification_settings(
         self, *, notificationSettings: Sequence[NotificationSettingTypeDef], trustAnchorId: str
     ) -> PutNotificationSettingsResponseTypeDef:
         """
         Attaches a list of *notification settings* to a trust anchor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.put_notification_settings)
```

### Comparing `mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/client.pyi` & `mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -15,31 +15,35 @@
 """
 
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
+from .literals import CertificateFieldType
 from .paginator import (
     ListCrlsPaginator,
     ListProfilesPaginator,
     ListSubjectsPaginator,
     ListTrustAnchorsPaginator,
 )
 from .type_defs import (
     BlobTypeDef,
     CrlDetailResponseTypeDef,
+    DeleteAttributeMappingResponseTypeDef,
     ListCrlsResponseTypeDef,
     ListProfilesResponseTypeDef,
     ListSubjectsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTrustAnchorsResponseTypeDef,
+    MappingRuleTypeDef,
     NotificationSettingKeyTypeDef,
     NotificationSettingTypeDef,
     ProfileDetailResponseTypeDef,
+    PutAttributeMappingResponseTypeDef,
     PutNotificationSettingsResponseTypeDef,
     ResetNotificationSettingsResponseTypeDef,
     SourceTypeDef,
     SubjectDetailResponseTypeDef,
     TagTypeDef,
     TrustAnchorDetailResponseTypeDef,
 )
@@ -133,14 +137,28 @@
         certificate authority
         (CA).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.create_trust_anchor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#create_trust_anchor)
         """
 
+    def delete_attribute_mapping(
+        self,
+        *,
+        certificateField: CertificateFieldType,
+        profileId: str,
+        specifiers: Sequence[str] = ...,
+    ) -> DeleteAttributeMappingResponseTypeDef:
+        """
+        Delete an entry from the attribute mapping rules enforced by a given profile.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.delete_attribute_mapping)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#delete_attribute_mapping)
+        """
+
     def delete_crl(self, *, crlId: str) -> CrlDetailResponseTypeDef:
         """
         Deletes a certificate revocation list (CRL).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.delete_crl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#delete_crl)
         """
@@ -317,14 +335,29 @@
         Lists the trust anchors in the authenticated account and Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.list_trust_anchors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#list_trust_anchors)
         """
 
+    def put_attribute_mapping(
+        self,
+        *,
+        certificateField: CertificateFieldType,
+        mappingRules: Sequence[MappingRuleTypeDef],
+        profileId: str,
+    ) -> PutAttributeMappingResponseTypeDef:
+        """
+        Put an entry in the attribute mapping rules that will be enforced by a given
+        profile.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.put_attribute_mapping)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/client/#put_attribute_mapping)
+        """
+
     def put_notification_settings(
         self, *, notificationSettings: Sequence[NotificationSettingTypeDef], trustAnchorId: str
     ) -> PutNotificationSettingsResponseTypeDef:
         """
         Attaches a list of *notification settings* to a trust anchor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.put_notification_settings)
```

### Comparing `mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/literals.py` & `mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,42 +2,44 @@
 Type annotations for rolesanywhere service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_rolesanywhere.literals import ListCrlsPaginatorName
+    from mypy_boto3_rolesanywhere.literals import CertificateFieldType
 
-    data: ListCrlsPaginatorName = "list_crls"
+    data: CertificateFieldType = "x509Issuer"
     ```
 """
 
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
+    "CertificateFieldType",
     "ListCrlsPaginatorName",
     "ListProfilesPaginatorName",
     "ListSubjectsPaginatorName",
     "ListTrustAnchorsPaginatorName",
     "NotificationChannelType",
     "NotificationEventType",
     "TrustAnchorTypeType",
     "IAMRolesAnywhereServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+CertificateFieldType = Literal["x509Issuer", "x509SAN", "x509Subject"]
 ListCrlsPaginatorName = Literal["list_crls"]
 ListProfilesPaginatorName = Literal["list_profiles"]
 ListSubjectsPaginatorName = Literal["list_subjects"]
 ListTrustAnchorsPaginatorName = Literal["list_trust_anchors"]
 NotificationChannelType = Literal["ALL"]
 NotificationEventType = Literal["CA_CERTIFICATE_EXPIRY", "END_ENTITY_CERTIFICATE_EXPIRY"]
 TrustAnchorTypeType = Literal["AWS_ACM_PCA", "CERTIFICATE_BUNDLE", "SELF_SIGNED_REPOSITORY"]
@@ -130,14 +132,15 @@
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
```

### Comparing `mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/literals.pyi` & `mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -2,42 +2,44 @@
 Type annotations for rolesanywhere service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_rolesanywhere.literals import ListCrlsPaginatorName
+    from mypy_boto3_rolesanywhere.literals import CertificateFieldType
 
-    data: ListCrlsPaginatorName = "list_crls"
+    data: CertificateFieldType = "x509Issuer"
     ```
 """
 
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
+    "CertificateFieldType",
     "ListCrlsPaginatorName",
     "ListProfilesPaginatorName",
     "ListSubjectsPaginatorName",
     "ListTrustAnchorsPaginatorName",
     "NotificationChannelType",
     "NotificationEventType",
     "TrustAnchorTypeType",
     "IAMRolesAnywhereServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+CertificateFieldType = Literal["x509Issuer", "x509SAN", "x509Subject"]
 ListCrlsPaginatorName = Literal["list_crls"]
 ListProfilesPaginatorName = Literal["list_profiles"]
 ListSubjectsPaginatorName = Literal["list_subjects"]
 ListTrustAnchorsPaginatorName = Literal["list_trust_anchors"]
 NotificationChannelType = Literal["ALL"]
 NotificationEventType = Literal["CA_CERTIFICATE_EXPIRY", "END_ENTITY_CERTIFICATE_EXPIRY"]
 TrustAnchorTypeType = Literal["AWS_ACM_PCA", "CERTIFICATE_BUNDLE", "SELF_SIGNED_REPOSITORY"]
@@ -130,14 +132,15 @@
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
```

### Comparing `mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/paginator.py` & `mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/paginator.pyi` & `mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/type_defs.py` & `mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 Type annotations for rolesanywhere service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_rolesanywhere.type_defs import BlobTypeDef
+    from mypy_boto3_rolesanywhere.type_defs import MappingRuleTypeDef
 
-    data: BlobTypeDef = ...
+    data: MappingRuleTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
 
-from .literals import NotificationEventType, TrustAnchorTypeType
+from .literals import CertificateFieldType, NotificationEventType, TrustAnchorTypeType
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 12):
     from typing import NotRequired
@@ -30,63 +30,75 @@
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "MappingRuleTypeDef",
     "BlobTypeDef",
     "TagTypeDef",
     "NotificationSettingTypeDef",
     "CredentialSummaryTypeDef",
     "CrlDetailTypeDef",
     "ResponseMetadataTypeDef",
+    "DeleteAttributeMappingRequestRequestTypeDef",
     "InstancePropertyTypeDef",
-    "ProfileDetailTypeDef",
     "PaginatorConfigTypeDef",
     "ListRequestRequestTypeDef",
     "SubjectSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "NotificationSettingDetailTypeDef",
     "NotificationSettingKeyTypeDef",
     "ScalarCrlRequestRequestTypeDef",
     "ScalarProfileRequestRequestTypeDef",
     "ScalarSubjectRequestRequestTypeDef",
     "ScalarTrustAnchorRequestRequestTypeDef",
     "SourceDataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateProfileRequestRequestTypeDef",
+    "AttributeMappingTypeDef",
+    "PutAttributeMappingRequestRequestTypeDef",
     "UpdateCrlRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "ImportCrlRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "PutNotificationSettingsRequestRequestTypeDef",
     "CrlDetailResponseTypeDef",
     "ListCrlsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "SubjectDetailTypeDef",
-    "ListProfilesResponseTypeDef",
-    "ProfileDetailResponseTypeDef",
     "ListRequestListCrlsPaginateTypeDef",
     "ListRequestListProfilesPaginateTypeDef",
     "ListRequestListSubjectsPaginateTypeDef",
     "ListRequestListTrustAnchorsPaginateTypeDef",
     "ListSubjectsResponseTypeDef",
     "ResetNotificationSettingsRequestRequestTypeDef",
     "SourceTypeDef",
+    "ProfileDetailTypeDef",
     "SubjectDetailResponseTypeDef",
     "CreateTrustAnchorRequestRequestTypeDef",
     "TrustAnchorDetailTypeDef",
     "UpdateTrustAnchorRequestRequestTypeDef",
+    "DeleteAttributeMappingResponseTypeDef",
+    "ListProfilesResponseTypeDef",
+    "ProfileDetailResponseTypeDef",
+    "PutAttributeMappingResponseTypeDef",
     "ListTrustAnchorsResponseTypeDef",
     "PutNotificationSettingsResponseTypeDef",
     "ResetNotificationSettingsResponseTypeDef",
     "TrustAnchorDetailResponseTypeDef",
 )
 
+MappingRuleTypeDef = TypedDict(
+    "MappingRuleTypeDef",
+    {
+        "specifier": str,
+    },
+)
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
@@ -130,39 +142,30 @@
         "RequestId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
         "HostId": NotRequired[str],
     },
 )
+DeleteAttributeMappingRequestRequestTypeDef = TypedDict(
+    "DeleteAttributeMappingRequestRequestTypeDef",
+    {
+        "certificateField": CertificateFieldType,
+        "profileId": str,
+        "specifiers": NotRequired[Sequence[str]],
+    },
+)
 InstancePropertyTypeDef = TypedDict(
     "InstancePropertyTypeDef",
     {
         "failed": NotRequired[bool],
         "properties": NotRequired[Dict[str, str]],
         "seenAt": NotRequired[datetime],
     },
 )
-ProfileDetailTypeDef = TypedDict(
-    "ProfileDetailTypeDef",
-    {
-        "createdAt": NotRequired[datetime],
-        "createdBy": NotRequired[str],
-        "durationSeconds": NotRequired[int],
-        "enabled": NotRequired[bool],
-        "managedPolicyArns": NotRequired[List[str]],
-        "name": NotRequired[str],
-        "profileArn": NotRequired[str],
-        "profileId": NotRequired[str],
-        "requireInstanceProperties": NotRequired[bool],
-        "roleArns": NotRequired[List[str]],
-        "sessionPolicy": NotRequired[str],
-        "updatedAt": NotRequired[datetime],
-    },
-)
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": NotRequired[int],
         "PageSize": NotRequired[int],
         "StartingToken": NotRequired[str],
     },
@@ -254,14 +257,29 @@
         "durationSeconds": NotRequired[int],
         "managedPolicyArns": NotRequired[Sequence[str]],
         "name": NotRequired[str],
         "roleArns": NotRequired[Sequence[str]],
         "sessionPolicy": NotRequired[str],
     },
 )
+AttributeMappingTypeDef = TypedDict(
+    "AttributeMappingTypeDef",
+    {
+        "certificateField": NotRequired[CertificateFieldType],
+        "mappingRules": NotRequired[List[MappingRuleTypeDef]],
+    },
+)
+PutAttributeMappingRequestRequestTypeDef = TypedDict(
+    "PutAttributeMappingRequestRequestTypeDef",
+    {
+        "certificateField": CertificateFieldType,
+        "mappingRules": Sequence[MappingRuleTypeDef],
+        "profileId": str,
+    },
+)
 UpdateCrlRequestRequestTypeDef = TypedDict(
     "UpdateCrlRequestRequestTypeDef",
     {
         "crlId": str,
         "crlData": NotRequired[BlobTypeDef],
         "name": NotRequired[str],
     },
@@ -335,29 +353,14 @@
         "lastSeenAt": NotRequired[datetime],
         "subjectArn": NotRequired[str],
         "subjectId": NotRequired[str],
         "updatedAt": NotRequired[datetime],
         "x509Subject": NotRequired[str],
     },
 )
-ListProfilesResponseTypeDef = TypedDict(
-    "ListProfilesResponseTypeDef",
-    {
-        "nextToken": str,
-        "profiles": List[ProfileDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-ProfileDetailResponseTypeDef = TypedDict(
-    "ProfileDetailResponseTypeDef",
-    {
-        "profile": ProfileDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 ListRequestListCrlsPaginateTypeDef = TypedDict(
     "ListRequestListCrlsPaginateTypeDef",
     {
         "pageSize": NotRequired[int],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
@@ -400,14 +403,32 @@
 SourceTypeDef = TypedDict(
     "SourceTypeDef",
     {
         "sourceData": NotRequired[SourceDataTypeDef],
         "sourceType": NotRequired[TrustAnchorTypeType],
     },
 )
+ProfileDetailTypeDef = TypedDict(
+    "ProfileDetailTypeDef",
+    {
+        "attributeMappings": NotRequired[List[AttributeMappingTypeDef]],
+        "createdAt": NotRequired[datetime],
+        "createdBy": NotRequired[str],
+        "durationSeconds": NotRequired[int],
+        "enabled": NotRequired[bool],
+        "managedPolicyArns": NotRequired[List[str]],
+        "name": NotRequired[str],
+        "profileArn": NotRequired[str],
+        "profileId": NotRequired[str],
+        "requireInstanceProperties": NotRequired[bool],
+        "roleArns": NotRequired[List[str]],
+        "sessionPolicy": NotRequired[str],
+        "updatedAt": NotRequired[datetime],
+    },
+)
 SubjectDetailResponseTypeDef = TypedDict(
     "SubjectDetailResponseTypeDef",
     {
         "subject": SubjectDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -438,14 +459,43 @@
     "UpdateTrustAnchorRequestRequestTypeDef",
     {
         "trustAnchorId": str,
         "name": NotRequired[str],
         "source": NotRequired[SourceTypeDef],
     },
 )
+DeleteAttributeMappingResponseTypeDef = TypedDict(
+    "DeleteAttributeMappingResponseTypeDef",
+    {
+        "profile": ProfileDetailTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ListProfilesResponseTypeDef = TypedDict(
+    "ListProfilesResponseTypeDef",
+    {
+        "nextToken": str,
+        "profiles": List[ProfileDetailTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ProfileDetailResponseTypeDef = TypedDict(
+    "ProfileDetailResponseTypeDef",
+    {
+        "profile": ProfileDetailTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+PutAttributeMappingResponseTypeDef = TypedDict(
+    "PutAttributeMappingResponseTypeDef",
+    {
+        "profile": ProfileDetailTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ListTrustAnchorsResponseTypeDef = TypedDict(
     "ListTrustAnchorsResponseTypeDef",
     {
         "nextToken": str,
         "trustAnchors": List[TrustAnchorDetailTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/type_defs.pyi` & `mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 Type annotations for rolesanywhere service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_rolesanywhere.type_defs import BlobTypeDef
+    from mypy_boto3_rolesanywhere.type_defs import MappingRuleTypeDef
 
-    data: BlobTypeDef = ...
+    data: MappingRuleTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
 
-from .literals import NotificationEventType, TrustAnchorTypeType
+from .literals import CertificateFieldType, NotificationEventType, TrustAnchorTypeType
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 12):
     from typing import NotRequired
@@ -30,63 +30,75 @@
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "MappingRuleTypeDef",
     "BlobTypeDef",
     "TagTypeDef",
     "NotificationSettingTypeDef",
     "CredentialSummaryTypeDef",
     "CrlDetailTypeDef",
     "ResponseMetadataTypeDef",
+    "DeleteAttributeMappingRequestRequestTypeDef",
     "InstancePropertyTypeDef",
-    "ProfileDetailTypeDef",
     "PaginatorConfigTypeDef",
     "ListRequestRequestTypeDef",
     "SubjectSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "NotificationSettingDetailTypeDef",
     "NotificationSettingKeyTypeDef",
     "ScalarCrlRequestRequestTypeDef",
     "ScalarProfileRequestRequestTypeDef",
     "ScalarSubjectRequestRequestTypeDef",
     "ScalarTrustAnchorRequestRequestTypeDef",
     "SourceDataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateProfileRequestRequestTypeDef",
+    "AttributeMappingTypeDef",
+    "PutAttributeMappingRequestRequestTypeDef",
     "UpdateCrlRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "ImportCrlRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "PutNotificationSettingsRequestRequestTypeDef",
     "CrlDetailResponseTypeDef",
     "ListCrlsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "SubjectDetailTypeDef",
-    "ListProfilesResponseTypeDef",
-    "ProfileDetailResponseTypeDef",
     "ListRequestListCrlsPaginateTypeDef",
     "ListRequestListProfilesPaginateTypeDef",
     "ListRequestListSubjectsPaginateTypeDef",
     "ListRequestListTrustAnchorsPaginateTypeDef",
     "ListSubjectsResponseTypeDef",
     "ResetNotificationSettingsRequestRequestTypeDef",
     "SourceTypeDef",
+    "ProfileDetailTypeDef",
     "SubjectDetailResponseTypeDef",
     "CreateTrustAnchorRequestRequestTypeDef",
     "TrustAnchorDetailTypeDef",
     "UpdateTrustAnchorRequestRequestTypeDef",
+    "DeleteAttributeMappingResponseTypeDef",
+    "ListProfilesResponseTypeDef",
+    "ProfileDetailResponseTypeDef",
+    "PutAttributeMappingResponseTypeDef",
     "ListTrustAnchorsResponseTypeDef",
     "PutNotificationSettingsResponseTypeDef",
     "ResetNotificationSettingsResponseTypeDef",
     "TrustAnchorDetailResponseTypeDef",
 )
 
+MappingRuleTypeDef = TypedDict(
+    "MappingRuleTypeDef",
+    {
+        "specifier": str,
+    },
+)
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
@@ -130,39 +142,30 @@
         "RequestId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
         "HostId": NotRequired[str],
     },
 )
+DeleteAttributeMappingRequestRequestTypeDef = TypedDict(
+    "DeleteAttributeMappingRequestRequestTypeDef",
+    {
+        "certificateField": CertificateFieldType,
+        "profileId": str,
+        "specifiers": NotRequired[Sequence[str]],
+    },
+)
 InstancePropertyTypeDef = TypedDict(
     "InstancePropertyTypeDef",
     {
         "failed": NotRequired[bool],
         "properties": NotRequired[Dict[str, str]],
         "seenAt": NotRequired[datetime],
     },
 )
-ProfileDetailTypeDef = TypedDict(
-    "ProfileDetailTypeDef",
-    {
-        "createdAt": NotRequired[datetime],
-        "createdBy": NotRequired[str],
-        "durationSeconds": NotRequired[int],
-        "enabled": NotRequired[bool],
-        "managedPolicyArns": NotRequired[List[str]],
-        "name": NotRequired[str],
-        "profileArn": NotRequired[str],
-        "profileId": NotRequired[str],
-        "requireInstanceProperties": NotRequired[bool],
-        "roleArns": NotRequired[List[str]],
-        "sessionPolicy": NotRequired[str],
-        "updatedAt": NotRequired[datetime],
-    },
-)
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": NotRequired[int],
         "PageSize": NotRequired[int],
         "StartingToken": NotRequired[str],
     },
@@ -254,14 +257,29 @@
         "durationSeconds": NotRequired[int],
         "managedPolicyArns": NotRequired[Sequence[str]],
         "name": NotRequired[str],
         "roleArns": NotRequired[Sequence[str]],
         "sessionPolicy": NotRequired[str],
     },
 )
+AttributeMappingTypeDef = TypedDict(
+    "AttributeMappingTypeDef",
+    {
+        "certificateField": NotRequired[CertificateFieldType],
+        "mappingRules": NotRequired[List[MappingRuleTypeDef]],
+    },
+)
+PutAttributeMappingRequestRequestTypeDef = TypedDict(
+    "PutAttributeMappingRequestRequestTypeDef",
+    {
+        "certificateField": CertificateFieldType,
+        "mappingRules": Sequence[MappingRuleTypeDef],
+        "profileId": str,
+    },
+)
 UpdateCrlRequestRequestTypeDef = TypedDict(
     "UpdateCrlRequestRequestTypeDef",
     {
         "crlId": str,
         "crlData": NotRequired[BlobTypeDef],
         "name": NotRequired[str],
     },
@@ -335,29 +353,14 @@
         "lastSeenAt": NotRequired[datetime],
         "subjectArn": NotRequired[str],
         "subjectId": NotRequired[str],
         "updatedAt": NotRequired[datetime],
         "x509Subject": NotRequired[str],
     },
 )
-ListProfilesResponseTypeDef = TypedDict(
-    "ListProfilesResponseTypeDef",
-    {
-        "nextToken": str,
-        "profiles": List[ProfileDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-ProfileDetailResponseTypeDef = TypedDict(
-    "ProfileDetailResponseTypeDef",
-    {
-        "profile": ProfileDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 ListRequestListCrlsPaginateTypeDef = TypedDict(
     "ListRequestListCrlsPaginateTypeDef",
     {
         "pageSize": NotRequired[int],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
@@ -400,14 +403,32 @@
 SourceTypeDef = TypedDict(
     "SourceTypeDef",
     {
         "sourceData": NotRequired[SourceDataTypeDef],
         "sourceType": NotRequired[TrustAnchorTypeType],
     },
 )
+ProfileDetailTypeDef = TypedDict(
+    "ProfileDetailTypeDef",
+    {
+        "attributeMappings": NotRequired[List[AttributeMappingTypeDef]],
+        "createdAt": NotRequired[datetime],
+        "createdBy": NotRequired[str],
+        "durationSeconds": NotRequired[int],
+        "enabled": NotRequired[bool],
+        "managedPolicyArns": NotRequired[List[str]],
+        "name": NotRequired[str],
+        "profileArn": NotRequired[str],
+        "profileId": NotRequired[str],
+        "requireInstanceProperties": NotRequired[bool],
+        "roleArns": NotRequired[List[str]],
+        "sessionPolicy": NotRequired[str],
+        "updatedAt": NotRequired[datetime],
+    },
+)
 SubjectDetailResponseTypeDef = TypedDict(
     "SubjectDetailResponseTypeDef",
     {
         "subject": SubjectDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -438,14 +459,43 @@
     "UpdateTrustAnchorRequestRequestTypeDef",
     {
         "trustAnchorId": str,
         "name": NotRequired[str],
         "source": NotRequired[SourceTypeDef],
     },
 )
+DeleteAttributeMappingResponseTypeDef = TypedDict(
+    "DeleteAttributeMappingResponseTypeDef",
+    {
+        "profile": ProfileDetailTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ListProfilesResponseTypeDef = TypedDict(
+    "ListProfilesResponseTypeDef",
+    {
+        "nextToken": str,
+        "profiles": List[ProfileDetailTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ProfileDetailResponseTypeDef = TypedDict(
+    "ProfileDetailResponseTypeDef",
+    {
+        "profile": ProfileDetailTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+PutAttributeMappingResponseTypeDef = TypedDict(
+    "PutAttributeMappingResponseTypeDef",
+    {
+        "profile": ProfileDetailTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ListTrustAnchorsResponseTypeDef = TypedDict(
     "ListTrustAnchorsResponseTypeDef",
     {
         "nextToken": str,
         "trustAnchors": List[TrustAnchorDetailTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere.egg-info/PKG-INFO` & `mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rolesanywhere
-Version: 1.34.76
-Summary: Type annotations for boto3.IAMRolesAnywhere 1.34.76 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.87
+Summary: Type annotations for boto3.IAMRolesAnywhere 1.34.87 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rolesanywhere)](https://pepy.tech/project/mypy-boto3-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAMRolesAnywhere 1.34.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[boto3.IAMRolesAnywhere 1.34.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -309,35 +309,35 @@
 `mypy_boto3_rolesanywhere.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 Full list of `IAMRolesAnywhere` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/literals/).
 
 ```python
-from mypy_boto3_rolesanywhere.literals import ListCrlsPaginatorName
+from mypy_boto3_rolesanywhere.literals import CertificateFieldType
 
 
-def check_value(value: ListCrlsPaginatorName) -> bool: ...
+def check_value(value: CertificateFieldType) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_rolesanywhere.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
 Full list of `IAMRolesAnywhere` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/type_defs/).
 
 ```python
-from mypy_boto3_rolesanywhere.type_defs import BlobTypeDef
+from mypy_boto3_rolesanywhere.type_defs import MappingRuleTypeDef
 
 
-def get_value() -> BlobTypeDef:
+def get_value() -> MappingRuleTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt` & `mypy_boto3_rolesanywhere-1.34.87/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.34.76/setup.py` & `mypy_boto3_rolesanywhere-1.34.87/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rolesanywhere",
-    version="1.34.76",
+    version="1.34.87",
     packages=["mypy_boto3_rolesanywhere"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.IAMRolesAnywhere 1.34.76 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.IAMRolesAnywhere 1.34.87 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

