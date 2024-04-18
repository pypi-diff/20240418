# Comparing `tmp/tencentcloud-sdk-python-config-3.0.1130.tar.gz` & `tmp/tencentcloud-sdk-python-config-3.0.1131.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-config-3.0.1130.tar", last modified: Mon Apr 15 20:40:44 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-config-3.0.1131.tar", last modified: Wed Apr 17 20:37:34 2024, max compression
```

## Comparing `tencentcloud-sdk-python-config-3.0.1130.tar` & `tencentcloud-sdk-python-config-3.0.1131.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:40:44.000000 tencentcloud-sdk-python-config-3.0.1130/
--rw-r--r--   0 root         (0) root         (0)     1675 2024-04-15 20:40:44.000000 tencentcloud-sdk-python-config-3.0.1130/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:40:44.000000 tencentcloud-sdk-python-config-3.0.1130/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      631 2024-04-15 20:40:44.000000 tencentcloud-sdk-python-config-3.0.1130/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:40:44.000000 tencentcloud-sdk-python-config-3.0.1130/tencentcloud/config/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:40:44.000000 tencentcloud-sdk-python-config-3.0.1130/tencentcloud/config/v20220802/
--rw-r--r--   0 root         (0) root         (0)     1002 2024-04-15 20:40:44.000000 tencentcloud-sdk-python-config-3.0.1130/tencentcloud/config/v20220802/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    40671 2024-04-15 20:40:44.000000 tencentcloud-sdk-python-config-3.0.1130/tencentcloud/config/v20220802/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:40:44.000000 tencentcloud-sdk-python-config-3.0.1130/tencentcloud/config/v20220802/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3670 2024-04-15 20:40:44.000000 tencentcloud-sdk-python-config-3.0.1130/tencentcloud/config/v20220802/config_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:40:44.000000 tencentcloud-sdk-python-config-3.0.1130/tencentcloud/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-04-15 20:40:44.000000 tencentcloud-sdk-python-config-3.0.1130/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:40:44.000000 tencentcloud-sdk-python-config-3.0.1130/tencentcloud_sdk_python_config.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1675 2024-04-15 20:40:44.000000 tencentcloud-sdk-python-config-3.0.1130/tencentcloud_sdk_python_config.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-15 20:40:44.000000 tencentcloud-sdk-python-config-3.0.1130/tencentcloud_sdk_python_config.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 20:40:44.000000 tencentcloud-sdk-python-config-3.0.1130/tencentcloud_sdk_python_config.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      528 2024-04-15 20:40:44.000000 tencentcloud-sdk-python-config-3.0.1130/tencentcloud_sdk_python_config.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-15 20:40:44.000000 tencentcloud-sdk-python-config-3.0.1130/tencentcloud_sdk_python_config.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1079 2024-04-15 20:40:44.000000 tencentcloud-sdk-python-config-3.0.1130/setup.py
--rw-r--r--   0 root         (0) root         (0)      746 2024-04-15 20:40:44.000000 tencentcloud-sdk-python-config-3.0.1130/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:37:34.000000 tencentcloud-sdk-python-config-3.0.1131/
+-rw-r--r--   0 root         (0) root         (0)     1675 2024-04-17 20:37:34.000000 tencentcloud-sdk-python-config-3.0.1131/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:37:34.000000 tencentcloud-sdk-python-config-3.0.1131/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-17 20:37:34.000000 tencentcloud-sdk-python-config-3.0.1131/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:37:34.000000 tencentcloud-sdk-python-config-3.0.1131/tencentcloud/config/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:37:34.000000 tencentcloud-sdk-python-config-3.0.1131/tencentcloud/config/v20220802/
+-rw-r--r--   0 root         (0) root         (0)     1002 2024-04-17 20:37:34.000000 tencentcloud-sdk-python-config-3.0.1131/tencentcloud/config/v20220802/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    40671 2024-04-17 20:37:34.000000 tencentcloud-sdk-python-config-3.0.1131/tencentcloud/config/v20220802/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 20:37:34.000000 tencentcloud-sdk-python-config-3.0.1131/tencentcloud/config/v20220802/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3670 2024-04-17 20:37:34.000000 tencentcloud-sdk-python-config-3.0.1131/tencentcloud/config/v20220802/config_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 20:37:34.000000 tencentcloud-sdk-python-config-3.0.1131/tencentcloud/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2024-04-17 20:37:34.000000 tencentcloud-sdk-python-config-3.0.1131/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:37:34.000000 tencentcloud-sdk-python-config-3.0.1131/tencentcloud_sdk_python_config.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1675 2024-04-17 20:37:34.000000 tencentcloud-sdk-python-config-3.0.1131/tencentcloud_sdk_python_config.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-17 20:37:34.000000 tencentcloud-sdk-python-config-3.0.1131/tencentcloud_sdk_python_config.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 20:37:34.000000 tencentcloud-sdk-python-config-3.0.1131/tencentcloud_sdk_python_config.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      528 2024-04-17 20:37:34.000000 tencentcloud-sdk-python-config-3.0.1131/tencentcloud_sdk_python_config.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-17 20:37:34.000000 tencentcloud-sdk-python-config-3.0.1131/tencentcloud_sdk_python_config.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1079 2024-04-17 20:37:34.000000 tencentcloud-sdk-python-config-3.0.1131/setup.py
+-rw-r--r--   0 root         (0) root         (0)      746 2024-04-17 20:37:34.000000 tencentcloud-sdk-python-config-3.0.1131/README.rst
```

### Comparing `tencentcloud-sdk-python-config-3.0.1130/PKG-INFO` & `tencentcloud-sdk-python-config-3.0.1131/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-config
-Version: 3.0.1130
+Version: 3.0.1131
 Summary: Tencent Cloud Config SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-config-3.0.1130/tencentcloud/__init__.py` & `tencentcloud-sdk-python-config-3.0.1131/tencentcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.1130'
+__version__ = '3.0.1131'
```

### Comparing `tencentcloud-sdk-python-config-3.0.1130/tencentcloud/config/v20220802/errorcodes.py` & `tencentcloud-sdk-python-config-3.0.1131/tencentcloud/config/v20220802/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-config-3.0.1130/tencentcloud/config/v20220802/models.py` & `tencentcloud-sdk-python-config-3.0.1131/tencentcloud/config/v20220802/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-config-3.0.1130/tencentcloud/config/v20220802/config_client.py` & `tencentcloud-sdk-python-config-3.0.1131/tencentcloud/config/v20220802/config_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-config-3.0.1130/tencentcloud_sdk_python_config.egg-info/PKG-INFO` & `tencentcloud-sdk-python-config-3.0.1131/tencentcloud_sdk_python_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-config
-Version: 3.0.1130
+Version: 3.0.1131
 Summary: Tencent Cloud Config SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-config-3.0.1130/tencentcloud_sdk_python_config.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-config-3.0.1131/tencentcloud_sdk_python_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-config-3.0.1130/setup.py` & `tencentcloud-sdk-python-config-3.0.1131/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-config',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1130"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1131"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Config SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-config-3.0.1130/README.rst` & `tencentcloud-sdk-python-config-3.0.1131/README.rst`

 * *Files identical despite different names*
