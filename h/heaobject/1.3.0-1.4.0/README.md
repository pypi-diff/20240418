# Comparing `tmp/heaobject-1.3.0.tar.gz` & `tmp/heaobject-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaobject-1.3.0.tar", last modified: Tue Apr  9 20:33:04 2024, max compression
+gzip compressed data, was "heaobject-1.4.0.tar", last modified: Thu Apr 18 01:58:27 2024, max compression
```

## Comparing `heaobject-1.3.0.tar` & `heaobject-1.4.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 20:33:04.823929 heaobject-1.3.0/
--rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:08.000000 heaobject-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     4577 2024-04-09 20:33:04.822379 heaobject-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3071 2024-04-09 20:32:03.000000 heaobject-1.3.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-09 20:33:04.823929 heaobject-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2603 2024-04-09 20:32:18.000000 heaobject-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:33:04.760568 heaobject-1.3.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-09 20:33:04.810910 heaobject-1.3.0/src/heaobject/
--rw-rw-rw-   0        0        0     1247 2023-12-16 22:23:08.000000 heaobject-1.3.0/src/heaobject/__init__.py
--rw-rw-rw-   0        0        0     4970 2024-04-08 19:24:00.000000 heaobject-1.3.0/src/heaobject/account.py
--rw-rw-rw-   0        0        0    15629 2024-04-08 21:10:04.000000 heaobject-1.3.0/src/heaobject/activity.py
--rw-rw-rw-   0        0        0     4030 2023-12-16 22:23:08.000000 heaobject-1.3.0/src/heaobject/aws.py
--rw-rw-rw-   0        0        0     6945 2023-12-16 22:23:08.000000 heaobject-1.3.0/src/heaobject/awss3key.py
--rw-rw-rw-   0        0        0     7587 2024-04-08 19:25:10.000000 heaobject-1.3.0/src/heaobject/bucket.py
--rw-rw-rw-   0        0        0     9918 2024-04-09 02:58:26.000000 heaobject-1.3.0/src/heaobject/data.py
--rw-rw-rw-   0        0        0     2604 2023-12-16 22:23:08.000000 heaobject-1.3.0/src/heaobject/dataadapter.py
--rw-rw-rw-   0        0        0      272 2022-03-11 01:28:08.000000 heaobject-1.3.0/src/heaobject/dataelement.py
--rw-rw-rw-   0        0        0     1601 2022-03-11 01:28:08.000000 heaobject-1.3.0/src/heaobject/datamodel.py
--rw-rw-rw-   0        0        0      430 2022-03-11 01:28:08.000000 heaobject-1.3.0/src/heaobject/datapattern.py
--rw-rw-rw-   0        0        0      238 2023-12-16 22:23:08.000000 heaobject-1.3.0/src/heaobject/datatransform.py
--rw-rw-rw-   0        0        0      353 2023-12-16 22:23:08.000000 heaobject-1.3.0/src/heaobject/error.py
--rw-rw-rw-   0        0        0    22016 2024-04-09 02:44:56.000000 heaobject-1.3.0/src/heaobject/folder.py
--rw-rw-rw-   0        0        0     4662 2024-04-08 21:18:25.000000 heaobject-1.3.0/src/heaobject/keychain.py
--rw-rw-rw-   0        0        0     2859 2024-04-09 17:09:46.000000 heaobject-1.3.0/src/heaobject/mimetype.py
--rw-rw-rw-   0        0        0     9112 2024-04-08 21:14:14.000000 heaobject-1.3.0/src/heaobject/organization.py
--rw-rw-rw-   0        0        0     7773 2024-04-08 19:27:20.000000 heaobject-1.3.0/src/heaobject/person.py
--rw-rw-rw-   0        0        0     5129 2024-04-09 03:35:48.000000 heaobject-1.3.0/src/heaobject/project.py
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:08.000000 heaobject-1.3.0/src/heaobject/py.typed
--rw-rw-rw-   0        0        0      211 2024-04-08 21:13:57.000000 heaobject-1.3.0/src/heaobject/record.py
--rw-rw-rw-   0        0        0    24659 2024-04-08 19:28:44.000000 heaobject-1.3.0/src/heaobject/registry.py
--rw-rw-rw-   0        0        0    76096 2024-04-08 22:19:18.000000 heaobject-1.3.0/src/heaobject/root.py
--rw-rw-rw-   0        0        0      597 2024-04-08 21:13:45.000000 heaobject-1.3.0/src/heaobject/settings.py
--rw-rw-rw-   0        0        0       66 2024-03-26 22:41:59.000000 heaobject-1.3.0/src/heaobject/source.py
--rw-rw-rw-   0        0        0     1165 2023-12-16 22:23:08.000000 heaobject-1.3.0/src/heaobject/source2target.py
--rw-rw-rw-   0        0        0     4074 2024-04-08 21:13:30.000000 heaobject-1.3.0/src/heaobject/storage.py
--rw-rw-rw-   0        0        0     9678 2024-04-08 21:11:57.000000 heaobject-1.3.0/src/heaobject/trash.py
--rw-rw-rw-   0        0        0     1135 2024-03-26 22:41:59.000000 heaobject-1.3.0/src/heaobject/user.py
--rw-rw-rw-   0        0        0      498 2023-12-16 22:23:08.000000 heaobject-1.3.0/src/heaobject/util.py
--rw-rw-rw-   0        0        0     6618 2024-04-08 21:11:29.000000 heaobject-1.3.0/src/heaobject/volume.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:33:04.820833 heaobject-1.3.0/src/heaobject.egg-info/
--rw-rw-rw-   0        0        0     4577 2024-04-09 20:33:04.000000 heaobject-1.3.0/src/heaobject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      995 2024-04-09 20:33:04.000000 heaobject-1.3.0/src/heaobject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 20:33:04.000000 heaobject-1.3.0/src/heaobject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-04-09 20:33:04.000000 heaobject-1.3.0/src/heaobject.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-09 20:33:04.000000 heaobject-1.3.0/src/heaobject.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 01:58:27.040990 heaobject-1.4.0/
+-rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:08.000000 heaobject-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0     4708 2024-04-18 01:58:27.038983 heaobject-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3202 2024-04-18 01:57:27.000000 heaobject-1.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-18 01:58:27.040990 heaobject-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2603 2024-04-18 01:57:54.000000 heaobject-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 01:58:26.981137 heaobject-1.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-18 01:58:27.026978 heaobject-1.4.0/src/heaobject/
+-rw-rw-rw-   0        0        0     1247 2023-12-16 22:23:08.000000 heaobject-1.4.0/src/heaobject/__init__.py
+-rw-rw-rw-   0        0        0     4970 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/account.py
+-rw-rw-rw-   0        0        0    15629 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/activity.py
+-rw-rw-rw-   0        0        0     4030 2023-12-16 22:23:08.000000 heaobject-1.4.0/src/heaobject/aws.py
+-rw-rw-rw-   0        0        0     6945 2023-12-16 22:23:08.000000 heaobject-1.4.0/src/heaobject/awss3key.py
+-rw-rw-rw-   0        0        0     7587 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/bucket.py
+-rw-rw-rw-   0        0        0     9918 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/data.py
+-rw-rw-rw-   0        0        0     2604 2023-12-16 22:23:08.000000 heaobject-1.4.0/src/heaobject/dataadapter.py
+-rw-rw-rw-   0        0        0      272 2022-03-11 01:28:08.000000 heaobject-1.4.0/src/heaobject/dataelement.py
+-rw-rw-rw-   0        0        0     1601 2022-03-11 01:28:08.000000 heaobject-1.4.0/src/heaobject/datamodel.py
+-rw-rw-rw-   0        0        0      430 2022-03-11 01:28:08.000000 heaobject-1.4.0/src/heaobject/datapattern.py
+-rw-rw-rw-   0        0        0      238 2023-12-16 22:23:08.000000 heaobject-1.4.0/src/heaobject/datatransform.py
+-rw-rw-rw-   0        0        0      353 2023-12-16 22:23:08.000000 heaobject-1.4.0/src/heaobject/error.py
+-rw-rw-rw-   0        0        0    22016 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/folder.py
+-rw-rw-rw-   0        0        0     4662 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/keychain.py
+-rw-rw-rw-   0        0        0     2859 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/mimetype.py
+-rw-rw-rw-   0        0        0     9112 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/organization.py
+-rw-rw-rw-   0        0        0    10842 2024-04-18 01:33:48.000000 heaobject-1.4.0/src/heaobject/person.py
+-rw-rw-rw-   0        0        0     5129 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/project.py
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:08.000000 heaobject-1.4.0/src/heaobject/py.typed
+-rw-rw-rw-   0        0        0      211 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/record.py
+-rw-rw-rw-   0        0        0    24659 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/registry.py
+-rw-rw-rw-   0        0        0    76096 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/root.py
+-rw-rw-rw-   0        0        0      597 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/settings.py
+-rw-rw-rw-   0        0        0       66 2024-03-26 22:41:59.000000 heaobject-1.4.0/src/heaobject/source.py
+-rw-rw-rw-   0        0        0     1165 2023-12-16 22:23:08.000000 heaobject-1.4.0/src/heaobject/source2target.py
+-rw-rw-rw-   0        0        0     4074 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/storage.py
+-rw-rw-rw-   0        0        0    10289 2024-04-18 01:52:57.000000 heaobject-1.4.0/src/heaobject/trash.py
+-rw-rw-rw-   0        0        0     1135 2024-03-26 22:41:59.000000 heaobject-1.4.0/src/heaobject/user.py
+-rw-rw-rw-   0        0        0      498 2023-12-16 22:23:08.000000 heaobject-1.4.0/src/heaobject/util.py
+-rw-rw-rw-   0        0        0     6618 2024-04-09 20:34:56.000000 heaobject-1.4.0/src/heaobject/volume.py
+drwxrwxrwx   0        0        0        0 2024-04-18 01:58:27.037983 heaobject-1.4.0/src/heaobject.egg-info/
+-rw-rw-rw-   0        0        0     4708 2024-04-18 01:58:26.000000 heaobject-1.4.0/src/heaobject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      995 2024-04-18 01:58:26.000000 heaobject-1.4.0/src/heaobject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 01:58:26.000000 heaobject-1.4.0/src/heaobject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-04-18 01:58:26.000000 heaobject-1.4.0/src/heaobject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-18 01:58:26.000000 heaobject-1.4.0/src/heaobject.egg-info/top_level.txt
```

### Comparing `heaobject-1.3.0/LICENSE` & `heaobject-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaobject-1.3.0/PKG-INFO` & `heaobject-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaobject
-Version: 1.3.0
+Version: 1.4.0
 Summary: Data and other classes that are passed into and out of HEA REST APIs.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,18 @@
 Requires-Dist: mimetype-description~=0.1.0
 
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.4.0
+* Added "deleted" attribute to the trash module's TrashItem class.
+* Added Group class to the person module.
+
 ## Version 1.3.0
 * Added type_display_name attribute to all HEA objects.
 
 ## Version 1.2.0
 * Created AbstractAssociation base class for complex associations between desktop objects.
 * Used it for the association between organizations and accounts, and volumes and accounts.
```

### Comparing `heaobject-1.3.0/README.md` & `heaobject-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.4.0
+* Added "deleted" attribute to the trash module's TrashItem class.
+* Added Group class to the person module.
+
 ## Version 1.3.0
 * Added type_display_name attribute to all HEA objects.
 
 ## Version 1.2.0
 * Created AbstractAssociation base class for complex associations between desktop objects.
 * Used it for the association between organizations and accounts, and volumes and accounts.
```

### Comparing `heaobject-1.3.0/setup.py` & `heaobject-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(name='heaobject',
-                 version='1.3.0',
+                 version='1.4.0',
                  description='Data and other classes that are passed into and out of HEA REST APIs.',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://risr.hci.utah.edu',
                  author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
                  author_email='Andrew.Post@hci.utah.edu',
                  python_requires='>=3.10',
```

### Comparing `heaobject-1.3.0/src/heaobject/__init__.py` & `heaobject-1.4.0/src/heaobject/__init__.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.3.0/src/heaobject/account.py` & `heaobject-1.4.0/src/heaobject/account.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.3.0/src/heaobject/activity.py` & `heaobject-1.4.0/src/heaobject/activity.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.3.0/src/heaobject/aws.py` & `heaobject-1.4.0/src/heaobject/aws.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.3.0/src/heaobject/awss3key.py` & `heaobject-1.4.0/src/heaobject/awss3key.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.3.0/src/heaobject/bucket.py` & `heaobject-1.4.0/src/heaobject/bucket.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.3.0/src/heaobject/data.py` & `heaobject-1.4.0/src/heaobject/data.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.3.0/src/heaobject/dataadapter.py` & `heaobject-1.4.0/src/heaobject/dataadapter.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.3.0/src/heaobject/datamodel.py` & `heaobject-1.4.0/src/heaobject/datamodel.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.3.0/src/heaobject/folder.py` & `heaobject-1.4.0/src/heaobject/folder.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.3.0/src/heaobject/keychain.py` & `heaobject-1.4.0/src/heaobject/keychain.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.3.0/src/heaobject/mimetype.py` & `heaobject-1.4.0/src/heaobject/mimetype.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.3.0/src/heaobject/organization.py` & `heaobject-1.4.0/src/heaobject/organization.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.3.0/src/heaobject/person.py` & `heaobject-1.4.0/src/heaobject/person.py`

 * *Files 21% similar despite different names*

```diff
@@ -129,14 +129,15 @@
     this class supports compatibility with file systems with role-based authorization like Amazon Web Services S3
     buckets. The id and name attributes are synchronized with the role attribute such that setting one automatically
     populates the others.
     """
     def __init__(self):
         super().__init__()
         self.__role: str | None = None
+        self.__display_name: str | None = None
 
     @property
     def id(self) -> str | None:
         """
         The role, base64-encoded using this module's encode_role() function. Setting this attribute automatically
         generates values for the name and role attributes.
         """
@@ -165,19 +166,86 @@
         The role. Setting this attribute automatically generates values for the id and name attributes.
         """
         return self.__role
 
     @role.setter
     def role(self, role: str | None):
         self.__role = str(role) if role is not None else role
+        if self.__display_name is None:
+            self.__display_name = self.__role
 
     @property
     def type_display_name(self) -> str:
         return 'Role'
 
+    @property
+    def display_name(self) -> str:
+        return self.__display_name if self.__display_name is not None else super().display_name
+
+    @display_name.setter
+    def display_name(self, display_name: str):
+        self.__display_name = str(display_name) if display_name is not None else None
+
+class Group(AbstractDesktopObject):
+    """
+    A user group, for authorization purposes. The id and name attributes are synchronized with the group attribute such
+    that setting one automatically populates the others.
+    """
+    def __init__(self):
+        super().__init__()
+        self.__group: str | None = None
+        self.__display_name: str | None = None
+
+    @property
+    def id(self) -> str | None:
+        """
+        The group, base64-encoded using this module's encode_group() function. Setting this attribute automatically
+        generates values for the name and group attributes.
+        """
+        return self.name
+
+    @id.setter
+    def id(self, id_: str | None):
+        self.name = id_
+
+    @property
+    def name(self) -> str | None:
+        """
+        The group, base64-encoded using this module's encode_group() function. Setting this attribute automatically
+        generates values for the id and group attributes.
+        """
+        group_ = self.group
+        return encode_group(group_) if group_ is not None else None
+
+    @name.setter
+    def name(self, name: str | None):
+        self.group = decode_group(name) if name is not None else None
+
+    @property
+    def group(self) -> str | None:
+        return self.__group
+
+    @group.setter
+    def group(self, group: str | None):
+        self.__group = str(group) if group is not None else None
+        if self.__display_name is None:
+            self.__display_name = self.__group
+
+    @property
+    def type_display_name(self) -> str:
+        return 'Group'
+
+    @property
+    def display_name(self) -> str:
+        return self.__display_name if self.__display_name is not None else super().display_name
+
+    @display_name.setter
+    def display_name(self, display_name: str):
+        self.__display_name = str(display_name) if display_name is not None else None
+
 
 def encode_role(role: str) -> str:
     """
     Encodes a role string using the Base 64 URL- and filesystem-safe alphabet, which replaces '+' with '-' and '/' with
     '_' in the base 64 alphabet as described in the IETF RFC 4648 specification section 5.
 
     :param role: the role string (required).
@@ -190,14 +258,32 @@
     Decodes a string encoded using this module's encode_role() function.
 
     :param role_encoded: the encoded role string (required).
     :returns: the decoded data as a utf-8 string.
     """
     return urlsafe_b64decode(role_encoded).decode(ROLE_ENCODING)
 
+def encode_group(group: str) -> str:
+    """
+    Encodes a group string using the Base 64 URL- and filesystem-safe alphabet, which replaces '+' with '-' and '/' with
+    '_' in the base 64 alphabet as described in the IETF RFC 4648 specification section 5.
+
+    :param group: the group string (required).
+    :returns: returns the encoded data as a utf-8 string.
+    """
+    return encode_role(group)
+
+def decode_group(group_encoded: str) -> str:
+    """
+    Decodes a string encoded using this module's encode_group() function.
+
+    :param group_encoded: the encoded group string (required).
+    :returns: the decoded data as a utf-8 string.
+    """
+    return decode_role(group_encoded)
 
 def get_system_person(id_: str) -> Person:
     """
     Gets a Person object for the system user with the given id_ (from heaobject.user).
 
     :param id_: the id of the system user (required).
     :returns: the Person object.
```

### Comparing `heaobject-1.3.0/src/heaobject/project.py` & `heaobject-1.4.0/src/heaobject/project.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.3.0/src/heaobject/registry.py` & `heaobject-1.4.0/src/heaobject/registry.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.3.0/src/heaobject/root.py` & `heaobject-1.4.0/src/heaobject/root.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.3.0/src/heaobject/settings.py` & `heaobject-1.4.0/src/heaobject/settings.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.3.0/src/heaobject/source2target.py` & `heaobject-1.4.0/src/heaobject/source2target.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.3.0/src/heaobject/storage.py` & `heaobject-1.4.0/src/heaobject/storage.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.3.0/src/heaobject/trash.py` & `heaobject-1.4.0/src/heaobject/trash.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 """
 from abc import ABC, abstractmethod
 from heaobject.aws import S3_URI_PATTERN, s3_uri, S3StorageClassMixin
 from heaobject.awss3key import KeyDecodeException, decode_key, encode_key, is_folder
 from heaobject.data import AWSS3FileObject
 from heaobject.folder import AWSS3Folder
 from .root import AbstractDesktopObject, HasSize, View, desktop_object_type_for_name
-
+from datetime import date
+from typing import Optional
+from dateutil import parser as dateparser
 
 class TrashItem(AbstractDesktopObject, View, ABC):
     """
     Abstract base class for trash items. Trash items are an alternative
     representation of the desktop object that was put in the trash.
     """
     @abstractmethod
     def __init__(self) -> None:
         super().__init__()
-        self.__original_location: str | None = None
+        self.__deleted: date | None = None
 
     @property
     @abstractmethod
     def original_location(self) -> str | None:
         """
         The object's original location. The format of the location string is
         unique for different subclasses.
@@ -32,14 +34,29 @@
 
     @original_location.setter
     @abstractmethod
     def original_location(self, original_location: str | None):
         pass
 
     @property
+    def deleted(self) -> Optional[date]:
+        """
+        The date the deleted object was deleted (the date the objects' delete marker was created).
+        """
+        return self.__deleted
+
+
+    @deleted.setter
+    def deleted(self, deleted: date | None):
+        if deleted is None or isinstance(deleted, date):
+            self.__deleted = deleted
+        else:
+            self.__deleted = dateparser.isoparse(deleted) # TODO Use datetime.fromisoformat after we switch to python 3.11.
+
+    @property
     def human_readable_original_location(self) -> str | None:
         """
         The object's original location in human readable form. By default, it
         mirrors the value of the original_location property.
         """
         return self.original_location
```

### Comparing `heaobject-1.3.0/src/heaobject/user.py` & `heaobject-1.4.0/src/heaobject/user.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.3.0/src/heaobject/volume.py` & `heaobject-1.4.0/src/heaobject/volume.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.3.0/src/heaobject.egg-info/PKG-INFO` & `heaobject-1.4.0/src/heaobject.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaobject
-Version: 1.3.0
+Version: 1.4.0
 Summary: Data and other classes that are passed into and out of HEA REST APIs.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,18 @@
 Requires-Dist: mimetype-description~=0.1.0
 
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.4.0
+* Added "deleted" attribute to the trash module's TrashItem class.
+* Added Group class to the person module.
+
 ## Version 1.3.0
 * Added type_display_name attribute to all HEA objects.
 
 ## Version 1.2.0
 * Created AbstractAssociation base class for complex associations between desktop objects.
 * Used it for the association between organizations and accounts, and volumes and accounts.
```

### Comparing `heaobject-1.3.0/src/heaobject.egg-info/SOURCES.txt` & `heaobject-1.4.0/src/heaobject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

