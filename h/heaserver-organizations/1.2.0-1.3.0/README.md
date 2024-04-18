# Comparing `tmp/heaserver-organizations-1.2.0.tar.gz` & `tmp/heaserver_organizations-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-organizations-1.2.0.tar", last modified: Fri Apr  5 18:48:23 2024, max compression
+gzip compressed data, was "heaserver_organizations-1.3.0.tar", last modified: Thu Apr 18 04:02:10 2024, max compression
```

## Comparing `heaserver-organizations-1.2.0.tar` & `heaserver_organizations-1.3.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 18:48:23.120495 heaserver-organizations-1.2.0/
--rw-rw-rw-   0        0        0      261 2022-03-14 19:48:11.000000 heaserver-organizations-1.2.0/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 21:21:27.000000 heaserver-organizations-1.2.0/.gitignore
--rw-rw-rw-   0        0        0     1663 2023-12-18 21:21:27.000000 heaserver-organizations-1.2.0/Dockerfile
--rw-rw-rw-   0        0        0    11625 2022-03-14 19:48:11.000000 heaserver-organizations-1.2.0/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 21:21:27.000000 heaserver-organizations-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5120 2024-04-05 18:48:23.119495 heaserver-organizations-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3730 2024-04-05 18:45:22.000000 heaserver-organizations-1.2.0/README.md
--rw-rw-rw-   0        0        0     1749 2023-12-18 21:21:27.000000 heaserver-organizations-1.2.0/RELEASING.md
--rw-rw-rw-   0        0        0      404 2024-03-20 04:10:28.000000 heaserver-organizations-1.2.0/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-04-05 18:48:23.016844 heaserver-organizations-1.2.0/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-04-05 18:48:23.016844 heaserver-organizations-1.2.0/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-05 18:48:23.086496 heaserver-organizations-1.2.0/integrationtests/heaserver/organizationintegrationtest/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver-organizations-1.2.0/integrationtests/heaserver/organizationintegrationtest/__init__.py
--rw-rw-rw-   0        0        0    10658 2024-04-05 02:18:47.000000 heaserver-organizations-1.2.0/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py
--rw-rw-rw-   0        0        0      402 2023-12-18 21:21:27.000000 heaserver-organizations-1.2.0/integrationtests/heaserver/organizationintegrationtest/test_all.py
--rw-rw-rw-   0        0        0    14702 2024-04-05 02:18:40.000000 heaserver-organizations-1.2.0/integrationtests/heaserver/organizationintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      111 2023-12-18 21:21:27.000000 heaserver-organizations-1.2.0/pytest.ini
--rw-rw-rw-   0        0        0      362 2023-12-18 21:21:27.000000 heaserver-organizations-1.2.0/requirements_dev.txt
--rw-rw-rw-   0        0        0     6574 2023-12-18 21:21:27.000000 heaserver-organizations-1.2.0/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-04-05 18:48:23.121496 heaserver-organizations-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1911 2024-04-05 18:47:37.000000 heaserver-organizations-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:48:23.018843 heaserver-organizations-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 18:48:23.017844 heaserver-organizations-1.2.0/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-05 18:48:23.088497 heaserver-organizations-1.2.0/src/heaserver/organization/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver-organizations-1.2.0/src/heaserver/organization/__init__.py
--rw-rw-rw-   0        0        0    28882 2024-04-04 23:11:21.000000 heaserver-organizations-1.2.0/src/heaserver/organization/service.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:48:23.089497 heaserver-organizations-1.2.0/src/heaserver/organization/wstl/
--rw-rw-rw-   0        0        0    22819 2024-04-04 16:00:27.000000 heaserver-organizations-1.2.0/src/heaserver/organization/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-04-05 18:48:23.118495 heaserver-organizations-1.2.0/src/heaserver_organizations.egg-info/
--rw-rw-rw-   0        0        0     5120 2024-04-05 18:48:22.000000 heaserver-organizations-1.2.0/src/heaserver_organizations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      997 2024-04-05 18:48:23.000000 heaserver-organizations-1.2.0/src/heaserver_organizations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 18:48:22.000000 heaserver-organizations-1.2.0/src/heaserver_organizations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-04-05 18:48:22.000000 heaserver-organizations-1.2.0/src/heaserver_organizations.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-05 18:48:22.000000 heaserver-organizations-1.2.0/src/heaserver_organizations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-05 18:48:22.000000 heaserver-organizations-1.2.0/src/heaserver_organizations.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 18:48:23.019843 heaserver-organizations-1.2.0/tests/
-drwxrwxrwx   0        0        0        0 2024-04-05 18:48:23.019843 heaserver-organizations-1.2.0/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-05 18:48:23.117495 heaserver-organizations-1.2.0/tests/heaserver/organizationtest/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver-organizations-1.2.0/tests/heaserver/organizationtest/__init__.py
--rw-rw-rw-   0        0        0     1783 2023-12-18 21:21:27.000000 heaserver-organizations-1.2.0/tests/heaserver/organizationtest/test_all.py
--rw-rw-rw-   0        0        0     6794 2024-04-05 02:18:18.000000 heaserver-organizations-1.2.0/tests/heaserver/organizationtest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-04-18 04:02:10.685517 heaserver_organizations-1.3.0/
+-rw-rw-rw-   0        0        0      261 2022-03-14 19:48:11.000000 heaserver_organizations-1.3.0/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 21:21:27.000000 heaserver_organizations-1.3.0/.gitignore
+-rw-rw-rw-   0        0        0     1663 2023-12-18 21:21:27.000000 heaserver_organizations-1.3.0/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2022-03-14 19:48:11.000000 heaserver_organizations-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 21:21:27.000000 heaserver_organizations-1.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5183 2024-04-18 04:02:10.683521 heaserver_organizations-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3793 2024-04-11 17:15:42.000000 heaserver_organizations-1.3.0/README.md
+-rw-rw-rw-   0        0        0     1749 2023-12-18 21:21:27.000000 heaserver_organizations-1.3.0/RELEASING.md
+-rw-rw-rw-   0        0        0      404 2024-03-20 04:10:28.000000 heaserver_organizations-1.3.0/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-04-18 04:02:10.520206 heaserver_organizations-1.3.0/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-04-18 04:02:10.521205 heaserver_organizations-1.3.0/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-18 04:02:10.625476 heaserver_organizations-1.3.0/integrationtests/heaserver/organizationintegrationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.3.0/integrationtests/heaserver/organizationintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0    10758 2024-04-08 23:26:43.000000 heaserver_organizations-1.3.0/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py
+-rw-rw-rw-   0        0        0      402 2023-12-18 21:21:27.000000 heaserver_organizations-1.3.0/integrationtests/heaserver/organizationintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0    14802 2024-04-08 23:26:37.000000 heaserver_organizations-1.3.0/integrationtests/heaserver/organizationintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 21:21:27.000000 heaserver_organizations-1.3.0/pytest.ini
+-rw-rw-rw-   0        0        0      362 2023-12-18 21:21:27.000000 heaserver_organizations-1.3.0/requirements_dev.txt
+-rw-rw-rw-   0        0        0     6574 2023-12-18 21:21:27.000000 heaserver_organizations-1.3.0/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-04-18 04:02:10.685517 heaserver_organizations-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1911 2024-04-18 04:01:32.000000 heaserver_organizations-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 04:02:10.524212 heaserver_organizations-1.3.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-18 04:02:10.522207 heaserver_organizations-1.3.0/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-18 04:02:10.628473 heaserver_organizations-1.3.0/src/heaserver/organization/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.3.0/src/heaserver/organization/__init__.py
+-rw-rw-rw-   0        0        0    28882 2024-04-05 18:49:42.000000 heaserver_organizations-1.3.0/src/heaserver/organization/service.py
+drwxrwxrwx   0        0        0        0 2024-04-18 04:02:10.630477 heaserver_organizations-1.3.0/src/heaserver/organization/wstl/
+-rw-rw-rw-   0        0        0    23163 2024-04-11 17:16:54.000000 heaserver_organizations-1.3.0/src/heaserver/organization/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-04-18 04:02:10.682518 heaserver_organizations-1.3.0/src/heaserver_organizations.egg-info/
+-rw-rw-rw-   0        0        0     5183 2024-04-18 04:02:10.000000 heaserver_organizations-1.3.0/src/heaserver_organizations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      997 2024-04-18 04:02:10.000000 heaserver_organizations-1.3.0/src/heaserver_organizations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 04:02:10.000000 heaserver_organizations-1.3.0/src/heaserver_organizations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-04-18 04:02:10.000000 heaserver_organizations-1.3.0/src/heaserver_organizations.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-18 04:02:10.000000 heaserver_organizations-1.3.0/src/heaserver_organizations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-18 04:02:10.000000 heaserver_organizations-1.3.0/src/heaserver_organizations.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 04:02:10.525209 heaserver_organizations-1.3.0/tests/
+drwxrwxrwx   0        0        0        0 2024-04-18 04:02:10.526208 heaserver_organizations-1.3.0/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-18 04:02:10.677517 heaserver_organizations-1.3.0/tests/heaserver/organizationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.3.0/tests/heaserver/organizationtest/__init__.py
+-rw-rw-rw-   0        0        0     1783 2023-12-18 21:21:27.000000 heaserver_organizations-1.3.0/tests/heaserver/organizationtest/test_all.py
+-rw-rw-rw-   0        0        0     6894 2024-04-08 23:26:24.000000 heaserver_organizations-1.3.0/tests/heaserver/organizationtest/testcase.py
```

### Comparing `heaserver-organizations-1.2.0/Dockerfile` & `heaserver_organizations-1.3.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver-organizations-1.2.0/LICENSE` & `heaserver_organizations-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-organizations-1.2.0/PKG-INFO` & `heaserver_organizations-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-organizations
-Version: 1.2.0
+Version: 1.3.0
 Summary: a service for managing organization information for research laboratories and other research groups
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-organizations,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,25 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.2.0
+Requires-Dist: heaserver~=1.4.1
 
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.3.0
+* Return the type_display_name attribute.
+
 ## Version 1.2.0
 * Improved performance accessing an organization's AWS accounts.
 * heaobject.organization.Organization objects now have an accounts attribute that mirrors the contents of the existing
 aws_account_ids attribute and will support other heaobject.account.Account subclasses in the future.
 
 ## Version 1.1.0
 * Pass desktop object permissions back to clients.
```

### Comparing `heaserver-organizations-1.2.0/README.md` & `heaserver_organizations-1.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.3.0
+* Return the type_display_name attribute.
+
 ## Version 1.2.0
 * Improved performance accessing an organization's AWS accounts.
 * heaobject.organization.Organization objects now have an accounts attribute that mirrors the contents of the existing
 aws_account_ids attribute and will support other heaobject.account.Account subclasses in the future.
 
 ## Version 1.1.0
 * Pass desktop object permissions back to clients.
```

### Comparing `heaserver-organizations-1.2.0/RELEASING.md` & `heaserver_organizations-1.3.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-organizations-1.2.0/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py` & `heaserver_organizations-1.3.0/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,16 @@
             "aws_account_ids": [],
             "admin_ids": [],
             "principal_investigator_id": "23423DAFSDF12adfasdf3",
             "manager_ids": [],
             "member_ids": [],
             'type': 'heaobject.organization.Organization',
             'version': None,
-            'accounts': []
+            'accounts': [],
+            'type_display_name': 'Organization'
         },
         {
             "id": "0123456789ab0123456789ab",
             "source": None,
             "source_detail": None,
             "name": "Reximus",
             "display_name": "Reximus",
@@ -55,15 +56,16 @@
             "aws_account_ids": [],
             "admin_ids": [],
             "principal_investigator_id": "11234867890b0123a56789ab",
             "manager_ids": [],
             "member_ids": ['0123456789ab0123456789ab'],
             'type': 'heaobject.organization.Organization',
             'version': None,
-            'accounts': []
+            'accounts': [],
+            'type_display_name': 'Organization'
         }
     ],
     'filesystems': [{
         'id': '666f6f2d6261722d71757578',
         'created': None,
         'derived_by': None,
         'derived_from': [],
```

### Comparing `heaserver-organizations-1.2.0/integrationtests/heaserver/organizationintegrationtest/testcase.py` & `heaserver_organizations-1.3.0/integrationtests/heaserver/organizationintegrationtest/testcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,16 @@
             "aws_account_ids": [],
             "admin_ids": [],
             "principal_investigator_id": "23423DAFSDF12adfasdf3",
             "manager_ids": ['666f6f2d6261722d71757578'],
             "member_ids": ['0123456789ab0123456789ab'],
             'type': 'heaobject.organization.Organization',
             'mime_type': 'application/x.organization',
-            'accounts': []
+            'accounts': [],
+            'type_display_name': 'Organization'
         },
         {
             "id": "0123456789ab0123456789ab",
             "source": None,
             "source_detail": None,
             "name": "Reximus",
             "display_name": "Reximus",
@@ -59,15 +60,16 @@
             "aws_account_ids": [],
             "admin_ids": [],
             "principal_investigator_id": "11234867890b0123a56789ab",
             "manager_ids": ["11234867890b0123a56789ab"],
             "member_ids": [],
             'type': 'heaobject.organization.Organization',
             'mime_type': 'application/x.organization',
-            'accounts': []
+            'accounts': [],
+            'type_display_name': 'Organization'
         }
     ],
     CollectionKey(name='filesystems', db_manager_cls=MockDockerMongoManager): [{
         'id': '666f6f2d6261722d71757578',
         'created': None,
         'derived_by': None,
         'derived_from': [],
```

### Comparing `heaserver-organizations-1.2.0/run-swaggerui.py` & `heaserver_organizations-1.3.0/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver-organizations-1.2.0/setup.py` & `heaserver_organizations-1.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-organizations',
-    version='1.2.0',
+    version='1.3.0',
     description="a service for managing organization information for research laboratories and other research groups",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.organization'],
     package_data={'heaserver.organization': ['wstl/*.json']},
-    install_requires=['heaserver~=1.2.0'],
+    install_requires=['heaserver~=1.4.1'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
         'Environment :: Web Environment',
```

### Comparing `heaserver-organizations-1.2.0/src/heaserver/organization/service.py` & `heaserver_organizations-1.3.0/src/heaserver/organization/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-organizations-1.2.0/src/heaserver/organization/wstl/all.json` & `heaserver_organizations-1.3.0/src/heaserver/organization/wstl/all.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999953007518797%*

 * *Differences: {"'wstl'": "{'actions': {7: {'inputs': {4: {'name': 'type_display_name', 'value': 'Organization'}, "*

 * *           "insert: [(3, OrderedDict([('name', 'type'), ('readOnly', True), ('required', True), "*

 * *           "('value', 'heaobject.organization.Organization'), ('hea', OrderedDict([('display', "*

 * *           'False)]))]))]}}}}'}*

```diff
@@ -77,21 +77,30 @@
                             "display": false
                         },
                         "name": "name",
                         "prompt": "Name",
                         "required": false
                     },
                     {
+                        "hea": {
+                            "display": false
+                        },
                         "name": "type",
-                        "prompt": "Type",
                         "readOnly": true,
                         "required": true,
                         "value": "heaobject.organization.Organization"
                     },
                     {
+                        "name": "type_display_name",
+                        "prompt": "Type",
+                        "readOnly": true,
+                        "required": true,
+                        "value": "Organization"
+                    },
+                    {
                         "name": "description",
                         "prompt": "Description",
                         "type": "textarea"
                     },
                     {
                         "hea": {
                             "display": false
```

### Comparing `heaserver-organizations-1.2.0/src/heaserver_organizations.egg-info/PKG-INFO` & `heaserver_organizations-1.3.0/src/heaserver_organizations.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-organizations
-Version: 1.2.0
+Version: 1.3.0
 Summary: a service for managing organization information for research laboratories and other research groups
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-organizations,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,25 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.2.0
+Requires-Dist: heaserver~=1.4.1
 
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.3.0
+* Return the type_display_name attribute.
+
 ## Version 1.2.0
 * Improved performance accessing an organization's AWS accounts.
 * heaobject.organization.Organization objects now have an accounts attribute that mirrors the contents of the existing
 aws_account_ids attribute and will support other heaobject.account.Account subclasses in the future.
 
 ## Version 1.1.0
 * Pass desktop object permissions back to clients.
```

### Comparing `heaserver-organizations-1.2.0/src/heaserver_organizations.egg-info/SOURCES.txt` & `heaserver_organizations-1.3.0/src/heaserver_organizations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-organizations-1.2.0/tests/heaserver/organizationtest/test_all.py` & `heaserver_organizations-1.3.0/tests/heaserver/organizationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-organizations-1.2.0/tests/heaserver/organizationtest/testcase.py` & `heaserver_organizations-1.3.0/tests/heaserver/organizationtest/testcase.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
             "aws_account_ids": [],
             "principal_investigator_id": "23423DAFSDF12adfasdf3",
             "manager_ids": [],
             "member_ids": [],
             "admin_ids": [],
             'type': 'heaobject.organization.Organization',
             'mime_type': 'application/x.organization',
-            'accounts': []
+            'accounts': [],
+            'type_display_name': 'Organization'
         },
         {
             "id": "0123456789ab0123456789ab",
             "source": None,
             'source_detail': None,
             "name": "Reximus",
             "display_name": "Reximus",
@@ -50,15 +51,16 @@
             "aws_account_ids": [],
             "principal_investigator_id": "11234867890b0123a56789ab",
             "manager_ids": ["11234867890b0123a56789ab"],
             "member_ids": [],
             "admin_ids": [],
             'type': 'heaobject.organization.Organization',
             'mime_type': 'application/x.organization',
-            'accounts': []
+            'accounts': [],
+            'type_display_name': 'Organization'
         }
     ],
     'people': [{
         'id': '666f6f2d6261722d71757578',
         'created': None,
         'derived_by': None,
         'derived_from': [],
```

