# Comparing `tmp/pulumiverse_cockroach-0.2.2a1710169904.tar.gz` & `tmp/pulumiverse_cockroach-0.2.3a1713452126.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_cockroach-0.2.2a1710169904.tar", last modified: Mon Mar 11 15:14:34 2024, max compression
+gzip compressed data, was "pulumiverse_cockroach-0.2.3a1713452126.tar", last modified: Thu Apr 18 14:58:41 2024, max compression
```

## Comparing `pulumiverse_cockroach-0.2.2a1710169904.tar` & `pulumiverse_cockroach-0.2.3a1713452126.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:14:34.409119 pulumiverse_cockroach-0.2.2a1710169904/
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-03-11 15:14:34.409119 pulumiverse_cockroach-0.2.2a1710169904/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:14:34.409119 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/
--rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34510 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    15408 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/allow_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    14772 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/api_oidc_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8274 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/ca_cert.py
--rw-r--r--   0 runner    (1001) docker     (127)    24577 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    13069 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/cmek.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:14:34.409119 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     8157 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/finalize_version_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/get_cluster_cert.py
--rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/get_cockroach_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/get_connection_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/get_person_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    26512 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/log_export_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    14860 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/metric_export_cloudwatch_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12006 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/metric_export_datadog_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    44018 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/private_endpoint_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/private_endpoint_services.py
--rw-r--r--   0 runner    (1001) docker     (127)    11634 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/private_endpoint_trusted_owner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9785 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/sql_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/user_role_grants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/version_deferral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:14:34.409119 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 15:14:34.409119 pulumiverse_cockroach-0.2.2a1710169904/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-03-11 15:14:34.000000 pulumiverse_cockroach-0.2.2a1710169904/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:58:41.179000 pulumiverse_cockroach-0.2.3a1713452126/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-18 14:58:41.179000 pulumiverse_cockroach-0.2.3a1713452126/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:58:41.179000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34510 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15408 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14772 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/api_oidc_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8274 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/ca_cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24577 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13069 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/cmek.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:58:41.179000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8157 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/finalize_version_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/get_cluster_cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/get_cockroach_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/get_connection_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/get_person_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26512 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/log_export_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14860 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/metric_export_cloudwatch_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12006 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/metric_export_datadog_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44018 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/private_endpoint_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/private_endpoint_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11634 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/private_endpoint_trusted_owner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9785 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/sql_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/user_role_grants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/version_deferral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:58:41.179000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-18 14:58:41.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-18 14:58:41.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:58:41.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:58:41.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-18 14:58:41.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 14:58:41.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 14:58:41.179000 pulumiverse_cockroach-0.2.3a1713452126/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/setup.py
```

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/PKG-INFO` & `pulumiverse_cockroach-0.2.3a1713452126/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_cockroach
-Version: 0.2.2a1710169904
+Version: 0.2.3a1713452126
 Summary: A Pulumi package to create and managed Cockroach DB resources in Pulumi programs.
 Home-page: https://www.cockroachlabs.com/
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-cockroach
 Keywords: pulumi cockroach pulumiverse
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/README.md` & `pulumiverse_cockroach-0.2.3a1713452126/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/__init__.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/_inputs.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/_utilities.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/allow_list.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/allow_list.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/api_oidc_config.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/api_oidc_config.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/ca_cert.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/ca_cert.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/cluster.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/cmek.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/cmek.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/config/vars.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/database.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/database.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/finalize_version_upgrade.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/finalize_version_upgrade.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/folder.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/folder.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/get_cluster_cert.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/get_cluster_cert.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/get_cockroach_cluster.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/get_cockroach_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/get_connection_string.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/get_connection_string.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/get_organization.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/get_organization.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/get_person_user.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/get_person_user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/log_export_config.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/log_export_config.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/maintenance_window.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/maintenance_window.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/metric_export_cloudwatch_config.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/metric_export_cloudwatch_config.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/metric_export_datadog_config.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/metric_export_datadog_config.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/outputs.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/private_endpoint_connection.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/private_endpoint_connection.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/private_endpoint_services.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/private_endpoint_services.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/private_endpoint_trusted_owner.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/private_endpoint_trusted_owner.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/provider.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/sql_user.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/sql_user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/user_role_grants.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/user_role_grants.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach/version_deferral.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/version_deferral.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach.egg-info/PKG-INFO` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-cockroach
-Version: 0.2.2a1710169904
+Version: 0.2.3a1713452126
 Summary: A Pulumi package to create and managed Cockroach DB resources in Pulumi programs.
 Home-page: https://www.cockroachlabs.com/
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-cockroach
 Keywords: pulumi cockroach pulumiverse
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/pulumiverse_cockroach.egg-info/SOURCES.txt` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.2a1710169904/setup.py` & `pulumiverse_cockroach-0.2.3a1713452126/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import errno
 import os
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.2.2a1710169904"
+VERSION = "0.2.3a1713452126"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "cockroach Pulumi Package - Development Version"
```

