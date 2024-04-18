# Comparing `tmp/dg_tta-1.0.8.tar.gz` & `tmp/dg_tta-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dg_tta-1.0.8.tar", max compression
+gzip compressed data, was "dg_tta-1.0.9.tar", max compression
```

## Comparing `dg_tta-1.0.8.tar` & `dg_tta-1.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rwxr-xr-x   0        0        0     1071 2023-12-19 20:23:25.759977 dg_tta-1.0.8/LICENSE
--rwxr-xr-x   0        0        0     3673 2023-12-20 13:00:54.996032 dg_tta-1.0.8/README.md
--rwxr-xr-x   0        0        0     1004 2023-12-20 12:48:06.956093 dg_tta-1.0.8/dg_tta/__build__.py
--rwxr-xr-x   0        0        0        0 2023-12-12 13:35:08.707451 dg_tta-1.0.8/dg_tta/__init__.py
--rwxr-xr-x   0        0        0   261146 2023-12-19 18:16:24.312507 dg_tta-1.0.8/dg_tta/__resources__/TS104_input_view.png
--rwxr-xr-x   0        0        0     2851 2023-12-19 17:58:59.681072 dg_tta-1.0.8/dg_tta/__resources__/check_tta_input.ipynb
--rwxr-xr-x   0        0        0    78835 2023-12-19 16:43:22.182361 dg_tta-1.0.8/dg_tta/__resources__/dummy_results/nnUNetTrainer_GIN_MIND__nnUNetPlans__3d_fullres/dataset.json
--rwxr-xr-x   0        0        0    92616 2023-12-19 16:43:22.185531 dg_tta-1.0.8/dg_tta/__resources__/dummy_results/nnUNetTrainer_GIN_MIND__nnUNetPlans__3d_fullres/dataset_fingerprint.json
--rwxr-xr-x   0        0        0    10645 2023-12-19 16:43:22.188147 dg_tta-1.0.8/dg_tta/__resources__/dummy_results/nnUNetTrainer_GIN_MIND__nnUNetPlans__3d_fullres/plans.json
--rwxr-xr-x   0        0        0    78835 2023-12-19 16:43:22.320047 dg_tta-1.0.8/dg_tta/__resources__/dummy_results/nnUNetTrainer_GIN__nnUNetPlans__3d_fullres/dataset.json
--rwxr-xr-x   0        0        0    92616 2023-12-19 16:43:22.312490 dg_tta-1.0.8/dg_tta/__resources__/dummy_results/nnUNetTrainer_GIN__nnUNetPlans__3d_fullres/dataset_fingerprint.json
--rwxr-xr-x   0        0        0    10645 2023-12-19 16:43:22.313690 dg_tta-1.0.8/dg_tta/__resources__/dummy_results/nnUNetTrainer_GIN__nnUNetPlans__3d_fullres/plans.json
--rwxr-xr-x   0        0        0    78835 2023-12-19 16:43:22.053618 dg_tta-1.0.8/dg_tta/__resources__/dummy_results/nnUNetTrainer_MIND__nnUNetPlans__3d_fullres/dataset.json
--rwxr-xr-x   0        0        0    92616 2023-12-19 16:43:22.058756 dg_tta-1.0.8/dg_tta/__resources__/dummy_results/nnUNetTrainer_MIND__nnUNetPlans__3d_fullres/dataset_fingerprint.json
--rwxr-xr-x   0        0        0    10645 2023-12-19 16:43:22.057925 dg_tta-1.0.8/dg_tta/__resources__/dummy_results/nnUNetTrainer_MIND__nnUNetPlans__3d_fullres/plans.json
--rwxr-xr-x   0        0        0     8257 2023-12-18 17:05:52.636375 dg_tta-1.0.8/dg_tta/gin.py
--rwxr-xr-x   0        0        0     5190 2023-12-18 17:05:28.570982 dg_tta-1.0.8/dg_tta/mind.py
--rwxr-xr-x   0        0        0        0 2023-12-18 17:32:53.200726 dg_tta-1.0.8/dg_tta/pretraining/__init__.py
--rwxr-xr-x   0        0        0     1413 2023-12-19 20:57:53.079598 dg_tta-1.0.8/dg_tta/pretraining/nnUNetTrainer_GIN.py
--rwxr-xr-x   0        0        0     1555 2023-12-19 20:57:48.508684 dg_tta-1.0.8/dg_tta/pretraining/nnUNetTrainer_GIN_MIND.py
--rwxr-xr-x   0        0        0     1355 2023-12-19 20:57:58.354646 dg_tta-1.0.8/dg_tta/pretraining/nnUNetTrainer_MIND.py
--rwxr-xr-x   0        0        0     7397 2023-12-20 12:48:52.333782 dg_tta-1.0.8/dg_tta/run.py
--rwxr-xr-x   0        0        0        0 2023-12-13 12:40:26.990987 dg_tta-1.0.8/dg_tta/tta/__init__.py
--rwxr-xr-x   0        0        0     6043 2023-12-18 17:09:06.723257 dg_tta-1.0.8/dg_tta/tta/augmentation_utils.py
--rwxr-xr-x   0        0        0    13993 2023-12-20 12:09:37.756765 dg_tta-1.0.8/dg_tta/tta/config_log_utils.py
--rwxr-xr-x   0        0        0     4513 2023-12-19 18:18:18.381813 dg_tta-1.0.8/dg_tta/tta/ipynb_utils.py
--rwxr-xr-x   0        0        0     1873 2023-12-20 08:23:23.991343 dg_tta-1.0.8/dg_tta/tta/model_utils.py
--rwxr-xr-x   0        0        0     6268 2023-12-20 12:01:32.519369 dg_tta-1.0.8/dg_tta/tta/nnunet_utils.py
--rwxr-xr-x   0        0        0     8545 2023-12-19 15:37:41.983491 dg_tta-1.0.8/dg_tta/tta/torch_utils.py
--rwxr-xr-x   0        0        0    19477 2023-12-20 12:10:48.284672 dg_tta-1.0.8/dg_tta/tta/tta.py
--rwxr-xr-x   0        0        0      777 2023-12-19 19:54:12.895283 dg_tta-1.0.8/dg_tta/utils.py
--rwxr-xr-x   0        0        0      759 2023-12-20 13:01:08.317712 dg_tta-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     4350 1970-01-01 00:00:00.000000 dg_tta-1.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1071 2023-12-19 20:23:25.759977 dg_tta-1.0.9/LICENSE
+-rwxr-xr-x   0        0        0     3673 2023-12-20 13:00:54.996032 dg_tta-1.0.9/README.md
+-rwxr-xr-x   0        0        0     1004 2023-12-20 12:48:06.956093 dg_tta-1.0.9/dg_tta/__build__.py
+-rwxr-xr-x   0        0        0        0 2023-12-12 13:35:08.707451 dg_tta-1.0.9/dg_tta/__init__.py
+-rwxr-xr-x   0        0        0   261146 2023-12-19 18:16:24.312507 dg_tta-1.0.9/dg_tta/__resources__/TS104_input_view.png
+-rwxr-xr-x   0        0        0     2851 2023-12-19 17:58:59.681072 dg_tta-1.0.9/dg_tta/__resources__/check_tta_input.ipynb
+-rwxr-xr-x   0        0        0    78835 2023-12-19 16:43:22.182361 dg_tta-1.0.9/dg_tta/__resources__/dummy_results/nnUNetTrainer_GIN_MIND__nnUNetPlans__3d_fullres/dataset.json
+-rwxr-xr-x   0        0        0    92616 2023-12-19 16:43:22.185531 dg_tta-1.0.9/dg_tta/__resources__/dummy_results/nnUNetTrainer_GIN_MIND__nnUNetPlans__3d_fullres/dataset_fingerprint.json
+-rwxr-xr-x   0        0        0    10645 2023-12-19 16:43:22.188147 dg_tta-1.0.9/dg_tta/__resources__/dummy_results/nnUNetTrainer_GIN_MIND__nnUNetPlans__3d_fullres/plans.json
+-rwxr-xr-x   0        0        0    78835 2023-12-19 16:43:22.320047 dg_tta-1.0.9/dg_tta/__resources__/dummy_results/nnUNetTrainer_GIN__nnUNetPlans__3d_fullres/dataset.json
+-rwxr-xr-x   0        0        0    92616 2023-12-19 16:43:22.312490 dg_tta-1.0.9/dg_tta/__resources__/dummy_results/nnUNetTrainer_GIN__nnUNetPlans__3d_fullres/dataset_fingerprint.json
+-rwxr-xr-x   0        0        0    10645 2023-12-19 16:43:22.313690 dg_tta-1.0.9/dg_tta/__resources__/dummy_results/nnUNetTrainer_GIN__nnUNetPlans__3d_fullres/plans.json
+-rwxr-xr-x   0        0        0    78835 2023-12-19 16:43:22.053618 dg_tta-1.0.9/dg_tta/__resources__/dummy_results/nnUNetTrainer_MIND__nnUNetPlans__3d_fullres/dataset.json
+-rwxr-xr-x   0        0        0    92616 2023-12-19 16:43:22.058756 dg_tta-1.0.9/dg_tta/__resources__/dummy_results/nnUNetTrainer_MIND__nnUNetPlans__3d_fullres/dataset_fingerprint.json
+-rwxr-xr-x   0        0        0    10645 2023-12-19 16:43:22.057925 dg_tta-1.0.9/dg_tta/__resources__/dummy_results/nnUNetTrainer_MIND__nnUNetPlans__3d_fullres/plans.json
+-rwxr-xr-x   0        0        0     8257 2023-12-18 17:05:52.636375 dg_tta-1.0.9/dg_tta/gin.py
+-rwxr-xr-x   0        0        0     5190 2023-12-18 17:05:28.570982 dg_tta-1.0.9/dg_tta/mind.py
+-rwxr-xr-x   0        0        0        0 2023-12-18 17:32:53.200726 dg_tta-1.0.9/dg_tta/pretraining/__init__.py
+-rwxr-xr-x   0        0        0     1413 2023-12-19 20:57:53.079598 dg_tta-1.0.9/dg_tta/pretraining/nnUNetTrainer_GIN.py
+-rwxr-xr-x   0        0        0     1555 2023-12-19 20:57:48.508684 dg_tta-1.0.9/dg_tta/pretraining/nnUNetTrainer_GIN_MIND.py
+-rwxr-xr-x   0        0        0     1355 2023-12-19 20:57:58.354646 dg_tta-1.0.9/dg_tta/pretraining/nnUNetTrainer_MIND.py
+-rwxr-xr-x   0        0        0     7397 2023-12-20 12:48:52.333782 dg_tta-1.0.9/dg_tta/run.py
+-rwxr-xr-x   0        0        0        0 2023-12-13 12:40:26.990987 dg_tta-1.0.9/dg_tta/tta/__init__.py
+-rwxr-xr-x   0        0        0     6043 2023-12-18 17:09:06.723257 dg_tta-1.0.9/dg_tta/tta/augmentation_utils.py
+-rwxr-xr-x   0        0        0    13986 2023-12-20 13:42:14.127556 dg_tta-1.0.9/dg_tta/tta/config_log_utils.py
+-rwxr-xr-x   0        0        0     4513 2023-12-19 18:18:18.381813 dg_tta-1.0.9/dg_tta/tta/ipynb_utils.py
+-rwxr-xr-x   0        0        0     1873 2023-12-20 08:23:23.991343 dg_tta-1.0.9/dg_tta/tta/model_utils.py
+-rwxr-xr-x   0        0        0     6268 2023-12-20 12:01:32.519369 dg_tta-1.0.9/dg_tta/tta/nnunet_utils.py
+-rwxr-xr-x   0        0        0     8545 2023-12-19 15:37:41.983491 dg_tta-1.0.9/dg_tta/tta/torch_utils.py
+-rwxr-xr-x   0        0        0    19477 2023-12-20 12:10:48.284672 dg_tta-1.0.9/dg_tta/tta/tta.py
+-rwxr-xr-x   0        0        0      777 2023-12-19 19:54:12.895283 dg_tta-1.0.9/dg_tta/utils.py
+-rwxr-xr-x   0        0        0      759 2023-12-20 13:53:57.602908 dg_tta-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4350 1970-01-01 00:00:00.000000 dg_tta-1.0.9/PKG-INFO
```

### Comparing `dg_tta-1.0.8/LICENSE` & `dg_tta-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/README.md` & `dg_tta-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/dg_tta/__build__.py` & `dg_tta-1.0.9/dg_tta/__build__.py`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/dg_tta/__resources__/TS104_input_view.png` & `dg_tta-1.0.9/dg_tta/__resources__/TS104_input_view.png`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/dg_tta/__resources__/check_tta_input.ipynb` & `dg_tta-1.0.9/dg_tta/__resources__/check_tta_input.ipynb`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/dg_tta/__resources__/dummy_results/nnUNetTrainer_GIN_MIND__nnUNetPlans__3d_fullres/dataset.json` & `dg_tta-1.0.9/dg_tta/__resources__/dummy_results/nnUNetTrainer_GIN_MIND__nnUNetPlans__3d_fullres/dataset.json`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/dg_tta/__resources__/dummy_results/nnUNetTrainer_GIN_MIND__nnUNetPlans__3d_fullres/dataset_fingerprint.json` & `dg_tta-1.0.9/dg_tta/__resources__/dummy_results/nnUNetTrainer_GIN_MIND__nnUNetPlans__3d_fullres/dataset_fingerprint.json`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/dg_tta/__resources__/dummy_results/nnUNetTrainer_GIN_MIND__nnUNetPlans__3d_fullres/plans.json` & `dg_tta-1.0.9/dg_tta/__resources__/dummy_results/nnUNetTrainer_GIN_MIND__nnUNetPlans__3d_fullres/plans.json`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/dg_tta/__resources__/dummy_results/nnUNetTrainer_GIN__nnUNetPlans__3d_fullres/dataset.json` & `dg_tta-1.0.9/dg_tta/__resources__/dummy_results/nnUNetTrainer_GIN__nnUNetPlans__3d_fullres/dataset.json`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/dg_tta/__resources__/dummy_results/nnUNetTrainer_GIN__nnUNetPlans__3d_fullres/dataset_fingerprint.json` & `dg_tta-1.0.9/dg_tta/__resources__/dummy_results/nnUNetTrainer_GIN__nnUNetPlans__3d_fullres/dataset_fingerprint.json`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/dg_tta/__resources__/dummy_results/nnUNetTrainer_GIN__nnUNetPlans__3d_fullres/plans.json` & `dg_tta-1.0.9/dg_tta/__resources__/dummy_results/nnUNetTrainer_GIN__nnUNetPlans__3d_fullres/plans.json`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/dg_tta/__resources__/dummy_results/nnUNetTrainer_MIND__nnUNetPlans__3d_fullres/dataset.json` & `dg_tta-1.0.9/dg_tta/__resources__/dummy_results/nnUNetTrainer_MIND__nnUNetPlans__3d_fullres/dataset.json`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/dg_tta/__resources__/dummy_results/nnUNetTrainer_MIND__nnUNetPlans__3d_fullres/dataset_fingerprint.json` & `dg_tta-1.0.9/dg_tta/__resources__/dummy_results/nnUNetTrainer_MIND__nnUNetPlans__3d_fullres/dataset_fingerprint.json`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/dg_tta/__resources__/dummy_results/nnUNetTrainer_MIND__nnUNetPlans__3d_fullres/plans.json` & `dg_tta-1.0.9/dg_tta/__resources__/dummy_results/nnUNetTrainer_MIND__nnUNetPlans__3d_fullres/plans.json`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/dg_tta/gin.py` & `dg_tta-1.0.9/dg_tta/gin.py`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/dg_tta/mind.py` & `dg_tta-1.0.9/dg_tta/mind.py`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/dg_tta/pretraining/nnUNetTrainer_GIN.py` & `dg_tta-1.0.9/dg_tta/pretraining/nnUNetTrainer_GIN.py`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/dg_tta/pretraining/nnUNetTrainer_GIN_MIND.py` & `dg_tta-1.0.9/dg_tta/pretraining/nnUNetTrainer_GIN_MIND.py`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/dg_tta/pretraining/nnUNetTrainer_MIND.py` & `dg_tta-1.0.9/dg_tta/pretraining/nnUNetTrainer_MIND.py`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/dg_tta/run.py` & `dg_tta-1.0.9/dg_tta/run.py`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/dg_tta/tta/augmentation_utils.py` & `dg_tta-1.0.9/dg_tta/tta/augmentation_utils.py`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/dg_tta/tta/config_log_utils.py` & `dg_tta-1.0.9/dg_tta/tta/config_log_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,15 +296,15 @@
     else:
         raise ValueError()
 
     dummy_results_path = get_resources_dir() / "dummy_results" / pretrainer_dir
     target_path = pretrained_weights_dir / pretrainer_dir
     target_path_weights = target_path / "fold_0" / "checkpoint_final.pth"
 
-    target_path.parent.mkdir(exist_ok=True)
+    target_path.mkdir(exist_ok=True)
     target_path_weights.parent.mkdir(exist_ok=True)
 
     # Copy dummy pretraining results (folder structure and nnUNet fils)
     shutil.copytree(dummy_results_path, target_path, dirs_exist_ok=True)
 
     if not target_path_weights.exists():
         subprocess.run(["wget", dl_link, "-O", target_path_weights])
```

### Comparing `dg_tta-1.0.8/dg_tta/tta/ipynb_utils.py` & `dg_tta-1.0.9/dg_tta/tta/ipynb_utils.py`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/dg_tta/tta/model_utils.py` & `dg_tta-1.0.9/dg_tta/tta/model_utils.py`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/dg_tta/tta/nnunet_utils.py` & `dg_tta-1.0.9/dg_tta/tta/nnunet_utils.py`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/dg_tta/tta/torch_utils.py` & `dg_tta-1.0.9/dg_tta/tta/torch_utils.py`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/dg_tta/tta/tta.py` & `dg_tta-1.0.9/dg_tta/tta/tta.py`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/dg_tta/utils.py` & `dg_tta-1.0.9/dg_tta/utils.py`

 * *Files identical despite different names*

### Comparing `dg_tta-1.0.8/pyproject.toml` & `dg_tta-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dg-tta"
-version = "1.0.8"
+version = "1.0.9"
 description = "DG-TTA: Out-of-domain medical image segmentation through Domain Generalization and Test-Time Adaptation"
 authors = [
     "Christian Weihsbach <christian.weihsbach@uni-luebeck.de>",
     "Christian N. Kruse <christian.kruse@tngtech.com>",
     "Alexander Bigalke <alexander.bigalke@uni-luebeck.de>",
     "Mattias P. Heinrich <mattias.heinrich@uni-luebeck.de>"
 ]
```

### Comparing `dg_tta-1.0.8/PKG-INFO` & `dg_tta-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dg-tta
-Version: 1.0.8
+Version: 1.0.9
 Summary: DG-TTA: Out-of-domain medical image segmentation through Domain Generalization and Test-Time Adaptation
 Author: Christian Weihsbach
 Author-email: christian.weihsbach@uni-luebeck.de
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

