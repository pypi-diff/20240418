# Comparing `tmp/nci_cidc_api_modules-1.0.5.tar.gz` & `tmp/nci_cidc_api_modules-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nci_cidc_api_modules-1.0.5.tar", last modified: Fri Apr 12 17:00:18 2024, max compression
+gzip compressed data, was "nci_cidc_api_modules-1.0.6.tar", last modified: Thu Apr 18 15:13:23 2024, max compression
```

## Comparing `nci_cidc_api_modules-1.0.5.tar` & `nci_cidc_api_modules-1.0.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:00:18.276310 nci_cidc_api_modules-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    40323 2024-04-12 17:00:18.276310 nci_cidc_api_modules-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    39309 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:00:18.264310 nci_cidc_api_modules-1.0.5/cidc_api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:00:18.268309 nci_cidc_api_modules-1.0.5/cidc_api/config/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/config/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/config/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/config/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/config/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:00:18.272310 nci_cidc_api_modules-1.0.5/cidc_api/csms/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/csms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/csms/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:00:18.272310 nci_cidc_api_modules-1.0.5/cidc_api/models/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31664 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/models/csms_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:00:18.272310 nci_cidc_api_modules-1.0.5/cidc_api/models/files/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/models/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    62309 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/models/files/details.py
--rw-r--r--   0 runner    (1001) docker     (127)    29172 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/models/files/facets.py
--rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/models/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)   120820 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/models/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/models/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:00:18.276310 nci_cidc_api_modules-1.0.5/cidc_api/shared/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11647 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/shared/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/shared/emails.py
--rw-r--r--   0 runner    (1001) docker     (127)    33746 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/shared/gcloud_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/cidc_api/shared/rest_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:00:18.276310 nci_cidc_api_modules-1.0.5/nci_cidc_api_modules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    40323 2024-04-12 17:00:18.000000 nci_cidc_api_modules-1.0.5/nci_cidc_api_modules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-12 17:00:18.000000 nci_cidc_api_modules-1.0.5/nci_cidc_api_modules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:00:18.000000 nci_cidc_api_modules-1.0.5/nci_cidc_api_modules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:00:18.000000 nci_cidc_api_modules-1.0.5/nci_cidc_api_modules.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-12 17:00:18.000000 nci_cidc_api_modules-1.0.5/nci_cidc_api_modules.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 17:00:18.000000 nci_cidc_api_modules-1.0.5/nci_cidc_api_modules.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/requirements.modules.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:00:18.276310 nci_cidc_api_modules-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:00:18.276310 nci_cidc_api_modules-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    17127 2024-04-12 17:00:14.000000 nci_cidc_api_modules-1.0.5/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:13:23.391672 nci_cidc_api_modules-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    40323 2024-04-18 15:13:23.387672 nci_cidc_api_modules-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    39309 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:13:23.383672 nci_cidc_api_modules-1.0.6/cidc_api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:13:23.383672 nci_cidc_api_modules-1.0.6/cidc_api/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/config/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/config/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/config/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/config/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:13:23.383672 nci_cidc_api_modules-1.0.6/cidc_api/csms/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/csms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/csms/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:13:23.387672 nci_cidc_api_modules-1.0.6/cidc_api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31664 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/models/csms_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:13:23.387672 nci_cidc_api_modules-1.0.6/cidc_api/models/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/models/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62309 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/models/files/details.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29172 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/models/files/facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/models/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120820 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/models/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:13:23.387672 nci_cidc_api_modules-1.0.6/cidc_api/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11647 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/shared/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/shared/emails.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33746 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/shared/gcloud_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/shared/rest_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:13:23.387672 nci_cidc_api_modules-1.0.6/nci_cidc_api_modules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    40323 2024-04-18 15:13:23.000000 nci_cidc_api_modules-1.0.6/nci_cidc_api_modules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-18 15:13:23.000000 nci_cidc_api_modules-1.0.6/nci_cidc_api_modules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:13:23.000000 nci_cidc_api_modules-1.0.6/nci_cidc_api_modules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:13:23.000000 nci_cidc_api_modules-1.0.6/nci_cidc_api_modules.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-18 15:13:23.000000 nci_cidc_api_modules-1.0.6/nci_cidc_api_modules.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 15:13:23.000000 nci_cidc_api_modules-1.0.6/nci_cidc_api_modules.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/requirements.modules.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 15:13:23.391672 nci_cidc_api_modules-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:13:23.387672 nci_cidc_api_modules-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    17127 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/tests/test_api.py
```

### Comparing `nci_cidc_api_modules-1.0.5/LICENSE` & `nci_cidc_api_modules-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.5/PKG-INFO` & `nci_cidc_api_modules-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nci_cidc_api_modules
-Version: 1.0.5
+Version: 1.0.6
 Summary: SQLAlchemy data models and configuration tools used in the NCI CIDC API
 Home-page: https://github.com/NCI-CIDC/cidc-api-gae
 License: MIT license
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: werkzeug==2.3.8
```

### Comparing `nci_cidc_api_modules-1.0.5/README.md` & `nci_cidc_api_modules-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.5/cidc_api/config/db.py` & `nci_cidc_api_modules-1.0.6/cidc_api/config/db.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.5/cidc_api/config/logging.py` & `nci_cidc_api_modules-1.0.6/cidc_api/config/logging.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.5/cidc_api/config/secrets.py` & `nci_cidc_api_modules-1.0.6/cidc_api/config/secrets.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.5/cidc_api/config/settings.py` & `nci_cidc_api_modules-1.0.6/cidc_api/config/settings.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.5/cidc_api/csms/auth.py` & `nci_cidc_api_modules-1.0.6/cidc_api/csms/auth.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.5/cidc_api/models/csms_api.py` & `nci_cidc_api_modules-1.0.6/cidc_api/models/csms_api.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.5/cidc_api/models/files/details.py` & `nci_cidc_api_modules-1.0.6/cidc_api/models/files/details.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.5/cidc_api/models/files/facets.py` & `nci_cidc_api_modules-1.0.6/cidc_api/models/files/facets.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.5/cidc_api/models/migrations.py` & `nci_cidc_api_modules-1.0.6/cidc_api/models/migrations.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.5/cidc_api/models/models.py` & `nci_cidc_api_modules-1.0.6/cidc_api/models/models.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.5/cidc_api/models/schemas.py` & `nci_cidc_api_modules-1.0.6/cidc_api/models/schemas.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.5/cidc_api/shared/auth.py` & `nci_cidc_api_modules-1.0.6/cidc_api/shared/auth.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.5/cidc_api/shared/emails.py` & `nci_cidc_api_modules-1.0.6/cidc_api/shared/emails.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.5/cidc_api/shared/gcloud_client.py` & `nci_cidc_api_modules-1.0.6/cidc_api/shared/gcloud_client.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.5/cidc_api/shared/rest_utils.py` & `nci_cidc_api_modules-1.0.6/cidc_api/shared/rest_utils.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.5/nci_cidc_api_modules.egg-info/PKG-INFO` & `nci_cidc_api_modules-1.0.6/nci_cidc_api_modules.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nci_cidc_api_modules
-Version: 1.0.5
+Version: 1.0.6
 Summary: SQLAlchemy data models and configuration tools used in the NCI CIDC API
 Home-page: https://github.com/NCI-CIDC/cidc-api-gae
 License: MIT license
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: werkzeug==2.3.8
```

### Comparing `nci_cidc_api_modules-1.0.5/nci_cidc_api_modules.egg-info/SOURCES.txt` & `nci_cidc_api_modules-1.0.6/nci_cidc_api_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.5/pyproject.toml` & `nci_cidc_api_modules-1.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,26 +17,27 @@
 [tool.poetry.dependencies]
 python = ">=3.9,<3.10"
 flask-cors = "3.0.9"
 flask-cachecontrol = "0.3.0"
 six = "1.13.0"
 python-jose = "3.0.1"
 psycopg2-binary = ">=2,<3"
-packaging = "19.2"
+packaging = ">=20.0.0"
 protobuf = "3.20.3"
 gunicorn = "^21.2.0"
 gevent = "23.9.1"
 psycogreen = "1.0.2"
 webargs = "6.0.0"
 dash = "2.15.0"
 markupsafe = "2.1.5"
+pyarrow="14.0.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=8.0.1,<8.1.0"
-black = "22.3.0"
+black = "24.3.0"
 pre-commit = "2.9.2"
 ipython = "8.13.0"
 flask-shell-ipython = "0.5.1"
 webdriver-manager = "^4.0.1"
 percy = "2.0.2"
 selenium = "3.141.0"
 bs4 = "0.0.1"
@@ -46,18 +47,18 @@
 werkzeug = "2.3.8"
 flask = "2.2.5"
 flask-migrate = "2.5.2"
 flask-sqlalchemy = "2.5.1"
 sqlalchemy = ">=1.3.0,<1.4.0"
 marshmallow = "3.19.0"
 marshmallow-sqlalchemy = "0.22.3"
-google-cloud-storage = ">=1.35.0,<1.36.0"
+google-cloud-storage = "1.35.1"
 google-cloud-secret-manager = "2.16.2"
 google-cloud-pubsub = "0.43.0"
-google-cloud-bigquery = "3.3.5"
+google-cloud-bigquery = "3.18.0"
 google-api-python-client = "2.64.0"
 pandas = ">=1,<2"
 python-dotenv = "0.10.3"
 requests = "2.31.0"
 jinja2 = "3.1.3"
 nci-cidc-schemas = "0.26.29"
```

### Comparing `nci_cidc_api_modules-1.0.5/setup.py` & `nci_cidc_api_modules-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.5/tests/test_api.py` & `nci_cidc_api_modules-1.0.6/tests/test_api.py`

 * *Files identical despite different names*

