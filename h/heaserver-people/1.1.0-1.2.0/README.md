# Comparing `tmp/heaserver-people-1.1.0.tar.gz` & `tmp/heaserver_people-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-people-1.1.0.tar", last modified: Tue Mar 26 23:05:43 2024, max compression
+gzip compressed data, was "heaserver_people-1.2.0.tar", last modified: Thu Apr 18 03:45:58 2024, max compression
```

## Comparing `heaserver-people-1.1.0.tar` & `heaserver_people-1.2.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 23:05:43.106121 heaserver-people-1.1.0/
--rw-rw-rw-   0        0        0      261 2023-12-18 20:25:25.000000 heaserver-people-1.1.0/.editorconfig
--rw-rw-rw-   0        0        0      353 2023-12-18 20:25:25.000000 heaserver-people-1.1.0/.gitignore
--rw-rw-rw-   0        0        0    11625 2023-12-18 20:25:26.000000 heaserver-people-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      243 2023-12-18 20:25:26.000000 heaserver-people-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5156 2024-03-26 23:05:43.104019 heaserver-people-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3798 2024-03-26 23:05:06.000000 heaserver-people-1.1.0/README.md
--rw-rw-rw-   0        0        0     1878 2023-12-18 20:25:26.000000 heaserver-people-1.1.0/RELEASING.md
-drwxrwxrwx   0        0        0        0 2024-03-26 23:05:43.059799 heaserver-people-1.1.0/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-03-26 23:05:43.075798 heaserver-people-1.1.0/integrationtests/.pytest_cache/
--rw-rw-rw-   0        0        0       39 2023-02-23 16:41:17.000000 heaserver-people-1.1.0/integrationtests/.pytest_cache/.gitignore
--rw-rw-rw-   0        0        0      194 2023-02-23 16:41:17.000000 heaserver-people-1.1.0/integrationtests/.pytest_cache/CACHEDIR.TAG
--rw-rw-rw-   0        0        0      303 2023-02-23 16:41:17.000000 heaserver-people-1.1.0/integrationtests/.pytest_cache/README.md
-drwxrwxrwx   0        0        0        0 2024-03-26 23:05:43.058851 heaserver-people-1.1.0/integrationtests/.pytest_cache/v/
-drwxrwxrwx   0        0        0        0 2024-03-26 23:05:43.077798 heaserver-people-1.1.0/integrationtests/.pytest_cache/v/cache/
--rw-rw-rw-   0        0        0        2 2023-02-23 16:42:55.000000 heaserver-people-1.1.0/integrationtests/.pytest_cache/v/cache/nodeids
--rw-rw-rw-   0        0        0        2 2023-02-23 16:42:55.000000 heaserver-people-1.1.0/integrationtests/.pytest_cache/v/cache/stepwise
-drwxrwxrwx   0        0        0        0 2024-03-26 23:05:43.059799 heaserver-people-1.1.0/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-26 23:05:43.081836 heaserver-people-1.1.0/integrationtests/heaserver/personintegrationtest/
--rw-rw-rw-   0        0        0        0 2023-12-18 20:25:26.000000 heaserver-people-1.1.0/integrationtests/heaserver/personintegrationtest/__init__.py
--rw-rw-rw-   0        0        0     4590 2024-03-26 23:05:06.000000 heaserver-people-1.1.0/integrationtests/heaserver/personintegrationtest/permissionstestcase.py
--rw-rw-rw-   0        0        0      547 2024-02-25 02:42:01.000000 heaserver-people-1.1.0/integrationtests/heaserver/personintegrationtest/test_all.py
--rw-rw-rw-   0        0        0     7809 2024-03-26 23:05:06.000000 heaserver-people-1.1.0/integrationtests/heaserver/personintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      111 2023-12-18 20:25:26.000000 heaserver-people-1.1.0/pytest.ini
--rw-rw-rw-   0        0        0      248 2023-12-18 20:25:26.000000 heaserver-people-1.1.0/requirements_dev.txt
--rw-rw-rw-   0        0        0       42 2024-03-26 23:05:43.106121 heaserver-people-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1854 2024-03-26 23:05:23.000000 heaserver-people-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-26 23:05:43.061799 heaserver-people-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-03-26 23:05:43.060799 heaserver-people-1.1.0/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-26 23:05:43.088835 heaserver-people-1.1.0/src/heaserver/person/
--rw-rw-rw-   0        0        0        0 2023-12-18 20:25:26.000000 heaserver-people-1.1.0/src/heaserver/person/__init__.py
--rw-rw-rw-   0        0        0     4121 2024-02-25 02:42:01.000000 heaserver-people-1.1.0/src/heaserver/person/keycloakmockmongotestcase.py
--rw-rw-rw-   0        0        0    23691 2024-03-26 23:05:06.000000 heaserver-people-1.1.0/src/heaserver/person/keycloakmongo.py
--rw-rw-rw-   0        0        0    10027 2024-03-26 23:05:06.000000 heaserver-people-1.1.0/src/heaserver/person/keycloakmongotestcase.py
--rw-rw-rw-   0        0        0    11491 2024-03-07 16:44:50.000000 heaserver-people-1.1.0/src/heaserver/person/service.py
--rw-rw-rw-   0        0        0     1772 2023-12-18 20:25:26.000000 heaserver-people-1.1.0/src/heaserver/person/testcasedata.py
-drwxrwxrwx   0        0        0        0 2024-03-26 23:05:43.089836 heaserver-people-1.1.0/src/heaserver/person/wstl/
--rw-rw-rw-   0        0        0    11409 2024-03-07 16:44:50.000000 heaserver-people-1.1.0/src/heaserver/person/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-03-26 23:05:43.102946 heaserver-people-1.1.0/src/heaserver_people.egg-info/
--rw-rw-rw-   0        0        0     5156 2024-03-26 23:05:43.000000 heaserver-people-1.1.0/src/heaserver_people.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1289 2024-03-26 23:05:43.000000 heaserver-people-1.1.0/src/heaserver_people.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 23:05:43.000000 heaserver-people-1.1.0/src/heaserver_people.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-03-26 23:05:43.000000 heaserver-people-1.1.0/src/heaserver_people.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-03-26 23:05:43.000000 heaserver-people-1.1.0/src/heaserver_people.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-26 23:05:43.000000 heaserver-people-1.1.0/src/heaserver_people.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-26 23:05:43.062799 heaserver-people-1.1.0/tests/
-drwxrwxrwx   0        0        0        0 2024-03-26 23:05:43.062799 heaserver-people-1.1.0/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-26 23:05:43.100835 heaserver-people-1.1.0/tests/heaserver/persontest/
--rw-rw-rw-   0        0        0        0 2023-12-18 20:25:26.000000 heaserver-people-1.1.0/tests/heaserver/persontest/__init__.py
--rw-rw-rw-   0        0        0     3926 2023-12-18 20:25:26.000000 heaserver-people-1.1.0/tests/heaserver/persontest/permissionstestcase.py
--rw-rw-rw-   0        0        0     1343 2023-12-18 20:25:26.000000 heaserver-people-1.1.0/tests/heaserver/persontest/test_all.py
--rw-rw-rw-   0        0        0     7111 2024-03-07 16:44:50.000000 heaserver-people-1.1.0/tests/heaserver/persontest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.826035 heaserver_people-1.2.0/
+-rw-rw-rw-   0        0        0      261 2023-12-18 20:25:25.000000 heaserver_people-1.2.0/.editorconfig
+-rw-rw-rw-   0        0        0      353 2023-12-18 20:25:25.000000 heaserver_people-1.2.0/.gitignore
+-rw-rw-rw-   0        0        0    11625 2023-12-18 20:25:26.000000 heaserver_people-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      243 2023-12-18 20:25:26.000000 heaserver_people-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5270 2024-04-18 03:45:58.824036 heaserver_people-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3912 2024-04-18 03:44:27.000000 heaserver_people-1.2.0/README.md
+-rw-rw-rw-   0        0        0     1878 2023-12-18 20:25:26.000000 heaserver_people-1.2.0/RELEASING.md
+drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.760036 heaserver_people-1.2.0/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.781083 heaserver_people-1.2.0/integrationtests/.pytest_cache/
+-rw-rw-rw-   0        0        0       39 2023-02-23 16:41:17.000000 heaserver_people-1.2.0/integrationtests/.pytest_cache/.gitignore
+-rw-rw-rw-   0        0        0      194 2023-02-23 16:41:17.000000 heaserver_people-1.2.0/integrationtests/.pytest_cache/CACHEDIR.TAG
+-rw-rw-rw-   0        0        0      303 2023-02-23 16:41:17.000000 heaserver_people-1.2.0/integrationtests/.pytest_cache/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.759065 heaserver_people-1.2.0/integrationtests/.pytest_cache/v/
+drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.784036 heaserver_people-1.2.0/integrationtests/.pytest_cache/v/cache/
+-rw-rw-rw-   0        0        0        2 2023-02-23 16:42:55.000000 heaserver_people-1.2.0/integrationtests/.pytest_cache/v/cache/nodeids
+-rw-rw-rw-   0        0        0        2 2023-02-23 16:42:55.000000 heaserver_people-1.2.0/integrationtests/.pytest_cache/v/cache/stepwise
+drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.760036 heaserver_people-1.2.0/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.789035 heaserver_people-1.2.0/integrationtests/heaserver/personintegrationtest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 20:25:26.000000 heaserver_people-1.2.0/integrationtests/heaserver/personintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0     4674 2024-04-11 18:14:29.000000 heaserver_people-1.2.0/integrationtests/heaserver/personintegrationtest/permissionstestcase.py
+-rw-rw-rw-   0        0        0      547 2024-02-25 02:42:01.000000 heaserver_people-1.2.0/integrationtests/heaserver/personintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0     7893 2024-04-11 18:14:17.000000 heaserver_people-1.2.0/integrationtests/heaserver/personintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 20:25:26.000000 heaserver_people-1.2.0/pytest.ini
+-rw-rw-rw-   0        0        0      248 2023-12-18 20:25:26.000000 heaserver_people-1.2.0/requirements_dev.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 03:45:58.826035 heaserver_people-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1854 2024-04-18 03:45:10.000000 heaserver_people-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.762034 heaserver_people-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.761068 heaserver_people-1.2.0/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.798035 heaserver_people-1.2.0/src/heaserver/person/
+-rw-rw-rw-   0        0        0        0 2023-12-18 20:25:26.000000 heaserver_people-1.2.0/src/heaserver/person/__init__.py
+-rw-rw-rw-   0        0        0     4121 2024-02-25 02:42:01.000000 heaserver_people-1.2.0/src/heaserver/person/keycloakmockmongotestcase.py
+-rw-rw-rw-   0        0        0    27189 2024-04-17 03:50:10.000000 heaserver_people-1.2.0/src/heaserver/person/keycloakmongo.py
+-rw-rw-rw-   0        0        0    10027 2024-03-26 23:05:06.000000 heaserver_people-1.2.0/src/heaserver/person/keycloakmongotestcase.py
+-rw-rw-rw-   0        0        0    16645 2024-04-11 22:04:52.000000 heaserver_people-1.2.0/src/heaserver/person/service.py
+-rw-rw-rw-   0        0        0     1772 2023-12-18 20:25:26.000000 heaserver_people-1.2.0/src/heaserver/person/testcasedata.py
+drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.799080 heaserver_people-1.2.0/src/heaserver/person/wstl/
+-rw-rw-rw-   0        0        0    14175 2024-04-11 22:04:18.000000 heaserver_people-1.2.0/src/heaserver/person/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.823037 heaserver_people-1.2.0/src/heaserver_people.egg-info/
+-rw-rw-rw-   0        0        0     5270 2024-04-18 03:45:58.000000 heaserver_people-1.2.0/src/heaserver_people.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1289 2024-04-18 03:45:58.000000 heaserver_people-1.2.0/src/heaserver_people.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 03:45:58.000000 heaserver_people-1.2.0/src/heaserver_people.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-04-18 03:45:58.000000 heaserver_people-1.2.0/src/heaserver_people.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-18 03:45:58.000000 heaserver_people-1.2.0/src/heaserver_people.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-18 03:45:58.000000 heaserver_people-1.2.0/src/heaserver_people.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.763038 heaserver_people-1.2.0/tests/
+drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.763038 heaserver_people-1.2.0/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.821041 heaserver_people-1.2.0/tests/heaserver/persontest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 20:25:26.000000 heaserver_people-1.2.0/tests/heaserver/persontest/__init__.py
+-rw-rw-rw-   0        0        0     4010 2024-04-11 18:14:03.000000 heaserver_people-1.2.0/tests/heaserver/persontest/permissionstestcase.py
+-rw-rw-rw-   0        0        0     1343 2023-12-18 20:25:26.000000 heaserver_people-1.2.0/tests/heaserver/persontest/test_all.py
+-rw-rw-rw-   0        0        0     7195 2024-04-11 18:13:51.000000 heaserver_people-1.2.0/tests/heaserver/persontest/testcase.py
```

### Comparing `heaserver-people-1.1.0/LICENSE` & `heaserver_people-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-people-1.1.0/PKG-INFO` & `heaserver_people-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-people
-Version: 1.1.0
+Version: 1.2.0
 Summary: A microservice designed to provide CRUD operations for the Person HEA object type
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-people,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,26 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.1.0
+Requires-Dist: heaserver~=1.4.1
 
 # HEA Person Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Person Microservice is A microservice designed to provide CRUD operations for the Person HEA object type.
 
+## Version 1.2.0
+* Added /groups endpoint.
+* Corrected 500 error with /roles endpoint in some circumstances.
+
 ## Version 1.1.0
 * System users are now included in the people API calls.
 
 ## Version 1.0.7
 * Improved performance.
 
 ## Version 1.0.6
```

### Comparing `heaserver-people-1.1.0/README.md` & `heaserver_people-1.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # HEA Person Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Person Microservice is A microservice designed to provide CRUD operations for the Person HEA object type.
 
+## Version 1.2.0
+* Added /groups endpoint.
+* Corrected 500 error with /roles endpoint in some circumstances.
+
 ## Version 1.1.0
 * System users are now included in the people API calls.
 
 ## Version 1.0.7
 * Improved performance.
 
 ## Version 1.0.6
```

### Comparing `heaserver-people-1.1.0/RELEASING.md` & `heaserver_people-1.2.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-people-1.1.0/integrationtests/heaserver/personintegrationtest/permissionstestcase.py` & `heaserver_people-1.2.0/integrationtests/heaserver/personintegrationtest/permissionstestcase.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,16 @@
         'source_detail': None,
         'first_name': 'Reximus',
         'last_name': 'Max',
         'type': Person.get_type_name(),
         'phone_number': None,
         'preferred_name': None,
         'email': None,
-        'title': None
+        'title': None,
+        'type_display_name': 'Person'
     },
         {
             'id': '0123456789ab0123456789ab',
             'created': None,
             'derived_by': None,
             'derived_from': [],
             'description': None,
@@ -70,15 +71,16 @@
             'source_detail': None,
             'first_name': 'Luximus',
             'last_name': 'Max',
             'type': Person.get_type_name(),
             'phone_number': None,
             'preferred_name': None,
             'email': None,
-            'title': None
+            'title': None,
+            'type_display_name': 'Person'
         }]}
 
 HEASERVER_REGISTRY_IMAGE = 'registry.gitlab.com/huntsman-cancer-institute/risr/hea/heaserver-registry:1.0.0'
 
 
 PermissionsTestCase = \
     get_test_case_cls_default(coll=service.MONGODB_PERSON_COLLECTION,
```

### Comparing `heaserver-people-1.1.0/integrationtests/heaserver/personintegrationtest/test_all.py` & `heaserver_people-1.2.0/integrationtests/heaserver/personintegrationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-people-1.1.0/integrationtests/heaserver/personintegrationtest/testcase.py` & `heaserver_people-1.2.0/integrationtests/heaserver/personintegrationtest/testcase.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,16 @@
         'source_detail': None,
         'first_name': 'Reximus',
         'last_name': 'Max',
         'type': Person.get_type_name(),
         'phone_number': None,
         'preferred_name': None,
         'email': 'reximus.max@example.com',
-        'title': None
+        'title': None,
+        'type_display_name': 'Person'
     },
         {
             'id': '0123456789ab0123456789ab',
             'created': None,
             'derived_by': None,
             'derived_from': [],
             'description': None,
@@ -61,15 +62,16 @@
             'source_detail': None,
             'first_name': 'Luximus',
             'last_name': 'Max',
             'type': Person.get_type_name(),
             'phone_number': None,
             'preferred_name': None,
             'email': 'luximus.max@example.com',
-            'title': None
+            'title': None,
+            'type_display_name': 'Person'
         }] + [system_person.to_dict() for system_person in get_system_people()]}
 
 HEASERVER_REGISTRY_IMAGE = 'registry.gitlab.com/huntsman-cancer-institute/risr/hea/heaserver-registry:1.0.0'
 
 
 TestCase = get_test_case_cls_default(coll=service.MONGODB_PERSON_COLLECTION,
                                      href='http://localhost:8080/people',
```

### Comparing `heaserver-people-1.1.0/setup.py` & `heaserver_people-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-people',
-    version='1.1.0',
+    version='1.2.0',
     description="A microservice designed to provide CRUD operations for the Person HEA object type",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.person'],
     package_data={'heaserver.person': ['wstl/*.json']},
-    install_requires=['heaserver~=1.1.0'],
+    install_requires=['heaserver~=1.4.1'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
         'Environment :: Web Environment',
```

### Comparing `heaserver-people-1.1.0/src/heaserver/person/keycloakmockmongotestcase.py` & `heaserver_people-1.2.0/src/heaserver/person/keycloakmockmongotestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-people-1.1.0/src/heaserver/person/keycloakmongo.py` & `heaserver_people-1.2.0/src/heaserver/person/keycloakmongo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import configparser
 from typing import Any
 from heaserver.service.db.mongo import MongoManager, Mongo
 from heaserver.service import appproperty
 from heaserver.service.client import get_property
 from heaserver.service.oidcclaimhdrs import SUB
-from heaobject.person import Person, Role, get_system_person, get_system_people
+from heaobject.person import Person, Role, get_system_person, get_system_people, Group
 from heaobject.user import NONE_USER, ALL_USERS, is_system_user
 from heaobject.root import ShareImpl, Permission
 from aiohttp.web import Request
 from yarl import URL
 import logging
 from pathlib import Path
 from datetime import datetime, timedelta
@@ -26,15 +26,15 @@
 DEFAULT_ADMIN_CLIENT_ID = 'admin-cli'
 DEFAULT_REALM = 'hea'
 DEFAULT_HOST = 'https://localhost:8444'
 DEFAULT_SECRET_FILE = '.secret'
 DEFAULT_VERIFY_SSL = True
 
 CONFIG_SECTION = 'Keycloak'
-KEYCLOAK_TEST_IMAGE = 'jboss/keycloak:15.0.2'
+KEYCLOAK_TEST_IMAGE = 'quay.io/keycloak/keycloak:15.0.2'
 
 _ACCESS_TOKEN_LOCK = Lock()
 
 
 class KeycloakCompatibility(Enum):
     """Keycloak compatibility levels:
         FIFTEEN: APIs prior to version 19. We have only tested with 15.
@@ -326,14 +326,42 @@
         """
         async for role_json in self.__get_my_roles_json(request):
             if role_json['name'] == role_name:
                 return True
         else:
             return False
 
+    async def get_current_user_groups(self, request: Request) -> list[Group]:
+        """
+        Gets the current user's groups.
+
+        :param request: the HTTP request (required).
+        :returns: a list of Group objects.
+        :raises ClientResponseError: if something went wrong getting group information.
+        :raises ValueError: if something went wrong getting group information.
+
+        """
+        return await self.__get_my_groups(request)
+
+    async def has_group_current_user(self, request: Request, group_name: str) -> bool:
+        """
+        Returns whether the current user has the given group.
+
+        :param request: the HTTP request (required).
+        :param group_name: the group to check (required).
+        :returns: True or False.
+        :raises ClientResponseError: if something went wrong getting group information.
+        :raises ValueError: if something went wrong getting group information.
+        """
+        async for group_json in self.__get_my_groups_json(request):
+            if group_json['name'] == group_name:
+                return True
+        else:
+            return False
+
     async def __get_my_roles(self, request: Request) -> list[Role]:
         """
         Gets the current user's roles.
 
         :param request: the HTTP request (request).
         :returns: a list of Role objects. Make a deep copy of this list if you want to modify any of its values.
         :raises ClientResponseError: if something went wrong getting role information.
@@ -396,14 +424,67 @@
                 for role_dict in await response_.json():
                     roles[role_dict['name']] = role_dict
         await gather(one(), two())
         logger.debug('roles are %s', roles)
         for role_ in roles.values():
             yield role_
 
+    async def __get_my_groups(self, request: Request) -> list[Role]:
+        """
+        Gets the current user's groups.
+
+        :param request: the HTTP request (request).
+        :returns: a list of Group objects. Make a deep copy of this list if you want to modify any of its values.
+        :raises ClientResponseError: if something went wrong getting group information.
+        :raises ValueError: if something went wrong getting group information.
+
+        """
+        logger = logging.getLogger(__name__)
+        sub = request.headers.get(SUB, NONE_USER)
+        cached_val = self.__ttl_cache.get(('my_groups', sub))
+        if cached_val is not None:
+            return cached_val
+        else:
+            values = [self.__new_group(sub, group_json) async for group_json in self.__get_my_groups_json(request)]
+            self.__ttl_cache[('my_groups', sub)] = values
+            return values
+
+    def __new_group(self, sub: str, group_dict: dict[str, Any]) -> Group:
+        """
+        Returns a Group object from Keycloak group json.
+
+        :param sub: the user id (required).
+        :param group_dict: the group json (required).
+        :return: a newly Group object.
+        """
+        group = Group()
+        group.group = group_dict['path']
+        group.owner = NONE_USER
+        share = ShareImpl()
+        share.user = sub
+        share.permissions = [Permission.VIEWER]
+        group.shares = [share]
+        return group
+
+    async def __get_my_groups_json(self, request: Request) -> AsyncGenerator[dict[str, Any], None]:
+        logger = logging.getLogger(__name__)
+        sub = request.headers.get(SUB, NONE_USER)
+        access_token = await self.get_keycloak_access_token(request)
+
+        session = request.app[appproperty.HEA_CLIENT_SESSION]
+
+        group_base_url = self._base_url / 'admin' / 'realms' / self.realm
+        session_get = partial(session.get,
+                            headers={'Authorization': f'Bearer {access_token}'},
+                            verify_ssl=self.verify_ssl)
+        async with session_get(group_base_url / 'users' / sub / 'groups') as response_:
+            for group_dict in await response_.json():
+                logger.debug('Returning group %s', group_dict)
+                yield group_dict
+
     @staticmethod
     def __keycloak_user_to_person(user: dict[str, Any]) -> Person:
         """
         Converts a user JSON object from Keycloak to a HEA Person object.
 
         :param user: a Keycloak user object as a JSON dict.
         :return: a Person object.
```

### Comparing `heaserver-people-1.1.0/src/heaserver/person/keycloakmongotestcase.py` & `heaserver_people-1.2.0/src/heaserver/person/keycloakmongotestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-people-1.1.0/src/heaserver/person/service.py` & `heaserver_people-1.2.0/src/heaserver/person/service.py`

 * *Files 20% similar despite different names*

```diff
@@ -63,22 +63,26 @@
     responses:
       '200':
         $ref: '#/components/responses/200'
       '404':
         $ref: '#/components/responses/404'
     """
     logger = logging.getLogger(__name__)
+    sub = request.headers.get(SUB, NONE_USER)
     try:
         person = await request.app[appproperty.HEA_DB].get_user(request, request.headers.get(SUB, NONE_USER))
     except ClientResponseError as e:
         if e.status == 404:
             person = None
         else:
             return response.status_generic(e.status, body=e.message)
-    return await response.get(request, person.to_dict() if person else None)
+    if person is not None:
+        return await response.get(request, person.to_dict(), permissions=person.get_permissions(sub))
+    else:
+        return await response.get(request, None)
 
 
 @routes.get('/people/{id}')
 @action(name='heaserver-people-person-get-properties', rel='hea-properties')
 @action(name='heaserver-people-person-get-self', rel='self', path='people/{id}')
 @action(name='heaserver-people-person-get-settings', rel='hea-system-menu-item hea-user-menu-item application/x.settingsobject application/x.collection', path='collections/heaobject.settings.SettingsObject')
 #@action(name='heaserver-people-person-get-organization-collection', rel='hea-system-menu-item application/x.collection', path='collections/heaobject.organization.Organization')
@@ -99,22 +103,26 @@
     responses:
       '200':
         $ref: '#/components/responses/200'
       '404':
         $ref: '#/components/responses/404'
     """
     logger = logging.getLogger(__name__)
+    sub = request.headers.get(SUB, NONE_USER)
     try:
         person = await request.app[appproperty.HEA_DB].get_user(request, request.match_info['id'])
     except ClientResponseError as e:
         if e.status == 404:
             person = None
         else:
             return response.status_generic(e.status, body=e.message)
-    return await response.get(request, person.to_dict() if person else None)
+    if person is not None:
+        return await response.get(request, person.to_dict(), permissions=person.get_permissions(sub))
+    else:
+        return await response.get(request, None)
 
 
 @routes.get('/people/byname/{name}')
 @action(name='heaserver-people-person-get-self', rel='self', path='people/{id}')
 async def get_person_by_name(request: web.Request) -> web.Response:
     """
     Gets the person with the specified id.
@@ -129,17 +137,21 @@
     responses:
       '200':
         $ref: '#/components/responses/200'
       '404':
         $ref: '#/components/responses/404'
     """
     logger = logging.getLogger(__name__)
+    sub = request.headers.get(SUB, NONE_USER)
     try:
         persons = await request.app[appproperty.HEA_DB].get_users(request, params={'name': request.match_info['name']})
-        return await response.get(request, persons[0].to_dict() if persons else None)
+        if persons:
+            return await response.get(request, persons[0].to_dict(), permissions=persons[0].get_permissions(sub))
+        else:
+            return await response.get(request, None)
     except ClientResponseError as e:
         return response.status_generic(e.status, body=e.message)
 
 
 @routes.get('/people')
 @routes.get('/people/')
 @action(name='heaserver-people-person-get-properties', rel='hea-properties')
@@ -158,64 +170,77 @@
     summary: All persons.
     tags:
         - heaserver-people
     responses:
       '200':
         $ref: '#/components/responses/200'
     """
+    sub = request.headers.get(SUB, NONE_USER)
     try:
         persons = await request.app[appproperty.HEA_DB].get_users(request)
-        return await response.get_all(request, [person.to_dict() for person in persons])
+        return await response.get_all(request, [person.to_dict() for person in persons],
+                                      permissions=[person.get_permissions(sub) for person in persons])
     except ClientResponseError as e:
         return response.status_generic(e.status, body=e.message)
 
 
 @routes.get('/roles')
 @routes.get('/roles/')
+@action(name='heaserver-people-role-get-properties', rel='hea-properties')
+@action(name='heaserver-people-role-get-self', rel='self', path='roles/{id}')
 async def get_all_roles(request: web.Request) -> web.Response:
     """
     Gets all roles for the current user.
     :param request: the HTTP request.
     :return: all roles.
     ---
     summary: All roles.
     tags:
         - heaserver-people
     responses:
       '200':
         $ref: '#/components/responses/200'
     """
+    sub = request.headers.get(SUB, NONE_USER)
     try:
-        roles = await request.app[appproperty.HEA_DB].get_oidc_userinfo(request)
-        return await response.get_all(request, [role.to_dict() for role in roles])
+        roles = await request.app[appproperty.HEA_DB].get_current_user_roles(request)
+        return await response.get_all(request, [role.to_dict() for role in roles],
+                                      permissions=[role.get_permissions(sub) for role in roles])
     except ClientResponseError as e:
         if e.status == 404:
             return await response.get_all(request, [])
         else:
             return response.status_generic(e.status, body=e.message)
 
 @routes.get('/roles/{id}')
+@action(name='heaserver-people-role-get-properties', rel='hea-properties')
+@action(name='heaserver-people-role-get-self', rel='self', path='roles/{id}')
 async def get_role(request: web.Request) -> web.Response:
     """
     Gets the requested role for the current user.
 
     :param request: the HTTP request.
     :return: all roles.
     ---
     summary: All roles.
     tags:
         - heaserver-people
     responses:
       '200':
         $ref: '#/components/responses/200'
     """
+    sub = request.headers.get(SUB, NONE_USER)
     id_ = request.match_info['id']
     try:
-        roles = await request.app[appproperty.HEA_DB].get_oidc_userinfo(request)
-        return await response.get(request, next((role.to_dict() for role in roles if role.id == id_), None))
+        roles = await request.app[appproperty.HEA_DB].get_current_user_roles(request)
+        role = next((role for role in roles if role.id == id_), None)
+        if role is not None:
+            return await response.get(request, role.to_dict(), permissions=role.get_permissions(sub))
+        else:
+            return await response.get(request, None)
     except ClientResponseError as e:
         if e.status == 404:
             return response.status_not_found()
         else:
             return response.status_generic(e.status, body=e.message)
 
 
@@ -257,13 +282,115 @@
             return response.status_not_found()
         else:
             return response.status_generic(e.status, body=e.message)
     except B64DecodeError as e:
         return response.status_not_found()
 
 
+@routes.get('/groups')
+@routes.get('/groups/')
+@action(name='heaserver-people-group-get-properties', rel='hea-properties')
+@action(name='heaserver-people-group-get-self', rel='self', path='groups/{id}')
+async def get_all_groups(request: web.Request) -> web.Response:
+    """
+    Gets all groups for the current user.
+    :param request: the HTTP request.
+    :return: all groups.
+    ---
+    summary: All groups.
+    tags:
+        - heaserver-people
+    responses:
+      '200':
+        $ref: '#/components/responses/200'
+    """
+    sub = request.headers.get(SUB, NONE_USER)
+    try:
+        groups = await request.app[appproperty.HEA_DB].get_current_user_groups(request)
+        return await response.get_all(request, [group.to_dict() for group in groups],
+                                      permissions=[group.get_permissions(sub) for group in groups])
+    except ClientResponseError as e:
+        if e.status == 404:
+            return await response.get_all(request, [])
+        else:
+            return response.status_generic(e.status, body=e.message)
+
+@routes.get('/groups/{id}')
+@action(name='heaserver-people-group-get-properties', rel='hea-properties')
+@action(name='heaserver-people-group-get-self', rel='self', path='groups/{id}')
+async def get_group(request: web.Request) -> web.Response:
+    """
+    Gets the requested group for the current user.
+
+    :param request: the HTTP request.
+    :return: all groups.
+    ---
+    summary: All groups.
+    tags:
+        - heaserver-people
+    responses:
+      '200':
+        $ref: '#/components/responses/200'
+    """
+    sub = request.headers.get(SUB, NONE_USER)
+    id_ = request.match_info['id']
+    try:
+        groups = await request.app[appproperty.HEA_DB].get_current_user_groups(request)
+        group = next((group for group in groups if group.id == id_), None)
+        if group is not None:
+            return await response.get(request, group.to_dict(), permissions=group.get_permissions(sub))
+        else:
+            return await response.get(request, None)
+    except ClientResponseError as e:
+        if e.status == 404:
+            return response.status_not_found()
+        else:
+            return response.status_generic(e.status, body=e.message)
+
+
+@routes.get('/groups/byname/{name}')
+async def get_group_by_name(request: web.Request) -> web.Response:
+    """
+    Gets the requested group for the current user. Requires an Authorization header with a valid Bearer token, in
+    addition to the usual OIDC_CLAIM_sub header.
+
+    :param request: the HTTP request.
+    :return: all groups.
+    ---
+    summary: All groups.
+    tags:
+        - heaserver-people
+    responses:
+      '200':
+        $ref: '#/components/responses/200'
+    """
+    logger = logging.getLogger(__name__)
+    name_encoded = request.match_info['name']
+    try:
+        name = urlsafe_b64decode(name_encoded).decode('utf-8')
+        if logger.getEffectiveLevel() == logging.DEBUG:
+            logger.debug('match_info %s', request.match_info)
+            logger.debug('headers %s', request.headers)
+            logger.debug('checking role %s', name)
+        has_group = await request.app[appproperty.HEA_DB].has_group_current_user(request, name)
+        if request.method == 'GET':
+            return has_group
+        else:
+            if has_group:
+                return response.status_ok()
+            else:
+                return response.status_not_found()
+    except ClientResponseError as e:
+        logger.exception('Got client response error')
+        if e.status == 404:
+            return response.status_not_found()
+        else:
+            return response.status_generic(e.status, body=e.message)
+    except B64DecodeError as e:
+        return response.status_not_found()
+
 def main() -> None:
     config = init_cmd_line(description='Read-only wrapper around Keycloak for accessing user information.',
                            default_port=8080)
     start(package_name='heaserver-people', db=KeycloakMongoManager, config=config, wstl_builder_factory=builder_factory(__package__))
```

### Comparing `heaserver-people-1.1.0/src/heaserver/person/testcasedata.py` & `heaserver_people-1.2.0/src/heaserver/person/testcasedata.py`

 * *Files identical despite different names*

### Comparing `heaserver-people-1.1.0/src/heaserver/person/wstl/all.json` & `heaserver_people-1.2.0/src/heaserver/person/wstl/all.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'wstl'": "{'actions': {insert: [(3, OrderedDict([('name', 'heaserver-people-role-get-self'), "*

 * *           "('description', 'View this role'), ('type', 'safe'), ('action', 'read'), ('target', "*

 * *           "'item read cj'), ('prompt', 'View')])), (4, OrderedDict([('name', "*

 * *           "'heaserver-people-group-get-self'), ('description', 'View this group'), ('type', "*

 * *           "'safe'), ('action', 'read'), ('target', 'item read cj'), ('prompt', 'View')])), (11, "*

 * *           "OrderedDict([('name', 'heaserve […]*

```diff
@@ -19,14 +19,30 @@
                 "name": "heaserver-people-person-get-self",
                 "prompt": "View",
                 "target": "item read cj",
                 "type": "safe"
             },
             {
                 "action": "read",
+                "description": "View this role",
+                "name": "heaserver-people-role-get-self",
+                "prompt": "View",
+                "target": "item read cj",
+                "type": "safe"
+            },
+            {
+                "action": "read",
+                "description": "View this group",
+                "name": "heaserver-people-group-get-self",
+                "prompt": "View",
+                "target": "item read cj",
+                "type": "safe"
+            },
+            {
+                "action": "read",
                 "description": "View and edit this person's settings",
                 "name": "heaserver-people-person-get-settings",
                 "prompt": "Settings",
                 "target": "item read cj",
                 "type": "safe"
             },
             {
@@ -224,14 +240,74 @@
                 "name": "heaserver-people-person-get-properties",
                 "prompt": "Properties",
                 "target": "item cj-template",
                 "type": "unsafe"
             },
             {
                 "action": "update",
+                "description": "View this role's properties",
+                "inputs": [
+                    {
+                        "hea": {
+                            "display": false
+                        },
+                        "name": "id",
+                        "prompt": "Id",
+                        "readOnly": true
+                    },
+                    {
+                        "name": "display_name",
+                        "prompt": "Name",
+                        "readOnly": true,
+                        "required": true
+                    },
+                    {
+                        "name": "type_display_name",
+                        "prompt": "Type",
+                        "readOnly": true,
+                        "required": true
+                    }
+                ],
+                "name": "heaserver-people-role-get-properties",
+                "prompt": "Properties",
+                "target": "item cj-template",
+                "type": "unsafe"
+            },
+            {
+                "action": "update",
+                "description": "View this group's properties",
+                "inputs": [
+                    {
+                        "hea": {
+                            "display": false
+                        },
+                        "name": "id",
+                        "prompt": "Id",
+                        "readOnly": true
+                    },
+                    {
+                        "name": "display_name",
+                        "prompt": "Name",
+                        "readOnly": true,
+                        "required": true
+                    },
+                    {
+                        "name": "type_display_name",
+                        "prompt": "Type",
+                        "readOnly": true,
+                        "required": true
+                    }
+                ],
+                "name": "heaserver-people-group-get-properties",
+                "prompt": "Properties",
+                "target": "item cj-template",
+                "type": "unsafe"
+            },
+            {
+                "action": "update",
                 "description": "Duplicate this person",
                 "inputs": [
                     {
                         "name": "display_name",
                         "prompt": "Name",
                         "required": true
                     },
```

### Comparing `heaserver-people-1.1.0/src/heaserver_people.egg-info/PKG-INFO` & `heaserver_people-1.2.0/src/heaserver_people.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-people
-Version: 1.1.0
+Version: 1.2.0
 Summary: A microservice designed to provide CRUD operations for the Person HEA object type
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-people,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,26 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.1.0
+Requires-Dist: heaserver~=1.4.1
 
 # HEA Person Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Person Microservice is A microservice designed to provide CRUD operations for the Person HEA object type.
 
+## Version 1.2.0
+* Added /groups endpoint.
+* Corrected 500 error with /roles endpoint in some circumstances.
+
 ## Version 1.1.0
 * System users are now included in the people API calls.
 
 ## Version 1.0.7
 * Improved performance.
 
 ## Version 1.0.6
```

### Comparing `heaserver-people-1.1.0/src/heaserver_people.egg-info/SOURCES.txt` & `heaserver_people-1.2.0/src/heaserver_people.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-people-1.1.0/tests/heaserver/persontest/permissionstestcase.py` & `heaserver_people-1.2.0/tests/heaserver/persontest/permissionstestcase.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,16 @@
         'name': 'reximus',
         'owner': NONE_USER,
         'shares': [],
         'source': None,
         'source_detail': None,
         'first_name': 'Reximus',
         'last_name': 'Texamus',
-        'type': 'heaobject.person.Person'
+        'type': 'heaobject.person.Person',
+        'type_display_name': 'Person'
     },
         {
             'id': '0123456789ab0123456789ab',
             'created': None,
             'derived_by': None,
             'derived_from': [],
             'description': None,
@@ -45,15 +46,16 @@
                 'user': TEST_USER,
                 'permissions': [Permission.VIEWER.name]
             }],
             'source': None,
             'source_detail': None,
             'first_name': 'Luximus',
             'last_name': 'Tuxamus',
-            'type': 'heaobject.person.Person'
+            'type': 'heaobject.person.Person',
+            'type_display_name': 'Person'
         }]}
 
 PermissionsTestCase = \
     get_test_case_cls_default(coll=service.MONGODB_PERSON_COLLECTION,
                               wstl_package=service.__package__,
                               db_manager_cls=KeycloakMockMongoManager,
                               href='http://localhost:8080/people',
```

### Comparing `heaserver-people-1.1.0/tests/heaserver/persontest/test_all.py` & `heaserver_people-1.2.0/tests/heaserver/persontest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-people-1.1.0/tests/heaserver/persontest/testcase.py` & `heaserver_people-1.2.0/tests/heaserver/persontest/testcase.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,16 @@
         'source_detail': None,
         'first_name': 'Reximus',
         'last_name': 'Max',
         'type': 'heaobject.person.Person',
         'title': None,
         'phone_number': None,
         'preferred_name': None,
-        'email': None
+        'email': None,
+        'type_display_name': 'Person'
     },
         {
             'id': 'system|test',
             'created': '2022-01-01T00:00:00',
             'derived_by': None,
             'derived_from': [],
             'description': None,
@@ -57,15 +58,16 @@
             'source_detail': None,
             'first_name': 'Luximus',
             'last_name': 'Max',
             'type': 'heaobject.person.Person',
             'title': None,
             'phone_number': None,
             'preferred_name': None,
-            'email': None
+            'email': None,
+            'type_display_name': 'Person'
         }]}
 
 
 TestCase = get_test_case_cls_default(coll=service.MONGODB_PERSON_COLLECTION,
                                      wstl_package=service.__package__,
                                      db_manager_cls=KeycloakMockMongoManager,
                                      href='http://localhost:8080/people',
```

