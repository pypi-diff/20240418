# Comparing `tmp/mlpro-int-river-0.1.3.tar.gz` & `tmp/mlpro_int_river-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpro-int-river-0.1.3.tar", last modified: Thu Feb 15 11:41:37 2024, max compression
+gzip compressed data, was "mlpro_int_river-0.1.4.tar", last modified: Thu Apr 18 17:44:00 2024, max compression
```

## Comparing `mlpro-int-river-0.1.3.tar` & `mlpro_int_river-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 11:41:37.006479 mlpro-int-river-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-02-15 11:41:27.000000 mlpro-int-river-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-02-15 11:41:37.006479 mlpro-int-river-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-02-15 11:41:27.000000 mlpro-int-river-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-15 11:41:28.000000 mlpro-int-river-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-02-15 11:41:37.006479 mlpro-int-river-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 11:41:37.002479 mlpro-int-river-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 11:41:37.002479 mlpro-int-river-0.1.3/src/mlpro_int_river/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 11:41:28.000000 mlpro-int-river-0.1.3/src/mlpro_int_river/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 11:41:37.006479 mlpro-int-river-0.1.3/src/mlpro_int_river/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-15 11:41:28.000000 mlpro-int-river-0.1.3/src/mlpro_int_river/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-02-15 11:41:28.000000 mlpro-int-river-0.1.3/src/mlpro_int_river/wrappers/anomalydetectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-02-15 11:41:28.000000 mlpro-int-river-0.1.3/src/mlpro_int_river/wrappers/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    41593 2024-02-15 11:41:28.000000 mlpro-int-river-0.1.3/src/mlpro_int_river/wrappers/clusteranalyzers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11945 2024-02-15 11:41:28.000000 mlpro-int-river-0.1.3/src/mlpro_int_river/wrappers/streams.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 11:41:37.006479 mlpro-int-river-0.1.3/src/mlpro_int_river.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-02-15 11:41:36.000000 mlpro-int-river-0.1.3/src/mlpro_int_river.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-02-15 11:41:36.000000 mlpro-int-river-0.1.3/src/mlpro_int_river.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 11:41:36.000000 mlpro-int-river-0.1.3/src/mlpro_int_river.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-15 11:41:36.000000 mlpro-int-river-0.1.3/src/mlpro_int_river.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-15 11:41:36.000000 mlpro-int-river-0.1.3/src/mlpro_int_river.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 11:41:37.006479 mlpro-int-river-0.1.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-02-15 11:41:28.000000 mlpro-int-river-0.1.3/test/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:44:00.470367 mlpro_int_river-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-18 17:43:55.000000 mlpro_int_river-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-18 17:44:00.470367 mlpro_int_river-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-18 17:43:55.000000 mlpro_int_river-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-18 17:43:56.000000 mlpro_int_river-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-18 17:44:00.474367 mlpro_int_river-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:44:00.466367 mlpro_int_river-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:44:00.470367 mlpro_int_river-0.1.4/src/mlpro_int_river/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-18 17:43:56.000000 mlpro_int_river-0.1.4/src/mlpro_int_river/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:44:00.470367 mlpro_int_river-0.1.4/src/mlpro_int_river/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-18 17:43:56.000000 mlpro_int_river-0.1.4/src/mlpro_int_river/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-04-18 17:43:56.000000 mlpro_int_river-0.1.4/src/mlpro_int_river/wrappers/anomalydetectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-18 17:43:56.000000 mlpro_int_river-0.1.4/src/mlpro_int_river/wrappers/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41611 2024-04-18 17:43:56.000000 mlpro_int_river-0.1.4/src/mlpro_int_river/wrappers/clusteranalyzers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-18 17:43:56.000000 mlpro_int_river-0.1.4/src/mlpro_int_river/wrappers/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:44:00.470367 mlpro_int_river-0.1.4/src/mlpro_int_river.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-18 17:44:00.000000 mlpro_int_river-0.1.4/src/mlpro_int_river.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-18 17:44:00.000000 mlpro_int_river-0.1.4/src/mlpro_int_river.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 17:44:00.000000 mlpro_int_river-0.1.4/src/mlpro_int_river.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-18 17:44:00.000000 mlpro_int_river-0.1.4/src/mlpro_int_river.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-18 17:44:00.000000 mlpro_int_river-0.1.4/src/mlpro_int_river.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:44:00.470367 mlpro_int_river-0.1.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-18 17:43:56.000000 mlpro_int_river-0.1.4/test/test_examples.py
```

### Comparing `mlpro-int-river-0.1.3/LICENSE` & `mlpro_int_river-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpro-int-river-0.1.3/PKG-INFO` & `mlpro_int_river-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: mlpro-int-river
-Version: 0.1.3
+Version: 0.1.4
 Summary: MLPro: Integration River
-Home-page: https://mlpro_int_river.readthedocs.io
+Home-page: https://mlpro-int-river.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro-int-river.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: full
-Requires-Dist: mlpro[full]>=1.3.1; extra == "full"
+Requires-Dist: mlpro[full]>=1.4.0; extra == "full"
 Requires-Dist: river>=0.21.0; extra == "full"
 
 [![CI](https://github.com/fhswf/MLPro-Int-River/actions/workflows/ci.yml/badge.svg)](https://github.com/fhswf/MLPro-Int-River/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/mlpro-int-river/badge/?version=latest)](https://mlpro-int-river.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/mlpro-int-river.svg)](https://badge.fury.io/py/mlpro-int-river)
 <!---
 [![Anaconda-Version Badge](https://anaconda.org/mlpro-int-river/mlpro-int-river/badges/version.svg)](https://anaconda.org/mlpro-int-river/mlpro)
```

### Comparing `mlpro-int-river-0.1.3/README.md` & `mlpro_int_river-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mlpro-int-river-0.1.3/setup.cfg` & `mlpro_int_river-0.1.4/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [metadata]
 name = mlpro-int-river
-version = 0.1.3
+version = 0.1.4
 author = MLPro Team
 author_email = mlpro@listen.fh-swf.de
 description = MLPro: Integration River
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://mlpro_int_river.readthedocs.io
+url = https://mlpro-int-river.readthedocs.io
 project_urls = 
 	Bug Tracker = https://mlpro-int-river.readthedocs.io
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 
@@ -22,14 +22,14 @@
 include_package_data = True
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 full = 
-	mlpro[full]>=1.3.1
+	mlpro[full]>=1.4.0
 	river>=0.21.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `mlpro-int-river-0.1.3/src/mlpro_int_river/wrappers/anomalydetectors.py` & `mlpro_int_river-0.1.4/src/mlpro_int_river/wrappers/anomalydetectors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 ## -------------------------------------------------------------------------------------------------
 ## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
 ## -- Package : mlpro.wrappers.river
 ## -- Module  : anomalydetectors.py
 ## -------------------------------------------------------------------------------------------------
 ## -- History :
-## -- 2023-06-23  1.0.0     SP       Creation
-## -- 2023-06-23  1.0.0     SP       First version release
+## -- yyyy-mm-dd  Ver.      Auth.    Description
+## -- 2023-06-23  1.0.0     SK       Creation
+## -- 2023-06-23  1.0.0     SK       First version release
+## -- 2024-04-10  1.0.1     DA       Refactoring
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 1.0.0 (2023-05-12)
+Ver. 1.0.1 (2024-04-10)
 
 This module provides wrapper functionalities to incorporate anomaly detector algorithms of the 
 River ecosystem. This module includes two algorithms from River that are embedded to MLPro, such as:
 
 1) Half Space Tree (HST)
 1) One Class SVM
 
 Learn more:
 https://www.riverml.xyz/
 
 """
 
-from mlpro_int_river.wrappers.basics import *
-from mlpro.oa.streams.basics import Instance, List
-from mlpro.oa.streams.tasks.anomalydetectors import *
+from mlpro.bf.various import Log
+from mlpro.bf.streams import StreamTask
+from mlpro_int_river.wrappers import WrapperRiver
+from mlpro.oa.streams.tasks.anomalydetectors import AnomalyDetector, Anomaly
 from river import anomaly
 
-class HST(AnomalyDetector):
 
-    C_NAME          = 'HST Anomaly Detector'
+
+
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class HST (WrapperRiver, AnomalyDetector):
+
     C_TYPE          = 'Anomaly Detector'
+    C_NAME          = 'River-HST'
 
 ## -------------------------------------------------------------------------------------------------
     def __init__(self,
                  p_no_trees = 5,
                  p_height = 3,
                  p_window_size = 3,
                  p_sizeof_instance_list = 100,
@@ -75,21 +83,23 @@
             # Perform anomaly detection on the current data points
             hst.learn_one(self.data_points)
             self.anomaly_scores = hst.score_one(self.data_points[-1])
                 
             # Determine if the data point is an anomaly based on its outlier score
             if self.anomaly_scores < 0:
                 self.counter += 1
-                event_obj = AnomalyEvent(p_raising_object=self, p_kwargs=self.data_points[-1]) 
+                event_obj = Anomaly(p_raising_object=self, p_kwargs=self.data_points[-1]) 
                 handler = self.event_handler
                 self.register_event_handler(event_obj.C_NAME, handler)
                 self._raise_event(event_obj.C_NAME, event_obj)
 
 
 
+
+
 ## -------------------------------------------------------------------------------------------------
 ## -------------------------------------------------------------------------------------------------
 class SVM(AnomalyDetector):
 
     C_NAME          = 'OneClassSVM Anomaly Detector'
     C_TYPE          = 'Anomaly Detector'
 
@@ -134,16 +144,11 @@
             # Perform anomaly detection on the current data points
             svm.learn_one(self.data_points)
             self.anomaly_scores = svm.score_one(self.data_points[-1])
                 
             # Determine if the data point is an anomaly based on its outlier score
             if self.anomaly_scores < 0:
                 self.counter += 1
-                event_obj = AnomalyEvent(p_raising_object=self, p_kwargs=self.data_points[-1]) 
+                event_obj = Anomaly(p_raising_object=self, p_kwargs=self.data_points[-1]) 
                 handler = self.event_handler
                 self.register_event_handler(event_obj.C_NAME, handler)
                 self._raise_event(event_obj.C_NAME, event_obj)
-
-
-
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
```

### Comparing `mlpro-int-river-0.1.3/src/mlpro_int_river/wrappers/basics.py` & `mlpro_int_river-0.1.4/src/mlpro_int_river/wrappers/basics.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,28 +23,29 @@
 ## --                                - Refatoring of classes WrStream*
 ## --                                - Class WrStreamProviderRiver: detects now all River data sets
 ## --                                - Conversion to subpackage with modules for
 ## --                                    - native River streams
 ## --                                    - selected cluster algorithms
 ## --                                    - selected algorithms for anomaly detection 
 ## -- 2024-02-15  2.1.0     DA       Updated minimum version of river to 0.21.0
+## -- 2024-04-10  2.1.1     DA       Refactoring
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 2.1.0 (2024-02-15)
+Ver. 2.1.1 (2024-04-10)
 
-This module contains the abstract root class for all river wraper classes.
+This module contains the abstract root class for all river wrapper classes.
 
 Learn more:
 https://www.riverml.xyz/
 
 """
 
 from mlpro.bf.various import ScientificObject
-from mlpro.wrappers.models import Wrapper
+from mlpro.wrappers import Wrapper
 
 
 
 
 ## -------------------------------------------------------------------------------------------------
 ## -------------------------------------------------------------------------------------------------
 class WrapperRiver (Wrapper):
```

### Comparing `mlpro-int-river-0.1.3/src/mlpro_int_river/wrappers/clusteranalyzers.py` & `mlpro_int_river-0.1.4/src/mlpro_int_river/wrappers/clusteranalyzers.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,18 +19,19 @@
 ## -- 2023-12-21  1.0.8     SY       Add renormalization method on all wrapped algorithms
 ## -- 2023-12-22  1.0.9     DA/SY    Bugfix 
 ## -- 2023-12-25  1.0.10    DA       Bugfix in WrClusterAnalyzerRiver2MLPro._adapt()
 ## -- 2023-12-29  1.0.11    DA/SY    Disabled renormalization of CluStream, DBStream, DenStream
 ## -- 2024-01-05  1.0.12    DA       All classed: refactoring of naming (C_NAME)
 ## -- 2024-02-04  1.1.0     SY       Updating WrRiverDenStream2MLPro, WrRiverStreamKMeans2MLPro due
 ## --                                to visualization errors
+## -- 2024-02-24  1.1.1     DA       Class WrClusterAnalyzerRiver2MLPro: package constants removed
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 1.1.0 (2024-02-04)
+Ver. 1.1.1 (2024-02-24)
 
 This module provides wrapper classes from River to MLPro, specifically for cluster analyzers. This
 module includes three clustering algorithms from River that are embedded to MLPro, such as:
 
 1) DBSTREAM (https://riverml.xyz/latest/api/cluster/DBSTREAM/)
 
 2) CluStream (https://riverml.xyz/latest/api/cluster/CluStream/)
@@ -44,15 +45,15 @@
 Learn more:
 https://www.riverml.xyz/
 
 """
 
 
 from mlpro.bf.streams import Instance, List
-from mlpro_int_river.wrappers.basics import WrapperRiver
+from mlpro_int_river.wrappers import WrapperRiver
 from mlpro.bf.math.normalizers import Normalizer
 from mlpro.oa.streams.tasks.clusteranalyzers import ClusterAnalyzer, Cluster, ClusterCentroid
 from mlpro.bf.mt import Task as MLTask
 from mlpro.bf.various import Log
 from mlpro.bf.streams import *
 from river import base, cluster
 from typing import List, Tuple
@@ -86,17 +87,14 @@
         Set up type of logging. Default: Log.C_LOG_ALL.
     p_kwargs : dict
         Further optional named parameters. 
         
     """
 
     C_TYPE              = 'River Cluster Analyzer'
-    
-    C_WRAPPED_PACKAGE   = 'river'
-    C_MINIMUM_VERSION   = '0.15.0'
 
 
 ## -------------------------------------------------------------------------------------------------
     def __init__(self,
                  p_cls_cluster,
                  p_river_algo:base.Clusterer,
                  p_name:str = None,
```

### Comparing `mlpro-int-river-0.1.3/src/mlpro_int_river/wrappers/streams.py` & `mlpro_int_river-0.1.4/src/mlpro_int_river/wrappers/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,19 @@
 ## -- 2022-11-08  1.3.1     DA       Corrections
 ## -- 2022-11-19  1.4.0     DA       Method WrStreamRiver._get_string(): new parameter p_name
 ## -- 2022-12-09  1.4.1     DA       Bugfix
 ## -- 2023-04-16  2.0.0     DA       - New root class WrapperRiver
 ## --                                - New wrappers for River cluster analyzers
 ## --                                - Refatoring of classes WrStream*
 ## --                                - Class WrStreamProviderRiver: detects now all River data sets 
+## -- 2024-02-17  2.0.1     DA       Class WrStreamProviderRiver: correction C_TYPE
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 2.0.0 (2023-04-16)
+Ver. 2.0.1 (2024-02-17)
 
 This module provides wrapper classes to embed River stream functionalities into MLPro. 
 
 Learn more:
 https://www.riverml.xyz/
 
 """
@@ -53,21 +54,23 @@
 
     Parameters
     ----------
     p_logging
         Log level of stream objects (see constants of class Log). Default: Log.C_LOG_ALL.
     """
 
-    C_NAME              = 'Native Streams'
+    C_NAME              = 'River'
 
 ## -------------------------------------------------------------------------------------------------
     def __init__(self, p_logging = Log.C_LOG_ALL):
 
         self._river_streams = {}
 
+        self.C_TYPE = StreamProvider.C_TYPE
+
         WrapperRiver.__init__(self, p_logging=p_logging)
         StreamProvider.__init__(self, p_logging = p_logging)
 
 
 ## -------------------------------------------------------------------------------------------------
     def _get_stream_list(self, p_mode=Mode.C_MODE_SIM, p_logging=Log.C_LOG_ALL, **p_kwargs) -> list:
         """
```

### Comparing `mlpro-int-river-0.1.3/src/mlpro_int_river.egg-info/PKG-INFO` & `mlpro_int_river-0.1.4/src/mlpro_int_river.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: mlpro-int-river
-Version: 0.1.3
+Version: 0.1.4
 Summary: MLPro: Integration River
-Home-page: https://mlpro_int_river.readthedocs.io
+Home-page: https://mlpro-int-river.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro-int-river.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: full
-Requires-Dist: mlpro[full]>=1.3.1; extra == "full"
+Requires-Dist: mlpro[full]>=1.4.0; extra == "full"
 Requires-Dist: river>=0.21.0; extra == "full"
 
 [![CI](https://github.com/fhswf/MLPro-Int-River/actions/workflows/ci.yml/badge.svg)](https://github.com/fhswf/MLPro-Int-River/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/mlpro-int-river/badge/?version=latest)](https://mlpro-int-river.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/mlpro-int-river.svg)](https://badge.fury.io/py/mlpro-int-river)
 <!---
 [![Anaconda-Version Badge](https://anaconda.org/mlpro-int-river/mlpro-int-river/badges/version.svg)](https://anaconda.org/mlpro-int-river/mlpro)
```

### Comparing `mlpro-int-river-0.1.3/src/mlpro_int_river.egg-info/SOURCES.txt` & `mlpro_int_river-0.1.4/src/mlpro_int_river.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlpro-int-river-0.1.3/test/test_examples.py` & `mlpro_int_river-0.1.4/test/test_examples.py`

 * *Files identical despite different names*

