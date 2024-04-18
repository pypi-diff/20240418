# Comparing `tmp/eks_token-0.1.4.tar.gz` & `tmp/eks_token-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eks_token-0.1.4.tar", last modified: Tue Sep 19 06:43:04 2023, max compression
+gzip compressed data, was "eks_token-0.2.0.tar", last modified: Thu Apr 18 07:31:11 2024, max compression
```

## Comparing `eks_token-0.1.4.tar` & `eks_token-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 06:43:04.615750 eks_token-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2023-09-19 06:42:51.000000 eks_token-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2023-09-19 06:43:04.615750 eks_token-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2023-09-19 06:42:51.000000 eks_token-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 06:43:04.615750 eks_token-0.1.4/eks_token/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-09-19 06:42:51.000000 eks_token-0.1.4/eks_token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2023-09-19 06:42:51.000000 eks_token-0.1.4/eks_token/logics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 06:43:04.615750 eks_token-0.1.4/eks_token.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2023-09-19 06:43:04.000000 eks_token-0.1.4/eks_token.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-09-19 06:43:04.000000 eks_token-0.1.4/eks_token.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-19 06:43:04.000000 eks_token-0.1.4/eks_token.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-09-19 06:43:04.000000 eks_token-0.1.4/eks_token.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-09-19 06:43:04.000000 eks_token-0.1.4/eks_token.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-19 06:43:04.615750 eks_token-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      713 2023-09-19 06:42:51.000000 eks_token-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:31:11.534186 eks_token-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-18 07:31:02.000000 eks_token-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-18 07:31:11.534186 eks_token-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-18 07:31:02.000000 eks_token-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:31:11.534186 eks_token-0.2.0/eks_token/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-18 07:31:02.000000 eks_token-0.2.0/eks_token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-18 07:31:02.000000 eks_token-0.2.0/eks_token/logics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:31:11.534186 eks_token-0.2.0/eks_token.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-18 07:31:11.000000 eks_token-0.2.0/eks_token.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-18 07:31:11.000000 eks_token-0.2.0/eks_token.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 07:31:11.000000 eks_token-0.2.0/eks_token.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 07:31:11.000000 eks_token-0.2.0/eks_token.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 07:31:11.000000 eks_token-0.2.0/eks_token.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 07:31:11.534186 eks_token-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-18 07:31:02.000000 eks_token-0.2.0/setup.py
```

### Comparing `eks_token-0.1.4/LICENSE` & `eks_token-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eks_token-0.1.4/PKG-INFO` & `eks_token-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: eks_token
-Version: 0.1.4
+Version: 0.2.0
 Summary: EKS Token package, an alternate to "aws eks get-token ..." CLI
 Home-page: https://github.com/peak-ai/eks-token
 Author: Peak AI
 Author-email: support@peak.ai
 Keywords: eks k8s boto3 awscli python aws
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: awscli>=1.27.8
 
 # eks-token
 EKS Token package, an alternate to "aws eks get-token ..." CLI
 
 ![CodeQuality](https://github.com/peak-ai/eks-token/workflows/CodeQL/badge.svg) ![Publish](https://github.com/peak-ai/eks-token/workflows/Upload%20Python%20Package/badge.svg) ![stable](https://img.shields.io/github/v/release/peak-ai/eks-token) ![](https://img.shields.io/github/v/release/peak-ai/eks-token?include_prereleases) ![](https://img.shields.io/github/license/peak-ai/eks-token) ![](https://img.shields.io/github/languages/count/peak-ai/eks-token) ![](https://img.shields.io/github/languages/top/peak-ai/eks-token) ![](https://img.shields.io/github/issues-raw/peak-ai/eks-token) ![](https://img.shields.io/github/issues-pr-raw/peak-ai/eks-token) ![](https://img.shields.io/github/languages/code-size/peak-ai/eks-token) ![](https://img.shields.io/github/repo-size/peak-ai/eks-token)
 
 ![logo](https://raw.githubusercontent.com/peak-ai/eks-token/main/eks-iam.png)
```

### Comparing `eks_token-0.1.4/README.md` & `eks_token-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `eks_token-0.1.4/eks_token/logics.py` & `eks_token-0.2.0/eks_token/logics.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,14 @@
         return token_expiration.strftime('%Y-%m-%dT%H:%M:%SZ')
     
 def get_token(cluster_name: str, role_arn: str = None) -> dict:
     sts_client = client_factory.get_sts_client(role_arn=role_arn)
     token = TokenGenerator(sts_client).get_token(cluster_name)
     return {
             "kind": "ExecCredential",
-            "apiVersion": "client.authentication.k8s.io/v1alpha1",
+            "apiVersion": "client.authentication.k8s.io/v1beta1",
             "spec": {},
             "status": {
                 "expirationTimestamp": get_expiration_time(),
                 "token": token
             }
-        }
+        }
```

### Comparing `eks_token-0.1.4/eks_token.egg-info/PKG-INFO` & `eks_token-0.2.0/eks_token.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
-Name: eks-token
-Version: 0.1.4
+Name: eks_token
+Version: 0.2.0
 Summary: EKS Token package, an alternate to "aws eks get-token ..." CLI
 Home-page: https://github.com/peak-ai/eks-token
 Author: Peak AI
 Author-email: support@peak.ai
 Keywords: eks k8s boto3 awscli python aws
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: awscli>=1.27.8
 
 # eks-token
 EKS Token package, an alternate to "aws eks get-token ..." CLI
 
 ![CodeQuality](https://github.com/peak-ai/eks-token/workflows/CodeQL/badge.svg) ![Publish](https://github.com/peak-ai/eks-token/workflows/Upload%20Python%20Package/badge.svg) ![stable](https://img.shields.io/github/v/release/peak-ai/eks-token) ![](https://img.shields.io/github/v/release/peak-ai/eks-token?include_prereleases) ![](https://img.shields.io/github/license/peak-ai/eks-token) ![](https://img.shields.io/github/languages/count/peak-ai/eks-token) ![](https://img.shields.io/github/languages/top/peak-ai/eks-token) ![](https://img.shields.io/github/issues-raw/peak-ai/eks-token) ![](https://img.shields.io/github/issues-pr-raw/peak-ai/eks-token) ![](https://img.shields.io/github/languages/code-size/peak-ai/eks-token) ![](https://img.shields.io/github/repo-size/peak-ai/eks-token)
 
 ![logo](https://raw.githubusercontent.com/peak-ai/eks-token/main/eks-iam.png)
```

### Comparing `eks_token-0.1.4/setup.py` & `eks_token-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme:
     long_description = readme.read()
 
 setup(
     name='eks_token',
-    version='0.1.4',
+    version='0.2.0',
     author='Peak AI',
     author_email='support@peak.ai',
     description='EKS Token package, an alternate to "aws eks get-token ..." CLI',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/peak-ai/eks-token',
     packages=find_packages(),
```

