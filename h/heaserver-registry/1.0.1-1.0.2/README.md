# Comparing `tmp/heaserver-registry-1.0.1.tar.gz` & `tmp/heaserver_registry-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-registry-1.0.1.tar", last modified: Tue Mar  5 22:27:23 2024, max compression
+gzip compressed data, was "heaserver_registry-1.0.2.tar", last modified: Thu Apr 18 02:22:07 2024, max compression
```

## Comparing `heaserver-registry-1.0.1.tar` & `heaserver_registry-1.0.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-03-05 22:27:23.862440 heaserver-registry-1.0.1/
--rw-rw-rw-   0        0        0      261 2022-03-11 23:00:39.000000 heaserver-registry-1.0.1/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 23:38:46.000000 heaserver-registry-1.0.1/.gitignore
--rw-rw-rw-   0        0        0     1658 2023-12-18 23:38:46.000000 heaserver-registry-1.0.1/Dockerfile
--rw-rw-rw-   0        0        0    11625 2022-03-11 23:00:39.000000 heaserver-registry-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 23:38:46.000000 heaserver-registry-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4658 2024-03-05 22:27:23.861441 heaserver-registry-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3434 2024-03-05 22:24:18.000000 heaserver-registry-1.0.1/README.md
--rw-rw-rw-   0        0        0     1878 2023-12-18 23:38:46.000000 heaserver-registry-1.0.1/RELEASING.md
--rw-rw-rw-   0        0        0      329 2023-12-18 23:38:46.000000 heaserver-registry-1.0.1/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-03-05 22:27:23.802247 heaserver-registry-1.0.1/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-03-05 22:27:23.802247 heaserver-registry-1.0.1/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-05 22:27:23.830375 heaserver-registry-1.0.1/integrationtests/heaserver/registryintegrationtest/
--rw-rw-rw-   0        0        0        0 2022-03-11 23:00:39.000000 heaserver-registry-1.0.1/integrationtests/heaserver/registryintegrationtest/__init__.py
--rw-rw-rw-   0        0        0     7795 2023-12-18 23:38:46.000000 heaserver-registry-1.0.1/integrationtests/heaserver/registryintegrationtest/collectiontestcase.py
--rw-rw-rw-   0        0        0     3991 2023-12-18 23:38:46.000000 heaserver-registry-1.0.1/integrationtests/heaserver/registryintegrationtest/componentpermissionstestcase.py
--rw-rw-rw-   0        0        0     8715 2023-12-18 23:38:46.000000 heaserver-registry-1.0.1/integrationtests/heaserver/registryintegrationtest/componenttestcase.py
--rw-rw-rw-   0        0        0    21073 2023-12-18 23:38:46.000000 heaserver-registry-1.0.1/integrationtests/heaserver/registryintegrationtest/test_all.py
--rw-rw-rw-   0        0        0     1418 2023-12-18 23:38:46.000000 heaserver-registry-1.0.1/integrationtests/heaserver/registryintegrationtest/test_all_with_bad_permissions.py
--rw-rw-rw-   0        0        0      111 2023-12-18 23:38:46.000000 heaserver-registry-1.0.1/pytest.ini
--rw-rw-rw-   0        0        0      248 2023-12-18 23:38:46.000000 heaserver-registry-1.0.1/requirements_dev.txt
--rw-rw-rw-   0        0        0     3014 2023-12-18 23:38:46.000000 heaserver-registry-1.0.1/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-03-05 22:27:23.862440 heaserver-registry-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2439 2024-03-05 22:26:44.000000 heaserver-registry-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-05 22:27:23.804371 heaserver-registry-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-03-05 22:27:23.803335 heaserver-registry-1.0.1/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-05 22:27:23.832376 heaserver-registry-1.0.1/src/heaserver/registry/
--rw-rw-rw-   0        0        0        0 2022-03-11 23:00:39.000000 heaserver-registry-1.0.1/src/heaserver/registry/__init__.py
--rw-rw-rw-   0        0        0    37352 2024-03-01 23:56:48.000000 heaserver-registry-1.0.1/src/heaserver/registry/service.py
-drwxrwxrwx   0        0        0        0 2024-03-05 22:27:23.833376 heaserver-registry-1.0.1/src/heaserver/registry/wstl/
--rw-rw-rw-   0        0        0    13493 2024-03-05 18:52:20.000000 heaserver-registry-1.0.1/src/heaserver/registry/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-03-05 22:27:23.859440 heaserver-registry-1.0.1/src/heaserver_registry.egg-info/
--rw-rw-rw-   0        0        0     4658 2024-03-05 22:27:23.000000 heaserver-registry-1.0.1/src/heaserver_registry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1920 2024-03-05 22:27:23.000000 heaserver-registry-1.0.1/src/heaserver_registry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-05 22:27:23.000000 heaserver-registry-1.0.1/src/heaserver_registry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2024-03-05 22:27:23.000000 heaserver-registry-1.0.1/src/heaserver_registry.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-03-05 22:27:23.000000 heaserver-registry-1.0.1/src/heaserver_registry.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-05 22:27:23.000000 heaserver-registry-1.0.1/src/heaserver_registry.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-05 22:27:23.805370 heaserver-registry-1.0.1/tests/
-drwxrwxrwx   0        0        0        0 2024-03-05 22:27:23.805370 heaserver-registry-1.0.1/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-05 22:27:23.849439 heaserver-registry-1.0.1/tests/heaserver/registrytest/
--rw-rw-rw-   0        0        0        0 2022-03-11 23:00:39.000000 heaserver-registry-1.0.1/tests/heaserver/registrytest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-05 22:27:23.858440 heaserver-registry-1.0.1/tests/heaserver/registrytest/__pycache__/
--rw-rw-rw-   0        0        0     2208 2023-07-03 21:35:26.000000 heaserver-registry-1.0.1/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.14464
--rw-rw-rw-   0        0        0     2208 2023-07-03 21:35:26.000000 heaserver-registry-1.0.1/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.1528
--rw-rw-rw-   0        0        0     2208 2023-07-03 21:35:26.000000 heaserver-registry-1.0.1/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.23164
--rw-rw-rw-   0        0        0     2208 2023-07-03 21:35:26.000000 heaserver-registry-1.0.1/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.23260
--rw-rw-rw-   0        0        0     2208 2023-07-03 21:35:26.000000 heaserver-registry-1.0.1/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.31268
--rw-rw-rw-   0        0        0     2921 2023-11-10 05:23:52.000000 heaserver-registry-1.0.1/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.20740
--rw-rw-rw-   0        0        0     7436 2023-12-18 23:38:46.000000 heaserver-registry-1.0.1/tests/heaserver/registrytest/collectiontestcase.py
--rw-rw-rw-   0        0        0     3850 2023-12-18 23:38:46.000000 heaserver-registry-1.0.1/tests/heaserver/registrytest/componentpermissionstestcase.py
--rw-rw-rw-   0        0        0     8152 2024-03-01 23:56:48.000000 heaserver-registry-1.0.1/tests/heaserver/registrytest/componenttestcase.py
--rw-rw-rw-   0        0        0    19776 2023-12-18 23:38:46.000000 heaserver-registry-1.0.1/tests/heaserver/registrytest/test_all.py
--rw-rw-rw-   0        0        0     1418 2023-12-18 23:38:46.000000 heaserver-registry-1.0.1/tests/heaserver/registrytest/test_all_with_bad_permissions.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:22:07.414178 heaserver_registry-1.0.2/
+-rw-rw-rw-   0        0        0      261 2022-03-11 23:00:39.000000 heaserver_registry-1.0.2/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 23:38:46.000000 heaserver_registry-1.0.2/.gitignore
+-rw-rw-rw-   0        0        0     1658 2023-12-18 23:38:46.000000 heaserver_registry-1.0.2/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2022-03-11 23:00:39.000000 heaserver_registry-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 23:38:46.000000 heaserver_registry-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4790 2024-04-18 02:22:07.413179 heaserver_registry-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3566 2024-04-18 02:20:30.000000 heaserver_registry-1.0.2/README.md
+-rw-rw-rw-   0        0        0     1878 2023-12-18 23:38:46.000000 heaserver_registry-1.0.2/RELEASING.md
+-rw-rw-rw-   0        0        0      329 2023-12-18 23:38:46.000000 heaserver_registry-1.0.2/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-04-18 02:22:07.349180 heaserver_registry-1.0.2/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-04-18 02:22:07.350177 heaserver_registry-1.0.2/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-18 02:22:07.379177 heaserver_registry-1.0.2/integrationtests/heaserver/registryintegrationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-11 23:00:39.000000 heaserver_registry-1.0.2/integrationtests/heaserver/registryintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0     7887 2024-04-17 00:22:00.000000 heaserver_registry-1.0.2/integrationtests/heaserver/registryintegrationtest/collectiontestcase.py
+-rw-rw-rw-   0        0        0     3991 2023-12-18 23:38:46.000000 heaserver_registry-1.0.2/integrationtests/heaserver/registryintegrationtest/componentpermissionstestcase.py
+-rw-rw-rw-   0        0        0     9262 2024-04-17 02:40:54.000000 heaserver_registry-1.0.2/integrationtests/heaserver/registryintegrationtest/componenttestcase.py
+-rw-rw-rw-   0        0        0    23391 2024-04-17 02:54:48.000000 heaserver_registry-1.0.2/integrationtests/heaserver/registryintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0     1418 2023-12-18 23:38:46.000000 heaserver_registry-1.0.2/integrationtests/heaserver/registryintegrationtest/test_all_with_bad_permissions.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 23:38:46.000000 heaserver_registry-1.0.2/pytest.ini
+-rw-rw-rw-   0        0        0      248 2023-12-18 23:38:46.000000 heaserver_registry-1.0.2/requirements_dev.txt
+-rw-rw-rw-   0        0        0     3014 2023-12-18 23:38:46.000000 heaserver_registry-1.0.2/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-04-18 02:22:07.415177 heaserver_registry-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2439 2024-04-18 02:21:19.000000 heaserver_registry-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:22:07.352177 heaserver_registry-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-18 02:22:07.351177 heaserver_registry-1.0.2/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-18 02:22:07.381178 heaserver_registry-1.0.2/src/heaserver/registry/
+-rw-rw-rw-   0        0        0        0 2022-03-11 23:00:39.000000 heaserver_registry-1.0.2/src/heaserver/registry/__init__.py
+-rw-rw-rw-   0        0        0    38098 2024-04-17 03:30:21.000000 heaserver_registry-1.0.2/src/heaserver/registry/service.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:22:07.382179 heaserver_registry-1.0.2/src/heaserver/registry/wstl/
+-rw-rw-rw-   0        0        0    13493 2024-03-07 16:45:28.000000 heaserver_registry-1.0.2/src/heaserver/registry/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-04-18 02:22:07.412178 heaserver_registry-1.0.2/src/heaserver_registry.egg-info/
+-rw-rw-rw-   0        0        0     4790 2024-04-18 02:22:07.000000 heaserver_registry-1.0.2/src/heaserver_registry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1920 2024-04-18 02:22:07.000000 heaserver_registry-1.0.2/src/heaserver_registry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 02:22:07.000000 heaserver_registry-1.0.2/src/heaserver_registry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2024-04-18 02:22:07.000000 heaserver_registry-1.0.2/src/heaserver_registry.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-18 02:22:07.000000 heaserver_registry-1.0.2/src/heaserver_registry.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-18 02:22:07.000000 heaserver_registry-1.0.2/src/heaserver_registry.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 02:22:07.353179 heaserver_registry-1.0.2/tests/
+drwxrwxrwx   0        0        0        0 2024-04-18 02:22:07.353179 heaserver_registry-1.0.2/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-18 02:22:07.398182 heaserver_registry-1.0.2/tests/heaserver/registrytest/
+-rw-rw-rw-   0        0        0        0 2022-03-11 23:00:39.000000 heaserver_registry-1.0.2/tests/heaserver/registrytest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:22:07.410178 heaserver_registry-1.0.2/tests/heaserver/registrytest/__pycache__/
+-rw-rw-rw-   0        0        0     2208 2023-07-03 21:35:26.000000 heaserver_registry-1.0.2/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.14464
+-rw-rw-rw-   0        0        0     2208 2023-07-03 21:35:26.000000 heaserver_registry-1.0.2/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.1528
+-rw-rw-rw-   0        0        0     2208 2023-07-03 21:35:26.000000 heaserver_registry-1.0.2/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.23164
+-rw-rw-rw-   0        0        0     2208 2023-07-03 21:35:26.000000 heaserver_registry-1.0.2/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.23260
+-rw-rw-rw-   0        0        0     2208 2023-07-03 21:35:26.000000 heaserver_registry-1.0.2/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.31268
+-rw-rw-rw-   0        0        0     2921 2023-11-10 05:23:52.000000 heaserver_registry-1.0.2/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.20740
+-rw-rw-rw-   0        0        0     7528 2024-04-17 00:19:45.000000 heaserver_registry-1.0.2/tests/heaserver/registrytest/collectiontestcase.py
+-rw-rw-rw-   0        0        0     3850 2023-12-18 23:38:46.000000 heaserver_registry-1.0.2/tests/heaserver/registrytest/componentpermissionstestcase.py
+-rw-rw-rw-   0        0        0     8623 2024-04-17 00:31:26.000000 heaserver_registry-1.0.2/tests/heaserver/registrytest/componenttestcase.py
+-rw-rw-rw-   0        0        0    23342 2024-04-17 00:39:46.000000 heaserver_registry-1.0.2/tests/heaserver/registrytest/test_all.py
+-rw-rw-rw-   0        0        0     1418 2023-12-18 23:38:46.000000 heaserver_registry-1.0.2/tests/heaserver/registrytest/test_all_with_bad_permissions.py
```

### Comparing `heaserver-registry-1.0.1/Dockerfile` & `heaserver_registry-1.0.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver-registry-1.0.1/LICENSE` & `heaserver_registry-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-registry-1.0.1/PKG-INFO` & `heaserver_registry-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-registry
-Version: 1.0.1
+Version: 1.0.2
 Summary: The HEA registry service.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -20,23 +20,26 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.0.7
+Requires-Dist: heaserver~=1.4.1
 
 # HEA Server Registry Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/),
 Salt Lake City, UT
 
 The HEA Server Registry Microservice manages mappings of HEA Object types to the microservices for storing and
 retrieving them.
 
+## Version 1.0.2
+* When requesting desktop objects as a Collection+JSON document, add the permissions property to the document.
+
 ## Version 1.0.1
 * Made the collection object form template fields read-only, and added the type field.
 
 ## Version 1
 Initial release.
 
 ## Runtime requirements
```

### Comparing `heaserver-registry-1.0.1/README.md` & `heaserver_registry-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # HEA Server Registry Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/),
 Salt Lake City, UT
 
 The HEA Server Registry Microservice manages mappings of HEA Object types to the microservices for storing and
 retrieving them.
 
+## Version 1.0.2
+* When requesting desktop objects as a Collection+JSON document, add the permissions property to the document.
+
 ## Version 1.0.1
 * Made the collection object form template fields read-only, and added the type field.
 
 ## Version 1
 Initial release.
 
 ## Runtime requirements
```

### Comparing `heaserver-registry-1.0.1/RELEASING.md` & `heaserver_registry-1.0.2/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-registry-1.0.1/integrationtests/heaserver/registryintegrationtest/collectiontestcase.py` & `heaserver_registry-1.0.2/integrationtests/heaserver/registryintegrationtest/collectiontestcase.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,16 @@
         'source': None,
         'source_detail': None,
         'type': 'heaobject.registry.Collection',
         'url': 'folders',
         'mime_type': 'application/x.collection',
         'collection_type_name': Item.get_type_name(),
         'file_system_name': DEFAULT_FILE_SYSTEM,
-        'file_system_type': MongoDBFileSystem.get_type_name()
+        'file_system_type': MongoDBFileSystem.get_type_name(),
+        'type_display_name': 'Collection'
     },
         {
             'id': Folder.get_type_name(),
             'created': None,
             'derived_by': None,
             'derived_from': [],
             'description': None,
@@ -60,15 +61,16 @@
             'source': None,
             'source_detail': None,
             'type': 'heaobject.registry.Collection',
             'url': 'folders',
             'mime_type': 'application/x.collection',
             'collection_type_name': Folder.get_type_name(),
             'file_system_name': DEFAULT_FILE_SYSTEM,
-            'file_system_type': MongoDBFileSystem.get_type_name()
+            'file_system_type': MongoDBFileSystem.get_type_name(),
+            'type_display_name': 'Collection'
         }],
         CollectionKey(name=service.MONGODB_COMPONENT_COLLECTION, db_manager_cls=DockerMongoManager): [
         {
             'id': '0123456789ab0123456789ab',
             'created': None,
             'derived_by': None,
             'derived_from': [],
```

### Comparing `heaserver-registry-1.0.1/integrationtests/heaserver/registryintegrationtest/componentpermissionstestcase.py` & `heaserver_registry-1.0.2/integrationtests/heaserver/registryintegrationtest/componentpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-registry-1.0.1/integrationtests/heaserver/registryintegrationtest/componenttestcase.py` & `heaserver_registry-1.0.2/integrationtests/heaserver/registryintegrationtest/componenttestcase.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,16 +32,18 @@
             'resource_type_name': 'heaobject.folder.Folder',
             'base_path': 'folders',
             'file_system_name': 'DEFAULT_FILE_SYSTEM',
             'file_system_type': 'heaobject.volume.DefaultFileSystem',
             'resource_collection_type_display_name': 'heaobject.folder.Folder',
             'collection_accessor_users': [ALL_USERS],
             'creator_users': [],
-            'default_shares': []
-        }]
+            'default_shares': [],
+            'type_display_name': 'Resource'
+        }],
+        'type_display_name': 'Registry Component'
     },
         {
             'id': '0123456789ab0123456789ab',
             'created': None,
             'derived_by': None,
             'derived_from': [],
             'description': None,
@@ -61,27 +63,30 @@
                 'resource_type_name': 'heaobject.folder.Item',
                 'base_path': 'folders',
                 'file_system_name': 'DEFAULT_FILE_SYSTEM',
                 'file_system_type': 'heaobject.volume.DefaultFileSystem',
                 'resource_collection_type_display_name': 'heaobject.folder.Item',
                 'collection_accessor_users': [ALL_USERS],
                 'creator_users': [],
-                'default_shares': []
-            }]
+                'default_shares': [],
+                'type_display_name': 'Resource'
+            }],
+            'type_display_name': 'Registry Component'
         }]}
 
 db_store_2 = {
     service.MONGODB_COMPONENT_COLLECTION: [
         {
             'id': '0123456789ab0123456789ab',
             'created': None,
             'derived_by': None,
             'derived_from': [],
             'description': None,
             'display_name': 'Luximus',
+            'invites': [],
             'modified': None,
             'name': 'luximus',
             'owner': NONE_USER,
             'shares': [{
                 'type': 'heaobject.root.ShareImpl',
                 'invite': None,
                 'user': TEST_USER,
@@ -95,24 +100,27 @@
             'resources': [{
                 'type': 'heaobject.registry.Resource',
                 'resource_type_name': 'heaobject.folder.Item',
                 'base_path': 'folders',
                 'resource_collection_type_display_name': 'heaobject.folder.Item',
                 'collection_accessor_users': [ALL_USERS],
                 'creator_users': [],
-                'default_shares': []
-            }]
+                'default_shares': [],
+                'type_display_name': 'Resource'
+            }],
+            'type_display_name': 'Registry Component'
         },
         {
             'id': '666f6f2d6261722d71757578',
             'created': None,
             'derived_by': None,
             'derived_from': ['foo', 'bar'],
             'description': None,
             'display_name': 'Reximus',
+            'invites': [],
             'modified': None,
             'name': 'reximus',
             'owner': NONE_USER,
             'shares': [{
                 'type': 'heaobject.root.ShareImpl',
                 'invite': None,
                 'user': TEST_USER,
@@ -124,19 +132,22 @@
             'base_url': 'http://localhost/foo',
             'external_base_url': None,
             'resources': [{
                 'type': 'heaobject.registry.Resource',
                 'resource_type_name': 'heaobject.folder.Folder',
                 'base_path': 'folders',
                 'file_system_name': 'DEFAULT_FILE_SYSTEM',
+                'file_system_type': 'heaobject.volume.MongoDBFileSystem',
                 'resource_collection_type_display_name': 'heaobject.folder.Folder',
                 'collection_accessor_users': [ALL_USERS],
                 'creator_users': [],
-                'default_shares': []
-            }]
+                'default_shares': [],
+                'type_display_name': 'Resource'
+            }],
+            'type_display_name': 'Registry Component'
         }]}
 
 ComponentTestCase = get_test_case_cls_default(coll=service.MONGODB_COMPONENT_COLLECTION,
                                               href='http://localhost:8080/components',
                                               wstl_package=service.__package__,
                                               db_manager_cls=MockDockerMongoManager,
                                               fixtures=db_store,
```

### Comparing `heaserver-registry-1.0.1/integrationtests/heaserver/registryintegrationtest/test_all.py` & `heaserver_registry-1.0.2/integrationtests/heaserver/registryintegrationtest/test_all.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         del desktop_objects[coll][1]['resources'][0]['file_system_name']
         del desktop_objects[coll][1]['resources'][0]['file_system_type']
 
     async def test_no_file_system(self):
         expected = [{"collection": {
             "version": "1.0",
             "href": "http://localhost:8080/components/bytype/heaobject.folder.Folder",
+            "permissions": [["CHECK_DYNAMIC", "COOWNER", "CREATOR", "DELETER", "EDITOR", "SHARER", "VIEWER"]],
             "items": [{
                 "data": [
                     {
                         "name": "id",
                         "value": "666f6f2d6261722d71757578",
                         "prompt": "id",
                         "display": False},
@@ -140,14 +141,20 @@
                     {
                         "name": "type",
                         "value": "heaobject.registry.Component",
                         "prompt": "type",
                         "display": True
                     },
                     {
+                        "name": "type_display_name",
+                        "value": "Registry Component",
+                        "prompt": "type_display_name",
+                        "display": True
+                    },
+                    {
                         "section": "resources",
                         "index": 0,
                         "name": "resource_type_name",
                         "value": "heaobject.folder.Folder",
                         "prompt":
                             "resource_type_name",
                         "display": True},
@@ -164,26 +171,41 @@
                         "name": "file_system_name",
                         "value": "DEFAULT_FILE_SYSTEM",
                         "prompt": "file_system_name",
                         "display": True},
                     {
                         "section": "resources",
                         "index": 0,
+                        "name": "file_system_type",
+                        "value": "heaobject.volume.MongoDBFileSystem",
+                        "prompt": "file_system_type",
+                        "display": True},
+                    {
+                        "section": "resources",
+                        "index": 0,
                         "name": "type",
                         "value": "heaobject.registry.Resource",
                         "prompt": "type",
                         "display": True},
                     {
                         "section": "resources",
                         "index": 0,
                         "name": "resource_collection_type_display_name",
                         "value": "heaobject.folder.Folder",
                         "prompt": "resource_collection_type_display_name",
                         "display": True},
                     {
+                        "section": "resources",
+                        "index": 0,
+                        "name": "type_display_name",
+                        "value": "Resource",
+                        "prompt":
+                            "type_display_name",
+                        "display": True},
+                    {
                         "display": True,
                         "index": 0,
                         "name": "collection_accessor_users",
                         "prompt": "collection_accessor_users",
                         "section": "resources",
                         "value": ["system|all"]
                     },
@@ -237,15 +259,17 @@
 
 
 class TestGetResource2(ComponentTestCase2):
     _headers = {SUB: NONE_USER, hdrs.X_FORWARDED_HOST: 'localhost:8080'}
 
     async def test_no_file_system(self):
         expected = [{"collection": {"version": "1.0",
-                                  "href": "http://localhost:8080/components/bytype/heaobject.folder.Folder", "items": [{
+                                    "href": "http://localhost:8080/components/bytype/heaobject.folder.Folder",
+                                    "permissions": [["CHECK_DYNAMIC", "COOWNER", "CREATOR", "DELETER", "EDITOR", "SHARER", "VIEWER"]],
+            "items": [{
                 "data": [
                     {
                         "name": "id",
                         "value": "666f6f2d6261722d71757578",
                         "prompt": "id",
                         "display": False},
                     {
@@ -276,14 +300,26 @@
                     {
                         "name": "type",
                         "value": "heaobject.registry.Component",
                         "prompt": "type",
                         "display": True
                     },
                     {
+                        "name": "invites",
+                        "value": [],
+                        "prompt": "invites",
+                        "display": True
+                    },
+                    {
+                        "name": "type_display_name",
+                        "value": "Registry Component",
+                        "prompt": "type_display_name",
+                        "display": True
+                    },
+                    {
                         "name": "invite",
                         "index": 0,
                         "section": "shares",
                         "prompt": "invite",
                         "value": None,
                         "display": True
                     },
@@ -367,14 +403,21 @@
                         "name": "file_system_name",
                         "value": "DEFAULT_FILE_SYSTEM",
                         "prompt": "file_system_name",
                         "display": True},
                     {
                         "section": "resources",
                         "index": 0,
+                        "name": "file_system_type",
+                        "value": "heaobject.volume.MongoDBFileSystem",
+                        "prompt": "file_system_type",
+                        "display": True},
+                    {
+                        "section": "resources",
+                        "index": 0,
                         "name": "type",
                         "value": "heaobject.registry.Resource",
                         "prompt": "type",
                         "display": True},
                     {
                         "section": "resources",
                         "index": 0,
@@ -401,14 +444,22 @@
                     {
                         "display": True,
                         "index": 0,
                         "name": "default_shares",
                         "prompt": "default_shares",
                         "section": "resources",
                         "value": []
+                    },
+                    {
+                        "display": True,
+                        "index": 0,
+                        "name": "type_display_name",
+                        "prompt": "type_display_name",
+                        "section": "resources",
+                        "value": "Resource"
                     }],
                 "links": []}]}}]
         obj = await self.client.request('GET',
                                         (self._href / 'bytype' / 'heaobject.folder.Folder').path,
                                         headers=TestGetResource2._headers)
         self.assertEquals(_ordered(expected), _ordered(await obj.json()))
```

### Comparing `heaserver-registry-1.0.1/integrationtests/heaserver/registryintegrationtest/test_all_with_bad_permissions.py` & `heaserver_registry-1.0.2/integrationtests/heaserver/registryintegrationtest/test_all_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-registry-1.0.1/run-swaggerui.py` & `heaserver_registry-1.0.2/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver-registry-1.0.1/setup.py` & `heaserver_registry-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(name='heaserver-registry',
-                 version='1.0.1',
+                 version='1.0.2',
                  description='The HEA registry service.',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://risr.hci.utah.edu',
                  author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
                  author_email='Andrew.Post@hci.utah.edu',
                  python_requires='>=3.10',
                  package_dir={'': 'src'},
                  packages=['heaserver.registry'],
                  package_data={'heaserver.registry': ['wstl/*.json']},
                  install_requires=[
-                     'heaserver~=1.0.7'
+                     'heaserver~=1.4.1'
                  ],
                  classifiers=[
                      'Development Status :: 5 - Production/Stable',
                      'Intended Audience :: Developers',
                      'Intended Audience :: Science/Research',
                      'License :: OSI Approved :: Apache Software License',
                      'Framework :: AsyncIO',
```

### Comparing `heaserver-registry-1.0.1/src/heaserver/registry/service.py` & `heaserver_registry-1.0.2/src/heaserver/registry/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from heaserver.service import response, appproperty
 from heaserver.service.runner import init_cmd_line, routes, start, web
 from heaserver.service.db import mongo, mongoservicelib
 from heaserver.service.wstl import builder_factory, action
 from heaserver.service.oidcclaimhdrs import SUB
 from heaobject.registry import Component, Property, Collection
-from heaobject.root import Share, ShareImpl, Permission
+from heaobject.root import Share, ShareImpl, Permission, DesktopObjectDict
 from heaobject.volume import DEFAULT_FILE_SYSTEM, MongoDBFileSystem
 from heaobject.user import ALL_USERS, NONE_USER
 from typing import AsyncIterator
 
 MONGODB_COMPONENT_COLLECTION = 'components'
 MONGODB_PROPERTIES_COLLECTION = 'properties'
 MONGODB_COLLECTION_COLLECTION = 'collection'
@@ -124,14 +124,15 @@
               value: DEFAULT_FILE_SYSTEM
     responses:
       '200':
         $ref: '#/components/responses/200'
       '404':
         $ref: '#/components/responses/404'
     """
+    sub = request.headers.get(SUB, NONE_USER)
     type_ = request.match_info['type']
     file_system_name = request.match_info.get('filesystemname', DEFAULT_FILE_SYSTEM)
     file_system_type = request.match_info.get('filesystemtype', MongoDBFileSystem.get_type_name())
     cache_key = (request.headers.get(SUB, NONE_USER), MONGODB_COMPONENT_COLLECTION, f'type^{type_}', f'file_system_type^{file_system_type}', f'file_system_name^{file_system_name}')
     result = request.app[appproperty.HEA_CACHE].get(cache_key)
     if result is None:
         if file_system_name == DEFAULT_FILE_SYSTEM:
@@ -144,19 +145,27 @@
             query_clause.update({'file_system_type': {'$eq': file_system_type}})
         mongo_attributes = {'resources': {
             '$elemMatch': {
                 'resource_type_name': {'$eq': type_},
                 **query_clause
             }}}
 
-        result = await request.app[appproperty.HEA_DB].get(request,
+        result_dict = await request.app[appproperty.HEA_DB].get(request,
                                                         MONGODB_COMPONENT_COLLECTION,
                                                         mongoattributes=mongo_attributes)
-        request.app[appproperty.HEA_CACHE][cache_key] = result
-    return await response.get(request, result)
+        if result_dict is None:
+            return await response.get(request, None)
+        component = Component()
+        component.from_dict(result_dict)
+        result_dict_ = component.to_dict()
+        permissions = component.get_permissions(sub)
+        request.app[appproperty.HEA_CACHE][cache_key] = (result_dict_, permissions)
+        return await response.get(request, result_dict_, permissions=permissions)
+    else:
+        return await response.get(request, result[0], permissions=result[1])
 
 
 @routes.get('/components')
 @routes.get('/components/')
 @action('heaserver-registry-component-get-properties', rel='hea-properties')
 @action('heaserver-registry-component-duplicate', rel='hea-duplicator', path='components/{id}/duplicator')
 async def get_all_components(request: web.Request) -> web.Response:
@@ -930,29 +939,32 @@
     summary: All collections.
     tags:
         - heaserver-registry-collection
     responses:
       '200':
         $ref: '#/components/responses/200'
     """
-    collections = []
+    sub = request.headers.get(SUB, NONE_USER)
+    collections: list[DesktopObjectDict] = []
+    permissions: list[list[Permission]] = []
     for obj in await mongoservicelib.get_all_dict(request, MONGODB_COMPONENT_COLLECTION):
         for resource in obj['resources']:
             c = Collection()
             c.id = resource['resource_type_name']
             c.name = resource['resource_type_name']
             c.display_name = resource['resource_collection_type_display_name']
             c.collection_type_name = resource['resource_type_name']
             c.url = resource['base_path']
             share = ShareImpl()
             share.user = ALL_USERS
             share.permissions = [Permission.VIEWER, Permission.CHECK_DYNAMIC]
             c.shares = [share]
             collections.append(c.to_dict())
-    return await response.get_all(request, collections)
+            permissions.append(c.get_permissions(sub))
+    return await response.get_all(request, collections, permissions=permissions)
 
 
 @routes.get('/collections/{id}')
 @action(name='heaserver-registry-collection-get-open-choices', rel='hea-opener-choices', path='collections/{id}/opener')
 @action(name='heaserver-registry-collection-get-properties', rel='hea-properties')
 @action(name='heaserver-registry-collection-get-self', rel='self', path='collections/{id}')
 async def get_collection(request: web.Request) -> web.Response:
@@ -1053,14 +1065,15 @@
     config = init_cmd_line(description='Registry of HEA services, HEA web clients, and other web sites of interest',
                            default_port=8080)
     start(db=mongo.MongoManager,
           wstl_builder_factory=builder_factory(__package__), config=config)
 
 
 async def _get_collection(request: web.Request) -> web.Response:
+    sub = request.headers.get(SUB, NONE_USER)
     mongo_attributes = {'resources': {
         '$elemMatch': {
             'resource_type_name': {'$eq': request.match_info['id']},
         }}}
     for obj in await mongoservicelib.get_all_dict(request, MONGODB_COMPONENT_COLLECTION, mongoattributes=mongo_attributes):
         for resource_dict in (r for r in obj['resources'] if r['resource_type_name'] == request.match_info['id']):
             c = Collection()
@@ -1077,9 +1090,9 @@
                 share = ShareImpl()
                 share.user = collection_accessor_user
                 share.permissions = [Permission.VIEWER, Permission.CHECK_DYNAMIC]
                 if collection_accessor_user in creator_users_set:
                     share.add_permission(Permission.CREATOR)
                 shares.append(share)
             c.shares = shares
-            return await response.get(request, c.to_dict())
+            return await response.get(request, c.to_dict(), c.get_permissions(sub))
     return await response.get(request, None)
```

### Comparing `heaserver-registry-1.0.1/src/heaserver/registry/wstl/all.json` & `heaserver_registry-1.0.2/src/heaserver/registry/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-registry-1.0.1/src/heaserver_registry.egg-info/PKG-INFO` & `heaserver_registry-1.0.2/src/heaserver_registry.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-registry
-Version: 1.0.1
+Version: 1.0.2
 Summary: The HEA registry service.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -20,23 +20,26 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.0.7
+Requires-Dist: heaserver~=1.4.1
 
 # HEA Server Registry Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/),
 Salt Lake City, UT
 
 The HEA Server Registry Microservice manages mappings of HEA Object types to the microservices for storing and
 retrieving them.
 
+## Version 1.0.2
+* When requesting desktop objects as a Collection+JSON document, add the permissions property to the document.
+
 ## Version 1.0.1
 * Made the collection object form template fields read-only, and added the type field.
 
 ## Version 1
 Initial release.
 
 ## Runtime requirements
```

### Comparing `heaserver-registry-1.0.1/src/heaserver_registry.egg-info/SOURCES.txt` & `heaserver_registry-1.0.2/src/heaserver_registry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-registry-1.0.1/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.14464` & `heaserver_registry-1.0.2/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.14464`

 * *Files identical despite different names*

### Comparing `heaserver-registry-1.0.1/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.1528` & `heaserver_registry-1.0.2/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.1528`

 * *Files identical despite different names*

### Comparing `heaserver-registry-1.0.1/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.23164` & `heaserver_registry-1.0.2/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.23164`

 * *Files identical despite different names*

### Comparing `heaserver-registry-1.0.1/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.23260` & `heaserver_registry-1.0.2/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.23260`

 * *Files identical despite different names*

### Comparing `heaserver-registry-1.0.1/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.31268` & `heaserver_registry-1.0.2/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.31268`

 * *Files identical despite different names*

### Comparing `heaserver-registry-1.0.1/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.20740` & `heaserver_registry-1.0.2/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.20740`

 * *Files identical despite different names*

### Comparing `heaserver-registry-1.0.1/tests/heaserver/registrytest/collectiontestcase.py` & `heaserver_registry-1.0.2/tests/heaserver/registrytest/collectiontestcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,16 @@
         'source': None,
         'source_detail': None,
         'type': Collection.get_type_name(),
         'url': 'folders',
         'mime_type': 'application/x.collection',
         'collection_type_name': Item.get_type_name(),
         'file_system_name': DEFAULT_FILE_SYSTEM,
-        'file_system_type': MongoDBFileSystem.get_type_name()
+        'file_system_type': MongoDBFileSystem.get_type_name(),
+        'type_display_name': 'Collection'
     },
         {
             'id': Folder.get_type_name(),
             'created': None,
             'derived_by': None,
             'derived_from': [],
             'description': None,
@@ -58,15 +59,16 @@
             'source': None,
             'source_detail': None,
             'type': Collection.get_type_name(),
             'url': 'folders',
             'mime_type': 'application/x.collection',
             'collection_type_name': Folder.get_type_name(),
             'file_system_name': DEFAULT_FILE_SYSTEM,
-            'file_system_type': MongoDBFileSystem.get_type_name()
+            'file_system_type': MongoDBFileSystem.get_type_name(),
+            'type_display_name': 'Collection'
         }],
         service.MONGODB_COMPONENT_COLLECTION: [
         {
             'id': '0123456789ab0123456789ab',
             'created': None,
             'derived_by': None,
             'derived_from': [],
```

### Comparing `heaserver-registry-1.0.1/tests/heaserver/registrytest/componentpermissionstestcase.py` & `heaserver_registry-1.0.2/tests/heaserver/registrytest/componentpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-registry-1.0.1/tests/heaserver/registrytest/componenttestcase.py` & `heaserver_registry-1.0.2/tests/heaserver/registrytest/componenttestcase.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,16 +31,18 @@
             'resource_type_name': 'heaobject.folder.Folder',
             'base_path': 'folders',
             'file_system_name': 'DEFAULT_FILE_SYSTEM',
             'file_system_type': 'heaobject.volume.DefaultFileSystem',
             'resource_collection_type_display_name': 'heaobject.folder.Folder',
             'collection_accessor_users': [ALL_USERS],
             'creator_users': [],
-            'default_shares': []
-        }]
+            'default_shares': [],
+            'type_display_name': 'Resource'
+        }],
+        'type_display_name': 'Registry Component'
     },
         {
             'id': '0123456789ab0123456789ab',
             'created': None,
             'derived_by': None,
             'derived_from': [],
             'description': None,
@@ -60,16 +62,18 @@
                 'resource_type_name': 'heaobject.folder.Item',
                 'base_path': 'folders',
                 'file_system_name': 'DEFAULT_FILE_SYSTEM',
                 'file_system_type': 'heaobject.volume.DefaultFileSystem',
                 'resource_collection_type_display_name': 'heaobject.folder.Item',
                 'collection_accessor_users': [ALL_USERS],
                 'creator_users': [],
-                'default_shares': []
-            }]
+                'default_shares': [],
+                'type_display_name': 'Resource'
+            }],
+            'type_display_name': 'Registry Component'
         }]}
 
 ComponentTestCase = get_test_case_cls_default(coll=service.MONGODB_COMPONENT_COLLECTION,
                                               href='http://localhost:8080/components',
                                               wstl_package=service.__package__,
                                               fixtures=db_store,
                                               get_actions=[
@@ -90,14 +94,15 @@
 db_store_2 = {
     service.MONGODB_COMPONENT_COLLECTION: [
         {
             'id': '0123456789ab0123456789ab',
             'created': None,
             'derived_by': None,
             'derived_from': [],
+            'invites': [],
             'description': None,
             'display_name': 'Luximus',
             'modified': None,
             'name': 'luximus',
             'owner': NONE_USER,
             'shares': [{
                 'type': 'heaobject.root.ShareImpl',
@@ -109,22 +114,25 @@
             'source_detail': None,
             'type': 'heaobject.registry.Component',
             'base_url': 'http://localhost/foo',
             'resources': [{
                 'type': 'heaobject.registry.Resource',
                 'resource_type_name': 'heaobject.folder.Item',
                 'base_path': 'folders',
-                'resource_collection_type_display_name': 'heaobject.folder.Item'
-            }]
+                'resource_collection_type_display_name': 'heaobject.folder.Item',
+                'type_display_name': 'Resource'
+            }],
+            'type_display_name': 'Registry Component'
         },
         {
             'id': '666f6f2d6261722d71757578',
             'created': None,
             'derived_by': None,
             'derived_from': [],
+            'invites': [],
             'description': None,
             'display_name': 'Reximus',
             'modified': None,
             'name': 'reximus',
             'owner': NONE_USER,
             'shares': [{
                 'type': 'heaobject.root.ShareImpl',
@@ -138,15 +146,17 @@
             'base_url': 'http://localhost/foo',
             'resources': [{
                 'type': 'heaobject.registry.Resource',
                 'resource_type_name': 'heaobject.folder.Folder',
                 'base_path': 'folders',
                 'file_system_name': 'DEFAULT_FILE_SYSTEM',
                 'resource_collection_type_display_name': 'heaobject.folder.Folder',
-            }]
+                'type_display_name': 'Resource'
+            }],
+            'type_display_name': 'Registry Component'
         }]}
 
 ComponentTestCase2 = get_test_case_cls_default(coll=service.MONGODB_COMPONENT_COLLECTION,
                                                href='http://localhost:8080/components',
                                                wstl_package=service.__package__,
                                                fixtures=db_store_2,
                                                get_actions=[
```

### Comparing `heaserver-registry-1.0.1/tests/heaserver/registrytest/test_all.py` & `heaserver_registry-1.0.2/tests/heaserver/registrytest/test_all.py`

 * *Files 18% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         del desktop_objects[coll][1]["resources"][0]["file_system_name"]
         del desktop_objects[coll][1]["resources"][0]["file_system_type"]
 
     async def test_no_file_system(self):
         expected = [{"collection": {
             "version": "1.0",
             "href": "http://localhost:8080/components/bytype/heaobject.folder.Folder",
+            "permissions": [["CHECK_DYNAMIC", "COOWNER", "CREATOR", "DELETER", "EDITOR", "SHARER", "VIEWER"]],
             "items": [{
                 "data": [
                     {
                         "name": "id",
                         "value": "666f6f2d6261722d71757578",
                         "prompt": "id",
                         "display": False},
@@ -144,14 +145,20 @@
                     {
                         "name": "external_base_url",
                         "value": None,
                         "prompt": "external_base_url",
                         "display": True
                     },
                     {
+                        "name": "type_display_name",
+                        "value": "Registry Component",
+                        "prompt": "type_display_name",
+                        "display": True
+                    },
+                    {
                         "section": "resources",
                         "index": 0,
                         "name": "resource_type_name",
                         "value": "heaobject.folder.Folder",
                         "prompt":
                             "resource_type_name",
                         "display": True
@@ -207,14 +214,30 @@
                     {
                         "display": True,
                         "index": 0,
                         "name": "default_shares",
                         "prompt": "default_shares",
                         "section": "resources",
                         "value": []
+                    },
+                    {
+                        "section": "resources",
+                        "index": 0,
+                        "name": "file_system_type",
+                        "value": "heaobject.volume.MongoDBFileSystem",
+                        "prompt": "file_system_type",
+                        "display": True
+                    },
+                    {
+                        "section": "resources",
+                        "index": 0,
+                        "name": "type_display_name",
+                        "value": "Resource",
+                        "prompt": "type_display_name",
+                        "display": True
                     }],
                 "links": []}]}}]
         obj = await self.client.request("GET",
                                         (self._href / "bytype" / "heaobject.folder.Folder").path,
                                         headers=self._headers)
         self.assertEquals(_ordered(expected), _ordered(await obj.json()))
 
@@ -242,22 +265,41 @@
 class TestGetResource2(ComponentTestCase2):
     _headers = {SUB: NONE_USER, hdrs.X_FORWARDED_HOST: "localhost:8080"}
 
     async def test_no_file_system(self):
         expected = [{"collection": {
             "version": "1.0",
             "href": "http://localhost:8080/components/bytype/heaobject.folder.Folder",
+            "permissions": [["CHECK_DYNAMIC", "COOWNER", "CREATOR", "DELETER", "EDITOR", "SHARER", "VIEWER"]],
             "items": [{
                 "data": [
                     {
                         "name": "id",
                         "value": "666f6f2d6261722d71757578",
                         "prompt": "id",
                         "display": False},
                     {
+                        "name": "type_display_name",
+                        "value": "Registry Component",
+                        "prompt": "type_display_name",
+                        "display": True
+                    },
+                    {
+                        "name": "invites",
+                        "value": [],
+                        "prompt": "invites",
+                        "display": True
+                    },
+                    {
+                        "name": "external_base_url",
+                        "value": None,
+                        "prompt": "external_base_url",
+                        "display": True
+                    },
+                    {
                         "name": "created",
                         "value": None,
                         "prompt": "created",
                         "display": True},
                     {
                         "name": "derived_by",
                         "value": None,
@@ -379,15 +421,57 @@
                     },
                     {
                         "section": "resources",
                         "index": 0,
                         "name": "resource_collection_type_display_name",
                         "value": "heaobject.folder.Folder",
                         "prompt": "resource_collection_type_display_name",
-                        "display": True}],
+                        "display": True
+                    },
+                    {
+                        "section": "resources",
+                        "index": 0,
+                        "name": "file_system_type",
+                        "value": "heaobject.volume.MongoDBFileSystem",
+                        "prompt": "file_system_type",
+                        "display": True
+                    },
+                    {
+                        "section": "resources",
+                        "index": 0,
+                        "name": "type_display_name",
+                        "value": "Resource",
+                        "prompt": "type_display_name",
+                        "display": True
+                    },
+                    {
+                        "section": "resources",
+                        "index": 0,
+                        "name": "collection_accessor_users",
+                        "value": [],
+                        "prompt": "collection_accessor_users",
+                        "display": True
+                    },
+                    {
+                        "section": "resources",
+                        "index": 0,
+                        "name": "creator_users",
+                        "value": [],
+                        "prompt": "creator_users",
+                        "display": True
+                    },
+                    {
+                        "section": "resources",
+                        "index": 0,
+                        "name": "default_shares",
+                        "value": [],
+                        "prompt": "default_shares",
+                        "display": True
+                    }
+                    ],
                 "links": []}]}}]
         obj = await self.client.request('GET',
                                         (self._href / 'bytype' / 'heaobject.folder.Folder').path,
                                         headers=TestGetResource2._headers)
         self.assertEquals(_ordered(expected), _ordered(await obj.json()))
 
     async def test_no_file_system_status(self):
```

### Comparing `heaserver-registry-1.0.1/tests/heaserver/registrytest/test_all_with_bad_permissions.py` & `heaserver_registry-1.0.2/tests/heaserver/registrytest/test_all_with_bad_permissions.py`

 * *Files identical despite different names*

