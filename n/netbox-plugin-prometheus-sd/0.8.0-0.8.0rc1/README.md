# Comparing `tmp/netbox_plugin_prometheus_sd-0.8.0.tar.gz` & `tmp/netbox_plugin_prometheus_sd-0.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_plugin_prometheus_sd-0.8.0.tar", max compression
+gzip compressed data, was "netbox_plugin_prometheus_sd-0.8.0rc1.tar", max compression
```

## Comparing `netbox_plugin_prometheus_sd-0.8.0.tar` & `netbox_plugin_prometheus_sd-0.8.0rc1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1069 2024-04-18 17:53:19.269106 netbox_plugin_prometheus_sd-0.8.0/LICENSE
--rw-r--r--   0        0        0     5446 2024-04-18 17:53:19.269106 netbox_plugin_prometheus_sd-0.8.0/README.md
--rw-r--r--   0        0        0      488 2024-04-18 17:53:19.273106 netbox_plugin_prometheus_sd-0.8.0/netbox_prometheus_sd/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 17:53:19.273106 netbox_plugin_prometheus_sd-0.8.0/netbox_prometheus_sd/api/__init__.py
--rw-r--r--   0        0        0     7182 2024-04-18 17:53:19.273106 netbox_plugin_prometheus_sd-0.8.0/netbox_prometheus_sd/api/serializers.py
--rw-r--r--   0        0        0      381 2024-04-18 17:53:19.273106 netbox_plugin_prometheus_sd-0.8.0/netbox_prometheus_sd/api/urls.py
--rw-r--r--   0        0        0     5815 2024-04-18 17:53:19.273106 netbox_plugin_prometheus_sd-0.8.0/netbox_prometheus_sd/api/utils.py
--rw-r--r--   0        0        0     3354 2024-04-18 17:53:19.273106 netbox_plugin_prometheus_sd-0.8.0/netbox_prometheus_sd/api/views.py
--rw-r--r--   0        0        0       50 2024-04-18 17:53:19.273106 netbox_plugin_prometheus_sd-0.8.0/netbox_prometheus_sd/tests/__init__.py
--rw-r--r--   0        0        0     3514 2024-04-18 17:53:19.273106 netbox_plugin_prometheus_sd-0.8.0/netbox_prometheus_sd/tests/test_api.py
--rwxr-xr-x   0        0        0    13166 2024-04-18 17:53:19.273106 netbox_plugin_prometheus_sd-0.8.0/netbox_prometheus_sd/tests/test_serializers.py
--rw-r--r--   0        0        0     6974 2024-04-18 17:53:19.273106 netbox_plugin_prometheus_sd-0.8.0/netbox_prometheus_sd/tests/utils.py
--rw-r--r--   0        0        0      616 2024-04-18 17:53:29.193103 netbox_plugin_prometheus_sd-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     6102 1970-01-01 00:00:00.000000 netbox_plugin_prometheus_sd-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-12-25 10:29:12.080071 netbox_plugin_prometheus_sd-0.8.0rc1/LICENSE
+-rw-r--r--   0        0        0     4905 2023-12-25 10:29:12.080071 netbox_plugin_prometheus_sd-0.8.0rc1/README.md
+-rw-r--r--   0        0        0      488 2023-12-25 10:29:12.084071 netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-25 10:29:12.084071 netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/api/__init__.py
+-rw-r--r--   0        0        0     7182 2023-12-25 10:29:12.084071 netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/api/serializers.py
+-rw-r--r--   0        0        0      381 2023-12-25 10:29:12.084071 netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/api/urls.py
+-rw-r--r--   0        0        0     5815 2023-12-25 10:29:12.084071 netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/api/utils.py
+-rw-r--r--   0        0        0     3354 2023-12-25 10:29:12.084071 netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/api/views.py
+-rw-r--r--   0        0        0       50 2023-12-25 10:29:12.084071 netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/tests/__init__.py
+-rw-r--r--   0        0        0     3514 2023-12-25 10:29:12.084071 netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/tests/test_api.py
+-rwxr-xr-x   0        0        0    13166 2023-12-25 10:29:12.084071 netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/tests/test_serializers.py
+-rw-r--r--   0        0        0     6974 2023-12-25 10:29:12.084071 netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/tests/utils.py
+-rw-r--r--   0        0        0      621 2023-12-25 10:29:21.991980 netbox_plugin_prometheus_sd-0.8.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     5564 1970-01-01 00:00:00.000000 netbox_plugin_prometheus_sd-0.8.0rc1/PKG-INFO
```

### Comparing `netbox_plugin_prometheus_sd-0.8.0/LICENSE` & `netbox_plugin_prometheus_sd-0.8.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_plugin_prometheus_sd-0.8.0/README.md` & `netbox_plugin_prometheus_sd-0.8.0rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -117,15 +117,7 @@
 invoke create-user
 ```
 
 Visit http://localhost:8000 and log in with the new user.
 You can now define Netbox entities and test around.
 
 API endpoints for testing can be found at http://localhost:8000/api/plugins/prometheus-sd/
-
-## Conventional Commits
-
-This repository follows the Conventional Commits specification for versioning and changelog generation.
-Conventional Commits provide a standardized way of writing commit messages to convey semantic meaning
-about the changes made. Each commit message follows a defined format that includes a type,
-an optional scope, and a message. The types typically include features, fixes, documentation, and more.
-By adhering to this convention, we ensure clear and automated versioning, release notes, and changelog generation.
```

### Comparing `netbox_plugin_prometheus_sd-0.8.0/netbox_prometheus_sd/api/serializers.py` & `netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_prometheus_sd-0.8.0/netbox_prometheus_sd/api/utils.py` & `netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/api/utils.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_prometheus_sd-0.8.0/netbox_prometheus_sd/api/views.py` & `netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_prometheus_sd-0.8.0/netbox_prometheus_sd/tests/test_api.py` & `netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_prometheus_sd-0.8.0/netbox_prometheus_sd/tests/test_serializers.py` & `netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_prometheus_sd-0.8.0/netbox_prometheus_sd/tests/utils.py` & `netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/tests/utils.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_prometheus_sd-0.8.0/pyproject.toml` & `netbox_plugin_prometheus_sd-0.8.0rc1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "netbox-plugin-prometheus-sd"
-version = "0.8.0" # placeholder
+version = "0.8.0-rc1" # placeholder
 description = "A Netbox plugin to provide Netbox entires to Prometheus HTTP service discovery"
 authors = ["Felix Peters <felix.peters@breuninger.de>"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     { include = "netbox_prometheus_sd" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 [tool.poetry.dev-dependencies]
-black = "^24.4"
+black = "^23.12"
 invoke = "^2.2.0"
-pylint = "^3.1.0"
+pylint = "^3.0.3"
 pylint-django = "^2.5.5"
-yamllint = "^1.35.1"
+yamllint = "^1.33.0"
 typed-ast = "^1.5.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `netbox_plugin_prometheus_sd-0.8.0/PKG-INFO` & `netbox_plugin_prometheus_sd-0.8.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-plugin-prometheus-sd
-Version: 0.8.0
+Version: 0.8.0rc1
 Summary: A Netbox plugin to provide Netbox entires to Prometheus HTTP service discovery
 License: MIT
 Author: Felix Peters
 Author-email: felix.peters@breuninger.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -135,14 +135,7 @@
 ```
 
 Visit http://localhost:8000 and log in with the new user.
 You can now define Netbox entities and test around.
 
 API endpoints for testing can be found at http://localhost:8000/api/plugins/prometheus-sd/
 
-## Conventional Commits
-
-This repository follows the Conventional Commits specification for versioning and changelog generation.
-Conventional Commits provide a standardized way of writing commit messages to convey semantic meaning
-about the changes made. Each commit message follows a defined format that includes a type,
-an optional scope, and a message. The types typically include features, fixes, documentation, and more.
-By adhering to this convention, we ensure clear and automated versioning, release notes, and changelog generation.
```

