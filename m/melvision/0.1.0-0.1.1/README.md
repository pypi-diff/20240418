# Comparing `tmp/melvision-0.1.0.tar.gz` & `tmp/melvision-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melvision-0.1.0.tar", last modified: Wed Apr 17 14:37:34 2024, max compression
+gzip compressed data, was "melvision-0.1.1.tar", last modified: Thu Apr 18 09:43:38 2024, max compression
```

## Comparing `melvision-0.1.0.tar` & `melvision-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 14:37:34.213792 melvision-0.1.0/
--rw-rw-rw-   0        0        0      426 2024-04-17 14:37:34.213792 melvision-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-17 14:37:34.213792 melvision-0.1.0/melvision/
--rw-rw-rw-   0        0        0        0 2024-04-17 13:38:27.000000 melvision-0.1.0/melvision/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 14:37:34.213792 melvision-0.1.0/melvision/models/
--rw-rw-rw-   0        0        0        0 2024-04-17 14:19:41.000000 melvision-0.1.0/melvision/models/__init__.py
--rw-rw-rw-   0        0        0     1926 2024-04-17 13:41:41.000000 melvision-0.1.0/melvision/models/alexnet.py
--rw-rw-rw-   0        0        0     6004 2024-04-17 13:41:41.000000 melvision-0.1.0/melvision/models/googlenet.py
--rw-rw-rw-   0        0        0     8762 2024-04-17 13:41:41.000000 melvision-0.1.0/melvision/models/resnet.py
--rw-rw-rw-   0        0        0     5443 2024-04-17 13:41:41.000000 melvision-0.1.0/melvision/models/vgg.py
--rw-rw-rw-   0        0        0      522 2024-04-17 14:22:12.000000 melvision-0.1.0/melvision/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-17 14:37:34.213792 melvision-0.1.0/melvision.egg-info/
--rw-rw-rw-   0        0        0      426 2024-04-17 14:37:34.000000 melvision-0.1.0/melvision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2024-04-17 14:37:34.000000 melvision-0.1.0/melvision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 14:37:34.000000 melvision-0.1.0/melvision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-17 14:37:34.000000 melvision-0.1.0/melvision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 14:37:34.213792 melvision-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      555 2024-04-17 14:30:08.000000 melvision-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:43:38.488374 melvision-0.1.1/
+-rw-rw-rw-   0        0        0      426 2024-04-18 09:43:38.488374 melvision-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-18 09:43:38.488374 melvision-0.1.1/melvision/
+-rw-rw-rw-   0        0        0        0 2024-04-17 13:38:27.000000 melvision-0.1.1/melvision/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:43:38.488374 melvision-0.1.1/melvision/models/
+-rw-rw-rw-   0        0        0      216 2024-04-18 09:36:01.000000 melvision-0.1.1/melvision/models/__init__.py
+-rw-rw-rw-   0        0        0     1926 2024-04-17 13:41:41.000000 melvision-0.1.1/melvision/models/alexnet.py
+-rw-rw-rw-   0        0        0     6044 2024-04-18 08:12:20.000000 melvision-0.1.1/melvision/models/googlenet.py
+-rw-rw-rw-   0        0        0     8762 2024-04-17 13:41:41.000000 melvision-0.1.1/melvision/models/resnet.py
+-rw-rw-rw-   0        0        0     5443 2024-04-17 13:41:41.000000 melvision-0.1.1/melvision/models/vgg.py
+-rw-rw-rw-   0        0        0      522 2024-04-17 14:22:12.000000 melvision-0.1.1/melvision/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:43:38.488374 melvision-0.1.1/melvision.egg-info/
+-rw-rw-rw-   0        0        0      426 2024-04-18 09:43:38.000000 melvision-0.1.1/melvision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2024-04-18 09:43:38.000000 melvision-0.1.1/melvision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 09:43:38.000000 melvision-0.1.1/melvision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-18 09:43:38.000000 melvision-0.1.1/melvision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 09:43:38.488374 melvision-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      555 2024-04-18 09:39:29.000000 melvision-0.1.1/setup.py
```

### Comparing `melvision-0.1.0/melvision/models/alexnet.py` & `melvision-0.1.1/melvision/models/alexnet.py`

 * *Files identical despite different names*

### Comparing `melvision-0.1.0/melvision/models/googlenet.py` & `melvision-0.1.1/melvision/models/googlenet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import torch
 import torch.nn as nn
 from ..utils import load_pretrained_weights
 
 
+__all__ = ["GoogLeNet", "googlenet"]
+
 class BasicConv2d(nn.Module):
     def __init__(self, in_channels, out_channels, **kwargs):
         super(BasicConv2d, self).__init__()
         self.conv = nn.Conv2d(in_channels, out_channels, bias=False, **kwargs)
         self.bn = nn.BatchNorm2d(out_channels, eps=0.001)
         self.relu = nn.ReLU(inplace=True)
```

### Comparing `melvision-0.1.0/melvision/models/resnet.py` & `melvision-0.1.1/melvision/models/resnet.py`

 * *Files identical despite different names*

### Comparing `melvision-0.1.0/melvision/models/vgg.py` & `melvision-0.1.1/melvision/models/vgg.py`

 * *Files identical despite different names*

### Comparing `melvision-0.1.0/melvision/utils.py` & `melvision-0.1.1/melvision/utils.py`

 * *Files identical despite different names*

### Comparing `melvision-0.1.0/setup.py` & `melvision-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="melvision",
-    version="0.1.0",
+    version="0.1.1",
     author="Melvin Hwang",
     author_email="huang667399@gmail.com",
     description="A convenient deep learning and image processing library.",
     long_description_content_type="text/markdown",
     url="https://github.com/Manuel667399/melvision",
     packages=setuptools.find_packages(),
     classifiers=[
```

