# Comparing `tmp/panoptica-0.6.3-py3-none-any.whl.zip` & `tmp/panoptica-0.6.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 32016 bytes, number of entries: 24
+Zip file size: 32176 bytes, number of entries: 24
 -rw-r--r--  2.0 unx      403 b- defN 80-Jan-01 00:00 panoptica/__init__.py
 -rw-r--r--  2.0 unx     7728 b- defN 80-Jan-01 00:00 panoptica/_functionals.py
 -rw-r--r--  2.0 unx     6420 b- defN 80-Jan-01 00:00 panoptica/instance_approximator.py
 -rw-r--r--  2.0 unx     3981 b- defN 80-Jan-01 00:00 panoptica/instance_evaluator.py
 -rw-r--r--  2.0 unx    12130 b- defN 80-Jan-01 00:00 panoptica/instance_matcher.py
 -rw-r--r--  2.0 unx      592 b- defN 80-Jan-01 00:00 panoptica/metrics/__init__.py
 -rw-r--r--  2.0 unx     4065 b- defN 80-Jan-01 00:00 panoptica/metrics/assd.py
 -rw-r--r--  2.0 unx     1743 b- defN 80-Jan-01 00:00 panoptica/metrics/cldice.py
 -rw-r--r--  2.0 unx     2170 b- defN 80-Jan-01 00:00 panoptica/metrics/dice.py
 -rw-r--r--  2.0 unx     1552 b- defN 80-Jan-01 00:00 panoptica/metrics/iou.py
--rw-r--r--  2.0 unx    10522 b- defN 80-Jan-01 00:00 panoptica/metrics/metrics.py
--rw-r--r--  2.0 unx    10687 b- defN 80-Jan-01 00:00 panoptica/panoptic_evaluator.py
--rw-r--r--  2.0 unx    14236 b- defN 80-Jan-01 00:00 panoptica/panoptic_result.py
+-rw-r--r--  2.0 unx    10544 b- defN 80-Jan-01 00:00 panoptica/metrics/metrics.py
+-rw-r--r--  2.0 unx    10631 b- defN 80-Jan-01 00:00 panoptica/panoptic_evaluator.py
+-rw-r--r--  2.0 unx    15425 b- defN 80-Jan-01 00:00 panoptica/panoptic_result.py
 -rw-r--r--  2.0 unx      412 b- defN 80-Jan-01 00:00 panoptica/timing.py
 -rw-r--r--  2.0 unx      387 b- defN 80-Jan-01 00:00 panoptica/utils/__init__.py
 -rw-r--r--  2.0 unx      793 b- defN 80-Jan-01 00:00 panoptica/utils/citation_reminder.py
 -rw-r--r--  2.0 unx     1161 b- defN 80-Jan-01 00:00 panoptica/utils/constants.py
 -rw-r--r--  2.0 unx     5398 b- defN 80-Jan-01 00:00 panoptica/utils/edge_case_handling.py
 -rw-r--r--  2.0 unx     2859 b- defN 80-Jan-01 00:00 panoptica/utils/numpy_utils.py
 -rw-r--r--  2.0 unx    14094 b- defN 80-Jan-01 00:00 panoptica/utils/processing_pair.py
--rw-r--r--  2.0 unx     1506 b- defN 80-Jan-01 00:00 panoptica-0.6.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     5021 b- defN 80-Jan-01 00:00 panoptica-0.6.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 panoptica-0.6.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2010 b- defN 16-Jan-01 00:00 panoptica-0.6.3.dist-info/RECORD
-24 files, 109958 bytes uncompressed, 28774 bytes compressed:  73.8%
+-rw-r--r--  2.0 unx     1506 b- defN 80-Jan-01 00:00 panoptica-0.6.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5021 b- defN 80-Jan-01 00:00 panoptica-0.6.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 panoptica-0.6.4.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2010 b- defN 16-Jan-01 00:00 panoptica-0.6.4.dist-info/RECORD
+24 files, 111113 bytes uncompressed, 28934 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -54,20 +54,20 @@
 
 Filename: panoptica/utils/numpy_utils.py
 Comment: 
 
 Filename: panoptica/utils/processing_pair.py
 Comment: 
 
-Filename: panoptica-0.6.3.dist-info/LICENSE
+Filename: panoptica-0.6.4.dist-info/LICENSE
 Comment: 
 
-Filename: panoptica-0.6.3.dist-info/METADATA
+Filename: panoptica-0.6.4.dist-info/METADATA
 Comment: 
 
-Filename: panoptica-0.6.3.dist-info/WHEEL
+Filename: panoptica-0.6.4.dist-info/WHEEL
 Comment: 
 
-Filename: panoptica-0.6.3.dist-info/RECORD
+Filename: panoptica-0.6.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## panoptica/metrics/metrics.py

```diff
@@ -171,14 +171,15 @@
 class MetricType(_Enum_Compare):
     """Different type of metrics
 
     Args:
         _Enum_Compare (_type_): _description_
     """
 
+    NO_PRINT = auto()
     MATCHING = auto()
     GLOBAL = auto()
     INSTANCE = auto()
 
 
 class MetricCouldNotBeComputedException(Exception):
     """Exception for when a Metric cannot be computed"""
```

## panoptica/panoptic_evaluator.py

```diff
@@ -142,15 +142,14 @@
     processing_pair.crop_data()
 
     if isinstance(processing_pair, SemanticPair):
         assert (
             instance_approximator is not None
         ), "Got SemanticPair but not InstanceApproximator"
         print("-- Got SemanticPair, will approximate instances")
-        processing_pair = instance_approximator.approximate_instances(processing_pair)
         start = perf_counter()
         processing_pair = instance_approximator.approximate_instances(processing_pair)
         if log_times:
             print(f"-- Approximation took {perf_counter() - start} seconds")
         debug_data["UnmatchedInstanceMap"] = processing_pair.copy()
 
     # Second Phase: Instance Matching
@@ -181,14 +180,15 @@
             processing_pair,
             eval_metrics=eval_metrics,
             edge_case_handler=edge_case_handler,
         )
 
     if isinstance(processing_pair, MatchedInstancePair):
         print("-- Got MatchedInstancePair, will evaluate instances")
+        start = perf_counter()
         processing_pair = evaluate_matched_instance(
             processing_pair,
             eval_metrics=eval_metrics,
             decision_metric=decision_metric,
             decision_threshold=decision_threshold,
             edge_case_handler=edge_case_handler,
         )
```

## panoptica/panoptic_result.py

```diff
@@ -9,14 +9,15 @@
     Evaluation_Metric,
     Metric,
     MetricCouldNotBeComputedException,
     MetricMode,
     MetricType,
     _compute_centerline_dice_coefficient,
     _compute_dice_coefficient,
+    _average_symmetric_surface_distance,
 )
 from panoptica.utils import EdgeCaseHandler
 
 
 class PanopticaResult(object):
     def __init__(
         self,
@@ -90,14 +91,28 @@
         self.fn: int
         self._add_metric(
             "fn",
             MetricType.MATCHING,
             fn,
             long_name="False Negatives",
         )
+        self.prec: int
+        self._add_metric(
+            "prec",
+            MetricType.NO_PRINT,
+            prec,
+            long_name="Precision (positive predictive value)",
+        )
+        self.rec: int
+        self._add_metric(
+            "rec",
+            MetricType.NO_PRINT,
+            rec,
+            long_name="Recall (sensitivity)",
+        )
         self.rq: float
         self._add_metric(
             "rq",
             MetricType.MATCHING,
             rq,
             long_name="Recognition Quality / F1-Score",
         )
@@ -115,14 +130,22 @@
         self.global_bin_cldsc: int
         self._add_metric(
             "global_bin_cldsc",
             MetricType.GLOBAL,
             global_bin_cldsc,
             long_name="Global Binary Centerline Dice",
         )
+        #
+        self.global_bin_assd: int
+        self._add_metric(
+            "global_bin_assd",
+            MetricType.GLOBAL,
+            global_bin_assd,
+            long_name="Global Binary Average Symmetric Surface Distance",
+        )
         # endregion
         #
         # region IOU
         self.sq: float
         self._add_metric(
             "sq",
             MetricType.INSTANCE,
@@ -266,14 +289,16 @@
         if print_errors:
             for k, v in metric_errors.items():
                 print(f"Metric {k}: {v}")
 
     def __str__(self) -> str:
         text = ""
         for metric_type in MetricType:
+            if metric_type == MetricType.NO_PRINT:
+                continue
             text += f"\n+++ {metric_type.name} +++\n"
             for k, v in self._evaluation_metrics.items():
                 if v.metric_type != metric_type:
                     continue
                 if k.endswith("_std"):
                     continue
                 if v._was_calculated and not v._error:
@@ -356,14 +381,22 @@
     return res.num_pred_instances - res.tp
 
 
 def fn(res: PanopticaResult):
     return res.num_ref_instances - res.tp
 
 
+def prec(res: PanopticaResult):
+    return res.tp / (res.tp + res.fp)
+
+
+def rec(res: PanopticaResult):
+    return res.tp / (res.tp + res.fn)
+
+
 def rq(res: PanopticaResult):
     """
     Calculate the Recognition Quality (RQ) based on TP, FP, and FN.
 
     Returns:
         float: Recognition Quality (RQ).
     """
@@ -452,14 +485,24 @@
     pred_binary = res._prediction_arr.copy()
     ref_binary = res._reference_arr.copy()
     pred_binary[pred_binary != 0] = 1
     ref_binary[ref_binary != 0] = 1
     return _compute_centerline_dice_coefficient(ref_binary, pred_binary)
 
 
+def global_bin_assd(res: PanopticaResult):
+    if res.tp == 0:
+        return 0.0
+    pred_binary = res._prediction_arr.copy()
+    ref_binary = res._reference_arr.copy()
+    pred_binary[pred_binary != 0] = 1
+    ref_binary[ref_binary != 0] = 1
+    return _average_symmetric_surface_distance(ref_binary, pred_binary)
+
+
 # endregion
 
 
 if __name__ == "__main__":
     c = PanopticaResult(
         reference_arr=np.zeros([5, 5, 5]),
         prediction_arr=np.zeros([5, 5, 5]),
```

## Comparing `panoptica-0.6.3.dist-info/LICENSE` & `panoptica-0.6.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `panoptica-0.6.3.dist-info/METADATA` & `panoptica-0.6.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panoptica
-Version: 0.6.3
+Version: 0.6.4
 Summary: Panoptic Quality (PQ) computation for binary masks.
 Home-page: https://github.com/BrainLesion/panoptica
 Author: Florian Kofler
 Author-email: florian.kofler@tum.de
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

## Comparing `panoptica-0.6.3.dist-info/RECORD` & `panoptica-0.6.4.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 panoptica/instance_evaluator.py,sha256=H1xhNVHm--3goGRa8TaBgHlJjPqPZ1wTArzAWtrSbFM,3981
 panoptica/instance_matcher.py,sha256=qdWH_gcr0JNdkQYjasl0X4m0gVvjssqGslbDuknmPN4,12130
 panoptica/metrics/__init__.py,sha256=mZfy5NDkjW5h-gZADEqjenJwKL3ivSqdcbWe0aJGUaE,592
 panoptica/metrics/assd.py,sha256=qZQma7Aqe-S2Z50YwLMNjZDV4MCpHndv3sGJ3hIA0b0,4065
 panoptica/metrics/cldice.py,sha256=MF8J74raAOG-vwPZPY7mR6QAiskNjCcb6KrllzQ5UB4,1743
 panoptica/metrics/dice.py,sha256=-59NLFbiu_nnaVCigScEvsj5ouSYB1-PrwGRclB0-ig,2170
 panoptica/metrics/iou.py,sha256=NbGjq6tUhdOyRvK8nMhM4E6vo4a1O6ZCzJTSl650KEo,1552
-panoptica/metrics/metrics.py,sha256=rvhXgXYUm9A3tpLkVgb0noCO9MuIvPGCrIZUyYKTUSA,10522
-panoptica/panoptic_evaluator.py,sha256=SNcmD6iJHvShn-2mMBFrqSpsXLN78b_zZbazG3pmKG8,10687
-panoptica/panoptic_result.py,sha256=IugwQMjxcvZpRhCeWFRIiMjQk4BBwLmlW89TTT4DHuk,14236
+panoptica/metrics/metrics.py,sha256=APuPFajcaiAuNXk5E-48s_wnE2VDTA3tg8S5jvf_NRg,10544
+panoptica/panoptic_evaluator.py,sha256=mrmQyly-B1OwEoawkzsCQMnMVyFv3i9LmzffkLkUK4Q,10631
+panoptica/panoptic_result.py,sha256=5liP4wM5FDcDZ0n1NjkzMJMqVJCOYWl62T7bLRyOz70,15425
 panoptica/timing.py,sha256=6gj43QyVodoAoTZ3k3645XZiIwrKEFtuDktvhV3wpF4,412
 panoptica/utils/__init__.py,sha256=RIw9TbCEfV-Dh6Ao7Ni8Lp5quJ3i4aTBL_yQ5x5LIt8,387
 panoptica/utils/citation_reminder.py,sha256=Hr6eU-5tQWpEWrR3roTHcpckUSHzuVU4rO8BWFwVpPo,793
 panoptica/utils/constants.py,sha256=_UAQkSQH2qxUCKoZXcz7-jDt3soCgp3fDQ32ABQvdng,1161
 panoptica/utils/edge_case_handling.py,sha256=sWWCRzqpupFXLP1c7-drYrxCdUhGwssE0hzK9eNL23Y,5398
 panoptica/utils/numpy_utils.py,sha256=CwY0jESaIHRlEH9iD7EnLhQYki8ndE_IxBi01UcEiSk,2859
 panoptica/utils/processing_pair.py,sha256=lnofIFWID4JvqmotcPNFymOKqxE5kTwplNlTwX6R6zs,14094
-panoptica-0.6.3.dist-info/LICENSE,sha256=snRxISApNqezxuidHHiQaF_LGd5KjbxGiXKZg3kjqs4,1506
-panoptica-0.6.3.dist-info/METADATA,sha256=iVIAJaZ9mH833EbHMqSlVDlnEnuWOVsI36rlBpAqoY4,5021
-panoptica-0.6.3.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-panoptica-0.6.3.dist-info/RECORD,,
+panoptica-0.6.4.dist-info/LICENSE,sha256=snRxISApNqezxuidHHiQaF_LGd5KjbxGiXKZg3kjqs4,1506
+panoptica-0.6.4.dist-info/METADATA,sha256=OLtfQ78jb7XJut1M_raYUf0U6cQtNhCNlXkDYIIfKls,5021
+panoptica-0.6.4.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+panoptica-0.6.4.dist-info/RECORD,,
```

