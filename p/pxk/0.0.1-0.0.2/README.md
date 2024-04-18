# Comparing `tmp/pxk-0.0.1.tar.gz` & `tmp/pxk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pxk-0.0.1.tar", max compression
+gzip compressed data, was "pxk-0.0.2.tar", max compression
```

## Comparing `pxk-0.0.1.tar` & `pxk-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1066 2024-04-14 14:53:14.227750 pxk-0.0.1/LICENSE
--rw-r--r--   0        0        0     1627 2024-04-14 18:15:45.487042 pxk-0.0.1/README.md
--rw-r--r--   0        0        0       82 2024-04-18 14:15:57.602753 pxk-0.0.1/pxk/Constants.py
--rw-r--r--   0        0        0      152 2024-04-18 14:15:57.603074 pxk-0.0.1/pxk/__init__.py
--rw-r--r--   0        0        0      404 2024-04-18 14:15:57.603378 pxk-0.0.1/pxk/conftest.py
--rw-r--r--   0        0        0     7021 2024-04-18 14:15:57.603704 pxk-0.0.1/pxk/k8_client.py
--rw-r--r--   0        0        0     4023 2024-04-18 14:15:57.604007 pxk-0.0.1/pxk/ms_socketserver.py
--rw-r--r--   0        0        0     5739 2024-04-18 14:15:57.604426 pxk-0.0.1/pxk/plugin.py
--rw-r--r--   0        0        0      763 2024-04-18 14:15:57.604735 pxk-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2553 1970-01-01 00:00:00.000000 pxk-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-14 14:53:14.227750 pxk-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1709 2024-04-18 14:46:00.812102 pxk-0.0.2/README.md
+-rw-r--r--   0        0        0       82 2024-04-18 14:15:57.602753 pxk-0.0.2/pxk/Constants.py
+-rw-r--r--   0        0        0      152 2024-04-18 14:15:57.603074 pxk-0.0.2/pxk/__init__.py
+-rw-r--r--   0        0        0      404 2024-04-18 14:15:57.603378 pxk-0.0.2/pxk/conftest.py
+-rw-r--r--   0        0        0     7021 2024-04-18 14:15:57.603704 pxk-0.0.2/pxk/k8_client.py
+-rw-r--r--   0        0        0     4023 2024-04-18 14:15:57.604007 pxk-0.0.2/pxk/ms_socketserver.py
+-rw-r--r--   0        0        0     5739 2024-04-18 14:15:57.604426 pxk-0.0.2/pxk/plugin.py
+-rw-r--r--   0        0        0      763 2024-04-18 14:47:19.657416 pxk-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2635 1970-01-01 00:00:00.000000 pxk-0.0.2/PKG-INFO
```

### Comparing `pxk-0.0.1/LICENSE` & `pxk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pxk-0.0.1/README.md` & `pxk-0.0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # Pytest-xdist-kubernetes
   
 The pytest-xdist-plugin extends pytest-xdist with new kubernetes pod communication. It is capable of creating Kubernetes deployment using the given namespace and docker image, run tests from pods, and display the result at the end from the terminal.  
 
 ## How to Install
 In order to use the plugin, >= Python 3.9 is required. Can be installed with the following command:  
 ```bash
-pip install pytest-xdist-kubernetes
+pip install pxk
 ```
 
 ## How to Use
 By giving <code>--tx='pod'</code> as part of the xdist command, it triggers Pytest-xdist-kubernetes plugin.
 ```bash
 pytest {test files to run} -n {number of pods per deployment} --tx='pod'
 ```
 On top of the existing pytest-xdist library, various options have been added to support running tests from kubernetes pods remotely.
 ```bash
-pytest --namespace='custom namspace' --custom_image='custom image' {test files to run} -n {number of pods per deployment} --tx='pod'
+pytest --namespace='{custom namspace}' --custom_image='{custom image}' {test files to run} -n {number of pods per deployment} --tx='pod'
 ```
 Logger is included as part of the functions added by the plugin. You can check the progress of the plugin by specifying:
 ```bash
 --log-cli-level INFO
 ```  
 Since the plugin relies on xdist library's task scheduler for distributing tasks, you can specify how you would like to distribute tasks across multiple pods. By default, it evenly distributes test files.  
 But if you would like each pod to run all the specified test files:
 ```bash
 pytest {testfiles to run} -n {number of pods per deployment} --tx='pod' --dist=each
 ```
-
+All the testfiles must be from the same folder. The plugin still needs to be tested in Windows OS.
 ## Reference
 The plugin uses Kubernetes API to create/delete kubernetes deployments.  
 https://github.com/kubernetes-client/python/blob/master/kubernetes/README.md
```

### Comparing `pxk-0.0.1/pxk/k8_client.py` & `pxk-0.0.2/pxk/k8_client.py`

 * *Files identical despite different names*

### Comparing `pxk-0.0.1/pxk/ms_socketserver.py` & `pxk-0.0.2/pxk/ms_socketserver.py`

 * *Files identical despite different names*

### Comparing `pxk-0.0.1/pxk/plugin.py` & `pxk-0.0.2/pxk/plugin.py`

 * *Files identical despite different names*

### Comparing `pxk-0.0.1/pyproject.toml` & `pxk-0.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pxk"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     "Aiden Seo <minwoo3180@gmail.com>", 
     "Daniel Stoller <danhstoller@gmail.com>", 
     "Dominique Pantin <dompantin@gmail.com>",
 ]
 description = "Automate the process of distributed testing on a Kubernetes cluster by extending the functionality of pytest-xdist, allowing users to efficiently run tests in parallel across multiple pods."
 readme = "README.md"
```

### Comparing `pxk-0.0.1/PKG-INFO` & `pxk-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pxk
-Version: 0.0.1
+Version: 0.0.2
 Summary: Automate the process of distributed testing on a Kubernetes cluster by extending the functionality of pytest-xdist, allowing users to efficiently run tests in parallel across multiple pods.
 License: MIT
 Author: Aiden Seo
 Author-email: minwoo3180@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: MIT License
@@ -23,32 +23,32 @@
 # Pytest-xdist-kubernetes
   
 The pytest-xdist-plugin extends pytest-xdist with new kubernetes pod communication. It is capable of creating Kubernetes deployment using the given namespace and docker image, run tests from pods, and display the result at the end from the terminal.  
 
 ## How to Install
 In order to use the plugin, >= Python 3.9 is required. Can be installed with the following command:  
 ```bash
-pip install pytest-xdist-kubernetes
+pip install pxk
 ```
 
 ## How to Use
 By giving <code>--tx='pod'</code> as part of the xdist command, it triggers Pytest-xdist-kubernetes plugin.
 ```bash
 pytest {test files to run} -n {number of pods per deployment} --tx='pod'
 ```
 On top of the existing pytest-xdist library, various options have been added to support running tests from kubernetes pods remotely.
 ```bash
-pytest --namespace='custom namspace' --custom_image='custom image' {test files to run} -n {number of pods per deployment} --tx='pod'
+pytest --namespace='{custom namspace}' --custom_image='{custom image}' {test files to run} -n {number of pods per deployment} --tx='pod'
 ```
 Logger is included as part of the functions added by the plugin. You can check the progress of the plugin by specifying:
 ```bash
 --log-cli-level INFO
 ```  
 Since the plugin relies on xdist library's task scheduler for distributing tasks, you can specify how you would like to distribute tasks across multiple pods. By default, it evenly distributes test files.  
 But if you would like each pod to run all the specified test files:
 ```bash
 pytest {testfiles to run} -n {number of pods per deployment} --tx='pod' --dist=each
 ```
-
+All the testfiles must be from the same folder. The plugin still needs to be tested in Windows OS.
 ## Reference
 The plugin uses Kubernetes API to create/delete kubernetes deployments.  
 https://github.com/kubernetes-client/python/blob/master/kubernetes/README.md
```

