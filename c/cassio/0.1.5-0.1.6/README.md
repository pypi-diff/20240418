# Comparing `tmp/cassio-0.1.5.tar.gz` & `tmp/cassio-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cassio-0.1.5.tar", last modified: Sat Feb 17 14:28:24 2024, max compression
+gzip compressed data, was "cassio-0.1.6.tar", max compression
```

## Comparing `cassio-0.1.5.tar` & `cassio-0.1.6.tar`

### file list

```diff
@@ -1,47 +1,34 @@
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2024-02-17 14:28:24.452396 cassio-0.1.5/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     3951 2024-02-17 14:28:24.452396 cassio-0.1.5/PKG-INFO
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2898 2024-02-17 14:27:39.000000 cassio-0.1.5/README.md
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       78 2024-02-17 14:28:24.452396 cassio-0.1.5/setup.cfg
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     1796 2024-02-17 14:26:31.000000 cassio-0.1.5/setup.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2024-02-17 14:28:24.448397 cassio-0.1.5/src/
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2024-02-17 14:28:24.448397 cassio-0.1.5/src/cassio/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)      192 2024-02-08 12:57:08.000000 cassio-0.1.5/src/cassio/__init__.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2024-02-17 14:28:24.448397 cassio-0.1.5/src/cassio/config/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)    14221 2024-02-08 16:33:37.000000 cassio-0.1.5/src/cassio/config/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2524 2024-02-15 08:55:35.000000 cassio-0.1.5/src/cassio/config/bundle_download.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     5566 2024-02-08 12:57:08.000000 cassio-0.1.5/src/cassio/config/bundle_management.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2024-02-17 14:28:24.448397 cassio-0.1.5/src/cassio/db_reader/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)      107 2024-02-08 12:57:08.000000 cassio-0.1.5/src/cassio/db_reader/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     9968 2024-02-08 16:33:37.000000 cassio-0.1.5/src/cassio/db_reader/multi_table_cassandra_reader.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2024-02-17 14:28:24.448397 cassio-0.1.5/src/cassio/history/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       79 2023-08-27 20:20:51.000000 cassio-0.1.5/src/cassio/history/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2410 2024-02-08 16:33:37.000000 cassio-0.1.5/src/cassio/history/stored_blob_history.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2024-02-17 14:28:24.448397 cassio-0.1.5/src/cassio/keyvalue/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       60 2023-08-27 20:20:51.000000 cassio-0.1.5/src/cassio/keyvalue/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2283 2024-02-08 12:57:08.000000 cassio-0.1.5/src/cassio/keyvalue/k_v_cache.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)        0 2024-02-08 12:57:08.000000 cassio-0.1.5/src/cassio/py.typed
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2024-02-17 14:28:24.452396 cassio-0.1.5/src/cassio/table/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     1230 2023-08-27 20:20:51.000000 cassio-0.1.5/src/cassio/table/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)    16656 2024-02-15 08:55:35.000000 cassio-0.1.5/src/cassio/table/base_table.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     5213 2024-02-08 12:57:08.000000 cassio-0.1.5/src/cassio/table/cql.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)    31290 2024-02-08 12:57:08.000000 cassio-0.1.5/src/cassio/table/mixins.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     1806 2024-02-08 13:44:39.000000 cassio-0.1.5/src/cassio/table/table_types.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2349 2023-08-27 20:20:51.000000 cassio-0.1.5/src/cassio/table/tables.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)      690 2024-02-08 13:31:40.000000 cassio-0.1.5/src/cassio/table/utils.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2024-02-17 14:28:24.452396 cassio-0.1.5/src/cassio/utils/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       80 2024-02-08 12:57:08.000000 cassio-0.1.5/src/cassio/utils/__init__.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2024-02-17 14:28:24.452396 cassio-0.1.5/src/cassio/utils/db_inspection/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     1024 2024-02-08 12:57:08.000000 cassio-0.1.5/src/cassio/utils/db_inspection/__init__.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2024-02-17 14:28:24.452396 cassio-0.1.5/src/cassio/utils/vector/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       80 2023-08-27 20:20:51.000000 cassio-0.1.5/src/cassio/utils/vector/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2663 2024-02-08 12:57:08.000000 cassio-0.1.5/src/cassio/utils/vector/distance_metrics.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2024-02-17 14:28:24.452396 cassio-0.1.5/src/cassio/vector/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       65 2023-08-27 20:20:51.000000 cassio-0.1.5/src/cassio/vector/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     4335 2024-02-08 16:33:37.000000 cassio-0.1.5/src/cassio/vector/vector_table.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2024-02-17 14:28:24.448397 cassio-0.1.5/src/cassio.egg-info/
--rw-r--r--   0 stefano   (1000) stefano   (1000)     3951 2024-02-17 14:28:24.000000 cassio-0.1.5/src/cassio.egg-info/PKG-INFO
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     1019 2024-02-17 14:28:24.000000 cassio-0.1.5/src/cassio.egg-info/SOURCES.txt
--rw-rw-r--   0 stefano   (1000) stefano   (1000)        1 2024-02-17 14:28:24.000000 cassio-0.1.5/src/cassio.egg-info/dependency_links.txt
--rw-rw-r--   0 stefano   (1000) stefano   (1000)      106 2024-02-17 14:28:24.000000 cassio-0.1.5/src/cassio.egg-info/entry_points.txt
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       48 2024-02-17 14:28:24.000000 cassio-0.1.5/src/cassio.egg-info/requires.txt
--rw-rw-r--   0 stefano   (1000) stefano   (1000)        7 2024-02-17 14:28:24.000000 cassio-0.1.5/src/cassio.egg-info/top_level.txt
+-rw-r--r--   0        0        0    11357 2023-05-19 09:38:04.396132 cassio-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2876 2024-04-18 12:49:42.988556 cassio-0.1.6/README.md
+-rw-r--r--   0        0        0     2050 2024-04-18 12:34:53.836026 cassio-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       58 2024-04-10 13:20:09.430203 cassio-0.1.6/src/cassio/__init__.py
+-rw-r--r--   0        0        0    14765 2024-04-10 13:56:55.786573 cassio-0.1.6/src/cassio/config/__init__.py
+-rw-r--r--   0        0        0     2513 2024-04-10 13:20:09.430203 cassio-0.1.6/src/cassio/config/bundle_download.py
+-rw-r--r--   0        0        0     5633 2024-04-10 13:20:09.430203 cassio-0.1.6/src/cassio/config/bundle_management.py
+-rw-r--r--   0        0        0      133 2024-04-10 13:20:09.430203 cassio-0.1.6/src/cassio/db_reader/__init__.py
+-rw-r--r--   0        0        0     9937 2024-04-10 13:20:09.430203 cassio-0.1.6/src/cassio/db_reader/multi_table_cassandra_reader.py
+-rw-r--r--   0        0        0       98 2024-04-10 13:20:09.430203 cassio-0.1.6/src/cassio/history/__init__.py
+-rw-r--r--   0        0        0     2394 2024-04-10 13:20:09.430203 cassio-0.1.6/src/cassio/history/stored_blob_history.py
+-rw-r--r--   0        0        0       69 2024-04-10 13:20:09.430203 cassio-0.1.6/src/cassio/keyvalue/__init__.py
+-rw-r--r--   0        0        0     2267 2024-04-10 13:20:09.430203 cassio-0.1.6/src/cassio/keyvalue/k_v_cache.py
+-rw-r--r--   0        0        0        0 2023-09-26 15:43:16.957372 cassio-0.1.6/src/cassio/py.typed
+-rw-r--r--   0        0        0     1230 2024-04-18 12:25:34.986580 cassio-0.1.6/src/cassio/table/__init__.py
+-rw-r--r--   0        0        0    20730 2024-04-18 12:25:34.986580 cassio-0.1.6/src/cassio/table/base_table.py
+-rw-r--r--   0        0        0     5393 2024-04-17 16:22:06.479524 cassio-0.1.6/src/cassio/table/cql.py
+-rw-r--r--   0        0        0      433 2024-04-17 16:22:06.479524 cassio-0.1.6/src/cassio/table/mixins/__init__.py
+-rw-r--r--   0        0        0      138 2024-04-17 16:22:06.479524 cassio-0.1.6/src/cassio/table/mixins/base_table.py
+-rw-r--r--   0        0        0     6531 2024-04-18 12:25:34.986580 cassio-0.1.6/src/cassio/table/mixins/clustered.py
+-rw-r--r--   0        0        0     2872 2024-04-17 16:22:06.479524 cassio-0.1.6/src/cassio/table/mixins/elastic_key.py
+-rw-r--r--   0        0        0    14450 2024-04-17 16:22:06.479524 cassio-0.1.6/src/cassio/table/mixins/metadata.py
+-rw-r--r--   0        0        0      777 2024-04-18 12:25:34.986580 cassio-0.1.6/src/cassio/table/mixins/type_normalizer.py
+-rw-r--r--   0        0        0     8622 2024-04-17 16:22:06.479524 cassio-0.1.6/src/cassio/table/mixins/vector.py
+-rw-r--r--   0        0        0     1806 2024-04-18 12:25:34.986580 cassio-0.1.6/src/cassio/table/table_types.py
+-rw-r--r--   0        0        0     2496 2024-04-17 16:22:06.479524 cassio-0.1.6/src/cassio/table/tables.py
+-rw-r--r--   0        0        0      674 2024-04-10 13:20:09.434203 cassio-0.1.6/src/cassio/table/utils.py
+-rw-r--r--   0        0        0       98 2024-04-10 13:20:09.434203 cassio-0.1.6/src/cassio/utils/__init__.py
+-rw-r--r--   0        0        0     1008 2024-04-10 13:20:09.434203 cassio-0.1.6/src/cassio/utils/db_inspection/__init__.py
+-rw-r--r--   0        0        0       80 2023-08-30 16:28:58.715340 cassio-0.1.6/src/cassio/utils/vector/__init__.py
+-rw-r--r--   0        0        0     2664 2024-04-10 13:20:09.434203 cassio-0.1.6/src/cassio/utils/vector/distance_metrics.py
+-rw-r--r--   0        0        0       78 2024-04-10 13:20:09.434203 cassio-0.1.6/src/cassio/vector/__init__.py
+-rw-r--r--   0        0        0     4365 2024-04-10 13:20:09.434203 cassio-0.1.6/src/cassio/vector/vector_table.py
+-rw-r--r--   0        0        0     4075 1970-01-01 00:00:00.000000 cassio-0.1.6/PKG-INFO
```

### Comparing `cassio-0.1.5/PKG-INFO` & `cassio-0.1.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: cassio
-Version: 0.1.5
+Version: 0.1.6
 Summary: A framework-agnostic Python library to seamlessly integrate Apache Cassandra(R) with ML/LLM/genAI workloads.
-Home-page: https://github.com/hemidactylus/cassio
+Home-page: https://cassio.org
+License: Apache-2.0
+Keywords: cassandra,ai,llm,genai,astradb
 Author: Stefano Lottini
 Author-email: stefano.lottini@datastax.com
-License: LICENSE.txt
-Keywords: cassandra,ai,llm,genai,astradb
-Platform: UNKNOWN
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8
+Requires-Dist: cassandra-driver (>=3.28.0,<4.0.0)
+Requires-Dist: numpy (>=1.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Project-URL: Repository, https://github.com/CassioML/cassio
 Description-Content-Type: text/markdown
 
 # cassIO
 
 A framework-agnostic Python library to seamlessly integrate Apache Cassandra with ML/LLM/genAI workloads.
 
 **Note**: this is currently an alpha release.
@@ -40,21 +43,27 @@
 For example usages and integration with higher-level LLM frameworks
 such as LangChain, please visit [cassio.org](https://cassio.org).
 
 ## CassIO developers
 
 ### Setup
 
-To develop `cassio`, use the `requirements-dev.txt`.
+To develop `cassio`, we use poetry
 
-To use the dev version in an integration (e.g. your branch of LangChain),
-`pip install -e .` in this `cassio` repo from within the virtual environment
-you are using to develop your integration.
+```shell
+pip install poetry
+```
+
+Use poetry to install dependencies
 
-#### Poetry
+```shell
+poetry install
+```
+
+#### Use cassio current code in other Poetry base projects
 
 If the integration is Poetry-based (e.g. LangChain itself), you should get this
 in your `pyproject.toml`:
 
 ```
 cassio = {path = "../../cassio", develop = true}
 ```
@@ -85,56 +94,54 @@
 
 At the moment we try to run tests under Python3.8 and Python3.10 to try and
 catch versions-specific issues
 (such as the newer `typing` syntax such as `typeA | typeB`, illegal on 3.8).
 
 ### Publishing
 
-- Bump version in setup.py
+- Bump version in pyproject.toml
 - Add to `CHANGES.txt`
 - Commit the very code that will be built:
 - `git tag v<x.y.z>; git push origin v<x.y.z>`
 
 ```
-rm dist/cassio*
 make build
-twine upload dist/cassio*  # (login to PyPI ...)
+poetry publish  # (login to PyPI ...)
 ```
 
 ### Testing
 
 Please run tests (and add some coverage for new features). This is not
 enforced other than to your conscience. Type `make` for the available tests.
 
 To run the full tests (except specific tests targeting Cassandra),
 there's `make test-all`.
 
 #### Unit testing
 
-You need a virtualenv with the `requirements-dev.txt` installed.
-
 ```
 make test-unit
 ```
 
 #### Integration with the DB
 
-You need a virtualenv with the `requirements-dev.txt` installed.
-
 Ensure the required environment variables are set (see for instance
 the provided `TEMPLATE.testing.env`).
 You need at least one of either Astra DB or a
 Cassandra (5+) cluster to use.
 
 Launch the tests with either of:
 
 ```
 make test-integration
+
 make test-astra-integration
 make test-cassandra-integration
+make test-testcontainerscassandra-integration
 ```
 
-The latter two above specify `TEST_DB_MODE` as either `LOCAL_CASSANDRA` or
-`ASTRA_DB`. _Ideally you should test with both, since some tests are
-skipped in either case._
+The last three above specify `TEST_DB_MODE` as either `LOCAL_CASSANDRA`, `TESTCONTAINERS_CASSANDRA` or
+`ASTRA_DB`. Refer to `TEMPLATE.testing.env` for required environment variables in the specific cases.
 
+_Note: Ideally you should test with both Astra DB and one Cassandra, since some tests are
+skipped in either case._
```

### Comparing `cassio-0.1.5/README.md` & `cassio-0.1.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -15,21 +15,27 @@
 For example usages and integration with higher-level LLM frameworks
 such as LangChain, please visit [cassio.org](https://cassio.org).
 
 ## CassIO developers
 
 ### Setup
 
-To develop `cassio`, use the `requirements-dev.txt`.
+To develop `cassio`, we use poetry
 
-To use the dev version in an integration (e.g. your branch of LangChain),
-`pip install -e .` in this `cassio` repo from within the virtual environment
-you are using to develop your integration.
+```shell
+pip install poetry
+```
+
+Use poetry to install dependencies
+
+```shell
+poetry install
+```
 
-#### Poetry
+#### Use cassio current code in other Poetry base projects
 
 If the integration is Poetry-based (e.g. LangChain itself), you should get this
 in your `pyproject.toml`:
 
 ```
 cassio = {path = "../../cassio", develop = true}
 ```
@@ -60,54 +66,53 @@
 
 At the moment we try to run tests under Python3.8 and Python3.10 to try and
 catch versions-specific issues
 (such as the newer `typing` syntax such as `typeA | typeB`, illegal on 3.8).
 
 ### Publishing
 
-- Bump version in setup.py
+- Bump version in pyproject.toml
 - Add to `CHANGES.txt`
 - Commit the very code that will be built:
 - `git tag v<x.y.z>; git push origin v<x.y.z>`
 
 ```
-rm dist/cassio*
 make build
-twine upload dist/cassio*  # (login to PyPI ...)
+poetry publish  # (login to PyPI ...)
 ```
 
 ### Testing
 
 Please run tests (and add some coverage for new features). This is not
 enforced other than to your conscience. Type `make` for the available tests.
 
 To run the full tests (except specific tests targeting Cassandra),
 there's `make test-all`.
 
 #### Unit testing
 
-You need a virtualenv with the `requirements-dev.txt` installed.
-
 ```
 make test-unit
 ```
 
 #### Integration with the DB
 
-You need a virtualenv with the `requirements-dev.txt` installed.
-
 Ensure the required environment variables are set (see for instance
 the provided `TEMPLATE.testing.env`).
 You need at least one of either Astra DB or a
 Cassandra (5+) cluster to use.
 
 Launch the tests with either of:
 
 ```
 make test-integration
+
 make test-astra-integration
 make test-cassandra-integration
+make test-testcontainerscassandra-integration
 ```
 
-The latter two above specify `TEST_DB_MODE` as either `LOCAL_CASSANDRA` or
-`ASTRA_DB`. _Ideally you should test with both, since some tests are
+The last three above specify `TEST_DB_MODE` as either `LOCAL_CASSANDRA`, `TESTCONTAINERS_CASSANDRA` or
+`ASTRA_DB`. Refer to `TEMPLATE.testing.env` for required environment variables in the specific cases.
+
+_Note: Ideally you should test with both Astra DB and one Cassandra, since some tests are
 skipped in either case._
```

### Comparing `cassio-0.1.5/src/cassio/config/__init__.py` & `cassio-0.1.6/src/cassio/config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import tempfile
 import shutil
 import os
 from typing import Any, Dict, List, Optional, Union
 
-from cassandra.cluster import Cluster, Session  # type: ignore
-from cassandra.auth import PlainTextAuthProvider  # type: ignore
+from cassandra.cluster import Cluster, Session
+from cassandra.auth import PlainTextAuthProvider
 
 from cassio.config.bundle_management import (
     init_string_to_bundle_path_and_options,
     infer_keyspace_from_bundle,
 )
 from cassio.config.bundle_download import download_astra_bundle_url
 
-
 ASTRA_CLOUD_AUTH_USERNAME = "token"
 DOWNLOADED_BUNDLE_FILE_NAME = "secure-connect-bundle_devopsapi.zip"
 
 default_session: Optional[Session] = None
 default_keyspace: Optional[str] = None
 
 
@@ -30,14 +29,15 @@
     keyspace: Optional[str] = None,
     contact_points: Optional[Union[str, List[str]]] = None,
     username: Optional[str] = None,
     password: Optional[str] = None,
     cluster_kwargs: Optional[Dict[str, Any]] = None,
     tempfile_basedir: Optional[str] = None,
     bundle_url_template: Optional[str] = None,
+    cloud_kwargs: Optional[Dict[str, Any]] = None,
 ) -> None:
     """
     Globally set the default Cassandra connection (/keyspace) for CassIO.
     This default will be used by all other db-requiring CassIO instantiations,
     unless passed to the respective classes' __init__.
 
     There are various ways to achieve this, depending on the passed parameters.
@@ -88,14 +88,16 @@
         `password` (optional str), password for Cassandra connection
         `cluster_kwargs` (optional dict), additional arguments to `Cluster(...)`.
         `tempfile_basedir` (optional str), where to create temporary work directories.
         `bundle_url_template` (optional str), url template for getting the database
             secure bundle. The "databaseId" variable is resolved with the actual value.
             Default (for Astra DB):
                 "https://api.astra.datastax.com/v2/databases/{database_id}/secureBundleURL"
+        `cloud_kwargs` (optional dict), additional arguments to `Cluster(cloud={...})`
+            (i.e. additional key-value pairs within the passed `cloud` dict).
 
     ASTRA DB:
     The Astra-related parameters are arranged in a chain of fallbacks.
     In case redundant information is supplied, these are the precedences:
         session > secure_connect_bundle > init_string
         token > (from init_string if any)
         keyspace > (from init_string if any) > (from bundle if any)
@@ -132,18 +134,24 @@
                 init_string,
                 token,
                 database_id,
                 keyspace,
                 contact_points,
                 username,
                 password,
-                cluster_kwargs,
+                # cluster_kwargs is allowed
+                # tempfile_basedir is allowed
+                bundle_url_template,
+                cloud_kwargs,
             )
         ):
-            raise ValueError("When auto=True, no arguments can be passed.")
+            raise ValueError(
+                "When auto=True, no arguments can be passed other than "
+                "tempfile_basedir and cluster_kwargs."
+            )
         # setting some arguments from environment variables
         if "CASSANDRA_CONTACT_POINTS" in os.environ:
             contact_points = os.environ["CASSANDRA_CONTACT_POINTS"]
             username = os.environ.get("CASSANDRA_USERNAME")
             password = os.environ.get("CASSANDRA_PASSWORD")
             keyspace = os.environ.get("CASSANDRA_KEYSPACE")
         elif any(
@@ -237,21 +245,21 @@
                         )
                     else:
                         chosen_auth_provider = None
                 #
                 if chosen_contact_points is None:
                     cluster = Cluster(
                         auth_provider=chosen_auth_provider,
-                        **(cluster_kwargs if cluster_kwargs is not None else {})
+                        **(cluster_kwargs if cluster_kwargs is not None else {}),
                     )
                 else:
                     cluster = Cluster(
                         contact_points=chosen_contact_points,
                         auth_provider=chosen_auth_provider,
-                        **(cluster_kwargs if cluster_kwargs is not None else {})
+                        **(cluster_kwargs if cluster_kwargs is not None else {}),
                     )
                 default_session = cluster.connect()
             elif is_astra_db:
                 # Astra DB
                 chosen_token = _first_valid(token_from_arg, token_from_is)
                 if chosen_token is None:
                     raise ValueError(
@@ -281,20 +289,23 @@
                 chosen_bundle = _first_valid(
                     bundle_from_download, chosen_bundle_pre_token
                 )
                 #
                 if chosen_bundle:
                     keyspace_from_bundle = infer_keyspace_from_bundle(chosen_bundle)
                     cluster = Cluster(
-                        cloud={"secure_connect_bundle": chosen_bundle},
+                        cloud={
+                            "secure_connect_bundle": chosen_bundle,
+                            **(cloud_kwargs if cloud_kwargs is not None else {}),
+                        },
                         auth_provider=PlainTextAuthProvider(
                             ASTRA_CLOUD_AUTH_USERNAME,
                             chosen_token,
                         ),
-                        **(cluster_kwargs if cluster_kwargs is not None else {})
+                        **(cluster_kwargs if cluster_kwargs is not None else {}),
                     )
                     default_session = cluster.connect()
                 else:
                     raise ValueError("No secure-connect-bundle was available.")
         # keyspace to be resolved in any case
         chosen_keyspace = _first_valid(
             keyspace_from_arg, keyspace_from_is, keyspace_from_bundle
```

### Comparing `cassio-0.1.5/src/cassio/config/bundle_download.py` & `cassio-0.1.6/src/cassio/config/bundle_download.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Facilities to manage the download of a secure-connect-bundle from an Astra DB
 token.
 """
 import logging
-import requests  # type: ignore
+import requests
 from typing import Optional
 
 
 DEFAULT_GET_BUNDLE_URL_TEMPLATE = (
     "https://api.astra.datastax.com/v2/databases/{database_id}/secureBundleURL"
 )
 
@@ -48,15 +48,15 @@
             ):
                 raise ValueError("Invalid or insufficient token.")
             else:
                 raise ValueError(
                     "Generic error when fetching the URL to the secure-bundle."
                 )
         else:
-            return response_json["downloadURL"]
+            return str(response_json["downloadURL"])
     else:
         raise ValueError(
             "Cannot get the secure-bundle URL. "
             "Check the provided database_id and token."
         )
```

### Comparing `cassio-0.1.5/src/cassio/config/bundle_management.py` & `cassio-0.1.6/src/cassio/config/bundle_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 USED_CONFIG_KEYS_AND_DEFAULTS = {
     "caCertLocation": "./ca.crt",
     "keyLocation": "./key",
     "certLocation": "./cert",
 }
 
 
-def encode_str(sng):
+def encode_str(sng: str) -> str:
     return base64.b64encode(sng.encode()).decode()
 
 
-def decode_str(b64):
+def decode_str(b64: str) -> str:
     return base64.b64decode(b64).decode()
 
 
 def _encode_from_string(s: str) -> str:
     return encode_str(s)
 
 
@@ -53,15 +53,15 @@
     """
     if bundle_path:
         try:
             bundle_zip = ZipFile(bundle_path)
             open_config = bundle_zip.open("config.json")
             ascii_lines = [line.decode() for line in open_config.readlines()]
             config = json.loads("".join(ascii_lines))
-            return config.get("keyspace")
+            return str(config["keyspace"]) if "keyspace" in config else None
         except Exception:
             return None
     else:
         return None
 
 
 def bundle_path_to_init_string(
@@ -143,15 +143,15 @@
             for f_name, f_contents in bundle_data.items():
                 bundle_zip_file.writestr(f_name, data=f_contents)
         return bundle_filepath, options_dict
     else:
         raise ValueError(f"Init string has unsupported or unknown version {version}.")
 
 
-def create_init_string_utility():
+def create_init_string_utility() -> None:
     # Utility command-line: converts the full bundle path (argument)
     # to an "init string" and prints it as an export line
     import sys
 
     if sys.argv[1:] == [] or len(sys.argv) > 4:
         cmd = sys.argv[0]
         print(f"Usage: {cmd} bundle_path [keyspace [token]]")
```

### Comparing `cassio-0.1.5/src/cassio/db_reader/multi_table_cassandra_reader.py` & `cassio-0.1.6/src/cassio/db_reader/multi_table_cassandra_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     Optional,
     Set,
     Tuple,
     TypeVar,
     Union,
 )
 
-from cassandra.query import PreparedStatement  # type: ignore
-from cassandra.concurrent import execute_concurrent, ExecutionResult  # type: ignore
+from cassandra.query import PreparedStatement
+from cassandra.concurrent import execute_concurrent, ExecutionResult
 
 from cassio.utils.db_inspection import table_partitionkey
 from cassio.config import check_resolve_session, check_resolve_keyspace
 from cassio.table.cql import SELECT_CQL_TEMPLATE
 from cassio.table.table_types import SessionType
 
 
@@ -199,14 +199,15 @@
             ).format(table_fqname=f"{self.keyspace}.{table_name}")
             for table_name, column_name_set in self.columns_by_table.items()
         }
         self.query_statements: Dict[str, PreparedStatement] = {
             table_name: self.session.prepare(cql_statement)
             for table_name, cql_statement in query_cql_map.items()
         }
+
         # reduction across all tables to all primary-key values needed
         # (this merger function makes the type checker happy over a lambda)
         def _set_merger(s1: Iterable[str], s2: Iterable[str]) -> Set[str]:
             return {itm for s in (s1, s2) for itm in s}
 
         self.input_parameters: Set[str] = reduce(
             _set_merger,
```

### Comparing `cassio-0.1.5/src/cassio/history/stored_blob_history.py` & `cassio-0.1.6/src/cassio/history/stored_blob_history.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 by some 'session id'. Overwrites are not supported by design.
 """
 
 import uuid
 from warnings import warn
 from typing import Any, Iterable, Optional
 
-from cassandra.cluster import Session  # type: ignore
+from cassandra.cluster import Session
 
 from cassio.table.tables import ClusteredCassandraTable
 
 
 class StoredBlobHistory:
     """
     This class is a rewriting of the StoredBlobHistory created for use in LangChain
```

### Comparing `cassio-0.1.5/src/cassio/keyvalue/k_v_cache.py` & `cassio-0.1.6/src/cassio/keyvalue/k_v_cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 handling of key-value storage on a Cassandra table.
 One row per partition, serializes a multiple partition key into a string
 """
 
 from warnings import warn
 from typing import Any, cast, Dict, List, Optional
 
-from cassandra.cluster import Session  # type: ignore
+from cassandra.cluster import Session
 
 from cassio.table.tables import ElasticCassandraTable
 
 
 class KVCache:
     """
     This class is a rewriting of the KVCache created for use in LangChain
```

### Comparing `cassio-0.1.5/src/cassio/table/__init__.py` & `cassio-0.1.6/src/cassio/table/__init__.py`

 * *Files identical despite different names*

### Comparing `cassio-0.1.5/src/cassio/table/base_table.py` & `cassio-0.1.6/src/cassio/table/base_table.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import asyncio
+import json
 from asyncio import InvalidStateError, Task
 import logging
 from typing import (
     Any,
     cast,
     Dict,
     List,
     Iterable,
     Optional,
     Set,
     Tuple,
     Union,
 )
 
-from cassandra.query import SimpleStatement, PreparedStatement  # type: ignore
-from cassandra.cluster import ResultSet  # type: ignore
-from cassandra.cluster import ResponseFuture  # type: ignore
+from cassandra.query import SimpleStatement, PreparedStatement
+from cassandra.cluster import ResultSet
+from cassandra.cluster import ResponseFuture
 
 from cassio.config import check_resolve_session, check_resolve_keyspace
 from cassio.table.table_types import (
     ColumnSpecType,
     RowType,
     SessionType,
     normalize_type_desc,
@@ -27,14 +28,15 @@
 from cassio.table.cql import (
     CQLOpType,
     CREATE_TABLE_CQL_TEMPLATE,
     TRUNCATE_TABLE_CQL_TEMPLATE,
     DELETE_CQL_TEMPLATE,
     SELECT_CQL_TEMPLATE,
     INSERT_ROW_CQL_TEMPLATE,
+    CREATE_INDEX_CQL_TEMPLATE,
 )
 from cassio.table.utils import call_wrapped_async
 
 
 class CustomLogger(logging.Logger):
     def trace(self, msg: str, *args: Any, **kwargs: Any) -> None:
         if self.isEnabledFor(5):
@@ -58,22 +60,24 @@
         table: str,
         session: Optional[SessionType] = None,
         keyspace: Optional[str] = None,
         ttl_seconds: Optional[int] = None,
         row_id_type: Union[str, List[str]] = ["TEXT"],
         skip_provisioning: bool = False,
         async_setup: bool = False,
+        body_index_options: Optional[List[Tuple[str, Any]]] = None,
     ) -> None:
         self.session = check_resolve_session(session)
         self.keyspace = check_resolve_keyspace(keyspace)
         self.table = table
         self.ttl_seconds = ttl_seconds
         self.row_id_type = normalize_type_desc(row_id_type)
         self.skip_provisioning = skip_provisioning
         self._prepared_statements: Dict[str, PreparedStatement] = {}
+        self._body_index_options = body_index_options
         self.db_setup_task: Optional[Task[None]] = None
         if async_setup:
             self.db_setup_task = asyncio.create_task(self.adb_setup())
         else:
             self.db_setup()
 
     def _schema_row_id(self) -> List[ColumnSpecType]:
@@ -89,21 +93,31 @@
         return []
 
     def _schema_da(self) -> List[ColumnSpecType]:
         return [
             ("body_blob", "TEXT"),
         ]
 
+    async def _aschema_da(self) -> List[ColumnSpecType]:
+        return self._schema_da()
+
     def _schema(self) -> Dict[str, List[ColumnSpecType]]:
         return {
             "pk": self._schema_pk(),
             "cc": self._schema_cc(),
             "da": self._schema_da(),
         }
 
+    async def _aschema(self) -> Dict[str, List[ColumnSpecType]]:
+        return {
+            "pk": self._schema_pk(),
+            "cc": self._schema_cc(),
+            "da": await self._aschema_da(),
+        }
+
     def _schema_primary_key(self) -> List[ColumnSpecType]:
         return self._schema_pk() + self._schema_cc()
 
     def _schema_collist(self) -> List[ColumnSpecType]:
         full_list = self._schema_da() + self._schema_cc() + self._schema_pk()
         return full_list
 
@@ -206,14 +220,42 @@
         self._ensure_db_setup()
         return self._clear(is_async=True)
 
     async def aclear(self) -> None:
         await self._aensure_db_setup()
         await call_wrapped_async(self.clear_async)
 
+    def _has_index_analyzers(self) -> bool:
+        if not self._body_index_options:
+            return False
+        for option in self._body_index_options:
+            if option[0] == "index_analyzer":
+                return True
+        return False
+
+    def _extract_index_analyzers(
+        self, args_dict: Any
+    ) -> Tuple[Any, List[str], Tuple[Any, ...]]:
+        rest_args = args_dict.copy()
+        where_clause_blocks: List[str] = []
+        where_clause_vals: List[Any] = []
+        if "body_search" in args_dict:
+            if not self._has_index_analyzers():
+                raise ValueError(
+                    "Cannot do body search because no index analyzer "
+                    "was configured on the table"
+                )
+            body_search_texts = rest_args.pop("body_search")
+            if not isinstance(body_search_texts, list):
+                body_search_texts = [body_search_texts]
+            for text in body_search_texts:
+                where_clause_blocks.append("body_blob : %s")
+                where_clause_vals.append(text)
+        return rest_args, where_clause_blocks, tuple(where_clause_vals)
+
     def _parse_select_core_params(
         self, **kwargs: Any
     ) -> Tuple[str, str, Tuple[Any, ...]]:
         n_kwargs = self._normalize_kwargs(kwargs)
         # TODO: work on a columns: Optional[List[str]] = None
         # (but with nuanced handling of the column-magic we have here)
         columns = None
@@ -225,17 +267,29 @@
             raise NotImplementedError("Column selection is not implemented.")
         #
         (
             rest_kwargs,
             where_clause_blocks,
             select_cql_vals,
         ) = self._extract_where_clause_blocks(n_kwargs)
+
+        (
+            rest_kwargs,
+            analyzer_clause_blocks,
+            analyzer_cql_vals,
+        ) = self._extract_index_analyzers(rest_kwargs)
+
         assert rest_kwargs == {}
-        where_clause = "WHERE " + " AND ".join(where_clause_blocks)
-        return columns_desc, where_clause, select_cql_vals
+
+        all_where_clauses = where_clause_blocks + analyzer_clause_blocks
+        if not all_where_clauses:
+            where_clause = ""
+        else:
+            where_clause = "WHERE " + " AND ".join(all_where_clauses)
+        return columns_desc, where_clause, select_cql_vals + analyzer_cql_vals
 
     def _get_select_cql(self, **kwargs: Any) -> Tuple[str, Tuple[Any, ...]]:
         columns_desc, where_clause, get_cql_vals = self._parse_select_core_params(
             **kwargs
         )
         limit_clause = ""
         limit_cql_vals: List[Any] = []
@@ -325,46 +379,101 @@
         self._ensure_db_setup()
         return self._put(is_async=True, **kwargs)
 
     async def aput(self, **kwargs: Any) -> None:
         await self._aensure_db_setup()
         await call_wrapped_async(self.put_async, **kwargs)
 
-    def _get_db_setup_cql(self) -> str:
-        _schema = self._schema()
+    def _get_db_setup_cql(self, schema: Dict[str, List[ColumnSpecType]]) -> str:
         column_specs = [
             f"{col_spec[0]} {col_spec[1]}"
             for _schema_grp in ["pk", "cc", "da"]
-            for col_spec in _schema[_schema_grp]
+            for col_spec in schema[_schema_grp]
         ]
-        pk_spec = ", ".join(col for col, _ in _schema["pk"])
-        cc_spec = ", ".join(col for col, _ in _schema["cc"])
-        primkey_spec = f"( ( {pk_spec} ) {',' if _schema['cc'] else ''} {cc_spec} )"
-        if _schema["cc"]:
+        pk_spec = ", ".join(col for col, _ in schema["pk"])
+        cc_spec = ", ".join(col for col, _ in schema["cc"])
+        primkey_spec = f"( ( {pk_spec} ) {',' if schema['cc'] else ''} {cc_spec} )"
+        if schema["cc"]:
             clu_core = ", ".join(
-                f"{col} {self.ordering_in_partition}" for col, _ in _schema["cc"]
+                f"{col} {self.ordering_in_partition}" for col, _ in schema["cc"]
             )
             clustering_spec = f"WITH CLUSTERING ORDER BY ({clu_core})"
         else:
             clustering_spec = ""
         #
         create_table_cql = CREATE_TABLE_CQL_TEMPLATE.format(
             columns_spec=" ".join(f"  {cs}," for cs in column_specs),
             primkey_spec=primkey_spec,
             clustering_spec=clustering_spec,
         )
         return create_table_cql
 
+    @staticmethod
+    def _get_create_index_cql(
+        index_name: str, index_column: str, index_options: List[Tuple[str, Any]]
+    ) -> str:
+        options_clause = ""
+        if len(index_options) > 0:
+            formatted_options = []
+            for option in index_options:
+                key, value = option
+                if isinstance(value, dict):
+                    formatted_options.append(f"'{key}': '{json.dumps(value)}'")
+                elif isinstance(value, str):
+                    formatted_options.append(f"'{key}': '{value}'")
+                elif isinstance(value, bool):
+                    if value:
+                        formatted_options.append(f"'{key}': true")
+                    else:
+                        formatted_options.append(f"'{key}': false")
+                else:
+                    raise ValueError("Unsupported index_option format")
+
+            formatted_options.sort()
+
+            options_text = ", ".join(formatted_options)
+
+            # this is double escaped because the cql will go through
+            # another format method before being executed
+            options_clause = f"WITH OPTIONS = {{{{ {options_text} }}}}"
+
+        return CREATE_INDEX_CQL_TEMPLATE.format(
+            index_name=index_name,
+            index_column=index_column,
+            options_clause=options_clause,
+        )
+
+    @staticmethod
+    def _get_create_analyzer_index_cql(index_options: List[Tuple[str, Any]]) -> str:
+        index_name = "idx_body"
+        index_column = "body_blob"
+        return BaseTable._get_create_index_cql(
+            index_name=index_name,
+            index_column=index_column,
+            index_options=index_options,
+        )
+
     def db_setup(self) -> None:
-        create_table_cql = self._get_db_setup_cql()
+        create_table_cql = self._get_db_setup_cql(self._schema())
         self.execute_cql(create_table_cql, op_type=CQLOpType.SCHEMA)
+        if self._body_index_options:
+            self.execute_cql(
+                self._get_create_analyzer_index_cql(self._body_index_options),
+                op_type=CQLOpType.SCHEMA,
+            )
 
     async def adb_setup(self) -> None:
-        create_table_cql = self._get_db_setup_cql()
+        schema = await self._aschema()
+        create_table_cql = self._get_db_setup_cql(schema)
         await self.aexecute_cql(create_table_cql, op_type=CQLOpType.SCHEMA)
+        if self._body_index_options:
+            await self.aexecute_cql(
+                self._get_create_analyzer_index_cql(self._body_index_options),
+                op_type=CQLOpType.SCHEMA,
+            )
 
     def _ensure_db_setup(self) -> None:
         if self.db_setup_task:
             try:
                 self.db_setup_task.result()
             except InvalidStateError:
                 raise ValueError(
```

### Comparing `cassio-0.1.5/src/cassio/table/cql.py` & `cassio-0.1.6/src/cassio/table/cql.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, List, Tuple, Union
 from enum import Enum
 
-from cassandra.query import SimpleStatement, PreparedStatement  # type: ignore
+from cassandra.query import SimpleStatement, PreparedStatement
 
 
 class CQLOpType(Enum):
     SCHEMA = 1
     WRITE = 2
     READ = 3
 
@@ -18,47 +18,60 @@
 
 SELECT_CQL_TEMPLATE = (
     """SELECT {columns_desc} FROM {{table_fqname}} {where_clause} {limit_clause};"""
 )
 
 INSERT_ROW_CQL_TEMPLATE = """INSERT INTO {{table_fqname}} ({columns_desc}) VALUES ({value_placeholders}) {ttl_spec} ;"""  # noqa: E501
 
-CREATE_INDEX_CQL_TEMPLATE = """CREATE CUSTOM INDEX IF NOT EXISTS {index_name}_{{table_name}} ON {{table_fqname}} ({index_column}) USING 'org.apache.cassandra.index.sai.StorageAttachedIndex';"""  # noqa: E501
+CREATE_INDEX_CQL_PREFIX = "CREATE CUSTOM INDEX IF NOT EXISTS {index_name}_{{table_name}} ON {{table_fqname}} "  # noqa: E501
 
-CREATE_KEYS_INDEX_CQL_TEMPLATE = """CREATE CUSTOM INDEX IF NOT EXISTS {index_name}_{{table_name}} ON {{table_fqname}} (KEYS({index_column})) USING 'org.apache.cassandra.index.sai.StorageAttachedIndex';"""  # noqa: E501
+CREATE_INDEX_CQL_TEMPLATE = (
+    CREATE_INDEX_CQL_PREFIX
+    + "({index_column}) USING 'org.apache.cassandra.index.sai.StorageAttachedIndex' {options_clause};"  # noqa: E501
+)
+
+CREATE_KEYS_INDEX_CQL_TEMPLATE = (
+    CREATE_INDEX_CQL_PREFIX
+    + "(KEYS({index_column})) USING 'org.apache.cassandra.index.sai.StorageAttachedIndex';"  # noqa: E501
+)
 
-CREATE_ENTRIES_INDEX_CQL_TEMPLATE = """CREATE CUSTOM INDEX IF NOT EXISTS {index_name}_{{table_name}} ON {{table_fqname}} (ENTRIES({index_column})) USING 'org.apache.cassandra.index.sai.StorageAttachedIndex';"""  # noqa: E501
+CREATE_ENTRIES_INDEX_CQL_TEMPLATE = (
+    CREATE_INDEX_CQL_PREFIX
+    + "(ENTRIES({index_column})) USING 'org.apache.cassandra.index.sai.StorageAttachedIndex';"  # noqa: E501
+    ""
+)
 
 SELECT_ANN_CQL_TEMPLATE = """SELECT {columns_desc} FROM {{table_fqname}} {where_clause} ORDER BY {vector_column} ANN OF %s {limit_clause};"""  # noqa: E501
 
 CQLStatementType = Union[str, SimpleStatement, PreparedStatement]
 StatementWithArgs = Tuple[CQLStatementType, Tuple[Any, ...]]
 StatementStrWithArgs = Tuple[str, Tuple[Any, ...]]
 
+
 # Mock DB session
 class MockDBSession:
     def __init__(self, verbose: bool = False):
         self.verbose = verbose
         self.statements: List[StatementWithArgs] = []
 
     @staticmethod
-    def getStatementBody(statement: CQLStatementType) -> str:
+    def get_statement_body(statement: CQLStatementType) -> str:
         if isinstance(statement, str):
             _statement = statement
         elif isinstance(statement, SimpleStatement):
             _statement = statement.query_string
         elif isinstance(statement, PreparedStatement):
             _statement = statement.query_string
         else:
             raise ValueError()
         return _statement
 
     @staticmethod
-    def normalizeCQLStatement(statement: CQLStatementType) -> str:
-        _statement = MockDBSession.getStatementBody(statement)
+    def normalize_cql_statement(statement: CQLStatementType) -> str:
+        _statement = MockDBSession.get_statement_body(statement)
         _s = (
             _statement.replace(";", " ")
             .replace("%s", " %s ")
             .replace("?", " ? ")
             .replace("=", " = ")
             .replace(")", " ) ")
             .replace("(", " ( ")
@@ -74,15 +87,15 @@
         return PreparedStatement(None, 0, 0, statement, "keyspace", None, None, None)
 
     def execute(
         self, statement: CQLStatementType, arguments: Tuple[Any, ...] = tuple()
     ) -> List[Any]:
         if self.verbose:
             #
-            st_body = self.getStatementBody(statement)
+            st_body = self.get_statement_body(statement)
             if isinstance(statement, str):
                 st_type = "STR"
                 placeholder_count = st_body.count("%s")
                 assert "?" not in st_body
             elif isinstance(statement, SimpleStatement):
                 st_type = "SIM"
                 placeholder_count = st_body.count("%s")
@@ -106,25 +119,31 @@
             return []
         else:
             return self.statements[-n:]
 
     def last(self, n: int) -> List[StatementStrWithArgs]:
         return [
             (
-                self.normalizeCQLStatement(stmt),
+                self.normalize_cql_statement(stmt),
                 data,
             )
             for stmt, data in self.last_raw(n)
         ]
 
     def assert_last_equal(
         self, expected_statements: List[StatementStrWithArgs]
     ) -> None:
         # used for testing
         last_executed = self.last(len(expected_statements))
         assert len(last_executed) == len(expected_statements)
         for s_exe, s_expe in zip(last_executed, expected_statements):
             assert s_exe[1] == s_expe[1], f"EXE#{str(s_exe[1])}# != EXPE#{s_expe[1]}#"
-            exe_cql = self.normalizeCQLStatement(s_exe[0])
-            expe_cql = self.normalizeCQLStatement(s_expe[0])
+            exe_cql = self.normalize_cql_statement(s_exe[0])
+            expe_cql = self.normalize_cql_statement(s_expe[0])
             assert exe_cql == expe_cql, f"EXE#{exe_cql}# != EXPE#{expe_cql}#"
         return None
+
+
+STANDARD_ANALYZER = ("index_analyzer", "STANDARD")
+LOWER_CASE_ANALYZER = ("case_sensitive", False)
+NORMALIZE_ANALYZER = ("normalize", True)
+ASCII_ANALYZER = ("ascii", True)
```

### Comparing `cassio-0.1.5/src/cassio/table/table_types.py` & `cassio-0.1.6/src/cassio/table/table_types.py`

 * *Files identical despite different names*

### Comparing `cassio-0.1.5/src/cassio/table/tables.py` & `cassio-0.1.6/src/cassio/table/tables.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from cassio.table.base_table import BaseTable
-from cassio.table.mixins import (
-    ClusteredMixin,
-    MetadataMixin,
-    VectorMixin,
-    ElasticKeyMixin,
-    #
-    TypeNormalizerMixin,
-)
+from cassio.table.mixins.clustered import ClusteredMixin
+from cassio.table.mixins.metadata import MetadataMixin
+from cassio.table.mixins.vector import VectorMixin
+from cassio.table.mixins.elastic_key import ElasticKeyMixin
+from cassio.table.mixins.type_normalizer import TypeNormalizerMixin
 
 
 class PlainCassandraTable(TypeNormalizerMixin, BaseTable):
     pass
 
 
 class ClusteredCassandraTable(TypeNormalizerMixin, ClusteredMixin, BaseTable):
```

### Comparing `cassio-0.1.5/src/cassio/table/utils.py` & `cassio-0.1.6/src/cassio/table/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 from typing import Callable, Any
 
-from cassandra.cluster import ResponseFuture  # type: ignore
+from cassandra.cluster import ResponseFuture
 
 
 async def call_wrapped_async(
     func: Callable[..., ResponseFuture], *args: Any, **kwargs: Any
 ) -> Any:
     loop = asyncio.get_event_loop()
     asyncio_future = loop.create_future()
```

### Comparing `cassio-0.1.5/src/cassio/utils/db_inspection/__init__.py` & `cassio-0.1.6/src/cassio/utils/db_inspection/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Inspection of a keyspace and its tables through metadata in the Session object.
 """
 
 from typing import Iterable, Tuple
 
-from cassandra.cluster import Session  # type: ignore
+from cassandra.cluster import Session
 
 ColumnType = Tuple[str, str]
 
 
 def table_primarykey(
     session: Session, keyspace: str, table: str
 ) -> Iterable[ColumnType]:
```

### Comparing `cassio-0.1.5/src/cassio/utils/vector/distance_metrics.py` & `cassio-0.1.6/src/cassio/utils/vector/distance_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List, Dict, Tuple, Callable
 
 import numpy as np
 
 VectorType = List[float]
 
+
 # distance definitions. These all work batched in the first argument.
 def distance_dot_product(
     embedding_vectors: List[VectorType], reference_embedding_vector: VectorType
 ) -> List[float]:
     """
     Given a list [emb_i] and a reference rEmb vector,
     return a list [distance_i] where each distance is
```

### Comparing `cassio-0.1.5/src/cassio/vector/vector_table.py` & `cassio-0.1.6/src/cassio/vector/vector_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 Note: This is to be replaced by direct usage of the table-class-hierarchy classes.
 """
 
 from warnings import warn
 from typing import List, Dict, Any, Optional
 
-from cassandra.cluster import ResponseFuture  # type: ignore
+from cassandra.cluster import ResponseFuture
 
 from cassio.table.table_types import RowType
 from cassio.table.tables import (
     MetadataVectorCassandraTable,
 )
 
 new_columns_to_legacy = {
@@ -87,15 +87,15 @@
         return [self._make_dict_legacy(rich_hit) for rich_hit in enriched_hits]
 
     def put(
         self,
         document: str,
         embedding_vector: List[float],
         document_id: Any,
-        metadata: Dict[str, Any] = {},
+        metadata: Optional[Dict[str, Any]] = None,
         ttl_seconds: Optional[int] = None,
         **kwargs: Any,
     ) -> None:
         self.table.put(
             row_id=document_id,
             body_blob=document,
             vector=embedding_vector,
@@ -105,16 +105,16 @@
         )
 
     def put_async(
         self,
         document: str,
         embedding_vector: List[float],
         document_id: Any,
-        metadata: Dict[str, Any],
-        ttl_seconds: int,
+        metadata: Optional[Dict[str, Any]] = None,
+        ttl_seconds: Optional[int] = None,
         **kwargs: Any,
     ) -> ResponseFuture:
         return self.table.put_async(
             row_id=document_id,
             body_blob=document,
             vector=embedding_vector,
             metadata=metadata or {},
```

