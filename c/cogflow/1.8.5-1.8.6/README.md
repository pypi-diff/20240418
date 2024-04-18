# Comparing `tmp/cogflow-1.8.5.tar.gz` & `tmp/cogflow-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cogflow-1.8.5.tar", last modified: Wed Apr 17 15:29:14 2024, max compression
+gzip compressed data, was "cogflow-1.8.6.tar", last modified: Wed Apr 17 15:43:55 2024, max compression
```

## Comparing `cogflow-1.8.5.tar` & `cogflow-1.8.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 15:29:14.235496 cogflow-1.8.5/
--rw-rw-rw-   0        0        0      401 2024-04-17 15:29:14.231198 cogflow-1.8.5/PKG-INFO
--rw-rw-rw-   0        0        0     4024 2024-04-15 10:04:49.000000 cogflow-1.8.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 15:29:14.205387 cogflow-1.8.5/cogflow/
--rw-rw-rw-   0        0        0      757 2024-04-17 15:25:52.000000 cogflow-1.8.5/cogflow/__init__.py
--rw-rw-rw-   0        0        0     5088 2024-04-16 13:26:15.000000 cogflow-1.8.5/cogflow/dataset_plugin.py
--rw-rw-rw-   0        0        0     8959 2024-04-17 15:27:00.000000 cogflow-1.8.5/cogflow/kubeflowplugin.py
--rw-rw-rw-   0        0        0    11107 2024-04-17 15:27:24.000000 cogflow-1.8.5/cogflow/mlflowplugin.py
--rw-rw-rw-   0        0        0      714 2024-04-17 14:53:54.000000 cogflow-1.8.5/cogflow/plugin_config.py
--rw-rw-rw-   0        0        0      620 2024-04-15 10:04:49.000000 cogflow-1.8.5/cogflow/plugin_status.py
--rw-rw-rw-   0        0        0      174 2024-04-15 10:04:49.000000 cogflow-1.8.5/cogflow/pluginerrors.py
--rw-rw-rw-   0        0        0     5494 2024-04-17 15:28:19.000000 cogflow-1.8.5/cogflow/pluginmanager.py
-drwxrwxrwx   0        0        0        0 2024-04-17 15:29:14.228969 cogflow-1.8.5/cogflow.egg-info/
--rw-rw-rw-   0        0        0      401 2024-04-17 15:29:13.000000 cogflow-1.8.5/cogflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2024-04-17 15:29:14.000000 cogflow-1.8.5/cogflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 15:29:13.000000 cogflow-1.8.5/cogflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2024-04-17 15:29:13.000000 cogflow-1.8.5/cogflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-17 15:29:13.000000 cogflow-1.8.5/cogflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 15:29:14.235496 cogflow-1.8.5/setup.cfg
--rw-rw-rw-   0        0        0     1594 2024-04-17 15:28:58.000000 cogflow-1.8.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 15:43:55.158767 cogflow-1.8.6/
+-rw-rw-rw-   0        0        0      401 2024-04-17 15:43:55.154091 cogflow-1.8.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4024 2024-04-15 10:04:49.000000 cogflow-1.8.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 15:43:55.130891 cogflow-1.8.6/cogflow/
+-rw-rw-rw-   0        0        0      757 2024-04-17 15:25:52.000000 cogflow-1.8.6/cogflow/__init__.py
+-rw-rw-rw-   0        0        0     5088 2024-04-16 13:26:15.000000 cogflow-1.8.6/cogflow/dataset_plugin.py
+-rw-rw-rw-   0        0        0     8959 2024-04-17 15:27:00.000000 cogflow-1.8.6/cogflow/kubeflowplugin.py
+-rw-rw-rw-   0        0        0    11107 2024-04-17 15:27:24.000000 cogflow-1.8.6/cogflow/mlflowplugin.py
+-rw-rw-rw-   0        0        0      714 2024-04-17 14:53:54.000000 cogflow-1.8.6/cogflow/plugin_config.py
+-rw-rw-rw-   0        0        0      620 2024-04-15 10:04:49.000000 cogflow-1.8.6/cogflow/plugin_status.py
+-rw-rw-rw-   0        0        0      174 2024-04-15 10:04:49.000000 cogflow-1.8.6/cogflow/pluginerrors.py
+-rw-rw-rw-   0        0        0     5492 2024-04-17 15:29:41.000000 cogflow-1.8.6/cogflow/pluginmanager.py
+drwxrwxrwx   0        0        0        0 2024-04-17 15:43:55.151788 cogflow-1.8.6/cogflow.egg-info/
+-rw-rw-rw-   0        0        0      401 2024-04-17 15:43:54.000000 cogflow-1.8.6/cogflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2024-04-17 15:43:55.000000 cogflow-1.8.6/cogflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 15:43:54.000000 cogflow-1.8.6/cogflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      214 2024-04-17 15:43:54.000000 cogflow-1.8.6/cogflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-17 15:43:54.000000 cogflow-1.8.6/cogflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 15:43:55.158767 cogflow-1.8.6/setup.cfg
+-rw-rw-rw-   0        0        0     1594 2024-04-17 15:43:42.000000 cogflow-1.8.6/setup.py
```

### Comparing `cogflow-1.8.5/README.md` & `cogflow-1.8.6/README.md`

 * *Files identical despite different names*

### Comparing `cogflow-1.8.5/cogflow/__init__.py` & `cogflow-1.8.6/cogflow/__init__.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.8.5/cogflow/dataset_plugin.py` & `cogflow-1.8.6/cogflow/dataset_plugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.8.5/cogflow/kubeflowplugin.py` & `cogflow-1.8.6/cogflow/kubeflowplugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.8.5/cogflow/mlflowplugin.py` & `cogflow-1.8.6/cogflow/mlflowplugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.8.5/cogflow/plugin_config.py` & `cogflow-1.8.6/cogflow/plugin_config.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.8.5/cogflow/plugin_status.py` & `cogflow-1.8.6/cogflow/plugin_status.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.8.5/cogflow/pluginmanager.py` & `cogflow-1.8.6/cogflow/pluginmanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from cogflow.kubeflowplugin import KubeflowPlugin
 from cogflow.mlflowplugin import MlflowPlugin
 from cogflow.dataset_plugin import DatasetPlugin
 from cogflow import plugin_status
 from cogflow.plugin_status import plugin_statuses
 
 
-
 class PluginManager:
     """
     Class responsible for managing plugins.
 
     Attributes:
         mlplugin (class): The Mlflow plugin class.
         kfplugin (class): The Kubeflow plugin class.
```

### Comparing `cogflow-1.8.5/setup.py` & `cogflow-1.8.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name="cogflow",
-    version="1.8.5",
+    version="1.8.6",
     author="Sai_kireeti",
     author_email="sai.kireeti@hiro-microdatacenters.nl",
     description="cog modules",
     packages=find_packages(),
     install_requires=[
         "mlflow==2.10.2",
         "kfp==1.8.22",
```

