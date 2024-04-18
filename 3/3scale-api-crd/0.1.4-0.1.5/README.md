# Comparing `tmp/3scale-api-crd-0.1.4.tar.gz` & `tmp/3scale-api-crd-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3scale-api-crd-0.1.4.tar", last modified: Fri Apr  5 13:00:33 2024, max compression
+gzip compressed data, was "3scale-api-crd-0.1.5.tar", last modified: Thu Apr 18 13:44:22 2024, max compression
```

## Comparing `3scale-api-crd-0.1.4.tar` & `3scale-api-crd-0.1.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:00:33.385916 3scale-api-crd-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:00:33.381916 3scale-api-crd-0.1.4/3scale_api_crd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-05 13:00:33.000000 3scale-api-crd-0.1.4/3scale_api_crd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-05 13:00:33.000000 3scale-api-crd-0.1.4/3scale_api_crd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:00:33.000000 3scale-api-crd-0.1.4/3scale_api_crd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-05 13:00:33.000000 3scale-api-crd-0.1.4/3scale_api_crd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 13:00:33.000000 3scale-api-crd-0.1.4/3scale_api_crd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-05 13:00:33.385916 3scale-api-crd-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:00:33.385916 3scale-api-crd-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:00:33.381916 3scale-api-crd-0.1.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:00:33.385916 3scale-api-crd-0.1.4/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/asserts.py
--rw-r--r--   0 runner    (1001) docker     (127)    18166 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_activedocs.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_application_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_backend_mapping_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_backend_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_backend_usages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_custom_tenant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_mapping_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_openapis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_policy_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_pricing_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_promotes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/tests/integration/test_integration_services.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:00:33.385916 3scale-api-crd-0.1.4/threescale_api_crd/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/threescale_api_crd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/threescale_api_crd/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/threescale_api_crd/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    22087 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/threescale_api_crd/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)   107696 2024-04-05 13:00:23.000000 3scale-api-crd-0.1.4/threescale_api_crd/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:22.149899 3scale-api-crd-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:22.145899 3scale-api-crd-0.1.5/3scale_api_crd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-18 13:44:22.000000 3scale-api-crd-0.1.5/3scale_api_crd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-18 13:44:22.000000 3scale-api-crd-0.1.5/3scale_api_crd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:44:22.000000 3scale-api-crd-0.1.5/3scale_api_crd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-18 13:44:22.000000 3scale-api-crd-0.1.5/3scale_api_crd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 13:44:22.000000 3scale-api-crd-0.1.5/3scale_api_crd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-18 13:44:22.149899 3scale-api-crd-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:44:22.149899 3scale-api-crd-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:22.145899 3scale-api-crd-0.1.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:22.149899 3scale-api-crd-0.1.5/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/tests/integration/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18166 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/tests/integration/test_integration_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/tests/integration/test_integration_activedocs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/tests/integration/test_integration_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/tests/integration/test_integration_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/tests/integration/test_integration_application_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/tests/integration/test_integration_backend_mapping_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/tests/integration/test_integration_backend_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/tests/integration/test_integration_backend_usages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/tests/integration/test_integration_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/tests/integration/test_integration_custom_tenant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/tests/integration/test_integration_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/tests/integration/test_integration_mapping_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/tests/integration/test_integration_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/tests/integration/test_integration_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/tests/integration/test_integration_openapis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/tests/integration/test_integration_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/tests/integration/test_integration_policy_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/tests/integration/test_integration_pricing_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/tests/integration/test_integration_promotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/tests/integration/test_integration_services.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:44:22.149899 3scale-api-crd-0.1.5/threescale_api_crd/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/threescale_api_crd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/threescale_api_crd/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/threescale_api_crd/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22179 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/threescale_api_crd/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)   107735 2024-04-18 13:44:20.000000 3scale-api-crd-0.1.5/threescale_api_crd/resources.py
```

### Comparing `3scale-api-crd-0.1.4/3scale_api_crd.egg-info/PKG-INFO` & `3scale-api-crd-0.1.5/3scale_api_crd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 3scale-api-crd
-Version: 0.1.4
+Version: 0.1.5
 Summary: 3scale CRD Python Client
 Home-page: https://github.com/3scale-qe/3scale-api-python-crd
 Author: Martin Kudlej
 Author-email: kudlej.martin@gmail.com
 Maintainer: Martin Kudlej
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `3scale-api-crd-0.1.4/3scale_api_crd.egg-info/SOURCES.txt` & `3scale-api-crd-0.1.5/3scale_api_crd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.4/LICENSE` & `3scale-api-crd-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.4/PKG-INFO` & `3scale-api-crd-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 3scale-api-crd
-Version: 0.1.4
+Version: 0.1.5
 Summary: 3scale CRD Python Client
 Home-page: https://github.com/3scale-qe/3scale-api-python-crd
 Author: Martin Kudlej
 Author-email: kudlej.martin@gmail.com
 Maintainer: Martin Kudlej
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `3scale-api-crd-0.1.4/README.md` & `3scale-api-crd-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.4/setup.py` & `3scale-api-crd-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.4/tests/integration/asserts.py` & `3scale-api-crd-0.1.5/tests/integration/asserts.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.4/tests/integration/conftest.py` & `3scale-api-crd-0.1.5/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.4/tests/integration/test_integration_accounts.py` & `3scale-api-crd-0.1.5/tests/integration/test_integration_accounts.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.4/tests/integration/test_integration_activedocs.py` & `3scale-api-crd-0.1.5/tests/integration/test_integration_activedocs.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.4/tests/integration/test_integration_application.py` & `3scale-api-crd-0.1.5/tests/integration/test_integration_application.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.4/tests/integration/test_integration_application_plan.py` & `3scale-api-crd-0.1.5/tests/integration/test_integration_application_plan.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.4/tests/integration/test_integration_backend_mapping_rules.py` & `3scale-api-crd-0.1.5/tests/integration/test_integration_backend_mapping_rules.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.4/tests/integration/test_integration_backend_metrics.py` & `3scale-api-crd-0.1.5/tests/integration/test_integration_backend_metrics.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.4/tests/integration/test_integration_backend_usages.py` & `3scale-api-crd-0.1.5/tests/integration/test_integration_backend_usages.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.4/tests/integration/test_integration_backends.py` & `3scale-api-crd-0.1.5/tests/integration/test_integration_backends.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.4/tests/integration/test_integration_custom_tenant.py` & `3scale-api-crd-0.1.5/tests/integration/test_integration_custom_tenant.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.4/tests/integration/test_integration_limit.py` & `3scale-api-crd-0.1.5/tests/integration/test_integration_limit.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.4/tests/integration/test_integration_mapping_rules.py` & `3scale-api-crd-0.1.5/tests/integration/test_integration_mapping_rules.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.4/tests/integration/test_integration_methods.py` & `3scale-api-crd-0.1.5/tests/integration/test_integration_methods.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.4/tests/integration/test_integration_metrics.py` & `3scale-api-crd-0.1.5/tests/integration/test_integration_metrics.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.4/tests/integration/test_integration_openapis.py` & `3scale-api-crd-0.1.5/tests/integration/test_integration_openapis.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.4/tests/integration/test_integration_policies.py` & `3scale-api-crd-0.1.5/tests/integration/test_integration_policies.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.4/tests/integration/test_integration_policy_registry.py` & `3scale-api-crd-0.1.5/tests/integration/test_integration_policy_registry.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.4/tests/integration/test_integration_pricing_rules.py` & `3scale-api-crd-0.1.5/tests/integration/test_integration_pricing_rules.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.4/tests/integration/test_integration_promotes.py` & `3scale-api-crd-0.1.5/tests/integration/test_integration_promotes.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.4/tests/integration/test_integration_services.py` & `3scale-api-crd-0.1.5/tests/integration/test_integration_services.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.4/threescale_api_crd/client.py` & `3scale-api-crd-0.1.5/threescale_api_crd/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 
 
 class ThreeScaleClientCRD(threescale_api.client.ThreeScaleClient):
     """
     Threescale client for CRD.
     """
 
-    def __init__(self, url, token, ocp_provider_ref=None, *args, **kwargs):
+    def __init__(self, url, token, ocp_provider_ref=None, ocp_namespace=None, *args, **kwargs):
         super().__init__(url, token, *args, **kwargs)
         self._ocp_provider_ref = ocp_provider_ref
-        self._ocp_namespace = ThreeScaleClientCRD.get_namespace()
+        self._ocp_namespace = ThreeScaleClientCRD.get_namespace(ocp_namespace)
         self._services = resources.Services(
             parent=self, instance_klass=resources.Service
         )
         self._active_docs = resources.ActiveDocs(
             parent=self, instance_klass=resources.ActiveDoc
         )
         self._policy_registry = resources.PoliciesRegistry(
@@ -43,20 +43,20 @@
             parent=self, instance_klass=resources.Promote
         )
         self._applications = resources.Applications(
             parent=self, account=None, instance_klass=resources.Application
         )
 
     @classmethod
-    def get_namespace(_ignore):
+    def get_namespace(_ignore, namespace):
         """
         Returns namespace. If there is no valid Openshift 'oc' session, returns "NOT LOGGED IN".
         """
         try:
-            return ocp.get_project_name()
+            return namespace or ocp.get_project_name()
         except OpenShiftPythonException:
             return "NOT LOGGED IN"
 
     @property
     def services(self) -> resources.Services:
         """Gets services client
         Returns(resources.Services): Services client
```

### Comparing `3scale-api-crd-0.1.4/threescale_api_crd/constants.py` & `3scale-api-crd-0.1.5/threescale_api_crd/constants.py`

 * *Files identical despite different names*

### Comparing `3scale-api-crd-0.1.4/threescale_api_crd/defaults.py` & `3scale-api-crd-0.1.5/threescale_api_crd/defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         ocp.set_default_loglevel(6)
         super().__init__(
             parent=parent,
             instance_klass=instance_klass,
             entity_name=entity_name,
             entity_collection=entity_collection,
         )
+        ocp.set_default_project(self.threescale_client.ocp_namespace)
 
     def get_list(self, typ="normal"):
         """Returns list of entities."""
         return []
 
     def get_selector(self, obj_name=None):
         """Returns OCP selector for objects."""
@@ -83,25 +84,25 @@
             **kwargs:
 
         Returns:
 
         """
         return self.fetch_crd_entity(name) or super().read_by_name(name, **kwargs)
 
-    #    def read(self, entity_id: int = None) -> 'DefaultResourceCRD':
-    #        """Read the instance, read will just create empty resource and lazyloads only if needed
-    #        Args:
-    #            entity_id(int): Entity id
-    #        Returns(DefaultResourceCRD): Default resource
-    #        """
-    #        LOG.debug(self._log_message("[READ] CRD Read ", entity_id=entity_id))
-    #        if self.is_crd_implemented():
-    #            self.fetch(entity_id=entity_id)
-    #        else:
-    #            return threescale_api.defaults.DefaultClient.read(self, entity_id, **kwargs)
+    def read(self, entity_id: int = None, **kwargs) -> 'DefaultResourceCRD':
+        """Read the instance, read will just create empty resource and lazyloads only if needed
+        Args:
+            entity_id(int): Entity id
+        Returns(DefaultResourceCRD): Default resource
+        """
+        LOG.debug(self._log_message("[READ] CRD Read ", entity_id=entity_id))
+        if self.is_crd_implemented():
+            return self.fetch(entity_id=entity_id, **kwargs)
+        else:
+            return threescale_api.defaults.DefaultClient.read(self, entity_id, **kwargs)
 
     def fetch(self, entity_id: int = None, **kwargs):
         """Fetches the entity dictionary
         Args:
             entity_id(int): Entity id
             **kwargs: Optional args
 
@@ -564,14 +565,16 @@
     def __init__(self, *args, crd=None, **kwargs):
         super().__init__(**kwargs)
         self._crd = crd
 
     @property
     def crd(self):
         """CRD object property."""
+        if not self._crd:
+            self.read()
         return self._crd or self.entity.get("crd", None)
 
     @crd.setter
     def crd(self, value):
         self._crd = value
 
     @property
```

### Comparing `3scale-api-crd-0.1.4/threescale_api_crd/resources.py` & `3scale-api-crd-0.1.5/threescale_api_crd/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1962,14 +1962,15 @@
             required_attrs = [
                 "endpoint",
                 "sandbox_endpoint",
                 "credentials_location",
                 "auth_user_key",
                 "auth_app_id",
                 "auth_app_key",
+                "api_test_path"
             ]
             if any([att not in entity for att in required_attrs]):
                 self.client.disable_crd_implemented()
                 self.parent.client.disable_crd_implemented()
                 tmp_proxy = self.parent.proxy.fetch()
                 for name in required_attrs:
                     self.entity[name] = tmp_proxy[name]
@@ -2048,15 +2049,15 @@
 class OIDCConfigs(threescale_api.resources.DefaultClient):
     """OIDC configs."""
 
     def update(self, params: dict = None, **kwargs):
         proxy = self.parent.list()
         oidc = proxy.oidc["oidc_configuration"]
         oidc.update(params["oidc_configuration"])
-        proxy.update(oidc=oidc)
+        return proxy.update(oidc=oidc)
 
     def read(self, params: dict = None, **kwargs):
         proxy = self.parent.list()
         return proxy.oidc
 
 
 class MappingRule(DefaultResourceCRD, threescale_api.resources.MappingRule):
```

