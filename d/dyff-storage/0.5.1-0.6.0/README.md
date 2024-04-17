# Comparing `tmp/dyff-storage-0.5.1.tar.gz` & `tmp/dyff_storage-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff-storage-0.5.1.tar", last modified: Thu Apr 11 02:32:43 2024, max compression
+gzip compressed data, was "dyff_storage-0.6.0.tar", last modified: Wed Apr 17 21:01:02 2024, max compression
```

## Comparing `dyff-storage-0.5.1.tar` & `dyff_storage-0.6.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:32:43.386708 dyff-storage-0.5.1/
--rw-rw-rw-   0 root         (0) root         (0)      701 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1706 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      520 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1681 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     2577 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       51 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3477 2024-04-11 02:32:43.385707 dyff-storage-0.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2328 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:32:43.374708 dyff-storage-0.5.1/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:32:43.380708 dyff-storage-0.5.1/dyff/storage/
--rw-rw-rw-   0 root         (0) root         (0)     2631 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:32:43.380708 dyff-storage-0.5.1/dyff/storage/backend/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:32:43.381708 dyff-storage-0.5.1/dyff/storage/backend/base/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/base/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3220 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/base/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     6196 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/base/command.py
--rw-rw-rw-   0 root         (0) root         (0)    12255 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/base/query.py
--rw-rw-rw-   0 root         (0) root         (0)     2754 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/base/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:32:43.381708 dyff-storage-0.5.1/dyff/storage/backend/gcloud/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/gcloud/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6656 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/gcloud/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:32:43.382708 dyff-storage-0.5.1/dyff/storage/backend/kafka/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/kafka/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9209 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/kafka/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:32:43.382708 dyff-storage-0.5.1/dyff/storage/backend/mock/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/mock/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/mock/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:32:43.383708 dyff-storage-0.5.1/dyff/storage/backend/mongodb/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/mongodb/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7184 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/mongodb/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    20365 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/mongodb/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:32:43.383708 dyff-storage-0.5.1/dyff/storage/backend/s3/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/s3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13410 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/s3/storage.py
--rw-rw-rw-   0 root         (0) root         (0)    10386 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/config.py
--rw-rw-rw-   0 root         (0) root         (0)      485 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/dynamic_import.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2088 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/paths.py
--rw-rw-rw-   0 root         (0) root         (0)      673 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/timestamp.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:32:43.385707 dyff-storage-0.5.1/dyff_storage.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3477 2024-04-11 02:32:43.000000 dyff-storage-0.5.1/dyff_storage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1176 2024-04-11 02:32:43.000000 dyff-storage-0.5.1/dyff_storage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 02:32:43.000000 dyff-storage-0.5.1/dyff_storage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       79 2024-04-11 02:32:43.000000 dyff-storage-0.5.1/dyff_storage.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-11 02:32:43.000000 dyff-storage-0.5.1/dyff_storage.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/makefile
--rw-rw-rw-   0 root         (0) root         (0)     1487 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 02:32:43.386708 dyff-storage-0.5.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:32:43.385707 dyff-storage-0.5.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1194 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:01:02.353937 dyff_storage-0.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)      701 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      520 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     2577 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       51 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3477 2024-04-17 21:01:02.352937 dyff_storage-0.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2328 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:01:02.335937 dyff_storage-0.6.0/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:01:02.344937 dyff_storage-0.6.0/dyff/storage/
+-rw-rw-rw-   0 root         (0) root         (0)     2937 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/dyff/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:01:02.344937 dyff_storage-0.6.0/dyff/storage/backend/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/dyff/storage/backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:01:02.345937 dyff_storage-0.6.0/dyff/storage/backend/base/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/dyff/storage/backend/base/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/dyff/storage/backend/base/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     6196 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/dyff/storage/backend/base/command.py
+-rw-rw-rw-   0 root         (0) root         (0)    12255 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/dyff/storage/backend/base/query.py
+-rw-rw-rw-   0 root         (0) root         (0)     3061 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/dyff/storage/backend/base/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:01:02.346937 dyff_storage-0.6.0/dyff/storage/backend/gcloud/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/dyff/storage/backend/gcloud/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6656 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/dyff/storage/backend/gcloud/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:01:02.347937 dyff_storage-0.6.0/dyff/storage/backend/kafka/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/dyff/storage/backend/kafka/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9209 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/dyff/storage/backend/kafka/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:01:02.347937 dyff_storage-0.6.0/dyff/storage/backend/mock/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/dyff/storage/backend/mock/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/dyff/storage/backend/mock/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:01:02.349937 dyff_storage-0.6.0/dyff/storage/backend/mongodb/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/dyff/storage/backend/mongodb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7184 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/dyff/storage/backend/mongodb/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    20365 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/dyff/storage/backend/mongodb/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:01:02.349937 dyff_storage-0.6.0/dyff/storage/backend/s3/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/dyff/storage/backend/s3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15018 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/dyff/storage/backend/s3/storage.py
+-rw-rw-rw-   0 root         (0) root         (0)    10386 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/dyff/storage/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      485 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/dyff/storage/dynamic_import.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/dyff/storage/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2952 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/dyff/storage/paths.py
+-rw-rw-rw-   0 root         (0) root         (0)      673 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/dyff/storage/timestamp.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/dyff/storage/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:01:02.352937 dyff_storage-0.6.0/dyff_storage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3477 2024-04-17 21:01:02.000000 dyff_storage-0.6.0/dyff_storage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1176 2024-04-17 21:01:02.000000 dyff_storage-0.6.0/dyff_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 21:01:02.000000 dyff_storage-0.6.0/dyff_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2024-04-17 21:01:02.000000 dyff_storage-0.6.0/dyff_storage.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-17 21:01:02.000000 dyff_storage-0.6.0/dyff_storage.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 21:01:02.353937 dyff_storage-0.6.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:01:02.351937 dyff_storage-0.6.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1194 2024-04-17 21:00:56.000000 dyff_storage-0.6.0/tests/test_import.py
```

### Comparing `dyff-storage-0.5.1/.gitignore` & `dyff_storage-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.1/.gitlab-ci.yml` & `dyff_storage-0.6.0/.gitlab-ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 include:
   - project: buildgarden/pipelines/gitlab
     ref: 0.2.2
     file:
       - gitlab-release.yml
   - project: buildgarden/pipelines/detect-secrets
-    ref: 0.1.0
+    ref: 0.2.1
     file:
       - detect-secrets.yml
   - project: buildgarden/pipelines/prettier
     ref: 0.3.2
     file:
       - prettier.yml
   - project: buildgarden/pipelines/python
```

### Comparing `dyff-storage-0.5.1/.licenserc.yaml` & `dyff_storage-0.6.0/.licenserc.yaml`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.1/.pre-commit-config.yaml` & `dyff_storage-0.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.1/.secrets.baseline` & `dyff_storage-0.6.0/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.1/CODE_OF_CONDUCT.md` & `dyff_storage-0.6.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.1/LICENSE` & `dyff_storage-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.1/PKG-INFO` & `dyff_storage-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-storage
-Version: 0.5.1
+Version: 0.6.0
 Summary: Python storage API for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-storage
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-storage/-/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dyff-storage-0.5.1/README.md` & `dyff_storage-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.1/dyff/storage/__init__.py` & `dyff_storage-0.6.0/dyff/storage/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from __future__ import annotations
 
 # mypy: disable-error-code="import-untyped"
 import functools
 from typing import BinaryIO, Iterable, Optional
 
-from dyff.schema.platform import Artifact, StorageSignedURL
+from dyff.schema.platform import Artifact, ArtifactURL, Entities, StorageSignedURL
 from dyff.storage import dynamic_import, paths
 from dyff.storage.backend.base.storage import StorageBackend
 from dyff.storage.config import config
 
 
 @functools.lru_cache()
 def _get_backend() -> StorageBackend:
@@ -66,14 +66,18 @@
         dataset_id,
         artifact,
         size_limit_bytes=size_limit_bytes,
         storage_path=storage_path,
     )
 
 
+def artifact_downlinks(entity_kind: Entities, entity_id: str) -> Iterable[ArtifactURL]:
+    return _get_backend().artifact_downlinks(entity_kind, entity_id)
+
+
 def object_md5hash(storage_path: str) -> bytes:
     return _get_backend().object_md5hash(storage_path)
 
 
 def artifact_md5hash(artifact: Artifact, storage_path: str) -> bytes:
     return _get_backend().artifact_md5hash(artifact, storage_path)
 
@@ -84,15 +88,20 @@
     return _get_backend().dataset_artifact_md5hash(
         dataset_id, artifact_path, storage_path=storage_path
     )
 
 
 __all__ = [
     "paths",
+    "artifact_downlinks",
     "artifact_md5hash",
     "dataset_artifact_md5hash",
     "download_recursive",
+    "get_object",
     "list_dir",
     "object_md5hash",
+    "put_object",
+    "signed_url_for_artifact_upload",
     "signed_url_for_dataset_upload",
     "storage_size",
+    "upload_recursive",
 ]
```

### Comparing `dyff-storage-0.5.1/dyff/storage/backend/base/auth.py` & `dyff_storage-0.6.0/dyff/storage/backend/base/auth.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.1/dyff/storage/backend/base/command.py` & `dyff_storage-0.6.0/dyff/storage/backend/base/command.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.1/dyff/storage/backend/base/query.py` & `dyff_storage-0.6.0/dyff/storage/backend/base/query.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.1/dyff/storage/backend/base/storage.py` & `dyff_storage-0.6.0/dyff/storage/backend/base/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 import abc
 from typing import BinaryIO, Iterable, Optional
 
-from dyff.schema.platform import Artifact, StorageSignedURL
+from dyff.schema.platform import Artifact, ArtifactURL, Entities, StorageSignedURL
 
 
 class StorageBackend(abc.ABC):
     @abc.abstractmethod
     def storage_size(self, path: str) -> int:
         """Get the total size, in bytes, of all objects stored under the ``path``
         prefix."""
@@ -64,14 +64,21 @@
         size_limit_bytes: Optional[int] = None,
         storage_path: Optional[str] = None,
     ) -> StorageSignedURL:
         """Create a temporary signed URL that can be used in a PUT request to upload an
         ``Artifact`` directly to storage."""
 
     @abc.abstractmethod
+    def artifact_downlinks(
+        self, entity_kind: Entities, entity_id: str
+    ) -> Iterable[ArtifactURL]:
+        """Create a list of temporary URLs that can be used in GET requests to download
+        all of the artifacts associated with an entity."""
+
+    @abc.abstractmethod
     def object_md5hash(self, storage_path: str) -> bytes:
         """Compute the MD5 hash of an object in storage."""
 
     def artifact_md5hash(self, artifact: Artifact, storage_path: str) -> bytes:
         return self.object_md5hash(f"{storage_path}/{artifact.path}")
 
     @abc.abstractmethod
```

### Comparing `dyff-storage-0.5.1/dyff/storage/backend/gcloud/storage.py` & `dyff_storage-0.6.0/dyff/storage/backend/gcloud/storage.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.1/dyff/storage/backend/kafka/command.py` & `dyff_storage-0.6.0/dyff/storage/backend/kafka/command.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.1/dyff/storage/backend/mock/command.py` & `dyff_storage-0.6.0/dyff/storage/backend/mock/command.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.1/dyff/storage/backend/mongodb/auth.py` & `dyff_storage-0.6.0/dyff/storage/backend/mongodb/auth.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.1/dyff/storage/backend/mongodb/query.py` & `dyff_storage-0.6.0/dyff/storage/backend/mongodb/query.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.1/dyff/storage/backend/s3/storage.py` & `dyff_storage-0.6.0/dyff/storage/backend/s3/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import minio
 import minio.api
 import minio.helpers
 import minio.time
 
 from dyff.schema.dataset import max_artifact_size_bytes
-from dyff.schema.platform import Artifact, StorageSignedURL
+from dyff.schema.platform import Artifact, ArtifactURL, Entities, StorageSignedURL
 from dyff.storage import paths
 from dyff.storage.backend.base.storage import StorageBackend
 from dyff.storage.config import config
 
 
 class _MyMinio(minio.Minio):
     def presigned_url_for_base(
@@ -313,14 +313,48 @@
         return self.signed_url_for_artifact_upload(
             artifact,
             storage_path,
             size_limit_bytes=size_limit_bytes,
             _internal_client=_internal_client,
         )
 
+    def artifact_downlinks(
+        self, entity_kind: Entities, entity_id: str, *, _internal_client: bool = False
+    ) -> Iterable[ArtifactURL]:
+        storage_root = paths.entity_artifacts_root(entity_kind, entity_id)
+        _root_bucket, root_path = _split_bucket_path(storage_root)
+        artifact_paths = self.list_dir(storage_root, recursive=True)
+        client = _get_client()
+
+        for artifact_path in artifact_paths:
+            bucket_name, bucket_path = _split_bucket_path(artifact_path)
+            relative_path = Path(bucket_path).relative_to(root_path)
+            # TODO: Populate contentType and digest
+            artifact = Artifact(path=relative_path)
+
+            # If the s3 provider is self-hosted (e.g. Minio), external clients
+            # connect to it at a different URL than internal clients. We must sign
+            # the correct URL, depending on which kind of client will use it.
+            if _internal_client and config.storage.s3.internal_endpoint is not None:
+                configured_url = config.storage.s3.internal_endpoint
+            else:
+                configured_url = config.storage.s3.endpoint
+
+            signed_url = client.presigned_url_for_base(
+                configured_url,
+                "GET",
+                bucket_name,
+                bucket_path,
+                expires=timedelta(hours=1),
+            )
+
+            headers: dict[str, str] = {}
+            signed_url = StorageSignedURL(url=signed_url, method="GET", headers=headers)
+            yield ArtifactURL(artifact=artifact, signedURL=signed_url)
+
     def object_md5hash(self, storage_path: str) -> bytes:
         bucket_name, bucket_path = _split_bucket_path(storage_path)
         client = _get_client()
 
         response = None
         try:
             response = client.get_object(bucket_name, bucket_path)
```

### Comparing `dyff-storage-0.5.1/dyff/storage/config.py` & `dyff_storage-0.6.0/dyff/storage/config.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.1/dyff/storage/paths.py` & `dyff_storage-0.6.0/dyff/storage/paths.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-FileCopyrightText: 2024 UL Research Institutes
 # SPDX-License-Identifier: Apache-2.0
 
+from dyff.schema.platform import Entities
 from dyff.storage.config import config
 
 
 def auditprocedure_notebook(auditprocedure_id: str) -> str:
     return f"{config.resources.auditprocedures.storage.url}/{auditprocedure_id}/notebook.ipynb"
 
 
@@ -33,14 +34,18 @@
     return f"{config.resources.datasets.storage.url}/{dataset_id}/tasks/{task_id}"
 
 
 def datasource_root(datasource_id: str) -> str:
     return f"{config.resources.datasources.storage.url}/{datasource_id}"
 
 
+def measurements_root(measurement_id: str) -> str:
+    return f"{config.resources.measurements.storage.url}/{measurement_id}"
+
+
 def module_root(module_id: str) -> str:
     return f"{config.resources.modules.storage.url}/{module_id}"
 
 
 def outputs_raw(evaluation_id: str) -> str:
     return f"{config.resources.outputs.storage.url}/{evaluation_id}/data"
 
@@ -54,13 +59,34 @@
     return f"{report_root(report_id)}/part-0.parquet"
 
 
 def report_root(report_id: str) -> str:
     return f"{config.resources.reports.storage.url}/{report_id}"
 
 
+def safetycase_root(safetycase_id: str) -> str:
+    return f"{config.resources.safetycases.storage.url}/{safetycase_id}"
+
+
 def inferenceservice_source_archive(inferenceservice_id: str) -> str:
     return f"{config.resources.inferenceservices.storage.url}/{inferenceservice_id}/source.tar.gz"
 
 
 def model_source_archive(model_id: str) -> str:
     return f"{config.resources.models.storage.url}/{model_id}/source.tar.gz"
+
+
+def entity_artifacts_root(self, kind: Entities, id: str) -> str:
+    if kind == Entities.Dataset:
+        return dataset_root(id)
+    elif kind == Entities.Evaluation:
+        return outputs_verified(id)
+    elif kind == Entities.Measurement:
+        return measurements_root(id)
+    elif kind == Entities.Module:
+        return module_root(id)
+    elif kind == Entities.Report:
+        return report_root(id)
+    elif kind == Entities.SafetyCase:
+        return safetycase_root(id)
+    else:
+        raise ValueError(f"entity kind {kind} has no associated artifacts")
```

### Comparing `dyff-storage-0.5.1/dyff/storage/timestamp.py` & `dyff_storage-0.6.0/dyff/storage/timestamp.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.1/dyff_storage.egg-info/PKG-INFO` & `dyff_storage-0.6.0/dyff_storage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-storage
-Version: 0.5.1
+Version: 0.6.0
 Summary: Python storage API for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-storage
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-storage/-/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dyff-storage-0.5.1/dyff_storage.egg-info/SOURCES.txt` & `dyff_storage-0.6.0/dyff_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.1/makefile` & `dyff_storage-0.6.0/makefile`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.1/pyproject.toml` & `dyff_storage-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.1/tests/test_import.py` & `dyff_storage-0.6.0/tests/test_import.py`

 * *Files identical despite different names*

