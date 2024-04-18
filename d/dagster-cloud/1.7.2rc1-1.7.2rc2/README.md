# Comparing `tmp/dagster-cloud-1.7.2rc1.tar.gz` & `tmp/dagster-cloud-1.7.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-cloud-1.7.2rc1.tar", last modified: Tue Apr 16 18:02:03 2024, max compression
+gzip compressed data, was "dagster-cloud-1.7.2rc2.tar", last modified: Tue Apr 16 20:40:43 2024, max compression
```

## Comparing `dagster-cloud-1.7.2rc1.tar` & `dagster-cloud-1.7.2rc2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:03.516521 dagster-cloud-1.7.2rc1/
--rw-r--r--   0 root         (0) root         (0)     3463 2024-04-16 18:02:03.516521 dagster-cloud-1.7.2rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1960 2024-04-16 17:50:53.000000 dagster-cloud-1.7.2rc1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:03.512521 dagster-cloud-1.7.2rc1/dagster_cloud/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:53.000000 dagster-cloud-1.7.2rc1/dagster_cloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-16 17:50:53.000000 dagster-cloud-1.7.2rc1/dagster_cloud/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:03.516521 dagster-cloud-1.7.2rc1/dagster_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3463 2024-04-16 18:02:03.000000 dagster-cloud-1.7.2rc1/dagster_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      253 2024-04-16 18:02:03.000000 dagster-cloud-1.7.2rc1/dagster_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 18:02:03.000000 dagster-cloud-1.7.2rc1/dagster_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      359 2024-04-16 18:02:03.000000 dagster-cloud-1.7.2rc1/dagster_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-16 18:02:03.000000 dagster-cloud-1.7.2rc1/dagster_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 18:02:03.516521 dagster-cloud-1.7.2rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2539 2024-04-16 17:50:53.000000 dagster-cloud-1.7.2rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:43.740617 dagster-cloud-1.7.2rc2/
+-rw-r--r--   0 root         (0) root         (0)     3463 2024-04-16 20:40:43.740617 dagster-cloud-1.7.2rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1960 2024-04-16 20:27:17.000000 dagster-cloud-1.7.2rc2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:43.740617 dagster-cloud-1.7.2rc2/dagster_cloud/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:27:17.000000 dagster-cloud-1.7.2rc2/dagster_cloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-16 20:27:17.000000 dagster-cloud-1.7.2rc2/dagster_cloud/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:43.740617 dagster-cloud-1.7.2rc2/dagster_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3463 2024-04-16 20:40:43.000000 dagster-cloud-1.7.2rc2/dagster_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      253 2024-04-16 20:40:43.000000 dagster-cloud-1.7.2rc2/dagster_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:40:43.000000 dagster-cloud-1.7.2rc2/dagster_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      359 2024-04-16 20:40:43.000000 dagster-cloud-1.7.2rc2/dagster_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-16 20:40:43.000000 dagster-cloud-1.7.2rc2/dagster_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 20:40:43.740617 dagster-cloud-1.7.2rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2539 2024-04-16 20:27:17.000000 dagster-cloud-1.7.2rc2/setup.py
```

### Comparing `dagster-cloud-1.7.2rc1/PKG-INFO` & `dagster-cloud-1.7.2rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-cloud
-Version: 1.7.2rc1
+Version: 1.7.2rc2
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster-cloud-1.7.2rc1/README.md` & `dagster-cloud-1.7.2rc2/README.md`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.2rc1/dagster_cloud.egg-info/PKG-INFO` & `dagster-cloud-1.7.2rc2/dagster_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-cloud
-Version: 1.7.2rc1
+Version: 1.7.2rc2
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster-cloud-1.7.2rc1/setup.py` & `dagster-cloud-1.7.2rc2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         "Slack": "https://dagster.io/slack",
         "Blog": "https://dagster.io/blog",
         "Newsletter": "https://dagster.io/newsletter-signup",
     },
     packages=find_packages(exclude=["dagster_cloud_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster-plus==1.7.2rc1",
+        "dagster-plus==1.7.2rc2",
     ],
     extras_require={
         "tests": [f"dagster-plus[tests]{pin}"],
         "insights": [f"dagster-plus[insights]{pin}"],
         "docker": [f"dagster-plus[docker]{pin}"],
         "kubernetes": [f"dagster-plus[kubernetes]{pin}"],
         "ecs": [f"dagster-plus[ecs]{pin}"],
```

