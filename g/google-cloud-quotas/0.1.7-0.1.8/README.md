# Comparing `tmp/google-cloud-quotas-0.1.7.tar.gz` & `tmp/google-cloud-quotas-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-quotas-0.1.7.tar", last modified: Wed Apr  3 01:21:51 2024, max compression
+gzip compressed data, was "google-cloud-quotas-0.1.8.tar", last modified: Thu Apr 18 14:31:36 2024, max compression
```

## Comparing `google-cloud-quotas-0.1.7.tar` & `google-cloud-quotas-0.1.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.433397 google-cloud-quotas-0.1.7/
--rw-rw-r--   0 root         (0)     1003    11358 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5271 2024-04-03 01:21:51.433397 google-cloud-quotas-0.1.7/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3910 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.421396 google-cloud-quotas-0.1.7/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.421396 google-cloud-quotas-0.1.7/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.425396 google-cloud-quotas-0.1.7/google/cloud/cloudquotas/
--rw-rw-r--   0 root         (0)     1003     1945 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.425396 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/
--rw-rw-r--   0 root         (0)     1003     1777 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3032 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.425396 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.429396 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/
--rw-rw-r--   0 root         (0)     1003      757 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/__init__.py
--rw-rw-r--   0 root         (0)     1003    43750 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/async_client.py
--rw-rw-r--   0 root         (0)     1003    59916 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/client.py
--rw-rw-r--   0 root         (0)     1003    11063 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.429396 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/
--rw-rw-r--   0 root         (0)     1003     1358 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10567 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18316 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18651 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    41049 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.429396 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/types/
--rw-rw-r--   0 root         (0)     1003     1515 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    10073 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/types/cloudquotas.py
--rw-rw-r--   0 root         (0)     1003    17916 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/types/resources.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.433397 google-cloud-quotas-0.1.7/google_cloud_quotas.egg-info/
--rw-r--r--   0 root         (0)     1003     5271 2024-04-03 01:21:51.000000 google-cloud-quotas-0.1.7/google_cloud_quotas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1541 2024-04-03 01:21:51.000000 google-cloud-quotas-0.1.7/google_cloud_quotas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-03 01:21:51.000000 google-cloud-quotas-0.1.7/google_cloud_quotas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-03 01:21:51.000000 google-cloud-quotas-0.1.7/google_cloud_quotas.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      305 2024-04-03 01:21:51.000000 google-cloud-quotas-0.1.7/google_cloud_quotas.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-04-03 01:21:51.000000 google-cloud-quotas-0.1.7/google_cloud_quotas.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-04-03 01:21:51.433397 google-cloud-quotas-0.1.7/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3170 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.433397 google-cloud-quotas-0.1.7/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.433397 google-cloud-quotas-0.1.7/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.433397 google-cloud-quotas-0.1.7/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.433397 google-cloud-quotas-0.1.7/tests/unit/gapic/cloudquotas_v1/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/tests/unit/gapic/cloudquotas_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   233345 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/tests/unit/gapic/cloudquotas_v1/test_cloud_quotas.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:36.452557 google-cloud-quotas-0.1.8/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5271 2024-04-18 14:31:36.452557 google-cloud-quotas-0.1.8/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3910 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:36.440557 google-cloud-quotas-0.1.8/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:36.440557 google-cloud-quotas-0.1.8/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:36.444557 google-cloud-quotas-0.1.8/google/cloud/cloudquotas/
+-rw-rw-r--   0 root         (0)     1003     1945 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/google/cloud/cloudquotas/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/google/cloud/cloudquotas/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/google/cloud/cloudquotas/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:36.444557 google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/
+-rw-rw-r--   0 root         (0)     1003     1777 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3032 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:36.444557 google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:36.444557 google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/services/cloud_quotas/
+-rw-rw-r--   0 root         (0)     1003      757 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/services/cloud_quotas/__init__.py
+-rw-rw-r--   0 root         (0)     1003    43750 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/services/cloud_quotas/async_client.py
+-rw-rw-r--   0 root         (0)     1003    59916 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/services/cloud_quotas/client.py
+-rw-rw-r--   0 root         (0)     1003    11063 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/services/cloud_quotas/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:36.448557 google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/
+-rw-rw-r--   0 root         (0)     1003     1358 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10567 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18316 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18651 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    41049 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:36.448557 google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1515 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10073 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/types/cloudquotas.py
+-rw-rw-r--   0 root         (0)     1003    17735 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/types/resources.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:36.448557 google-cloud-quotas-0.1.8/google_cloud_quotas.egg-info/
+-rw-r--r--   0 root         (0)     1003     5271 2024-04-18 14:31:36.000000 google-cloud-quotas-0.1.8/google_cloud_quotas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1541 2024-04-18 14:31:36.000000 google-cloud-quotas-0.1.8/google_cloud_quotas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-18 14:31:36.000000 google-cloud-quotas-0.1.8/google_cloud_quotas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-18 14:31:36.000000 google-cloud-quotas-0.1.8/google_cloud_quotas.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      305 2024-04-18 14:31:36.000000 google-cloud-quotas-0.1.8/google_cloud_quotas.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-04-18 14:31:36.000000 google-cloud-quotas-0.1.8/google_cloud_quotas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-04-18 14:31:36.452557 google-cloud-quotas-0.1.8/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3170 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:36.448557 google-cloud-quotas-0.1.8/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:36.448557 google-cloud-quotas-0.1.8/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:36.448557 google-cloud-quotas-0.1.8/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:36.452557 google-cloud-quotas-0.1.8/tests/unit/gapic/cloudquotas_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/tests/unit/gapic/cloudquotas_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   233345 2024-04-18 14:28:17.000000 google-cloud-quotas-0.1.8/tests/unit/gapic/cloudquotas_v1/test_cloud_quotas.py
```

### Comparing `google-cloud-quotas-0.1.7/LICENSE` & `google-cloud-quotas-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.7/MANIFEST.in` & `google-cloud-quotas-0.1.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.7/PKG-INFO` & `google-cloud-quotas-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-quotas
-Version: 0.1.7
+Version: 0.1.8
 Summary: Google Cloud Quotas API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-quotas
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-quotas-0.1.7/README.rst` & `google-cloud-quotas-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.7/google/cloud/cloudquotas/__init__.py` & `google-cloud-quotas-0.1.8/google/cloud/cloudquotas/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.7/google/cloud/cloudquotas/gapic_version.py` & `google-cloud-quotas-0.1.8/google/cloud/cloudquotas/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.7"  # {x-release-please-version}
+__version__ = "0.1.8"  # {x-release-please-version}
```

### Comparing `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/__init__.py` & `google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/gapic_metadata.json` & `google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/gapic_version.py` & `google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.7"  # {x-release-please-version}
+__version__ = "0.1.8"  # {x-release-please-version}
```

### Comparing `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/__init__.py` & `google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/__init__.py` & `google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/services/cloud_quotas/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/async_client.py` & `google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/services/cloud_quotas/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/client.py` & `google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/services/cloud_quotas/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/pagers.py` & `google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/services/cloud_quotas/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/__init__.py` & `google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/base.py` & `google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/grpc.py` & `google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/grpc_asyncio.py` & `google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/rest.py` & `google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/types/__init__.py` & `google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/types/cloudquotas.py` & `google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/types/cloudquotas.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/types/resources.py` & `google-cloud-quotas-0.1.8/google/cloud/cloudquotas_v1/types/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,26 +299,23 @@
         reconciling (bool):
             Output only. Is the quota preference pending
             Google Cloud approval and fulfillment.
         justification (str):
             The reason / justification for this quota
             preference.
         contact_email (str):
-            Input only. An email address that can be used for quota
-            related communication between the Google Cloud and the user
-            in case the Google Cloud needs further information to make a
-            decision on whether the user preferred quota can be granted.
+            Input only. An email address that can be used to contact the
+            the user, in case Google Cloud needs more information to
+            make a decision before additional quota can be granted.
 
-            The email address is optional for decrease quota
-            preferences. In another word, QuotaConfig.preferred_value is
-            smaller than the QuotaDetails.reset_value. It is required
-            for increase quota preferences. The Google account for the
-            email address must have quota update permission for the
-            project, folder or organization this quota preference is
-            for.
+            When requesting a quota increase, the email address is
+            required. When requesting a quota decrease, the email
+            address is optional. For example, the email address is
+            optional when the ``QuotaConfig.preferred_value`` is smaller
+            than the ``QuotaDetails.reset_value``.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     dimensions: MutableMapping[str, str] = proto.MapField(
```

### Comparing `google-cloud-quotas-0.1.7/google_cloud_quotas.egg-info/PKG-INFO` & `google-cloud-quotas-0.1.8/google_cloud_quotas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-quotas
-Version: 0.1.7
+Version: 0.1.8
 Summary: Google Cloud Quotas API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-quotas
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-quotas-0.1.7/google_cloud_quotas.egg-info/SOURCES.txt` & `google-cloud-quotas-0.1.8/google_cloud_quotas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.7/setup.py` & `google-cloud-quotas-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.7/tests/__init__.py` & `google-cloud-quotas-0.1.8/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.7/tests/unit/__init__.py` & `google-cloud-quotas-0.1.8/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.7/tests/unit/gapic/__init__.py` & `google-cloud-quotas-0.1.8/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.7/tests/unit/gapic/cloudquotas_v1/__init__.py` & `google-cloud-quotas-0.1.8/tests/unit/gapic/cloudquotas_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.7/tests/unit/gapic/cloudquotas_v1/test_cloud_quotas.py` & `google-cloud-quotas-0.1.8/tests/unit/gapic/cloudquotas_v1/test_cloud_quotas.py`

 * *Files identical despite different names*

