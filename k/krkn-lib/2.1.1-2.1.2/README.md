# Comparing `tmp/krkn_lib-2.1.1.tar.gz` & `tmp/krkn_lib-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krkn_lib-2.1.1.tar", max compression
+gzip compressed data, was "krkn_lib-2.1.2.tar", max compression
```

## Comparing `krkn_lib-2.1.1.tar` & `krkn_lib-2.1.2.tar`

### file list

```diff
@@ -1,37 +1,40 @@
--rw-r--r--   0        0        0    10173 2024-03-28 16:39:01.088531 krkn_lib-2.1.1/LICENSE
--rw-r--r--   0        0        0     1389 2024-03-28 16:39:01.088531 krkn_lib-2.1.1/README.md
--rw-r--r--   0        0        0     1130 2024-03-28 16:40:48.380710 krkn_lib-2.1.1/pyproject.toml
--rw-r--r--   0        0        0       39 2024-03-28 16:39:01.088531 krkn_lib-2.1.1/src/krkn_lib/k8s/__init__.py
--rw-r--r--   0        0        0    89882 2024-03-28 16:40:55.508718 krkn_lib-2.1.1/src/krkn_lib/k8s/krkn_kubernetes.py
--rw-r--r--   0        0        0      462 2024-03-28 16:39:01.088531 krkn_lib-2.1.1/src/krkn_lib/k8s/templates/node_exec_pod.j2
--rw-r--r--   0        0        0        0 2024-03-28 16:39:01.088531 krkn_lib-2.1.1/src/krkn_lib/models/__init__.py
--rw-r--r--   0        0        0       30 2024-03-28 16:39:01.088531 krkn_lib-2.1.1/src/krkn_lib/models/k8s/__init__.py
--rw-r--r--   0        0        0     3157 2024-03-28 16:39:01.088531 krkn_lib-2.1.1/src/krkn_lib/models/k8s/models.py
--rw-r--r--   0        0        0       30 2024-03-28 16:39:01.088531 krkn_lib-2.1.1/src/krkn_lib/models/krkn/__init__.py
--rw-r--r--   0        0        0     2002 2024-03-28 16:39:01.088531 krkn_lib-2.1.1/src/krkn_lib/models/krkn/models.py
--rw-r--r--   0        0        0       30 2024-03-28 16:39:01.088531 krkn_lib-2.1.1/src/krkn_lib/models/telemetry/__init__.py
--rw-r--r--   0        0        0     6810 2024-03-28 16:39:01.088531 krkn_lib-2.1.1/src/krkn_lib/models/telemetry/models.py
--rw-r--r--   0        0        0       38 2024-03-28 16:39:01.088531 krkn_lib-2.1.1/src/krkn_lib/ocp/__init__.py
--rw-r--r--   0        0        0    15592 2024-03-28 16:40:54.164717 krkn_lib-2.1.1/src/krkn_lib/ocp/krkn_openshift.py
--rw-r--r--   0        0        0        0 2024-03-28 16:39:01.088531 krkn_lib-2.1.1/src/krkn_lib/prometheus/__init__.py
--rw-r--r--   0        0        0     8761 2024-03-28 16:39:01.088531 krkn_lib-2.1.1/src/krkn_lib/prometheus/krkn_prometheus.py
--rw-r--r--   0        0        0        0 2024-03-28 16:39:01.088531 krkn_lib-2.1.1/src/krkn_lib/telemetry/__init__.py
--rw-r--r--   0        0        0     1854 2024-03-28 16:40:54.084717 krkn_lib-2.1.1/src/krkn_lib/telemetry/elastic.py
--rw-r--r--   0        0        0       49 2024-03-28 16:39:01.088531 krkn_lib-2.1.1/src/krkn_lib/telemetry/k8s/__init__.py
--rw-r--r--   0        0        0    26082 2024-03-28 16:40:54.092717 krkn_lib-2.1.1/src/krkn_lib/telemetry/k8s/krkn_telemetry_kubernetes.py
--rw-r--r--   0        0        0       48 2024-03-28 16:39:01.088531 krkn_lib-2.1.1/src/krkn_lib/telemetry/ocp/__init__.py
--rw-r--r--   0        0        0     7085 2024-03-28 16:39:01.088531 krkn_lib-2.1.1/src/krkn_lib/telemetry/ocp/krkn_telemetry_openshift.py
--rw-r--r--   0        0        0       33 2024-03-28 16:39:01.092531 krkn_lib-2.1.1/src/krkn_lib/tests/__init__.py
--rw-r--r--   0        0        0    12912 2024-03-28 16:39:01.092531 krkn_lib-2.1.1/src/krkn_lib/tests/base_test.py
--rw-r--r--   0        0        0     1334 2024-03-28 16:40:54.144717 krkn_lib-2.1.1/src/krkn_lib/tests/test_krkn_elastic.py
--rw-r--r--   0        0        0    34137 2024-03-28 16:39:01.092531 krkn_lib-2.1.1/src/krkn_lib/tests/test_krkn_kubernetes.py
--rw-r--r--   0        0        0     3858 2024-03-28 16:39:01.092531 krkn_lib-2.1.1/src/krkn_lib/tests/test_krkn_openshift.py
--rw-r--r--   0        0        0     8807 2024-03-28 16:39:01.092531 krkn_lib-2.1.1/src/krkn_lib/tests/test_krkn_prometheus.py
--rw-r--r--   0        0        0    13447 2024-03-28 16:39:01.092531 krkn_lib-2.1.1/src/krkn_lib/tests/test_krkn_telemetry_kubernetes.py
--rw-r--r--   0        0        0     6685 2024-03-28 16:39:01.092531 krkn_lib-2.1.1/src/krkn_lib/tests/test_krkn_telemetry_models.py
--rw-r--r--   0        0        0     1961 2024-03-28 16:39:01.092531 krkn_lib-2.1.1/src/krkn_lib/tests/test_krkn_telemetry_openshift.py
--rw-r--r--   0        0        0     9874 2024-03-28 16:40:54.140717 krkn_lib-2.1.1/src/krkn_lib/tests/test_utils.py
--rw-r--r--   0        0        0       68 2024-03-28 16:39:01.092531 krkn_lib-2.1.1/src/krkn_lib/utils/__init__.py
--rw-r--r--   0        0        0    13066 2024-03-28 16:40:54.112717 krkn_lib-2.1.1/src/krkn_lib/utils/functions.py
--rw-r--r--   0        0        0     3687 2024-03-28 16:39:01.092531 krkn_lib-2.1.1/src/krkn_lib/utils/safe_logger.py
--rw-r--r--   0        0        0     2545 1970-01-01 00:00:00.000000 krkn_lib-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0    10173 2024-04-18 14:24:46.633674 krkn_lib-2.1.2/LICENSE
+-rw-r--r--   0        0        0     1389 2024-04-18 14:24:46.633674 krkn_lib-2.1.2/README.md
+-rw-r--r--   0        0        0     1130 2024-04-18 14:26:35.366471 krkn_lib-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0       39 2024-04-18 14:24:46.633674 krkn_lib-2.1.2/src/krkn_lib/k8s/__init__.py
+-rw-r--r--   0        0        0   108622 2024-04-18 14:26:38.090491 krkn_lib-2.1.2/src/krkn_lib/k8s/krkn_kubernetes.py
+-rw-r--r--   0        0        0     7583 2024-04-18 14:26:38.090491 krkn_lib-2.1.2/src/krkn_lib/k8s/pods_monitor_pool.py
+-rw-r--r--   0        0        0      462 2024-04-18 14:24:46.633674 krkn_lib-2.1.2/src/krkn_lib/k8s/templates/node_exec_pod.j2
+-rw-r--r--   0        0        0        0 2024-04-18 14:24:46.633674 krkn_lib-2.1.2/src/krkn_lib/models/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-18 14:24:46.633674 krkn_lib-2.1.2/src/krkn_lib/models/k8s/__init__.py
+-rw-r--r--   0        0        0     6557 2024-04-18 14:26:38.158492 krkn_lib-2.1.2/src/krkn_lib/models/k8s/models.py
+-rw-r--r--   0        0        0       30 2024-04-18 14:24:46.633674 krkn_lib-2.1.2/src/krkn_lib/models/krkn/__init__.py
+-rw-r--r--   0        0        0     2002 2024-04-18 14:24:46.633674 krkn_lib-2.1.2/src/krkn_lib/models/krkn/models.py
+-rw-r--r--   0        0        0       30 2024-04-18 14:24:46.633674 krkn_lib-2.1.2/src/krkn_lib/models/telemetry/__init__.py
+-rw-r--r--   0        0        0     7108 2024-04-18 14:24:46.633674 krkn_lib-2.1.2/src/krkn_lib/models/telemetry/models.py
+-rw-r--r--   0        0        0       38 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/ocp/__init__.py
+-rw-r--r--   0        0        0    15592 2024-04-18 14:26:38.118491 krkn_lib-2.1.2/src/krkn_lib/ocp/krkn_openshift.py
+-rw-r--r--   0        0        0        0 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/prometheus/__init__.py
+-rw-r--r--   0        0        0     9039 2024-04-18 14:26:38.110491 krkn_lib-2.1.2/src/krkn_lib/prometheus/krkn_prometheus.py
+-rw-r--r--   0        0        0        0 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/telemetry/__init__.py
+-rw-r--r--   0        0        0     1998 2024-04-18 14:26:38.094491 krkn_lib-2.1.2/src/krkn_lib/telemetry/elastic.py
+-rw-r--r--   0        0        0       49 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/telemetry/k8s/__init__.py
+-rw-r--r--   0        0        0    26359 2024-04-18 14:26:38.102491 krkn_lib-2.1.2/src/krkn_lib/telemetry/k8s/krkn_telemetry_kubernetes.py
+-rw-r--r--   0        0        0       48 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/telemetry/ocp/__init__.py
+-rw-r--r--   0        0        0     7085 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/telemetry/ocp/krkn_telemetry_openshift.py
+-rw-r--r--   0        0        0       33 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/tests/__init__.py
+-rw-r--r--   0        0        0    13973 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/tests/base_test.py
+-rw-r--r--   0        0        0     1334 2024-04-18 14:26:38.134492 krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_elastic.py
+-rw-r--r--   0        0        0    48352 2024-04-18 14:26:38.150492 krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_kubernetes.py
+-rw-r--r--   0        0        0     1718 2024-04-18 14:26:38.142491 krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_kubernetes_models.py
+-rw-r--r--   0        0        0     5234 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_kubernetes_pods_monitor_pool.py
+-rw-r--r--   0        0        0     3858 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_openshift.py
+-rw-r--r--   0        0        0     8807 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_prometheus.py
+-rw-r--r--   0        0        0    13447 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_telemetry_kubernetes.py
+-rw-r--r--   0        0        0     8348 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_telemetry_models.py
+-rw-r--r--   0        0        0     1961 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_telemetry_openshift.py
+-rw-r--r--   0        0        0     9874 2024-04-18 14:26:38.154492 krkn_lib-2.1.2/src/krkn_lib/tests/test_utils.py
+-rw-r--r--   0        0        0       68 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/utils/__init__.py
+-rw-r--r--   0        0        0    13066 2024-04-18 14:26:38.114491 krkn_lib-2.1.2/src/krkn_lib/utils/functions.py
+-rw-r--r--   0        0        0     3687 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/utils/safe_logger.py
+-rw-r--r--   0        0        0     2545 1970-01-01 00:00:00.000000 krkn_lib-2.1.2/PKG-INFO
```

### Comparing `krkn_lib-2.1.1/LICENSE` & `krkn_lib-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.1/README.md` & `krkn_lib-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.1/pyproject.toml` & `krkn_lib-2.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "krkn-lib"
-version = "v2.1.1"
+version = "v2.1.2"
 description = "Foundation library for Kraken"
 authors = ["Red Hat Chaos Team"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/redhat-chaos/krkn"
 #packages = [{include= "src/krkn_lib"}]
```

### Comparing `krkn_lib-2.1.1/src/krkn_lib/k8s/krkn_kubernetes.py` & `krkn_lib-2.1.2/src/krkn_lib/k8s/krkn_kubernetes.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,36 +3,43 @@
 import logging
 import os
 import random
 import re
 import tempfile
 import threading
 import time
+import warnings
+from concurrent.futures import ThreadPoolExecutor, wait
+from functools import partial
 from queue import Queue
 from typing import Dict, List, Optional
 
 import arcaflow_lib_kubernetes
 import kubernetes
+import urllib3
 import yaml
 from jinja2 import Environment, PackageLoader
 from kubeconfig import KubeConfig
 from kubernetes import client, config, utils, watch
 from kubernetes.client.rest import ApiException
 from kubernetes.dynamic.client import DynamicClient
 from kubernetes.stream import stream
 from urllib3 import HTTPResponse
 
 from krkn_lib.models.k8s import (
     PVC,
+    AffectedPod,
     ApiRequestException,
     ChaosEngine,
     ChaosResult,
     Container,
     LitmusChaosObject,
     Pod,
+    PodsMonitorThread,
+    PodsStatus,
     Volume,
     VolumeMount,
 )
 from krkn_lib.models.telemetry import NodeInfo, Taint
 from krkn_lib.utils import filter_dictionary
 from krkn_lib.utils.safe_logger import SafeLogger
 
@@ -76,14 +83,19 @@
         >>> KrknKubernetes(log_writer, "/home/test/.kube/config")
 
         Initialization with kubeconfig string:
 
         >>> kubeconfig_string="apiVersion: v1 ....."
         >>> KrknKubernetes(log_writer, kubeconfig_string=kubeconfig_string)
         """
+        urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+        urllib3.disable_warnings(DeprecationWarning)
+        warnings.filterwarnings(
+            action="ignore", message="unclosed", category=ResourceWarning
+        )
 
         if kubeconfig_string is not None and kubeconfig_path is not None:
             raise Exception(
                 "please use either a kubeconfig path "
                 "or a valid kubeconfig string"
             )
 
@@ -2421,14 +2433,33 @@
             for status in response.status.container_statuses:
                 if not status.ready:
                     is_ready = False
             return is_ready
         except Exception:
             return False
 
+    def is_pod_terminating(self, pod_name: str, namespace: str) -> bool:
+        """
+        Checks if a pod is scheduled for deletion so it's terminating
+
+        :param pod_name:str: the name of the pod to check
+        :param namespace:str: the namespace of the pod to check
+        :return: True if is Terminating or False if not
+        """
+        try:
+            response = self.cli.read_namespaced_pod(
+                name=pod_name, namespace=namespace, pretty="true"
+            )
+            if response.metadata.deletion_timestamp:
+                return True
+
+            return False
+        except Exception:
+            return False
+
     def collect_cluster_events(
         self,
         start_timestamp: int,
         end_timestamp: int,
         local_timezone: str,
         cluster_timezone: str = "UTC",
         limit: int = 500,
@@ -2544,7 +2575,425 @@
             return json_obj["status"]["token"]
         except Exception as e:
             logging.error(
                 f"failed to create token for SA: {service_account} "
                 f"on namespace: {namespace} with error: {e}"
             )
             return None
+
+    def select_pods_by_label(self, label_selector: str) -> list[(str, str)]:
+        """
+        Selects the pods identified by a label_selector
+
+        :param label_selector: a label selector string
+            in the format "key=value"
+        :param max_timeout: the maximum time in seconds
+            to wait before considering the pod "not recovered" after the Chaos
+        :return: a list of pod_name and namespace tuples
+        """
+        pods_and_namespaces = self.get_all_pods(label_selector)
+        pods_and_namespaces = [(pod[0], pod[1]) for pod in pods_and_namespaces]
+        # select only running pods
+        pods_and_namespaces = [
+            pod
+            for pod in pods_and_namespaces
+            if not self.is_pod_terminating(pod[0], pod[1])
+        ]
+        return pods_and_namespaces
+
+    def select_pods_by_name_pattern_and_namespace_pattern(
+        self, pod_name_pattern: str, namespace_pattern: str
+    ) -> list[(str, str)]:
+        """
+        Selects the pods identified by a namespace_pattern
+        and a pod_name pattern.
+
+        :param pod_name_pattern: a pod_name pattern to match
+        :param namespace_pattern: a namespace pattern to match
+        :param max_timeout: the maximum time in seconds to wait
+            before considering the pod "not recovered" after the Chaos
+        :return: a list of pod_name and namespace tuples
+        """
+        namespace_re = re.compile(namespace_pattern)
+        podname_re = re.compile(pod_name_pattern)
+        namespaces = self.list_namespaces()
+        pods_and_namespaces = []
+        for namespace in namespaces:
+            if namespace_re.match(namespace):
+                pods = self.list_pods(namespace)
+                for pod in pods:
+                    if podname_re.match(pod):
+                        pods_and_namespaces.append((pod, namespace))
+        # select only running pods
+        pods_and_namespaces = [
+            (pod[0], pod[1])
+            for pod in pods_and_namespaces
+            if not self.is_pod_terminating(pod[0], pod[1])
+        ]
+        return pods_and_namespaces
+
+    def select_pods_by_namespace_pattern_and_label(
+        self, namespace_pattern: str, label_selector: str
+    ) -> list[(str, str)]:
+        """
+        Selects the pods identified by a label_selector
+        and a namespace pattern
+
+        :param namespace_pattern: a namespace pattern to match
+        :param label_selector: a label selector string
+            in the format "key=value"
+        :param max_timeout: the maximum time in seconds
+            to wait before considering the pod "not recovered" after the Chaos
+        :return: a list of pod_name and namespace tuples
+        """
+        namespace_re = re.compile(namespace_pattern)
+        pods_and_namespaces = self.get_all_pods(label_selector)
+        pods_and_namespaces = [
+            pod for pod in pods_and_namespaces if namespace_re.match(pod[1])
+        ]
+        # select only running pods
+        pods_and_namespaces = [
+            (pod[0], pod[1])
+            for pod in pods_and_namespaces
+            if not self.is_pod_terminating(pod[0], pod[1])
+        ]
+        return pods_and_namespaces
+
+    def monitor_pods_by_label(
+        self,
+        label_selector: str,
+        pods_and_namespaces: list[(str, str)],
+        max_timeout: int = 30,
+        event: threading.Event = None,
+    ) -> PodsMonitorThread:
+        """
+        Starts monitoring a list of pods identified as tuples
+        (pod_name, namespace) filtered by label selector
+        and collects infos about the pods recovery after a kill scenario.
+        Returns a PodsMonitorThread that can be joined after the scenario
+        to retrieve the PodsStatus object containing all the information
+        collected in background during the chaos run.
+
+        :param label_selector: the label selector used
+            to filter the pods to monitor (must be the
+            same used in `select_pods_by_label`)
+        :param pods_and_namespaces: the list of pods collected
+            by `select_pods_by_label` against which the changes
+            in the pods state is monitored
+        :param max_timeout: the expected time the pods should take
+            to recover. If the killed pods are replaced in this time frame,
+            but they didn't reach the Ready State, they will be marked as
+            unrecovered. If during the time frame the pods are not replaced
+            at all the error field of the PodsStatus structure will be
+            valorized with an exception.
+        :param event: a threading event can be passed to interrupt the process
+            before the timeout. Simply call set() method on the event passed
+            to make the thread return immediately
+        :return: a PodsMonitorThread structure that can be joined
+            in any place of the code, to collect the PodsStatus structure
+            returned, in order to make the process run in background
+            while a chaos scenario is performed.
+
+        """
+        pods_status = PodsStatus()
+        return self.__start_monitoring_pods(
+            pods_and_namespaces=pods_and_namespaces,
+            max_timeout=max_timeout,
+            pods_status=pods_status,
+            label_selector=label_selector,
+            event=event,
+        )
+
+    def monitor_pods_by_name_pattern_and_namespace_pattern(
+        self,
+        pod_name_pattern: str,
+        namespace_pattern: str,
+        pods_and_namespaces: list[(str, str)],
+        max_timeout=30,
+        event: threading.Event = None,
+    ) -> PodsMonitorThread:
+        """
+        Starts monitoring a list of pods identified as tuples
+        (pod_name, namespace) filtered by a pod name regex pattern
+        and a namespace regex pattern, and collects infos about the
+        pods recovery after a kill scenario. Returns a PodsMonitorThread
+        that can be joined after the scenario to retrieve the PodsStatus
+        object containing all the information collected in background during
+        the chaos run.
+
+        :param pod_name_pattern: a regex representing the
+            pod name pattern used to filter the pods to be monitored
+            (must be the same used in
+            `select_pods_by_name_pattern_and_namespace_pattern`)
+        :param namespace_pattern: a regex representing the namespace
+            pattern used to filter the pods to be monitored
+            (must be the same used in
+            `select_pods_by_name_pattern_and_namespace_pattern`)
+        :param pods_and_namespaces: the list of pods collected by
+            `select_pods_by_name_pattern_and_namespace_pattern` against
+            which the changes in the pods state is monitored
+        :param max_timeout: the expected time the pods should take to
+            recover. If the killed pods are replaced in this time frame,
+            but they didn't reach the Ready State, they will be marked as
+            unrecovered. If during the time frame the pods are not replaced
+            at all the error field of the PodsStatus structure will be
+            valorized with an exception.
+        :param event: a threading event can be passed to interrupt the process
+            before the timeout. Simply call set() method on the event passed
+            to make the thread return immediately
+        :return: a PodsMonitorThread structure that can be joined in any
+            place of the code, to collect the PodsStatus structure returned,
+            in order to make the process run in background while a chaos
+            scenario is performed.
+
+        """
+        pods_status = PodsStatus()
+        return self.__start_monitoring_pods(
+            pods_and_namespaces=pods_and_namespaces,
+            max_timeout=max_timeout,
+            pods_status=pods_status,
+            name_pattern=pod_name_pattern,
+            namespace_pattern=namespace_pattern,
+            event=event,
+        )
+
+    def monitor_pods_by_namespace_pattern_and_label(
+        self,
+        namespace_pattern: str,
+        label_selector: str,
+        pods_and_namespaces: list[(str, str)],
+        max_timeout=30,
+        event: threading.Event = None,
+    ) -> PodsMonitorThread:
+        """
+        Starts monitoring a list of pods identified as tuples
+        (pod_name, namespace) filtered by a namespace regex pattern
+        and a pod label selector, and collects infos about the
+        pods recovery after a kill scenario. Returns a PodsMonitorThread
+        that can be joined after the scenario to retrieve the PodsStatus
+        object containing all the information collected in background during
+        the chaos run.
+
+        :param label_selector: the label selector used to filter
+            the pods to monitor (must be the same used in
+            `select_pods_by_label`)
+        :param namespace_pattern: a regex representing the namespace
+            pattern used to filter the pods to be monitored (must be
+            the same used
+            in `select_pods_by_name_pattern_and_namespace_pattern`)
+        :param pods_and_namespaces: the list of pods collected by
+            `select_pods_by_name_pattern_and_namespace_pattern` against
+            which the changes in the pods state is monitored
+        :param max_timeout: the expected time the pods should take to recover.
+            If the killed pods are replaced in this time frame, but they
+            didn't reach the Ready State, they will be marked as unrecovered.
+            If during the time frame the pods are not replaced
+            at all the error field of the PodsStatus structure will be
+            valorized with an exception.
+        :param event: a threading event can be passed to interrupt the process
+            before the timeout. Simply call set() method on the event passed
+            to make the thread return immediately
+        :return: a PodsMonitorThread structure that can be joined in
+            any place of the code, to collect the PodsStatus structure
+            returned, in order to make the process run in background while
+            a chaos scenario is performed.
+
+        """
+        pods_status = PodsStatus()
+        return self.__start_monitoring_pods(
+            pods_and_namespaces=pods_and_namespaces,
+            max_timeout=max_timeout,
+            pods_status=pods_status,
+            label_selector=label_selector,
+            namespace_pattern=namespace_pattern,
+            event=event,
+        )
+
+    def __start_monitoring_pods(
+        self,
+        pods_and_namespaces: list[(str, str)],
+        pods_status: PodsStatus,
+        max_timeout: int,
+        label_selector: str = None,
+        pod_name: str = None,
+        namespace_pattern: str = None,
+        name_pattern: str = None,
+        event: threading.Event = None,
+    ) -> PodsMonitorThread:
+        executor = ThreadPoolExecutor()
+        future = executor.submit(
+            self.__monitor_pods_worker,
+            pods_and_namespaces=pods_and_namespaces,
+            pods_status=pods_status,
+            max_timeout=max_timeout,
+            label_selector=label_selector,
+            pod_name=pod_name,
+            namespace_pattern=namespace_pattern,
+            name_pattern=name_pattern,
+            event=event,
+        )
+
+        return PodsMonitorThread(executor, future)
+
+    def __monitor_pods_worker(
+        self,
+        pods_and_namespaces: [(str, str)],
+        pods_status: PodsStatus,
+        max_timeout: int,
+        label_selector: str = None,
+        pod_name: str = None,
+        namespace_pattern: str = None,
+        name_pattern: str = None,
+        event: threading.Event = None,
+    ) -> PodsStatus:
+        missing_pods = set()
+        pods_to_wait = set()
+        pods_already_watching = set()
+        start_time = time.time()
+        _event = threading.Event() if not event else event
+        if (
+            label_selector
+            and not pod_name
+            and not name_pattern
+            and not namespace_pattern
+        ):
+            select_method = partial(
+                self.select_pods_by_label,
+                label_selector=label_selector,
+            )
+        elif (
+            name_pattern
+            and namespace_pattern
+            and not pod_name
+            and not label_selector
+        ):
+            select_method = partial(
+                self.select_pods_by_name_pattern_and_namespace_pattern,
+                pod_name_pattern=name_pattern,
+                namespace_pattern=namespace_pattern,
+            )
+        elif (
+            namespace_pattern
+            and label_selector
+            and not pod_name
+            and not name_pattern
+        ):
+            select_method = partial(
+                self.select_pods_by_namespace_pattern_and_label,
+                namespace_pattern=namespace_pattern,
+                label_selector=label_selector,
+            )
+        else:
+            pods_status.error = (
+                "invalid parameter combination, "
+                "check hasn't been performed, aborting."
+            )
+            return pods_status
+
+        while time.time() - start_time <= max_timeout:
+            if event:
+                if event.is_set():
+                    return pods_status
+
+            time_offset = time.time() - start_time
+            remaining_time = max_timeout - time_offset
+            current_pods_and_namespaces = select_method()
+
+            # no pods have been killed or pods have been killed and
+            # respawned with the same names
+            if set(pods_and_namespaces) == set(current_pods_and_namespaces):
+                if len(missing_pods) == 0:
+                    continue
+                # in this case the pods to wait have been respawn
+                # with the same name
+                pods_to_wait.update(missing_pods)
+
+            # pods have been killed but respawned with different names
+            elif set(pods_and_namespaces) != set(
+                current_pods_and_namespaces
+            ) and len(pods_and_namespaces) <= len(current_pods_and_namespaces):
+                # in this case the pods to wait have been respawn
+                # with different names
+                pods_to_wait.update(
+                    set(current_pods_and_namespaces) - set(pods_and_namespaces)
+                )
+
+            # pods have been killed and are not
+            # respawned yet (missing pods names
+            # are collected
+            elif set(pods_and_namespaces) != set(
+                current_pods_and_namespaces
+            ) and len(pods_and_namespaces) > len(current_pods_and_namespaces):
+                # update on missing_pods set is idempotent since the tuple
+                # pod_name,namespace is unique in the cluster
+                missing_pods.update(
+                    set(pods_and_namespaces) - set(current_pods_and_namespaces)
+                )
+                continue
+            # no change has been made in the pod set,
+            # maybe is taking some time to
+            # inject the chaos, let's see the next iteration.
+            if len(pods_to_wait) == 0:
+                continue
+
+            futures = []
+
+            with ThreadPoolExecutor() as executor:
+                for pod_and_namespace in pods_to_wait:
+                    if pod_and_namespace not in pods_already_watching:
+                        future = executor.submit(
+                            self.__wait_until_pod_is_ready_worker,
+                            pod_name=pod_and_namespace[0],
+                            namespace=pod_and_namespace[1],
+                            event=_event,
+                        )
+                        futures.append(future)
+                        pods_already_watching.add(pod_and_namespace)
+
+                # this will wait all the futures to
+                # finish within the remaining time
+                done, undone = wait(futures, timeout=remaining_time)
+                _event.set()
+                for future in done:
+                    result = future.result()
+                    # sum the time elapsed waiting before the pod
+                    # has been rescheduled (rescheduling time)
+                    # to the effective recovery time of the pod
+                    result.pod_rescheduling_time = time.time() - start_time
+                    result.total_recovery_time = (
+                        result.pod_readiness_time
+                        + result.pod_rescheduling_time
+                    )
+
+                    pods_status.recovered.append(result)
+                for future in undone:
+                    result = future.result()
+                    pods_status.unrecovered.append(result)
+
+                missing_pods.clear()
+        # if there are missing pods, pods affected
+        # by the chaos did not restart after the chaos
+        # an exception will be set in the PodsStatus
+        # structure that will be catched at the end of
+        # the monitoring,
+        if len(missing_pods) > 0:
+            if not _event.is_set():
+                pods_status.error = f'{", ".join([f"pod: {p[0]} namespace:{p[1]}" for p in missing_pods])}'  # NOQA
+
+        return pods_status
+
+    def __wait_until_pod_is_ready_worker(
+        self, pod_name: str, namespace: str, event: threading.Event
+    ) -> AffectedPod:
+        start_time = time.time()
+        ready = False
+
+        while not ready and not event.is_set():
+            ready = self.is_pod_running(pod_name, namespace)
+        end_time = time.time()
+        pod = AffectedPod(
+            pod_name=pod_name,
+            namespace=namespace,
+        )
+        if not event.is_set():
+            pod.pod_readiness_time = end_time - start_time
+        return pod
```

### Comparing `krkn_lib-2.1.1/src/krkn_lib/models/krkn/models.py` & `krkn_lib-2.1.2/src/krkn_lib/models/krkn/models.py`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.1/src/krkn_lib/models/telemetry/models.py` & `krkn_lib-2.1.2/src/krkn_lib/models/telemetry/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import base64
 import json
 from dataclasses import dataclass
 
 import yaml
 
+from krkn_lib.models.k8s import PodsStatus
+
 
 @dataclass(order=False)
 class ScenarioTelemetry:
     """
     Scenario Telemetry collection
     """
 
@@ -25,26 +27,33 @@
     """
     exit_status: int
     """
     Exit Status of the Scenario Run
     """
     parameters_base64: str
     """
-        Scenario configuration file base64 encoded
+    Scenario configuration file base64 encoded
     """
     parameters: any
 
+    """
+    Pods affected by the chaos scenario
+    """
+
+    affected_pods: PodsStatus
+
     def __init__(self, json_object: any = None):
         if json_object is not None:
             self.start_timestamp = int(json_object.get("start_timestamp"))
             self.end_timestamp = int(json_object.get("end_timestamp"))
             self.scenario = json_object.get("scenario")
             self.exit_status = json_object.get("exit_status")
             self.parameters_base64 = json_object.get("parameters_base64")
             self.parameters = json_object.get("parameters")
+            self.affected_pods = PodsStatus(json_object.get("affected_pods"))
 
             if (
                 self.parameters_base64 is not None
                 and self.parameters_base64 != ""
             ):
                 try:
                     yaml_params = base64.b64decode(self.parameters_base64)
@@ -65,14 +74,15 @@
             # property are initialized so are available
             self.start_timestamp = 0
             self.end_timestamp = 0
             self.scenario = ""
             self.exit_status = 0
             self.parameters_base64 = ""
             self.parameters = {}
+            self.affected_pods = PodsStatus()
 
 
 @dataclass(order=False)
 class Taint:
     """
     Cluster Node Taint details
     """
@@ -189,14 +199,16 @@
     Cloud infrastructure (if available) of the target cluster
     """
     run_uuid: str = ""
     """
     Run uuid generated by Krkn for the Run
     """
 
+    affected_pods: PodsStatus = PodsStatus()
+
     def __init__(self, json_object: any = None):
         self.scenarios = list[ScenarioTelemetry]()
         self.node_summary_infos = list[NodeInfo]()
         self.node_taints = list[Taint]()
         self.kubernetes_objects_count = dict[str, int]()
         self.network_plugins = ["Unknown"]
         if json_object is not None:
```

### Comparing `krkn_lib-2.1.1/src/krkn_lib/ocp/krkn_openshift.py` & `krkn_lib-2.1.2/src/krkn_lib/ocp/krkn_openshift.py`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.1/src/krkn_lib/prometheus/krkn_prometheus.py` & `krkn_lib-2.1.2/src/krkn_lib/prometheus/krkn_prometheus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import logging
 import math
 import re
 import sys
 import time
+import warnings
 from datetime import datetime, timedelta
 from io import StringIO
 from typing import Optional
 
+import urllib3
 from prometheus_api_client import PrometheusConnect
 
 
 class KrknPrometheus:
     prom_cli: PrometheusConnect
 
     def __init__(
@@ -21,14 +23,20 @@
         Endpoint url and the bearer token to access it (optional if
         the endpoint doesn't need authentication).
 
         :param prometheus_url: the prometheus API endpoint
         :param prometheus_bearer_token: the bearer token to authenticate
             the query (optional).
         """
+
+        urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+        urllib3.disable_warnings(DeprecationWarning)
+        warnings.filterwarnings(
+            action="ignore", message="unclosed", category=ResourceWarning
+        )
         headers = {}
         if prometheus_bearer_token is not None:
             bearer = "Bearer " + prometheus_bearer_token
             headers = {"Authorization": bearer}
         try:
             self.prom_cli = PrometheusConnect(
                 url=prometheus_url, headers=headers, disable_ssl=True
```

### Comparing `krkn_lib-2.1.1/src/krkn_lib/telemetry/elastic.py` & `krkn_lib-2.1.2/src/krkn_lib/telemetry/elastic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import time
 
+import urllib3
 from elasticsearch import Elasticsearch
 
 from krkn_lib.utils.safe_logger import SafeLogger
 
 
 class KrknElastic:
     es = None
 
     def __init__(self, safe_logger: SafeLogger, elastic_url: str):
+        urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+        urllib3.disable_warnings(DeprecationWarning)
         self.safe_logger = safe_logger
         try:
             # create Elasticsearch object
             if elastic_url:
                 self.es = Elasticsearch(f"{elastic_url}:443")
         except Exception as e:
             self.safe_logger.error("Failed to initalize elasticsearch: %s" % e)
```

### Comparing `krkn_lib-2.1.1/src/krkn_lib/telemetry/k8s/krkn_telemetry_kubernetes.py` & `krkn_lib-2.1.2/src/krkn_lib/telemetry/k8s/krkn_telemetry_kubernetes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import base64
 import os
 import tempfile
 import threading
 import time
+import warnings
 from queue import Queue
 from typing import Optional
 
 import requests
+import urllib3
 import yaml
 from tzlocal import get_localzone
 
 import krkn_lib.utils as utils
 from krkn_lib.k8s import KrknKubernetes
 from krkn_lib.models.krkn import ChaosRunAlertSummary
 from krkn_lib.models.telemetry import ChaosRunTelemetry, ScenarioTelemetry
@@ -21,14 +23,19 @@
     kubecli: KrknKubernetes = None
     safe_logger: SafeLogger = None
     default_telemetry_group = "default"
 
     def __init__(
         self, safe_logger: SafeLogger, lib_kubernetes: KrknKubernetes
     ):
+        urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+        urllib3.disable_warnings(DeprecationWarning)
+        warnings.filterwarnings(
+            action="ignore", message="unclosed", category=ResourceWarning
+        )
         self.kubecli = lib_kubernetes
         self.safe_logger = safe_logger
 
     def collect_cluster_metadata(self, chaos_telemetry: ChaosRunTelemetry):
         """
         Collects useful cluster metadata:
         - cloud infrastructure
```

### Comparing `krkn_lib-2.1.1/src/krkn_lib/telemetry/ocp/krkn_telemetry_openshift.py` & `krkn_lib-2.1.2/src/krkn_lib/telemetry/ocp/krkn_telemetry_openshift.py`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.1/src/krkn_lib/tests/base_test.py` & `krkn_lib-2.1.2/src/krkn_lib/tests/base_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import cProfile
 import logging
 import random
 import string
 import sys
 import tempfile
+import threading
 import time
 import unittest
 from typing import Dict, List
 
 import requests
 import yaml
 from jinja2 import Environment, FileSystemLoader
@@ -22,41 +24,55 @@
 
 
 class BaseTest(unittest.TestCase):
     lib_k8s: KrknKubernetes
     lib_ocp: KrknOpenshift
     lib_telemetry_k8s: KrknTelemetryKubernetes
     lib_telemetry_ocp: KrknTelemetryOpenshift
+    pr: cProfile.Profile
 
     @classmethod
     def setUpClass(cls):
         cls.lib_k8s = KrknKubernetes(config.KUBE_CONFIG_DEFAULT_LOCATION)
         cls.lib_ocp = KrknOpenshift(config.KUBE_CONFIG_DEFAULT_LOCATION)
         cls.lib_telemetry_k8s = KrknTelemetryKubernetes(
             SafeLogger(), cls.lib_k8s
         )
         cls.lib_telemetry_ocp = KrknTelemetryOpenshift(
             SafeLogger(), cls.lib_ocp
         )
         host = cls.lib_k8s.api_client.configuration.host
         logging.disable(logging.CRITICAL)
+        # PROFILER
+        # """init each test"""
+        # cls.pr = cProfile.Profile()
+        # cls.pr.enable()
+        # print("\n<<<---")
         try:
             requests.get(host, timeout=2, verify=False)
         except ConnectTimeout:
             logging.error(
                 "Unable to connect to Kubernetes API %s.\n"
                 "To run the tests please setup a running k8s cluster.\n"
                 "To have a local working k8s cluster "
                 "visit https://minikube.sigs.k8s.io/docs/\n",
                 host,
             )
             sys.exit(1)
 
     @classmethod
     def tearDownClass(cls) -> None:
+        # PROFILER
+        # """finish any test"""
+        # p = Stats(cls.pr)
+        # p.strip_dirs()
+        # p.sort_stats("cumtime")
+        # p.print_stats()
+        # print
+        # "\n--->>>"
         pass
 
     def wait_pod(
         self, name: str, namespace: str = "default", timeout: int = 60
     ):
         runtime = 0
         while True:
@@ -103,14 +119,24 @@
 
     def depoy_alpine(self, name: str, namespace: str = "default"):
         environment = Environment(loader=FileSystemLoader("src/testdata/"))
         template = environment.get_template("alpine.j2")
         content = template.render(name=name, namespace=namespace)
         self.apply_template(content)
 
+    def deploy_delayed_readiness_pod(
+        self, name: str, namespace: str, delay: int, label: str = "readiness"
+    ):
+        environment = Environment(loader=FileSystemLoader("src/testdata/"))
+        template = environment.get_template("delayed_readiness_pod.j2")
+        content = template.render(
+            name=name, namespace=namespace, delay=delay, label=label
+        )
+        self.apply_template(content)
+
     def deploy_persistent_volume(
         self, name: str, storage_class: str, namespace: str
     ):
         template = self.template_to_pv(name, storage_class, namespace)
         self.apply_template(template)
 
     def deploy_persistent_volume_claim(
@@ -358,7 +384,14 @@
                 print("Service already present")
         except Exception as e:
             logging.error(
                 "Exception when calling " "CoreV1Api->create_service: %s",
                 str(e),
             )
             raise e
+
+    def background_delete_pod(self, pod_name: str, namespace: str):
+        thread = threading.Thread(
+            target=self.lib_k8s.delete_pod, args=(pod_name, namespace)
+        )
+        thread.daemon = True
+        thread.start()
```

### Comparing `krkn_lib-2.1.1/src/krkn_lib/tests/test_krkn_elastic.py` & `krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_elastic.py`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.1/src/krkn_lib/tests/test_krkn_openshift.py` & `krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_openshift.py`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.1/src/krkn_lib/tests/test_krkn_prometheus.py` & `krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_prometheus.py`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.1/src/krkn_lib/tests/test_krkn_telemetry_kubernetes.py` & `krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_telemetry_kubernetes.py`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.1/src/krkn_lib/tests/test_krkn_telemetry_models.py` & `krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_telemetry_models.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,36 @@
     def test_scenario_telemetry(self):
         test_valid_json = """
         {
             "start_timestamp": 1686141432,
             "end_timestamp": 1686141435,
             "scenario": "test",
             "exit_status": 0,
-            "parameters_base64": "cHJvcGVydHk6CiAgICB1bml0OiB1bml0CiAgICB0ZXN0OiB0ZXN0"
+            "parameters_base64": "cHJvcGVydHk6CiAgICB1bml0OiB1bml0CiAgICB0ZXN0OiB0ZXN0",
+            "affected_pods":{
+                "recovered":[
+                    {
+                        "pod_name":"test-pod",
+                        "namespace":"test-namespace",
+                        "pod_rescheduling_time":9.8,
+                        "pod_readiness_time":2.71,
+                        "total_recovery_time":3.14
+                    }
+                ],
+                "unrecovered":[
+                    {
+                        "pod_name":"failed-pod-1",
+                        "namespace":"failed-namespace"
+                    },
+                    {
+                        "pod_name":"failed-pod-2",
+                        "namespace":"failed-namespace"
+                    }
+                ]
+             }
         }
         """  # NOQA
         # wrong base64 format
         test_invalid_json_wrong_base64 = """
         {
             "start_timestamp": 1686141432,
             "end_timestamp": 1686141435,
@@ -39,14 +60,29 @@
         json_obj = json.loads(test_valid_json)
 
         telemetry = ScenarioTelemetry(json_obj)
         self.assertEqual(telemetry.start_timestamp, 1686141432)
         self.assertEqual(telemetry.end_timestamp, 1686141435)
         self.assertEqual(telemetry.scenario, "test")
         self.assertEqual(telemetry.exit_status, 0)
+        self.assertIsNotNone(telemetry.affected_pods)
+        self.assertEqual(len(telemetry.affected_pods.recovered), 1)
+        self.assertEqual(len(telemetry.affected_pods.unrecovered), 2)
+        for recovered in telemetry.affected_pods.recovered:
+            self.assertIsNotNone(recovered.pod_name)
+            self.assertIsNotNone(recovered.namespace)
+            self.assertIsNotNone(recovered.pod_readiness_time)
+            self.assertIsNotNone(recovered.pod_rescheduling_time)
+            self.assertIsNotNone(recovered.total_recovery_time)
+        for unrecovered in telemetry.affected_pods.unrecovered:
+            self.assertIsNotNone(unrecovered.pod_name)
+            self.assertIsNotNone(unrecovered.namespace)
+            self.assertIsNone(unrecovered.pod_readiness_time)
+            self.assertIsNone(unrecovered.pod_rescheduling_time)
+            self.assertIsNone(unrecovered.total_recovery_time)
         self.assertIsNotNone(telemetry.parameters)
         self.assertEqual(telemetry.parameters_base64, "")
         self.assertEqual(telemetry.parameters["property"]["unit"], "unit")
         self.assertEqual(telemetry.parameters["property"]["test"], "test")
         with self.assertRaises(Exception):
             ScenarioTelemetry(json.loads(test_invalid_json_wrong_base64))
         with self.assertRaises(Exception):
```

### Comparing `krkn_lib-2.1.1/src/krkn_lib/tests/test_krkn_telemetry_openshift.py` & `krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_telemetry_openshift.py`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.1/src/krkn_lib/tests/test_utils.py` & `krkn_lib-2.1.2/src/krkn_lib/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.1/src/krkn_lib/utils/functions.py` & `krkn_lib-2.1.2/src/krkn_lib/utils/functions.py`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.1/src/krkn_lib/utils/safe_logger.py` & `krkn_lib-2.1.2/src/krkn_lib/utils/safe_logger.py`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.1/PKG-INFO` & `krkn_lib-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krkn-lib
-Version: 2.1.1
+Version: 2.1.2
 Summary: Foundation library for Kraken
 Home-page: https://github.com/redhat-chaos/krkn
 License: Apache-2.0
 Author: Red Hat Chaos Team
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

