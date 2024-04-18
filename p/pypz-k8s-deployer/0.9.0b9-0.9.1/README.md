# Comparing `tmp/pypz-k8s-deployer-0.9.0b9.tar.gz` & `tmp/pypz_k8s_deployer-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypz-k8s-deployer-0.9.0b9.tar", last modified: Tue Feb 13 09:32:32 2024, max compression
+gzip compressed data, was "pypz_k8s_deployer-0.9.1.tar", last modified: Thu Apr 18 05:48:35 2024, max compression
```

## Comparing `pypz-k8s-deployer-0.9.0b9.tar` & `pypz_k8s_deployer-0.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:32.168144 pypz-k8s-deployer-0.9.0b9/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-13 09:32:19.000000 pypz-k8s-deployer-0.9.0b9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-02-13 09:32:32.168144 pypz-k8s-deployer-0.9.0b9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-02-13 09:32:19.000000 pypz-k8s-deployer-0.9.0b9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-13 09:32:19.000000 pypz-k8s-deployer-0.9.0b9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 09:32:32.168144 pypz-k8s-deployer-0.9.0b9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:32.168144 pypz-k8s-deployer-0.9.0b9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:32.168144 pypz-k8s-deployer-0.9.0b9/src/pypz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:32.168144 pypz-k8s-deployer-0.9.0b9/src/pypz/deployers/
--rw-r--r--   0 runner    (1001) docker     (127)    22085 2024-02-13 09:32:19.000000 pypz-k8s-deployer-0.9.0b9/src/pypz/deployers/k8s.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:32.168144 pypz-k8s-deployer-0.9.0b9/src/pypz_k8s_deployer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-02-13 09:32:32.000000 pypz-k8s-deployer-0.9.0b9/src/pypz_k8s_deployer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-02-13 09:32:32.000000 pypz-k8s-deployer-0.9.0b9/src/pypz_k8s_deployer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 09:32:32.000000 pypz-k8s-deployer-0.9.0b9/src/pypz_k8s_deployer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-13 09:32:32.000000 pypz-k8s-deployer-0.9.0b9/src/pypz_k8s_deployer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-13 09:32:32.000000 pypz-k8s-deployer-0.9.0b9/src/pypz_k8s_deployer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:35.143303 pypz_k8s_deployer-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 05:48:30.000000 pypz_k8s_deployer-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-18 05:48:35.143303 pypz_k8s_deployer-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-18 05:48:30.000000 pypz_k8s_deployer-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-18 05:48:30.000000 pypz_k8s_deployer-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 05:48:35.143303 pypz_k8s_deployer-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:35.139303 pypz_k8s_deployer-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:35.139303 pypz_k8s_deployer-0.9.1/src/pypz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:35.139303 pypz_k8s_deployer-0.9.1/src/pypz/deployers/
+-rw-r--r--   0 runner    (1001) docker     (127)    22155 2024-04-18 05:48:30.000000 pypz_k8s_deployer-0.9.1/src/pypz/deployers/k8s.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:35.143303 pypz_k8s_deployer-0.9.1/src/pypz_k8s_deployer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-18 05:48:35.000000 pypz_k8s_deployer-0.9.1/src/pypz_k8s_deployer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-18 05:48:35.000000 pypz_k8s_deployer-0.9.1/src/pypz_k8s_deployer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 05:48:35.000000 pypz_k8s_deployer-0.9.1/src/pypz_k8s_deployer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-18 05:48:35.000000 pypz_k8s_deployer-0.9.1/src/pypz_k8s_deployer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-18 05:48:35.000000 pypz_k8s_deployer-0.9.1/src/pypz_k8s_deployer.egg-info/top_level.txt
```

### Comparing `pypz-k8s-deployer-0.9.0b9/LICENSE` & `pypz_k8s_deployer-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypz-k8s-deployer-0.9.0b9/PKG-INFO` & `pypz_k8s_deployer-0.9.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: pypz-k8s-deployer
-Version: 0.9.0b9
+Version: 0.9.1
 Summary: This package provides the Kubernetes implementation of the deployer interface for pypz.
 Author-email: Laszlo Anka <laszlo.anka@gmail.com>
 License: Apache-2.0
 Keywords: pypz,k8s,kubernetes,deployer
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pypz-core
 Requires-Dist: kubernetes==v28.1.0
-Requires-Dist: certifi~=2023.7.22
+Requires-Dist: certifi~=2023.11.17
+Provides-Extra: static
+Requires-Dist: flake8~=7.0.0; extra == "static"
+Requires-Dist: flake8-html~=0.4.3; extra == "static"
+Requires-Dist: mypy~=1.8.0; extra == "static"
+Requires-Dist: coverage~=7.4.1; extra == "static"
 
 # Description
 
 This package contains the Kubernetes implementation of the deployer interface
 of *pypz*. It enables the deployment of the pipelines to a Kubernetes cluster.
 
 Check the [documentation](https://lazlowa.github.io/pypz-python/deployers/kubernetes.html) for
```

### Comparing `pypz-k8s-deployer-0.9.0b9/README.md` & `pypz_k8s_deployer-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pypz-k8s-deployer-0.9.0b9/pyproject.toml` & `pypz_k8s_deployer-0.9.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pypz-k8s-deployer"
-version = "0.9.0b9"
+version = "0.9.1"
 authors = [
     { name = "Laszlo Anka", email = "laszlo.anka@gmail.com" }
 ]
 description = "This package provides the Kubernetes implementation of the deployer interface for pypz."
 readme = "README.md"
 license = { text = "Apache-2.0" }
 requires-python = ">=3.11"
@@ -22,13 +22,21 @@
     "k8s",
     "kubernetes",
     "deployer"
 ]
 dependencies = [
     "pypz-core",
     "kubernetes==v28.1.0",
-    "certifi~=2023.7.22"
+    "certifi~=2023.11.17"
+]
+
+[project.optional-dependencies]
+static = [
+    "flake8 ~= 7.0.0",
+    "flake8-html ~= 0.4.3",
+    "mypy ~= 1.8.0",
+    "coverage ~= 7.4.1"
 ]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 namespaces = true
```

### Comparing `pypz-k8s-deployer-0.9.0b9/src/pypz/deployers/k8s.py` & `pypz_k8s_deployer-0.9.1/src/pypz/deployers/k8s.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     _env_var_operator_name = "PYPZ_OPERATOR_INSTANCE_NAME"
     _env_var_operator_exec_mode = "PYPZ_OPERATOR_EXEC_MODE"
 
     # ========================= static methods ==========================
 
     @staticmethod
     def sanitize(string: str) -> str:
-        return string.translate(str.maketrans({"_": "-", ".": "-"}))
+        return string.translate(str.maketrans({"_": "-", ".": "-"}))  # type: ignore
 
     # ========================= ctor ==========================
 
     def __init__(self,
                  namespace: str = "default",
                  configuration: Configuration = None,
                  config_file: Any = None):
@@ -306,23 +306,25 @@
         try:
             return self._core_v1_api.read_namespaced_pod_log(name=KubernetesDeployer.sanitize(operator_full_name),
                                                              namespace=self._namespace,
                                                              **kwargs)
         except ApiException as e:
             if 404 == e.status:
                 return None
+            raise
 
     # ========================= helper methods ==========================
 
     def _retrieve_config_secret(self, pipeline_name: str) -> Optional[V1Secret]:
         try:
             return self._core_v1_api.read_namespaced_secret(pipeline_name, self._namespace)
         except ApiException as e:
             if 404 == e.status:
                 return None
+            raise
 
     def _retrieve_deployed_pipeline_from_secret(self, secret: V1Secret) -> Optional[Pipeline]:
         if KubernetesDeployer._pipeline_config_secret_key not in secret.data:
             raise DeploymentException("Provided secret is not pipeline configuration secret")
 
         return Pipeline.create_from_string(base64.b64decode(
             secret.data[KubernetesDeployer._pipeline_config_secret_key]))
@@ -330,14 +332,15 @@
     def _retrieve_operator_pod(self, operator_full_name: str) -> Optional[V1Pod]:
         try:
             return self._core_v1_api.read_namespaced_pod(KubernetesDeployer.sanitize(operator_full_name),
                                                          self._namespace)
         except ApiException as e:
             if 404 == e.status:
                 return None
+            raise
 
     def _retrieve_operator_pods(self, pipeline_name: str) -> list[V1Pod]:
         return self._core_v1_api.list_namespaced_pod(
             self._namespace,
             label_selector=f"{KubernetesDeployer._label_key_part_of}={pipeline_name}"
         ).items
```

### Comparing `pypz-k8s-deployer-0.9.0b9/src/pypz_k8s_deployer.egg-info/PKG-INFO` & `pypz_k8s_deployer-0.9.1/src/pypz_k8s_deployer.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: pypz-k8s-deployer
-Version: 0.9.0b9
+Version: 0.9.1
 Summary: This package provides the Kubernetes implementation of the deployer interface for pypz.
 Author-email: Laszlo Anka <laszlo.anka@gmail.com>
 License: Apache-2.0
 Keywords: pypz,k8s,kubernetes,deployer
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pypz-core
 Requires-Dist: kubernetes==v28.1.0
-Requires-Dist: certifi~=2023.7.22
+Requires-Dist: certifi~=2023.11.17
+Provides-Extra: static
+Requires-Dist: flake8~=7.0.0; extra == "static"
+Requires-Dist: flake8-html~=0.4.3; extra == "static"
+Requires-Dist: mypy~=1.8.0; extra == "static"
+Requires-Dist: coverage~=7.4.1; extra == "static"
 
 # Description
 
 This package contains the Kubernetes implementation of the deployer interface
 of *pypz*. It enables the deployment of the pipelines to a Kubernetes cluster.
 
 Check the [documentation](https://lazlowa.github.io/pypz-python/deployers/kubernetes.html) for
```

