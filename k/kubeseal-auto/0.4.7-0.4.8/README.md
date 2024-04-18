# Comparing `tmp/kubeseal_auto-0.4.7.tar.gz` & `tmp/kubeseal_auto-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubeseal_auto-0.4.7.tar", max compression
+gzip compressed data, was "kubeseal_auto-0.4.8.tar", max compression
```

## Comparing `kubeseal_auto-0.4.7.tar` & `kubeseal_auto-0.4.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1067 2024-03-05 09:55:04.965085 kubeseal_auto-0.4.7/LICENSE
--rw-r--r--   0        0        0     2000 2024-03-05 09:55:04.965085 kubeseal_auto-0.4.7/README.md
--rw-r--r--   0        0        0      683 2024-03-05 09:55:04.965085 kubeseal_auto-0.4.7/pyproject.toml
--rwxr-xr-x   0        0        0     2529 2024-03-05 09:55:04.965085 kubeseal_auto-0.4.7/src/kubeseal_auto/cli.py
--rw-r--r--   0        0        0     3279 2024-03-05 09:55:04.965085 kubeseal_auto-0.4.7/src/kubeseal_auto/cluster.py
--rw-r--r--   0        0        0     2265 2024-03-05 09:55:04.965085 kubeseal_auto-0.4.7/src/kubeseal_auto/host.py
--rw-r--r--   0        0        0     9692 2024-03-05 09:55:04.965085 kubeseal_auto-0.4.7/src/kubeseal_auto/kubeseal.py
--rw-r--r--   0        0        0     2904 1970-01-01 00:00:00.000000 kubeseal_auto-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-18 09:34:04.427350 kubeseal_auto-0.4.8/LICENSE
+-rw-r--r--   0        0        0     2010 2024-04-18 09:34:04.427350 kubeseal_auto-0.4.8/README.md
+-rw-r--r--   0        0        0      682 2024-04-18 09:34:04.427350 kubeseal_auto-0.4.8/pyproject.toml
+-rwxr-xr-x   0        0        0     2529 2024-04-18 09:34:04.427350 kubeseal_auto-0.4.8/src/kubeseal_auto/cli.py
+-rw-r--r--   0        0        0     3279 2024-04-18 09:34:04.427350 kubeseal_auto-0.4.8/src/kubeseal_auto/cluster.py
+-rw-r--r--   0        0        0     2265 2024-04-18 09:34:04.427350 kubeseal_auto-0.4.8/src/kubeseal_auto/host.py
+-rw-r--r--   0        0        0     9692 2024-04-18 09:34:04.427350 kubeseal_auto-0.4.8/src/kubeseal_auto/kubeseal.py
+-rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 kubeseal_auto-0.4.8/PKG-INFO
```

### Comparing `kubeseal_auto-0.4.7/LICENSE` & `kubeseal_auto-0.4.8/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vadim Gedz
+Copyright (c) 2022-2024 Vadim Gedz
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `kubeseal_auto-0.4.7/README.md` & `kubeseal_auto-0.4.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 Additionally, a "detached" mode is supported:
 ```bash
 # Download sealed-secrets certificate for local signing
 kubeseal-auto --fetch
 # Generate SealedSecret with local certificate
 kubeseal-auto --cert <kubectl-context>-kubeseal-cert.crt
 ```
-> **Note**
-In the detached mode kubeseal-auto will not download the kubeseal binary and will look for it in the system $PATH.
+> [!IMPORTANT]
+> In the detached mode `kubeseal-auto` will not download the `kubeseal` binary and will look for it in the system $PATH.
 
 To select kubeconfig context:
 ```bash
 kubeseal-auto --select
 ```
 
 To append or change key values in the existing secret:
```

### Comparing `kubeseal_auto-0.4.7/pyproject.toml` & `kubeseal_auto-0.4.8/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "kubeseal-auto"
-version = "0.4.7"
+version = "0.4.8"
 description = "An interactive wrapper for kubeseal binary"
 authors = ["Vadim Gedz <vadims@linux-tech.io>"]
 license = "MIT"
 
 readme = "README.md"
 repository = "https://github.com/shini4i/kubeseal-auto"
 homepage = "https://github.com/shini4i/kubeseal-auto"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-kubernetes = "^23.3.0"
-click = "^8.1.2"
-questionary = "^1.10.0"
-icecream = "^2.1.2"
 PyYAML = "^6.0"
-colorama = "^0.4.4"
 requests = "^2.28.1"
+kubernetes = "^29.0.0"
+click = "^8.1.7"
+icecream = "^2.1.3"
+questionary = "^2.0.1"
+colorama = "^0.4.6"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `kubeseal_auto-0.4.7/src/kubeseal_auto/cli.py` & `kubeseal_auto-0.4.8/src/kubeseal_auto/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-__version__ = "0.4.7"
+__version__ = "0.4.8"
 
 import click
 import colorama
 from icecream import ic
 
 from kubeseal_auto.kubeseal import Kubeseal
```

### Comparing `kubeseal_auto-0.4.7/src/kubeseal_auto/cluster.py` & `kubeseal_auto-0.4.8/src/kubeseal_auto/cluster.py`

 * *Files identical despite different names*

### Comparing `kubeseal_auto-0.4.7/src/kubeseal_auto/host.py` & `kubeseal_auto-0.4.8/src/kubeseal_auto/host.py`

 * *Files identical despite different names*

### Comparing `kubeseal_auto-0.4.7/src/kubeseal_auto/kubeseal.py` & `kubeseal_auto-0.4.8/src/kubeseal_auto/kubeseal.py`

 * *Files identical despite different names*

### Comparing `kubeseal_auto-0.4.7/PKG-INFO` & `kubeseal_auto-0.4.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: kubeseal-auto
-Version: 0.4.7
+Version: 0.4.8
 Summary: An interactive wrapper for kubeseal binary
 Home-page: https://github.com/shini4i/kubeseal-auto
 License: MIT
 Author: Vadim Gedz
 Author-email: vadims@linux-tech.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: click (>=8.1.2,<9.0.0)
-Requires-Dist: colorama (>=0.4.4,<0.5.0)
-Requires-Dist: icecream (>=2.1.2,<3.0.0)
-Requires-Dist: kubernetes (>=23.3.0,<24.0.0)
-Requires-Dist: questionary (>=1.10.0,<2.0.0)
+Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: colorama (>=0.4.6,<0.5.0)
+Requires-Dist: icecream (>=2.1.3,<3.0.0)
+Requires-Dist: kubernetes (>=29.0.0,<30.0.0)
+Requires-Dist: questionary (>=2.0.1,<3.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Repository, https://github.com/shini4i/kubeseal-auto
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # kubeseal-auto
@@ -55,16 +55,16 @@
 Additionally, a "detached" mode is supported:
 ```bash
 # Download sealed-secrets certificate for local signing
 kubeseal-auto --fetch
 # Generate SealedSecret with local certificate
 kubeseal-auto --cert <kubectl-context>-kubeseal-cert.crt
 ```
-> **Note**
-In the detached mode kubeseal-auto will not download the kubeseal binary and will look for it in the system $PATH.
+> [!IMPORTANT]
+> In the detached mode `kubeseal-auto` will not download the `kubeseal` binary and will look for it in the system $PATH.
 
 To select kubeconfig context:
 ```bash
 kubeseal-auto --select
 ```
 
 To append or change key values in the existing secret:
```

