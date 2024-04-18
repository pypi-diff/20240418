# Comparing `tmp/paka-0.1.2.tar.gz` & `tmp/paka-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paka-0.1.2.tar", max compression
+gzip compressed data, was "paka-0.1.3.tar", max compression
```

## Comparing `paka-0.1.2.tar` & `paka-0.1.3.tar`

### file list

```diff
@@ -1,56 +1,64 @@
--rw-r--r--   0        0        0     1072 2024-04-10 23:12:18.012434 paka-0.1.2/LICENSE
--rw-r--r--   0        0        0     4429 2024-04-10 23:12:18.012434 paka-0.1.2/README.md
--rw-r--r--   0        0        0      153 2024-04-10 23:12:18.016434 paka-0.1.2/paka/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cli/__init__.py
--rw-r--r--   0        0        0     1608 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cli/__main__.py
--rw-r--r--   0        0        0     1141 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cli/build.py
--rw-r--r--   0        0        0     3227 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cli/cluster.py
--rw-r--r--   0        0        0     6690 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cli/function.py
--rw-r--r--   0        0        0     5874 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cli/job.py
--rw-r--r--   0        0        0      427 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cli/kubeconfig.py
--rw-r--r--   0        0        0     2197 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cli/model_group.py
--rw-r--r--   0        0        0     3188 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cli/run.py
--rw-r--r--   0        0        0     8779 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cli/utils.py
--rw-r--r--   0        0        0        0 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/aws/__init__.py
--rw-r--r--   0        0        0     1037 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/aws/cloudwatch.py
--rw-r--r--   0        0        0     3113 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/aws/cluster_autoscaler.py
--rw-r--r--   0        0        0      722 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/aws/container_registry.py
--rw-r--r--   0        0        0     2521 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/aws/ebs_csi_driver.py
--rw-r--r--   0        0        0    12118 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/aws/eks.py
--rw-r--r--   0        0        0     1432 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/aws/elb.py
--rw-r--r--   0        0        0      725 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/aws/object_store.py
--rw-r--r--   0        0        0     4078 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/aws/service_account.py
--rw-r--r--   0        0        0     1874 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/aws/utils.py
--rw-r--r--   0        0        0     4643 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/fluentbit.py
--rw-r--r--   0        0        0     1228 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/keda.py
--rw-r--r--   0        0        0     4920 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/knative.py
--rw-r--r--   0        0        0        0 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/manager/__init__.py
--rw-r--r--   0        0        0     1210 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/manager/aws.py
--rw-r--r--   0        0        0     2737 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/manager/base.py
--rw-r--r--   0        0        0      879 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/namespace.py
--rw-r--r--   0        0        0     3414 2024-04-10 23:12:18.020434 paka-0.1.2/paka/cluster/nvidia_device_plugin.py
--rw-r--r--   0        0        0     4237 2024-04-10 23:12:18.020434 paka-0.1.2/paka/cluster/prometheus.py
--rw-r--r--   0        0        0     4000 2024-04-10 23:12:18.020434 paka-0.1.2/paka/cluster/qdrant.py
--rw-r--r--   0        0        0     2325 2024-04-10 23:12:18.020434 paka-0.1.2/paka/cluster/redis.py
--rw-r--r--   0        0        0      935 2024-04-10 23:12:18.020434 paka-0.1.2/paka/cluster/zipkin.py
--rw-r--r--   0        0        0    15359 2024-04-10 23:12:18.020434 paka-0.1.2/paka/config.py
--rw-r--r--   0        0        0      115 2024-04-10 23:12:18.020434 paka-0.1.2/paka/constants.py
--rw-r--r--   0        0        0     3015 2024-04-10 23:12:18.020434 paka-0.1.2/paka/container/ecr.py
--rw-r--r--   0        0        0     2374 2024-04-10 23:12:18.020434 paka-0.1.2/paka/container/pack.py
--rw-r--r--   0        0        0    19164 2024-04-10 23:12:18.020434 paka-0.1.2/paka/k8s.py
--rw-r--r--   0        0        0        0 2024-04-10 23:12:18.020434 paka-0.1.2/paka/kube_resources/function/__init__.py
--rw-r--r--   0        0        0     5706 2024-04-10 23:12:18.020434 paka-0.1.2/paka/kube_resources/function/service.py
--rw-r--r--   0        0        0        0 2024-04-10 23:12:18.020434 paka-0.1.2/paka/kube_resources/job/__init__.py
--rw-r--r--   0        0        0     2342 2024-04-10 23:12:18.020434 paka-0.1.2/paka/kube_resources/job/autoscaler.py
--rw-r--r--   0        0        0     4142 2024-04-10 23:12:18.020434 paka-0.1.2/paka/kube_resources/job/worker.py
--rw-r--r--   0        0        0        0 2024-04-10 23:12:18.020434 paka-0.1.2/paka/kube_resources/model_group/__init__.py
--rw-r--r--   0        0        0     2012 2024-04-10 23:12:18.020434 paka-0.1.2/paka/kube_resources/model_group/ingress.py
--rw-r--r--   0        0        0      131 2024-04-10 23:12:18.020434 paka-0.1.2/paka/kube_resources/model_group/manifest.py
--rw-r--r--   0        0        0     9969 2024-04-10 23:12:18.020434 paka-0.1.2/paka/kube_resources/model_group/model.py
--rw-r--r--   0        0        0    17462 2024-04-10 23:12:18.020434 paka-0.1.2/paka/kube_resources/model_group/service.py
--rw-r--r--   0        0        0     1105 2024-04-10 23:12:18.020434 paka-0.1.2/paka/kube_resources/model_group/supported_models.py
--rw-r--r--   0        0        0      761 2024-04-10 23:12:18.020434 paka-0.1.2/paka/logger.py
--rw-r--r--   0        0        0     9750 2024-04-10 23:12:18.020434 paka-0.1.2/paka/utils.py
--rw-r--r--   0        0        0     1262 2024-04-10 23:12:18.020434 paka-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5394 1970-01-01 00:00:00.000000 paka-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-18 06:53:43.507527 paka-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4570 2024-04-18 06:53:43.507527 paka-0.1.3/README.md
+-rw-r--r--   0        0        0      153 2024-04-18 06:53:43.511527 paka-0.1.3/paka/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cli/__init__.py
+-rw-r--r--   0        0        0     1608 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cli/__main__.py
+-rw-r--r--   0        0        0     1141 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cli/build.py
+-rw-r--r--   0        0        0     3263 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cli/cluster.py
+-rw-r--r--   0        0        0     6726 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cli/function.py
+-rw-r--r--   0        0        0     5910 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cli/job.py
+-rw-r--r--   0        0        0      427 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cli/kubeconfig.py
+-rw-r--r--   0        0        0     2233 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cli/model_group.py
+-rw-r--r--   0        0        0     3188 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cli/run.py
+-rw-r--r--   0        0        0     8815 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cli/utils.py
+-rw-r--r--   0        0        0        0 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/aws/__init__.py
+-rw-r--r--   0        0        0     1037 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/aws/cloudwatch.py
+-rw-r--r--   0        0        0     3113 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/aws/cluster_autoscaler.py
+-rw-r--r--   0        0        0      722 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/aws/container_registry.py
+-rw-r--r--   0        0        0     2521 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/aws/ebs_csi_driver.py
+-rw-r--r--   0        0        0    12154 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/aws/eks.py
+-rw-r--r--   0        0        0     1468 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/aws/elb.py
+-rw-r--r--   0        0        0      725 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/aws/object_store.py
+-rw-r--r--   0        0        0     4078 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/aws/service_account.py
+-rw-r--r--   0        0        0     1874 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/aws/utils.py
+-rw-r--r--   0        0        0     4643 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/fluentbit.py
+-rw-r--r--   0        0        0     1228 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/keda.py
+-rw-r--r--   0        0        0     4956 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/knative.py
+-rw-r--r--   0        0        0        0 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/manager/__init__.py
+-rw-r--r--   0        0        0     1210 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/manager/aws.py
+-rw-r--r--   0        0        0     2773 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/manager/base.py
+-rw-r--r--   0        0        0      879 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/namespace.py
+-rw-r--r--   0        0        0     3414 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/nvidia_device_plugin.py
+-rw-r--r--   0        0        0     4273 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/prometheus.py
+-rw-r--r--   0        0        0     4000 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/qdrant.py
+-rw-r--r--   0        0        0     2325 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/redis.py
+-rw-r--r--   0        0        0      935 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/zipkin.py
+-rw-r--r--   0        0        0    15395 2024-04-18 06:53:43.511527 paka-0.1.3/paka/config.py
+-rw-r--r--   0        0        0      115 2024-04-18 06:53:43.511527 paka-0.1.3/paka/constants.py
+-rw-r--r--   0        0        0     3015 2024-04-18 06:53:43.511527 paka-0.1.3/paka/container/ecr.py
+-rw-r--r--   0        0        0     2374 2024-04-18 06:53:43.511527 paka-0.1.3/paka/container/pack.py
+-rw-r--r--   0        0        0    19188 2024-04-18 06:53:43.511527 paka-0.1.3/paka/k8s.py
+-rw-r--r--   0        0        0        0 2024-04-18 06:53:43.511527 paka-0.1.3/paka/kube_resources/function/__init__.py
+-rw-r--r--   0        0        0     5742 2024-04-18 06:53:43.511527 paka-0.1.3/paka/kube_resources/function/service.py
+-rw-r--r--   0        0        0        0 2024-04-18 06:53:43.511527 paka-0.1.3/paka/kube_resources/job/__init__.py
+-rw-r--r--   0        0        0     2342 2024-04-18 06:53:43.511527 paka-0.1.3/paka/kube_resources/job/autoscaler.py
+-rw-r--r--   0        0        0     4142 2024-04-18 06:53:43.511527 paka-0.1.3/paka/kube_resources/job/worker.py
+-rw-r--r--   0        0        0        0 2024-04-18 06:53:43.511527 paka-0.1.3/paka/kube_resources/model_group/__init__.py
+-rw-r--r--   0        0        0     2048 2024-04-18 06:53:43.511527 paka-0.1.3/paka/kube_resources/model_group/ingress.py
+-rw-r--r--   0        0        0      131 2024-04-18 06:53:43.511527 paka-0.1.3/paka/kube_resources/model_group/manifest.py
+-rw-r--r--   0        0        0    10074 2024-04-18 06:53:43.511527 paka-0.1.3/paka/kube_resources/model_group/model.py
+-rw-r--r--   0        0        0    17498 2024-04-18 06:53:43.511527 paka-0.1.3/paka/kube_resources/model_group/service.py
+-rw-r--r--   0        0        0     1105 2024-04-18 06:53:43.511527 paka-0.1.3/paka/kube_resources/model_group/supported_models.py
+-rw-r--r--   0        0        0      761 2024-04-18 06:53:43.511527 paka-0.1.3/paka/logger.py
+-rw-r--r--   0        0        0        0 2024-04-18 06:53:43.511527 paka-0.1.3/paka/model/__init__.py
+-rw-r--r--   0        0        0     3188 2024-04-18 06:53:43.511527 paka-0.1.3/paka/model/base_model.py
+-rw-r--r--   0        0        0     2473 2024-04-18 06:53:43.511527 paka-0.1.3/paka/model/hf_model.py
+-rw-r--r--   0        0        0     1485 2024-04-18 06:53:43.511527 paka-0.1.3/paka/model/http_model.py
+-rw-r--r--   0        0        0     1648 2024-04-18 06:53:43.511527 paka-0.1.3/paka/model/manifest.py
+-rw-r--r--   0        0        0     2374 2024-04-18 06:53:43.511527 paka-0.1.3/paka/model/progress_bar.py
+-rw-r--r--   0        0        0     2671 2024-04-18 06:53:43.511527 paka-0.1.3/paka/model/settings.py
+-rw-r--r--   0        0        0     9467 2024-04-18 06:53:43.511527 paka-0.1.3/paka/model/store.py
+-rw-r--r--   0        0        0     9786 2024-04-18 06:53:43.511527 paka-0.1.3/paka/utils.py
+-rw-r--r--   0        0        0     1459 2024-04-18 06:53:43.511527 paka-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5830 1970-01-01 00:00:00.000000 paka-0.1.3/PKG-INFO
```

### Comparing `paka-0.1.2/LICENSE` & `paka-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `paka-0.1.2/README.md` & `paka-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,16 @@
 ## Contributing
 - Open a PR
 - Format and lint code with `make lint`
 - Run tests with `make test`
 
 ## Dependencies
 - docker daemon
+- pack cli (https://buildpacks.io/docs/for-platform-operators/how-to/integrate-ci/pack/)
+- pulumi cli (https://www.pulumi.com/docs/install/)
 - aws cli and credentials for the AWS deployment
 ```bash
 # Make sure aws credentials and cli are set up. Your aws credentials should have access to the following services:
 # - S3
 # - ECR
 # - EKS
 # - EC2
```

### Comparing `paka-0.1.2/paka/cli/__main__.py` & `paka-0.1.3/paka/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.2/paka/cli/build.py` & `paka-0.1.3/paka/cli/build.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.2/paka/cli/cluster.py` & `paka-0.1.3/paka/cli/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import List
 
 import click
 import typer
 
 from paka.cli.utils import load_cluster_manager
 from paka.k8s import remove_crd_finalizers
```

### Comparing `paka-0.1.2/paka/cli/function.py` & `paka-0.1.3/paka/cli/function.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Literal, Optional
 
 import click
 import typer
 from kubernetes.dynamic.exceptions import NotFoundError
 from tabulate import tabulate
```

### Comparing `paka-0.1.2/paka/cli/job.py` & `paka-0.1.3/paka/cli/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 from typing import Optional
 
 import click
 import typer
 from kubernetes import client
```

### Comparing `paka-0.1.2/paka/cli/model_group.py` & `paka-0.1.3/paka/cli/model_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Set
 
 import boto3
 import typer
 from kubernetes import client
 from tabulate import tabulate
```

### Comparing `paka-0.1.2/paka/cli/run.py` & `paka-0.1.3/paka/cli/run.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.2/paka/cli/utils.py` & `paka-0.1.3/paka/cli/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import functools
 import os
 import re
 import subprocess
 from typing import Any, Optional
 
 import typer
```

### Comparing `paka-0.1.2/paka/cluster/aws/cloudwatch.py` & `paka-0.1.3/paka/cluster/aws/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.2/paka/cluster/aws/cluster_autoscaler.py` & `paka-0.1.3/paka/cluster/aws/cluster_autoscaler.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.2/paka/cluster/aws/container_registry.py` & `paka-0.1.3/paka/cluster/aws/container_registry.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.2/paka/cluster/aws/ebs_csi_driver.py` & `paka-0.1.3/paka/cluster/aws/ebs_csi_driver.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.2/paka/cluster/aws/eks.py` & `paka-0.1.3/paka/cluster/aws/eks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Optional
 
 import pulumi
 import pulumi_aws as aws
 import pulumi_awsx as awsx
 import pulumi_eks as eks
 import pulumi_kubernetes as k8s
```

### Comparing `paka-0.1.2/paka/cluster/aws/elb.py` & `paka-0.1.3/paka/cluster/aws/elb.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import json
 from typing import Optional
 
 import boto3
 from kubernetes import client, config
```

### Comparing `paka-0.1.2/paka/cluster/aws/object_store.py` & `paka-0.1.3/paka/cluster/aws/object_store.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.2/paka/cluster/aws/service_account.py` & `paka-0.1.3/paka/cluster/aws/service_account.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.2/paka/cluster/aws/utils.py` & `paka-0.1.3/paka/cluster/aws/utils.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.2/paka/cluster/fluentbit.py` & `paka-0.1.3/paka/cluster/fluentbit.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.2/paka/cluster/keda.py` & `paka-0.1.3/paka/cluster/keda.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.2/paka/cluster/knative.py` & `paka-0.1.3/paka/cluster/knative.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from functools import partial
 from typing import Any, Callable, Dict
 
 import pulumi
 import pulumi_kubernetes as k8s
 from pulumi import ResourceOptions
 from pulumi_kubernetes.yaml import ConfigFile
```

### Comparing `paka-0.1.2/paka/cluster/manager/aws.py` & `paka-0.1.3/paka/cluster/manager/aws.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.2/paka/cluster/manager/base.py` & `paka-0.1.3/paka/cluster/manager/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
 from typing import Any
 
 from pulumi import automation as auto
 
 from paka.config import CloudConfig, Config
 from paka.kube_resources.model_group.ingress import (
```

### Comparing `paka-0.1.2/paka/cluster/namespace.py` & `paka-0.1.3/paka/cluster/namespace.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.2/paka/cluster/nvidia_device_plugin.py` & `paka-0.1.3/paka/cluster/nvidia_device_plugin.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.2/paka/cluster/prometheus.py` & `paka-0.1.3/paka/cluster/prometheus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Any, Callable, Dict, Optional, Tuple
 
 import pulumi
 import pulumi_kubernetes as k8s
 from pulumi_kubernetes.helm.v3 import Chart, ChartOpts, FetchOpts
 
 from paka.config import CloudConfig
```

### Comparing `paka-0.1.2/paka/cluster/qdrant.py` & `paka-0.1.3/paka/cluster/qdrant.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.2/paka/cluster/redis.py` & `paka-0.1.3/paka/cluster/redis.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.2/paka/cluster/zipkin.py` & `paka-0.1.3/paka/cluster/zipkin.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.2/paka/config.py` & `paka-0.1.3/paka/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import re
 from typing import Any, Dict, List, Optional, Union
 
 from pydantic import BaseModel, field_validator, model_validator
 from ruamel.yaml import YAML
 
 from paka.utils import to_yaml
```

### Comparing `paka-0.1.2/paka/container/ecr.py` & `paka-0.1.3/paka/container/ecr.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.2/paka/container/pack.py` & `paka-0.1.3/paka/container/pack.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.2/paka/k8s.py` & `paka-0.1.3/paka/k8s.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,24 @@
+from __future__ import annotations
+
 import contextlib
 import os
 import re
 import select
 import socket
 import threading
 import time
 from functools import partial
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    List,
-    Literal,
-    Optional,
-    Protocol,
-    Tuple,
-    TypeAlias,
-)
+from typing import Any, Callable, Dict, List, Literal, Optional, Protocol, Tuple
 
 from kubernetes import client, config, watch
 from kubernetes.client.rest import ApiException
 from kubernetes.stream import portforward
 from ruamel.yaml import YAML
+from typing_extensions import TypeAlias
 
 from paka.logger import logger
 from paka.utils import get_project_data_dir, read_yaml_file
 
 KubernetesResourceKind: TypeAlias = Literal[
     "Deployment",
     "Service",
```

### Comparing `paka-0.1.2/paka/kube_resources/function/service.py` & `paka-0.1.3/paka/kube_resources/function/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import shlex
 from typing import Any, Literal, Tuple
 
 from kubernetes import client
 from kubernetes.dynamic import DynamicClient
 from kubernetes.dynamic.exceptions import NotFoundError
```

### Comparing `paka-0.1.2/paka/kube_resources/job/autoscaler.py` & `paka-0.1.3/paka/kube_resources/job/autoscaler.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.2/paka/kube_resources/job/worker.py` & `paka-0.1.3/paka/kube_resources/job/worker.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.2/paka/kube_resources/model_group/ingress.py` & `paka-0.1.3/paka/kube_resources/model_group/ingress.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import List
 
 from kubernetes import client
 
 from paka.k8s import CustomResource, apply_resource
 from paka.utils import kubify_name
```

### Comparing `paka-0.1.2/paka/kube_resources/model_group/model.py` & `paka-0.1.3/paka/kube_resources/model_group/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,26 @@
+from __future__ import annotations
+
 import concurrent.futures
 import hashlib
-from typing import Any, Dict, List
+from typing import TYPE_CHECKING, Any, Dict, List
 
 import boto3
 import requests
-from botocore.client import BaseClient, Config
+from botocore.client import Config
 from botocore.exceptions import ClientError
 
 from paka.kube_resources.model_group.manifest import Manifest
 from paka.kube_resources.model_group.supported_models import SUPPORTED_MODELS
 from paka.logger import logger
 from paka.utils import read_current_cluster_data, to_yaml
 
+if TYPE_CHECKING:
+    from mypy_boto3_s3.client import S3Client
+
 MODEL_PATH_PREFIX = "models"
 
 
 def delete_s3_file(bucket_name: str, s3_file_name: str) -> None:
     s3 = boto3.client("s3")
     if s3_file_exists(bucket_name, s3_file_name):
         s3.delete_object(Bucket=bucket_name, Key=s3_file_name)
@@ -44,15 +49,15 @@
 
 def save_string_to_s3(bucket_name: str, file_name: str, data: str) -> None:
     s3 = boto3.resource("s3")
     s3.Object(bucket_name, file_name).put(Body=data)
 
 
 def upload_part(
-    s3: BaseClient,
+    s3: "S3Client",
     bucket_name: str,
     s3_file_name: str,
     upload_id: str,
     part_number: int,
     chunk: bytes,
 ) -> Dict[str, Any]:
     part = s3.upload_part(
@@ -200,14 +205,15 @@
 
     Raises:
         Exception: If the model is not supported or if the SHA256 hash of the downloaded file does not match.
 
     Returns:
         None
     """
+
     if name not in SUPPORTED_MODELS:
         logger.error(
             f"Model {name} is not supported."
             f"Available models are: {', '.join(SUPPORTED_MODELS.keys())}"
         )
         raise Exception(f"Model {name} is not supported.")
```

### Comparing `paka-0.1.2/paka/kube_resources/model_group/service.py` & `paka-0.1.3/paka/kube_resources/model_group/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Any, List, Optional
 
 from kubernetes import client
 
 from paka.config import CloudConfig, CloudModelGroup, Config
 from paka.constants import ACCESS_ALL_SA
 from paka.k8s import CustomResource, apply_resource, try_load_kubeconfig
```

### Comparing `paka-0.1.2/paka/kube_resources/model_group/supported_models.py` & `paka-0.1.3/paka/kube_resources/model_group/supported_models.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.2/paka/logger.py` & `paka-0.1.3/paka/logger.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.2/paka/utils.py` & `paka-0.1.3/paka/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import json
 import os
 import random
 import re
 import string
 from functools import lru_cache
 from io import StringIO
```

### Comparing `paka-0.1.2/pyproject.toml` & `paka-0.1.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,63 @@
 [tool.poetry]
 name = "paka"
-version = "0.1.2"
+version = "0.1.3"
 description = "LLMOps tool designed to simplify the deployment and management of large language model (LLM) applications"
 authors = ["Jijun Leng"]
 readme = "README.md"
 
 [tool.codespell]
 check-filenames = true
 
 [tool.mypy]
 ignore_missing_imports = true
 disallow_untyped_defs = true
 check_untyped_defs = true
+plugins = "pydantic.mypy"
 
 [tool.isort]
 profile = "black"
 
 [tool.pytest.ini_options]
 filterwarnings = [
   "ignore:pkg_resources is deprecated:DeprecationWarning",
   "ignore:Waiting for.*:DeprecationWarning",
 ]
 
 [tool.poetry.scripts]
 paka = "paka.cli.__main__:main"
 
 [tool.poetry.dependencies]
-python = "^3.11"
-pydantic = "^2.5.2"
-ruamel-yaml = "^0.18.5"
-pulumi = "^3.96.2"
-pulumi-aws = "^6.13.3"
-typer = "^0.9.0"
-pulumi-eks = "^2.0.0"
-pulumi-awsx = "^2.3.0"
-pulumi-kubernetes = "^4.6.1"
+python = "^3.8"
+pydantic = { extras = ["mypy"], version = "^2.7.0" }
+ruamel-yaml = "^0.18.6"
+pulumi = "^3.113.0"
+pulumi-aws = "^6.31.0"
+typer = "^0.12.3"
+pulumi-eks = "^2.3.0"
+pulumi-awsx = "^2.7.0"
+pulumi-kubernetes = "^4.10.0"
 pathspec = "^0.12.1"
 requests = "^2.31.0"
-kubernetes = "^v29.0.0b1"
-boto3 = "^1.34.22"
+kubernetes = "^29.0.0"
+boto3 = "^1.34.86"
 tabulate = "^0.9.0"
+huggingface-hub = "^0.22.2"
+tqdm = "^4.66.2"
+typing-extensions = "^4.11.0"
 
 [tool.poetry.group.dev.dependencies]
 codespell = "^2.2.6"
-mypy = "^1.7.1"
-pre-commit = "^3.6.0"
-pytest = "^7.4.3"
+mypy = "^1.9.0"
+pre-commit = "3.5.0"
+pytest = "^8.1.1"
 pytest-snapshot = "^0.9.0"
-types-requests = "^2.31.0.20231231"
+types-requests = "2.31.0.6"
 isort = "^5.13.2"
 types-tabulate = "^0.9.0.20240106"
-pulumi-policy = "^1.9.0"
+pulumi-policy = "^1.11.0"
+moto = "^5.0.5"
+boto3-stubs = { extras = ["s3"], version = "^1.34.86" }
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `paka-0.1.2/PKG-INFO` & `paka-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 Metadata-Version: 2.1
 Name: paka
-Version: 0.1.2
+Version: 0.1.3
 Summary: LLMOps tool designed to simplify the deployment and management of large language model (LLM) applications
 Author: Jijun Leng
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: boto3 (>=1.34.22,<2.0.0)
-Requires-Dist: kubernetes (>=v29.0.0b1,<30.0.0)
+Requires-Dist: boto3 (>=1.34.86,<2.0.0)
+Requires-Dist: huggingface-hub (>=0.22.2,<0.23.0)
+Requires-Dist: kubernetes (>=29.0.0,<30.0.0)
 Requires-Dist: pathspec (>=0.12.1,<0.13.0)
-Requires-Dist: pulumi (>=3.96.2,<4.0.0)
-Requires-Dist: pulumi-aws (>=6.13.3,<7.0.0)
-Requires-Dist: pulumi-awsx (>=2.3.0,<3.0.0)
-Requires-Dist: pulumi-eks (>=2.0.0,<3.0.0)
-Requires-Dist: pulumi-kubernetes (>=4.6.1,<5.0.0)
-Requires-Dist: pydantic (>=2.5.2,<3.0.0)
+Requires-Dist: pulumi (>=3.113.0,<4.0.0)
+Requires-Dist: pulumi-aws (>=6.31.0,<7.0.0)
+Requires-Dist: pulumi-awsx (>=2.7.0,<3.0.0)
+Requires-Dist: pulumi-eks (>=2.3.0,<3.0.0)
+Requires-Dist: pulumi-kubernetes (>=4.10.0,<5.0.0)
+Requires-Dist: pydantic[mypy] (>=2.7.0,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: ruamel-yaml (>=0.18.5,<0.19.0)
+Requires-Dist: ruamel-yaml (>=0.18.6,<0.19.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
-Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: tqdm (>=4.66.2,<5.0.0)
+Requires-Dist: typer (>=0.12.3,<0.13.0)
+Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Welcome to Paka
 
 <img src="docs/img/paka.svg" alt="paka.svg" width="200" height="200">
 
 **paka** is a versatile LLMOps tool that simplifies the deployment and management of large language model (LLM) apps with a single command.
@@ -125,14 +131,16 @@
 ## Contributing
 - Open a PR
 - Format and lint code with `make lint`
 - Run tests with `make test`
 
 ## Dependencies
 - docker daemon
+- pack cli (https://buildpacks.io/docs/for-platform-operators/how-to/integrate-ci/pack/)
+- pulumi cli (https://www.pulumi.com/docs/install/)
 - aws cli and credentials for the AWS deployment
 ```bash
 # Make sure aws credentials and cli are set up. Your aws credentials should have access to the following services:
 # - S3
 # - ECR
 # - EKS
 # - EC2
```

