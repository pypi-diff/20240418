# Comparing `tmp/dagster-cloud-cli-1.7.2rc1.tar.gz` & `tmp/dagster-cloud-cli-1.7.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-cloud-cli-1.7.2rc1.tar", last modified: Tue Apr 16 18:02:17 2024, max compression
+gzip compressed data, was "dagster-cloud-cli-1.7.2rc2.tar", last modified: Tue Apr 16 20:40:54 2024, max compression
```

## Comparing `dagster-cloud-cli-1.7.2rc1.tar` & `dagster-cloud-cli-1.7.2rc2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:17.172550 dagster-cloud-cli-1.7.2rc1/
--rw-r--r--   0 root         (0) root         (0)      317 2024-04-16 18:02:17.172550 dagster-cloud-cli-1.7.2rc1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:17.172550 dagster-cloud-cli-1.7.2rc1/dagster_cloud_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      317 2024-04-16 18:02:16.000000 dagster-cloud-cli-1.7.2rc1/dagster_cloud_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      256 2024-04-16 18:02:17.000000 dagster-cloud-cli-1.7.2rc1/dagster_cloud_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 18:02:16.000000 dagster-cloud-cli-1.7.2rc1/dagster_cloud_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2024-04-16 18:02:16.000000 dagster-cloud-cli-1.7.2rc1/dagster_cloud_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-16 18:02:16.000000 dagster-cloud-cli-1.7.2rc1/dagster_cloud_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 18:02:16.000000 dagster-cloud-cli-1.7.2rc1/dagster_cloud_cli.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 18:02:17.172550 dagster-cloud-cli-1.7.2rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1042 2024-04-16 17:50:53.000000 dagster-cloud-cli-1.7.2rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:54.700640 dagster-cloud-cli-1.7.2rc2/
+-rw-r--r--   0 root         (0) root         (0)      317 2024-04-16 20:40:54.700640 dagster-cloud-cli-1.7.2rc2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:40:54.700640 dagster-cloud-cli-1.7.2rc2/dagster_cloud_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      317 2024-04-16 20:40:54.000000 dagster-cloud-cli-1.7.2rc2/dagster_cloud_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      256 2024-04-16 20:40:54.000000 dagster-cloud-cli-1.7.2rc2/dagster_cloud_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:40:54.000000 dagster-cloud-cli-1.7.2rc2/dagster_cloud_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2024-04-16 20:40:54.000000 dagster-cloud-cli-1.7.2rc2/dagster_cloud_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-16 20:40:54.000000 dagster-cloud-cli-1.7.2rc2/dagster_cloud_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:40:54.000000 dagster-cloud-cli-1.7.2rc2/dagster_cloud_cli.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 20:40:54.700640 dagster-cloud-cli-1.7.2rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-04-16 20:27:17.000000 dagster-cloud-cli-1.7.2rc2/setup.py
```

### Comparing `dagster-cloud-cli-1.7.2rc1/setup.py` & `dagster-cloud-cli-1.7.2rc2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 pin = "" if ver == "1!0+dev" else f"=={ver}"
 setup(
     name="dagster-cloud-cli",
     version=get_version(),
     author_email="hello@elementl.com",
     packages=find_packages(exclude=["dagster_cloud.cli_tests*"]),
     include_package_data=True,
-    install_requires=["dagster-plus-cli==1.7.2rc1"],
+    install_requires=["dagster-plus-cli==1.7.2rc2"],
     extras_require={
         "tests": [f"dagster-plus-cli[tests]{pin}"],
     },
     author="Elementl",
     license="Apache-2.0",
     classifiers=[
         "Programming Language :: Python :: 3.11",
```

