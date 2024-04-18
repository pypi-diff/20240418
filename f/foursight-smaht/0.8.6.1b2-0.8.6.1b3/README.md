# Comparing `tmp/foursight_smaht-0.8.6.1b2.tar.gz` & `tmp/foursight_smaht-0.8.6.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_smaht-0.8.6.1b2.tar", max compression
+gzip compressed data, was "foursight_smaht-0.8.6.1b3.tar", max compression
```

## Comparing `foursight_smaht-0.8.6.1b2.tar` & `foursight_smaht-0.8.6.1b3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1083 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/LICENSE.txt
--rw-r--r--   0        0        0        0 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/chalicelib_smaht/__init__.py
--rw-r--r--   0        0        0     1030 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/chalicelib_smaht/app_utils.py
--rw-r--r--   0        0        0      873 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/chalicelib_smaht/buckets.py
--rw-r--r--   0        0        0     4960 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/chalicelib_smaht/check_schedules.py
--rw-r--r--   0        0        0    14108 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/chalicelib_smaht/check_setup.json
--rw-r--r--   0        0        0     6530 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/chalicelib_smaht/check_setup.json-local
--rw-r--r--   0        0        0    13660 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/chalicelib_smaht/check_setup.json-smaht-wolf
--rw-r--r--   0        0        0      249 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/__init__.py
--rw-r--r--   0        0        0     5682 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/audit_checks.py
--rw-r--r--   0        0        0     2883 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/ecs_checks.py
--rw-r--r--   0        0        0     3919 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/es_checks.py
--rw-r--r--   0        0        0      262 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/helpers/confchecks.py
--rw-r--r--   0        0        0      333 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/helpers/constants.py
--rw-r--r--   0        0        0    12321 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/helpers/lifecycle_utils.py
--rw-r--r--   0        0        0     8518 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/helpers/linecount_dicts.py
--rw-r--r--   0        0        0     3993 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/helpers/utils.py
--rw-r--r--   0        0        0     1598 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/helpers/wfr_utils.py
--rw-r--r--   0        0        0     2572 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/helpers/wfrset_utils.py
--rw-r--r--   0        0        0     7577 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/lifecycle_checks.py
--rw-r--r--   0        0        0    22420 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/system_checks.py
--rw-r--r--   0        0        0    34795 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/wfr_checks.py
--rw-r--r--   0        0        0     2595 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/wrangler_checks.py
--rw-r--r--   0        0        0      773 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/chalicelib_smaht/deploy.py
--rw-r--r--   0        0        0      135 2024-04-16 20:00:10.845863 foursight_smaht-0.8.6.1b2/chalicelib_smaht/gitinfo.json
--rw-r--r--   0        0        0      601 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/chalicelib_smaht/package.py
--rw-r--r--   0        0        0      323 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/chalicelib_smaht/scripts/local_check_execution.py
--rw-r--r--   0        0        0      253 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/chalicelib_smaht/vars.py
--rw-r--r--   0        0        0     1573 2024-04-16 19:59:59.921796 foursight_smaht-0.8.6.1b2/pyproject.toml
--rw-r--r--   0        0        0     1323 1970-01-01 00:00:00.000000 foursight_smaht-0.8.6.1b2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-04-18 13:34:11.329257 foursight_smaht-0.8.6.1b3/LICENSE.txt
+-rw-r--r--   0        0        0        0 2024-04-18 13:34:11.329257 foursight_smaht-0.8.6.1b3/chalicelib_smaht/__init__.py
+-rw-r--r--   0        0        0     1030 2024-04-18 13:34:11.329257 foursight_smaht-0.8.6.1b3/chalicelib_smaht/app_utils.py
+-rw-r--r--   0        0        0      873 2024-04-18 13:34:11.329257 foursight_smaht-0.8.6.1b3/chalicelib_smaht/buckets.py
+-rw-r--r--   0        0        0     4960 2024-04-18 13:34:11.329257 foursight_smaht-0.8.6.1b3/chalicelib_smaht/check_schedules.py
+-rw-r--r--   0        0        0    14108 2024-04-18 13:34:11.333257 foursight_smaht-0.8.6.1b3/chalicelib_smaht/check_setup.json
+-rw-r--r--   0        0        0     6530 2024-04-18 13:34:11.333257 foursight_smaht-0.8.6.1b3/chalicelib_smaht/check_setup.json-local
+-rw-r--r--   0        0        0    13660 2024-04-18 13:34:11.333257 foursight_smaht-0.8.6.1b3/chalicelib_smaht/check_setup.json-smaht-wolf
+-rw-r--r--   0        0        0      249 2024-04-18 13:34:11.333257 foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/__init__.py
+-rw-r--r--   0        0        0     5682 2024-04-18 13:34:11.333257 foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/audit_checks.py
+-rw-r--r--   0        0        0     2883 2024-04-18 13:34:11.333257 foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/ecs_checks.py
+-rw-r--r--   0        0        0     3919 2024-04-18 13:34:11.333257 foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/es_checks.py
+-rw-r--r--   0        0        0      262 2024-04-18 13:34:11.333257 foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0      333 2024-04-18 13:34:11.333257 foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/helpers/constants.py
+-rw-r--r--   0        0        0    12321 2024-04-18 13:34:11.333257 foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/helpers/lifecycle_utils.py
+-rw-r--r--   0        0        0     8518 2024-04-18 13:34:11.333257 foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/helpers/linecount_dicts.py
+-rw-r--r--   0        0        0     3993 2024-04-18 13:34:11.333257 foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/helpers/utils.py
+-rw-r--r--   0        0        0     1598 2024-04-18 13:34:11.333257 foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/helpers/wfr_utils.py
+-rw-r--r--   0        0        0     2572 2024-04-18 13:34:11.333257 foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/helpers/wfrset_utils.py
+-rw-r--r--   0        0        0     7577 2024-04-18 13:34:11.333257 foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/lifecycle_checks.py
+-rw-r--r--   0        0        0    22420 2024-04-18 13:34:11.333257 foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/system_checks.py
+-rw-r--r--   0        0        0    34795 2024-04-18 13:34:11.333257 foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/wfr_checks.py
+-rw-r--r--   0        0        0     2595 2024-04-18 13:34:11.333257 foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/wrangler_checks.py
+-rw-r--r--   0        0        0      773 2024-04-18 13:34:11.333257 foursight_smaht-0.8.6.1b3/chalicelib_smaht/deploy.py
+-rw-r--r--   0        0        0      135 2024-04-18 13:34:23.385332 foursight_smaht-0.8.6.1b3/chalicelib_smaht/gitinfo.json
+-rw-r--r--   0        0        0      601 2024-04-18 13:34:11.333257 foursight_smaht-0.8.6.1b3/chalicelib_smaht/package.py
+-rw-r--r--   0        0        0      323 2024-04-18 13:34:11.333257 foursight_smaht-0.8.6.1b3/chalicelib_smaht/scripts/local_check_execution.py
+-rw-r--r--   0        0        0      253 2024-04-18 13:34:11.333257 foursight_smaht-0.8.6.1b3/chalicelib_smaht/vars.py
+-rw-r--r--   0        0        0     1573 2024-04-18 13:34:11.333257 foursight_smaht-0.8.6.1b3/pyproject.toml
+-rw-r--r--   0        0        0     1323 1970-01-01 00:00:00.000000 foursight_smaht-0.8.6.1b3/PKG-INFO
```

### Comparing `foursight_smaht-0.8.6.1b2/LICENSE.txt` & `foursight_smaht-0.8.6.1b3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.6.1b2/chalicelib_smaht/app_utils.py` & `foursight_smaht-0.8.6.1b3/chalicelib_smaht/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.6.1b2/chalicelib_smaht/buckets.py` & `foursight_smaht-0.8.6.1b3/chalicelib_smaht/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.6.1b2/chalicelib_smaht/check_schedules.py` & `foursight_smaht-0.8.6.1b3/chalicelib_smaht/check_schedules.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.6.1b2/chalicelib_smaht/check_setup.json` & `foursight_smaht-0.8.6.1b3/chalicelib_smaht/check_setup.json`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.6.1b2/chalicelib_smaht/check_setup.json-local` & `foursight_smaht-0.8.6.1b3/chalicelib_smaht/check_setup.json-local`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.6.1b2/chalicelib_smaht/check_setup.json-smaht-wolf` & `foursight_smaht-0.8.6.1b3/chalicelib_smaht/check_setup.json-smaht-wolf`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/audit_checks.py` & `foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/audit_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/ecs_checks.py` & `foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/es_checks.py` & `foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/es_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/helpers/lifecycle_utils.py` & `foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/helpers/lifecycle_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/helpers/linecount_dicts.py` & `foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/helpers/linecount_dicts.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/helpers/utils.py` & `foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/helpers/wfr_utils.py` & `foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/helpers/wfr_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/helpers/wfrset_utils.py` & `foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/helpers/wfrset_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/lifecycle_checks.py` & `foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/lifecycle_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/system_checks.py` & `foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/system_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/wfr_checks.py` & `foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/wfr_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.6.1b2/chalicelib_smaht/checks/wrangler_checks.py` & `foursight_smaht-0.8.6.1b3/chalicelib_smaht/checks/wrangler_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.6.1b2/chalicelib_smaht/deploy.py` & `foursight_smaht-0.8.6.1b3/chalicelib_smaht/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.6.1b2/chalicelib_smaht/package.py` & `foursight_smaht-0.8.6.1b3/chalicelib_smaht/package.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.6.1b2/pyproject.toml` & `foursight_smaht-0.8.6.1b3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight-smaht"
-version = "0.8.6.1b2"
+version = "0.8.6.1b3"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "chalicelib_smaht" }
 ]
 
@@ -22,15 +22,15 @@
 # https://stackoverflow.com/questions/68802324/elasticsearch-in-go-err-the-client-noticed-that-the-server-is-not-elasticsear
 elasticsearch = "7.13.4"
 elasticsearch-dsl = "^7.0.0"
 gitpython = "^3.1.2"
 pytz = "^2020.1"
 packaging = "^23.0"
 magma-suite = "^3.2.1"
-tibanna-ff = "3.3.3.1b2"
+tibanna-ff = "3.3.3.1b3"
 MarkupSafe = "^2.1.3"
 foursight-core = "^5.4.0"
 # use below for tests but not for deployment
 #foursight-core = { git = "https://github.com/4dn-dcic/foursight-core.git", branch="core2" }
 #portal-pipeline-utils = "2.1.0.1b1"
 # Need pytest-redis 3.0.2 or higher for pytest 7.4.2 (or higher).
 pytest = "^7.4.2"
```

### Comparing `foursight_smaht-0.8.6.1b2/PKG-INFO` & `foursight_smaht-0.8.6.1b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-smaht
-Version: 0.8.6.1b2
+Version: 0.8.6.1b3
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -25,9 +25,9 @@
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: google-api-python-client (>=1.12.5,<2.0.0)
 Requires-Dist: magma-suite (>=3.2.1,<4.0.0)
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: pytest (>=7.4.2,<8.0.0)
 Requires-Dist: pytest-redis (>=3.0.2,<4.0.0)
 Requires-Dist: pytz (>=2020.1,<2021.0)
-Requires-Dist: tibanna-ff (==3.3.3.1b2)
+Requires-Dist: tibanna-ff (==3.3.3.1b3)
 Requires-Dist: tzlocal (>=5.1,<6.0)
```

