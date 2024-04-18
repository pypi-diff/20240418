# Comparing `tmp/pxk-0.0.2.tar.gz` & `tmp/pxk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pxk-0.0.2.tar", max compression
+gzip compressed data, was "pxk-0.0.3.tar", max compression
```

## Comparing `pxk-0.0.2.tar` & `pxk-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1066 2024-04-14 14:53:14.227750 pxk-0.0.2/LICENSE
--rw-r--r--   0        0        0     1709 2024-04-18 14:46:00.812102 pxk-0.0.2/README.md
--rw-r--r--   0        0        0       82 2024-04-18 14:15:57.602753 pxk-0.0.2/pxk/Constants.py
--rw-r--r--   0        0        0      152 2024-04-18 14:15:57.603074 pxk-0.0.2/pxk/__init__.py
--rw-r--r--   0        0        0      404 2024-04-18 14:15:57.603378 pxk-0.0.2/pxk/conftest.py
--rw-r--r--   0        0        0     7021 2024-04-18 14:15:57.603704 pxk-0.0.2/pxk/k8_client.py
--rw-r--r--   0        0        0     4023 2024-04-18 14:15:57.604007 pxk-0.0.2/pxk/ms_socketserver.py
--rw-r--r--   0        0        0     5739 2024-04-18 14:15:57.604426 pxk-0.0.2/pxk/plugin.py
--rw-r--r--   0        0        0      763 2024-04-18 14:47:19.657416 pxk-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2635 1970-01-01 00:00:00.000000 pxk-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-14 14:53:14.227750 pxk-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2221 2024-04-18 19:43:32.805207 pxk-0.0.3/README.md
+-rw-r--r--   0        0        0       82 2024-04-18 18:59:58.799950 pxk-0.0.3/pxk/Constants.py
+-rw-r--r--   0        0        0      152 2024-04-18 18:59:58.800264 pxk-0.0.3/pxk/__init__.py
+-rw-r--r--   0        0        0      404 2024-04-18 18:59:58.800656 pxk-0.0.3/pxk/conftest.py
+-rw-r--r--   0        0        0     7021 2024-04-18 18:59:58.801108 pxk-0.0.3/pxk/k8_client.py
+-rw-r--r--   0        0        0     4023 2024-04-18 18:59:58.801644 pxk-0.0.3/pxk/ms_socketserver.py
+-rw-r--r--   0        0        0     5739 2024-04-18 18:59:58.802127 pxk-0.0.3/pxk/plugin.py
+-rw-r--r--   0        0        0      763 2024-04-18 19:45:35.664824 pxk-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3147 1970-01-01 00:00:00.000000 pxk-0.0.3/PKG-INFO
```

### Comparing `pxk-0.0.2/LICENSE` & `pxk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pxk-0.0.2/README.md` & `pxk-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -13,20 +13,25 @@
 ```bash
 pytest {test files to run} -n {number of pods per deployment} --tx='pod'
 ```
 On top of the existing pytest-xdist library, various options have been added to support running tests from kubernetes pods remotely.
 ```bash
 pytest --namespace='{custom namspace}' --custom_image='{custom image}' {test files to run} -n {number of pods per deployment} --tx='pod'
 ```
+When there are multiple images, multiple deployments get created and each deployment will contain its own image. The plugin will then try its best to evenly distribute the workers as much as possible. If the number of workers is less than the number of custom images, an exception would occur. Multiple custom images can be provided through the command:
+```bash
+pytest --namespace='{custom namspace}' --custom_image='{custom image1, custom image1}' {test files to run} -n {number of pods per deployment} --tx='pod'
+```
 Logger is included as part of the functions added by the plugin. You can check the progress of the plugin by specifying:
 ```bash
 --log-cli-level INFO
 ```  
 Since the plugin relies on xdist library's task scheduler for distributing tasks, you can specify how you would like to distribute tasks across multiple pods. By default, it evenly distributes test files.  
 But if you would like each pod to run all the specified test files:
 ```bash
 pytest {testfiles to run} -n {number of pods per deployment} --tx='pod' --dist=each
 ```
-All the testfiles must be from the same folder. The plugin still needs to be tested in Windows OS.
+All the testfiles must be from the same folder.  
+The plugin may have issues in Windows OS.
 ## Reference
 The plugin uses Kubernetes API to create/delete kubernetes deployments.  
 https://github.com/kubernetes-client/python/blob/master/kubernetes/README.md
```

### Comparing `pxk-0.0.2/pxk/k8_client.py` & `pxk-0.0.3/pxk/k8_client.py`

 * *Files identical despite different names*

### Comparing `pxk-0.0.2/pxk/ms_socketserver.py` & `pxk-0.0.3/pxk/ms_socketserver.py`

 * *Files identical despite different names*

### Comparing `pxk-0.0.2/pxk/plugin.py` & `pxk-0.0.3/pxk/plugin.py`

 * *Files identical despite different names*

### Comparing `pxk-0.0.2/pyproject.toml` & `pxk-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pxk"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     "Aiden Seo <minwoo3180@gmail.com>", 
     "Daniel Stoller <danhstoller@gmail.com>", 
     "Dominique Pantin <dompantin@gmail.com>",
 ]
 description = "Automate the process of distributed testing on a Kubernetes cluster by extending the functionality of pytest-xdist, allowing users to efficiently run tests in parallel across multiple pods."
 readme = "README.md"
```

### Comparing `pxk-0.0.2/PKG-INFO` & `pxk-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pxk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Automate the process of distributed testing on a Kubernetes cluster by extending the functionality of pytest-xdist, allowing users to efficiently run tests in parallel across multiple pods.
 License: MIT
 Author: Aiden Seo
 Author-email: minwoo3180@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: MIT License
@@ -35,20 +35,25 @@
 ```bash
 pytest {test files to run} -n {number of pods per deployment} --tx='pod'
 ```
 On top of the existing pytest-xdist library, various options have been added to support running tests from kubernetes pods remotely.
 ```bash
 pytest --namespace='{custom namspace}' --custom_image='{custom image}' {test files to run} -n {number of pods per deployment} --tx='pod'
 ```
+When there are multiple images, multiple deployments get created and each deployment will contain its own image. The plugin will then try its best to evenly distribute the workers as much as possible. If the number of workers is less than the number of custom images, an exception would occur. Multiple custom images can be provided through the command:
+```bash
+pytest --namespace='{custom namspace}' --custom_image='{custom image1, custom image1}' {test files to run} -n {number of pods per deployment} --tx='pod'
+```
 Logger is included as part of the functions added by the plugin. You can check the progress of the plugin by specifying:
 ```bash
 --log-cli-level INFO
 ```  
 Since the plugin relies on xdist library's task scheduler for distributing tasks, you can specify how you would like to distribute tasks across multiple pods. By default, it evenly distributes test files.  
 But if you would like each pod to run all the specified test files:
 ```bash
 pytest {testfiles to run} -n {number of pods per deployment} --tx='pod' --dist=each
 ```
-All the testfiles must be from the same folder. The plugin still needs to be tested in Windows OS.
+All the testfiles must be from the same folder.  
+The plugin may have issues in Windows OS.
 ## Reference
 The plugin uses Kubernetes API to create/delete kubernetes deployments.  
 https://github.com/kubernetes-client/python/blob/master/kubernetes/README.md
```

