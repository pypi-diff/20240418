# Comparing `tmp/projen-0.81.0.tar.gz` & `tmp/projen-0.81.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projen-0.81.0.tar", last modified: Thu Apr 11 22:49:54 2024, max compression
+gzip compressed data, was "projen-0.81.1.tar", last modified: Thu Apr 18 09:53:21 2024, max compression
```

## Comparing `projen-0.81.0.tar` & `projen-0.81.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:49:54.789281 projen-0.81.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-11 22:49:43.000000 projen-0.81.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-11 22:49:43.000000 projen-0.81.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-04-11 22:49:54.789281 projen-0.81.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    78674 2024-04-11 22:49:43.000000 projen-0.81.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-11 22:49:43.000000 projen-0.81.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 22:49:54.789281 projen-0.81.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-11 22:49:43.000000 projen-0.81.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:49:54.769281 projen-0.81.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:49:54.773281 projen-0.81.0/src/projen/
--rw-r--r--   0 runner    (1001) docker     (127)   651984 2024-04-11 22:49:43.000000 projen-0.81.0/src/projen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:49:54.773281 projen-0.81.0/src/projen/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-11 22:49:43.000000 projen-0.81.0/src/projen/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:49:54.777281 projen-0.81.0/src/projen/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-11 22:49:43.000000 projen-0.81.0/src/projen/_jsii/bin/projen
--rw-r--r--   0 runner    (1001) docker     (127)  2649940 2024-04-11 22:49:43.000000 projen-0.81.0/src/projen/_jsii/projen@0.81.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:49:54.777281 projen-0.81.0/src/projen/awscdk/
--rw-r--r--   0 runner    (1001) docker     (127)  1079302 2024-04-11 22:49:43.000000 projen-0.81.0/src/projen/awscdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:49:54.781281 projen-0.81.0/src/projen/build/
--rw-r--r--   0 runner    (1001) docker     (127)    52320 2024-04-11 22:49:43.000000 projen-0.81.0/src/projen/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:49:54.781281 projen-0.81.0/src/projen/cdk/
--rw-r--r--   0 runner    (1001) docker     (127)   510147 2024-04-11 22:49:43.000000 projen-0.81.0/src/projen/cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:49:54.781281 projen-0.81.0/src/projen/cdk8s/
--rw-r--r--   0 runner    (1001) docker     (127)   597384 2024-04-11 22:49:43.000000 projen-0.81.0/src/projen/cdk8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:49:54.781281 projen-0.81.0/src/projen/cdktf/
--rw-r--r--   0 runner    (1001) docker     (127)   224466 2024-04-11 22:49:43.000000 projen-0.81.0/src/projen/cdktf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:49:54.781281 projen-0.81.0/src/projen/circleci/
--rw-r--r--   0 runner    (1001) docker     (127)    75913 2024-04-11 22:49:43.000000 projen-0.81.0/src/projen/circleci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:49:54.781281 projen-0.81.0/src/projen/github/
--rw-r--r--   0 runner    (1001) docker     (127)   407630 2024-04-11 22:49:43.000000 projen-0.81.0/src/projen/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:49:54.781281 projen-0.81.0/src/projen/github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)   250737 2024-04-11 22:49:43.000000 projen-0.81.0/src/projen/github/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:49:54.781281 projen-0.81.0/src/projen/gitlab/
--rw-r--r--   0 runner    (1001) docker     (127)   202810 2024-04-11 22:49:43.000000 projen-0.81.0/src/projen/gitlab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:49:54.785281 projen-0.81.0/src/projen/java/
--rw-r--r--   0 runner    (1001) docker     (127)   183709 2024-04-11 22:49:43.000000 projen-0.81.0/src/projen/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:49:54.785281 projen-0.81.0/src/projen/javascript/
--rw-r--r--   0 runner    (1001) docker     (127)   844523 2024-04-11 22:49:43.000000 projen-0.81.0/src/projen/javascript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:49:43.000000 projen-0.81.0/src/projen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:49:54.785281 projen-0.81.0/src/projen/python/
--rw-r--r--   0 runner    (1001) docker     (127)   213158 2024-04-11 22:49:43.000000 projen-0.81.0/src/projen/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:49:54.785281 projen-0.81.0/src/projen/release/
--rw-r--r--   0 runner    (1001) docker     (127)   285447 2024-04-11 22:49:43.000000 projen-0.81.0/src/projen/release/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:49:54.785281 projen-0.81.0/src/projen/typescript/
--rw-r--r--   0 runner    (1001) docker     (127)   474506 2024-04-11 22:49:43.000000 projen-0.81.0/src/projen/typescript/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:49:54.785281 projen-0.81.0/src/projen/vscode/
--rw-r--r--   0 runner    (1001) docker     (127)    69040 2024-04-11 22:49:43.000000 projen-0.81.0/src/projen/vscode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:49:54.785281 projen-0.81.0/src/projen/web/
--rw-r--r--   0 runner    (1001) docker     (127)   797444 2024-04-11 22:49:43.000000 projen-0.81.0/src/projen/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:49:54.773281 projen-0.81.0/src/projen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-04-11 22:49:54.000000 projen-0.81.0/src/projen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-11 22:49:54.000000 projen-0.81.0/src/projen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:49:54.000000 projen-0.81.0/src/projen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-11 22:49:54.000000 projen-0.81.0/src/projen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 22:49:54.000000 projen-0.81.0/src/projen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.281163 projen-0.81.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-18 09:53:10.000000 projen-0.81.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 09:53:10.000000 projen-0.81.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-04-18 09:53:21.281163 projen-0.81.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    78674 2024-04-18 09:53:10.000000 projen-0.81.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-18 09:53:10.000000 projen-0.81.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 09:53:21.281163 projen-0.81.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-18 09:53:10.000000 projen-0.81.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.261162 projen-0.81.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.265162 projen-0.81.1/src/projen/
+-rw-r--r--   0 runner    (1001) docker     (127)   651984 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.265162 projen-0.81.1/src/projen/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.269162 projen-0.81.1/src/projen/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/_jsii/bin/projen
+-rw-r--r--   0 runner    (1001) docker     (127)  2649940 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/_jsii/projen@0.81.1.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.269162 projen-0.81.1/src/projen/awscdk/
+-rw-r--r--   0 runner    (1001) docker     (127)  1079302 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/awscdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.273162 projen-0.81.1/src/projen/build/
+-rw-r--r--   0 runner    (1001) docker     (127)    52320 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.273162 projen-0.81.1/src/projen/cdk/
+-rw-r--r--   0 runner    (1001) docker     (127)   510147 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.273162 projen-0.81.1/src/projen/cdk8s/
+-rw-r--r--   0 runner    (1001) docker     (127)   597384 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/cdk8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.273162 projen-0.81.1/src/projen/cdktf/
+-rw-r--r--   0 runner    (1001) docker     (127)   224466 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/cdktf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.277162 projen-0.81.1/src/projen/circleci/
+-rw-r--r--   0 runner    (1001) docker     (127)    75913 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/circleci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.277162 projen-0.81.1/src/projen/github/
+-rw-r--r--   0 runner    (1001) docker     (127)   407630 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.277162 projen-0.81.1/src/projen/github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)   250737 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/github/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.277162 projen-0.81.1/src/projen/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (127)   202810 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/gitlab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.277162 projen-0.81.1/src/projen/java/
+-rw-r--r--   0 runner    (1001) docker     (127)   183709 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.277162 projen-0.81.1/src/projen/javascript/
+-rw-r--r--   0 runner    (1001) docker     (127)   844523 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/javascript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.277162 projen-0.81.1/src/projen/python/
+-rw-r--r--   0 runner    (1001) docker     (127)   213158 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.277162 projen-0.81.1/src/projen/release/
+-rw-r--r--   0 runner    (1001) docker     (127)   285447 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/release/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.281163 projen-0.81.1/src/projen/typescript/
+-rw-r--r--   0 runner    (1001) docker     (127)   474506 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/typescript/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.281163 projen-0.81.1/src/projen/vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)    69040 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/vscode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.281163 projen-0.81.1/src/projen/web/
+-rw-r--r--   0 runner    (1001) docker     (127)   797444 2024-04-18 09:53:10.000000 projen-0.81.1/src/projen/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:21.265162 projen-0.81.1/src/projen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-04-18 09:53:21.000000 projen-0.81.1/src/projen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-18 09:53:21.000000 projen-0.81.1/src/projen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:53:21.000000 projen-0.81.1/src/projen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-18 09:53:21.000000 projen-0.81.1/src/projen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 09:53:21.000000 projen-0.81.1/src/projen.egg-info/top_level.txt
```

### Comparing `projen-0.81.0/LICENSE` & `projen-0.81.1/LICENSE`

 * *Files identical despite different names*

### Comparing `projen-0.81.0/PKG-INFO` & `projen-0.81.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.81.0
+Version: 0.81.1
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.81.0/README.md` & `projen-0.81.1/README.md`

 * *Files identical despite different names*

### Comparing `projen-0.81.0/setup.py` & `projen-0.81.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "projen",
-    "version": "0.81.0",
+    "version": "0.81.1",
     "description": "CDK for software projects",
     "license": "Apache-2.0",
     "url": "https://github.com/projen/projen.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -38,15 +38,15 @@
         "projen.release",
         "projen.typescript",
         "projen.vscode",
         "projen.web"
     ],
     "package_data": {
         "projen._jsii": [
-            "projen@0.81.0.jsii.tgz"
+            "projen@0.81.1.jsii.tgz"
         ],
         "projen": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `projen-0.81.0/src/projen/__init__.py` & `projen-0.81.1/src/projen/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.0/src/projen/awscdk/__init__.py` & `projen-0.81.1/src/projen/awscdk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -498,15 +498,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -2529,15 +2529,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -3647,15 +3647,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -6319,15 +6319,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -8213,15 +8213,15 @@
         :stability: experimental
         '''
         result = self._values.get("check_licenses")
         return typing.cast(typing.Optional[_LicenseCheckerOptions_80bcd362], result)
 
     @builtins.property
     def code_cov(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
+        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
 
         :default: false
 
         :stability: experimental
         '''
         result = self._values.get("code_cov")
         return typing.cast(typing.Optional[builtins.bool], result)
@@ -12287,15 +12287,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -14134,15 +14134,15 @@
         :stability: experimental
         '''
         result = self._values.get("check_licenses")
         return typing.cast(typing.Optional[_LicenseCheckerOptions_80bcd362], result)
 
     @builtins.property
     def code_cov(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
+        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
 
         :default: false
 
         :stability: experimental
         '''
         result = self._values.get("code_cov")
         return typing.cast(typing.Optional[builtins.bool], result)
@@ -15432,15 +15432,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -17328,15 +17328,15 @@
         :stability: experimental
         '''
         result = self._values.get("check_licenses")
         return typing.cast(typing.Optional[_LicenseCheckerOptions_80bcd362], result)
 
     @builtins.property
     def code_cov(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
+        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
 
         :default: false
 
         :stability: experimental
         '''
         result = self._values.get("code_cov")
         return typing.cast(typing.Optional[builtins.bool], result)
```

### Comparing `projen-0.81.0/src/projen/build/__init__.py` & `projen-0.81.1/src/projen/build/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.0/src/projen/cdk/__init__.py` & `projen-0.81.1/src/projen/cdk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1503,15 +1503,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -2230,15 +2230,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -4061,15 +4061,15 @@
         :stability: experimental
         '''
         result = self._values.get("check_licenses")
         return typing.cast(typing.Optional[_LicenseCheckerOptions_80bcd362], result)
 
     @builtins.property
     def code_cov(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
+        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
 
         :default: false
 
         :stability: experimental
         '''
         result = self._values.get("code_cov")
         return typing.cast(typing.Optional[builtins.bool], result)
@@ -5251,15 +5251,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -5980,15 +5980,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -7817,15 +7817,15 @@
         :stability: experimental
         '''
         result = self._values.get("check_licenses")
         return typing.cast(typing.Optional[_LicenseCheckerOptions_80bcd362], result)
 
     @builtins.property
     def code_cov(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
+        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
 
         :default: false
 
         :stability: experimental
         '''
         result = self._values.get("code_cov")
         return typing.cast(typing.Optional[builtins.bool], result)
```

### Comparing `projen-0.81.0/src/projen/cdk8s/__init__.py` & `projen-0.81.1/src/projen/cdk8s/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2658,15 +2658,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -3391,15 +3391,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -5204,15 +5204,15 @@
         :stability: experimental
         '''
         result = self._values.get("check_licenses")
         return typing.cast(typing.Optional[_LicenseCheckerOptions_80bcd362], result)
 
     @builtins.property
     def code_cov(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
+        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
 
         :default: false
 
         :stability: experimental
         '''
         result = self._values.get("code_cov")
         return typing.cast(typing.Optional[builtins.bool], result)
@@ -6178,15 +6178,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -6936,15 +6936,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -8796,15 +8796,15 @@
         :stability: experimental
         '''
         result = self._values.get("check_licenses")
         return typing.cast(typing.Optional[_LicenseCheckerOptions_80bcd362], result)
 
     @builtins.property
     def code_cov(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
+        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
 
         :default: false
 
         :stability: experimental
         '''
         result = self._values.get("code_cov")
         return typing.cast(typing.Optional[builtins.bool], result)
```

### Comparing `projen-0.81.0/src/projen/cdktf/__init__.py` & `projen-0.81.1/src/projen/cdktf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,15 +301,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -1029,15 +1029,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -2873,15 +2873,15 @@
         :stability: experimental
         '''
         result = self._values.get("check_licenses")
         return typing.cast(typing.Optional[_LicenseCheckerOptions_80bcd362], result)
 
     @builtins.property
     def code_cov(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
+        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
 
         :default: false
 
         :stability: experimental
         '''
         result = self._values.get("code_cov")
         return typing.cast(typing.Optional[builtins.bool], result)
```

### Comparing `projen-0.81.0/src/projen/circleci/__init__.py` & `projen-0.81.1/src/projen/circleci/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.0/src/projen/github/__init__.py` & `projen-0.81.1/src/projen/github/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2542,16 +2542,16 @@
         :stability: experimental
 
         Example::
 
             // Force any use of `actions/checkout` to use a pin a specific commit
             project.github.actions.set("actions/checkout", "actions/checkout@aaaaaa");
             
-            // But pin usage of `v3` to a different commit
-            project.github.actions.set("actions/checkout@v3", "actions/checkout@ffffff");
+            // But pin usage of `v4` to a different commit
+            project.github.actions.set("actions/checkout@v4", "actions/checkout@ffffff");
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__20166ac47381861e1a45b550a5e9646380c52a927fca9ebf00ec36dab0f295ed)
             check_type(argname="argument action", value=action, expected_type=type_hints["action"])
             check_type(argname="argument override", value=override, expected_type=type_hints["override"])
         return typing.cast(None, jsii.invoke(self, "set", [action, override]))
```

### Comparing `projen-0.81.0/src/projen/github/workflows/__init__.py` & `projen-0.81.1/src/projen/github/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.0/src/projen/gitlab/__init__.py` & `projen-0.81.1/src/projen/gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.0/src/projen/java/__init__.py` & `projen-0.81.1/src/projen/java/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.0/src/projen/javascript/__init__.py` & `projen-0.81.1/src/projen/javascript/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5279,15 +5279,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -6366,15 +6366,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -8040,15 +8040,15 @@
         :stability: experimental
         '''
         result = self._values.get("check_licenses")
         return typing.cast(typing.Optional[LicenseCheckerOptions], result)
 
     @builtins.property
     def code_cov(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
+        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
 
         :default: false
 
         :stability: experimental
         '''
         result = self._values.get("code_cov")
         return typing.cast(typing.Optional[builtins.bool], result)
```

### Comparing `projen-0.81.0/src/projen/python/__init__.py` & `projen-0.81.1/src/projen/python/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.0/src/projen/release/__init__.py` & `projen-0.81.1/src/projen/release/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.0/src/projen/typescript/__init__.py` & `projen-0.81.1/src/projen/typescript/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -965,15 +965,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -1729,15 +1729,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -3487,15 +3487,15 @@
         :stability: experimental
         '''
         result = self._values.get("check_licenses")
         return typing.cast(typing.Optional[_LicenseCheckerOptions_80bcd362], result)
 
     @builtins.property
     def code_cov(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
+        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
 
         :default: false
 
         :stability: experimental
         '''
         result = self._values.get("code_cov")
         return typing.cast(typing.Optional[builtins.bool], result)
@@ -4265,15 +4265,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -4725,15 +4725,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -5396,15 +5396,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -7156,15 +7156,15 @@
         :stability: experimental
         '''
         result = self._values.get("check_licenses")
         return typing.cast(typing.Optional[_LicenseCheckerOptions_80bcd362], result)
 
     @builtins.property
     def code_cov(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
+        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
 
         :default: false
 
         :stability: experimental
         '''
         result = self._values.get("code_cov")
         return typing.cast(typing.Optional[builtins.bool], result)
```

### Comparing `projen-0.81.0/src/projen/vscode/__init__.py` & `projen-0.81.1/src/projen/vscode/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.0/src/projen/web/__init__.py` & `projen-0.81.1/src/projen/web/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,15 +389,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -1048,15 +1048,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -2762,15 +2762,15 @@
         :stability: experimental
         '''
         result = self._values.get("check_licenses")
         return typing.cast(typing.Optional[_LicenseCheckerOptions_80bcd362], result)
 
     @builtins.property
     def code_cov(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
+        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
 
         :default: false
 
         :stability: experimental
         '''
         result = self._values.get("code_cov")
         return typing.cast(typing.Optional[builtins.bool], result)
@@ -3342,15 +3342,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -4052,15 +4052,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -5840,15 +5840,15 @@
         :stability: experimental
         '''
         result = self._values.get("check_licenses")
         return typing.cast(typing.Optional[_LicenseCheckerOptions_80bcd362], result)
 
     @builtins.property
     def code_cov(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
+        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
 
         :default: false
 
         :stability: experimental
         '''
         result = self._values.get("code_cov")
         return typing.cast(typing.Optional[builtins.bool], result)
@@ -6734,15 +6734,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -7446,15 +7446,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -8132,15 +8132,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -9894,15 +9894,15 @@
         :stability: experimental
         '''
         result = self._values.get("check_licenses")
         return typing.cast(typing.Optional[_LicenseCheckerOptions_80bcd362], result)
 
     @builtins.property
     def code_cov(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
+        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
 
         :default: false
 
         :stability: experimental
         '''
         result = self._values.get("code_cov")
         return typing.cast(typing.Optional[builtins.bool], result)
@@ -11034,15 +11034,15 @@
         :param artifacts_directory: (experimental) A directory which will contain build artifacts. Default: "dist"
         :param auto_approve_upgrades: (experimental) Automatically approve deps upgrade PRs, allowing them to be merged by mergify (if configued). Throw if set to true but ``autoApproveOptions`` are not defined. Default: - true
         :param build_workflow: (experimental) Define a GitHub workflow for building PRs. Default: - true if not a subproject
         :param build_workflow_options: (experimental) Options for PR build workflow.
         :param build_workflow_triggers: (deprecated) Build workflow triggers. Default: "{ pullRequest: {}, workflowDispatch: {} }"
         :param bundler_options: (experimental) Options for ``Bundler``.
         :param check_licenses: (experimental) Configure which licenses should be deemed acceptable for use by dependencies. This setting will cause the build to fail, if any prohibited or not allowed licenses ares encountered. Default: - no license checks are run during the build and all licenses will be accepted
-        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
+        :param code_cov: (experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``. Default: false
         :param code_cov_token_secret: (experimental) Define the secret name for a specified https://codecov.io/ token A secret is required to send coverage for private repositories. Default: - if this option is not specified, only public repositories are supported
         :param copyright_owner: (experimental) License copyright owner. Default: - defaults to the value of authorName or "" if ``authorName`` is undefined.
         :param copyright_period: (experimental) The copyright years to put in the LICENSE file. Default: - current year
         :param dependabot: (experimental) Use dependabot to handle dependency upgrades. Cannot be used in conjunction with ``depsUpgrade``. Default: false
         :param dependabot_options: (experimental) Options for dependabot. Default: - default options
         :param deps_upgrade: (experimental) Use tasks and github workflows to handle dependency upgrades. Cannot be used in conjunction with ``dependabot``. Default: true
         :param deps_upgrade_options: (experimental) Options for ``UpgradeDependencies``. Default: - default options
@@ -12722,15 +12722,15 @@
         :stability: experimental
         '''
         result = self._values.get("check_licenses")
         return typing.cast(typing.Optional[_LicenseCheckerOptions_80bcd362], result)
 
     @builtins.property
     def code_cov(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v3 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
+        '''(experimental) Define a GitHub workflow step for sending code coverage metrics to https://codecov.io/ Uses codecov/codecov-action@v4 A secret is required for private repos. Configured with ``@codeCovTokenSecret``.
 
         :default: false
 
         :stability: experimental
         '''
         result = self._values.get("code_cov")
         return typing.cast(typing.Optional[builtins.bool], result)
```

### Comparing `projen-0.81.0/src/projen.egg-info/PKG-INFO` & `projen-0.81.1/src/projen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.81.0
+Version: 0.81.1
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.81.0/src/projen.egg-info/SOURCES.txt` & `projen-0.81.1/src/projen.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/projen/py.typed
 src/projen.egg-info/PKG-INFO
 src/projen.egg-info/SOURCES.txt
 src/projen.egg-info/dependency_links.txt
 src/projen.egg-info/requires.txt
 src/projen.egg-info/top_level.txt
 src/projen/_jsii/__init__.py
-src/projen/_jsii/projen@0.81.0.jsii.tgz
+src/projen/_jsii/projen@0.81.1.jsii.tgz
 src/projen/_jsii/bin/projen
 src/projen/awscdk/__init__.py
 src/projen/build/__init__.py
 src/projen/cdk/__init__.py
 src/projen/cdk8s/__init__.py
 src/projen/cdktf/__init__.py
 src/projen/circleci/__init__.py
```

