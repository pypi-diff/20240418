# Comparing `tmp/spine_segmentation-0.3.1.tar.gz` & `tmp/spine_segmentation-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spine_segmentation-0.3.1.tar", max compression
+gzip compressed data, was "spine_segmentation-0.3.2.tar", max compression
```

## Comparing `spine_segmentation-0.3.1.tar` & `spine_segmentation-0.3.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     1211 2024-04-11 11:32:29.446351 spine_segmentation-0.3.1/README.md
--rw-r--r--   0        0        0     2382 2024-04-16 14:16:45.618370 spine_segmentation-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      122 2024-04-11 12:53:48.914194 spine_segmentation-0.3.1/spine_segmentation/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.3.1/spine_segmentation/annotators/__init__.py
--rw-r--r--   0        0        0    16308 2024-04-11 12:53:48.934194 spine_segmentation-0.3.1/spine_segmentation/annotators/annotator_base.py
--rw-r--r--   0        0        0     8225 2024-04-11 12:53:48.814193 spine_segmentation-0.3.1/spine_segmentation/annotators/vector_annotator.py
--rw-r--r--   0        0        0     2190 2024-04-11 12:53:48.766192 spine_segmentation-0.3.1/spine_segmentation/cli/cli.py
--rw-r--r--   0        0        0    12072 2024-04-10 12:31:20.207512 spine_segmentation-0.3.1/spine_segmentation/dataloader/statistics.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.3.1/spine_segmentation/datasets/__init__.py
--rw-r--r--   0        0        0     2868 2024-04-10 12:31:20.207512 spine_segmentation-0.3.1/spine_segmentation/datasets/augmentation.py
--rw-r--r--   0        0        0     4312 2024-04-11 12:53:48.806193 spine_segmentation-0.3.1/spine_segmentation/datasets/feature_dataset.py
--rw-r--r--   0        0        0     6696 2024-04-11 15:53:29.418496 spine_segmentation-0.3.1/spine_segmentation/datasets/metadata_prediction_dataset.py
--rw-r--r--   0        0        0     6372 2024-04-11 15:53:29.430496 spine_segmentation-0.3.1/spine_segmentation/datasets/patch_segmentation_dataset.py
--rw-r--r--   0        0        0     1360 2024-04-11 15:53:29.410496 spine_segmentation-0.3.1/spine_segmentation/datasets/path_helper.py
--rw-r--r--   0        0        0    14744 2024-04-11 15:47:48.534212 spine_segmentation-0.3.1/spine_segmentation/datasets/sample.py
--rw-r--r--   0        0        0    14989 2024-04-11 15:53:29.422496 spine_segmentation-0.3.1/spine_segmentation/datasets/segmentation_dataset.py
--rw-r--r--   0        0        0     2037 2024-04-11 12:53:48.782192 spine_segmentation-0.3.1/spine_segmentation/datasets/vector_table_graphs_dataset.py
--rw-r--r--   0        0        0     2581 2024-04-11 12:53:48.890194 spine_segmentation-0.3.1/spine_segmentation/evaluate/analyze_edge_cases.py
--rw-r--r--   0        0        0     2520 2024-04-11 12:53:48.798193 spine_segmentation-0.3.1/spine_segmentation/evaluate/analyze_index_list.py
--rw-r--r--   0        0        0     1659 2024-04-11 12:53:48.854193 spine_segmentation-0.3.1/spine_segmentation/evaluate/classic_ml.py
--rw-r--r--   0        0        0     1108 2024-04-10 12:31:20.207512 spine_segmentation-0.3.1/spine_segmentation/evaluate/eval_created_stats.py
--rw-r--r--   0        0        0    15527 2024-04-11 15:52:07.339228 spine_segmentation-0.3.1/spine_segmentation/evaluate/eval_instance_seg_model.py
--rw-r--r--   0        0        0     8215 2024-04-11 12:53:48.746192 spine_segmentation-0.3.1/spine_segmentation/evaluate/eval_splitting.py
--rw-r--r--   0        0        0     6109 2024-04-11 15:52:07.363228 spine_segmentation-0.3.1/spine_segmentation/evaluate/load_model.py
--rw-r--r--   0        0        0     4885 2024-04-11 12:53:48.882194 spine_segmentation-0.3.1/spine_segmentation/evaluate/metadata.py
--rw-r--r--   0        0        0     1627 2024-04-11 12:53:48.894194 spine_segmentation-0.3.1/spine_segmentation/evaluate/volume_size_in_gt.py
--rw-r--r--   0        0        0     8409 2024-04-16 14:15:30.172895 spine_segmentation-0.3.1/spine_segmentation/inference/instance_segmentation.py
--rw-r--r--   0        0        0     7105 2024-04-16 13:56:59.020327 spine_segmentation-0.3.1/spine_segmentation/inference/onnx_model.py
--rw-r--r--   0        0        0     7515 2024-04-11 12:53:48.906194 spine_segmentation-0.3.1/spine_segmentation/instance_separation/instance_separation.py
--rw-r--r--   0        0        0      304 2024-04-10 12:31:20.207512 spine_segmentation-0.3.1/spine_segmentation/losses/diffis1.py
--rw-r--r--   0        0        0     2093 2024-04-16 12:12:21.446441 spine_segmentation-0.3.1/spine_segmentation/model_downloader/model_downloader.py
--rw-r--r--   0        0        0      712 2024-04-11 12:53:48.850193 spine_segmentation-0.3.1/spine_segmentation/plotting/bmi.py
--rw-r--r--   0        0        0     8132 2024-04-11 12:53:48.778192 spine_segmentation-0.3.1/spine_segmentation/plotting/classification_correlation.py
--rw-r--r--   0        0        0     2566 2024-04-11 12:53:48.886194 spine_segmentation-0.3.1/spine_segmentation/plotting/patient_metadata.py
--rw-r--r--   0        0        0    10404 2024-04-11 12:53:48.826193 spine_segmentation-0.3.1/spine_segmentation/plotting/plot_slice.py
--rw-r--r--   0        0        0     1795 2024-04-11 12:53:48.938195 spine_segmentation-0.3.1/spine_segmentation/plotting/plot_statistics.py
--rw-r--r--   0        0        0     5823 2024-04-11 12:53:48.834193 spine_segmentation-0.3.1/spine_segmentation/plotting/read_npz_eval_per_roi_accuracy.py
--rw-r--r--   0        0        0     5767 2024-04-11 12:53:48.786192 spine_segmentation-0.3.1/spine_segmentation/plotting/show_plane_splitting_3d.py
--rw-r--r--   0        0        0      266 2024-04-11 12:53:48.858193 spine_segmentation-0.3.1/spine_segmentation/plotting/ydata_profile_report.py
--rw-r--r--   0        0        0      930 2024-04-11 15:55:12.773382 spine_segmentation-0.3.1/spine_segmentation/resources/paths.py
--rw-r--r--   0        0        0      933 2024-04-11 12:53:48.842193 spine_segmentation-0.3.1/spine_segmentation/resources/preloaded.py
--rw-r--r--   0        0        0       63 2024-04-11 09:34:14.336647 spine_segmentation-0.3.1/spine_segmentation/run.py
--rw-r--r--   0        0        0     4575 2024-04-10 12:31:20.207512 spine_segmentation-0.3.1/spine_segmentation/scripts/format_results.py
--rw-r--r--   0        0        0     4546 2024-04-11 12:53:48.866193 spine_segmentation-0.3.1/spine_segmentation/scripts/split_train_val_test.py
--rw-r--r--   0        0        0      210 2024-04-10 12:31:20.207512 spine_segmentation-0.3.1/spine_segmentation/scripts/test_patient_ids.txt
--rw-r--r--   0        0        0      112 2024-04-10 18:52:49.798849 spine_segmentation-0.3.1/spine_segmentation/spine_types/disc.py
--rw-r--r--   0        0        0     1317 2024-04-16 11:21:51.078669 spine_segmentation-0.3.1/spine_segmentation/spine_types/labels.py
--rw-r--r--   0        0        0      219 2024-04-10 12:31:20.207512 spine_segmentation-0.3.1/spine_segmentation/spine_types/line_segment.py
--rw-r--r--   0        0        0     2409 2024-04-10 12:31:20.207512 spine_segmentation-0.3.1/spine_segmentation/spine_types/plane.py
--rw-r--r--   0        0        0       67 2024-04-10 12:31:20.207512 spine_segmentation-0.3.1/spine_segmentation/spine_types/roi.py
--rw-r--r--   0        0        0      246 2024-04-10 12:31:20.207512 spine_segmentation-0.3.1/spine_segmentation/spine_types/spine.py
--rw-r--r--   0        0        0      116 2024-04-10 18:52:49.974852 spine_segmentation-0.3.1/spine_segmentation/spine_types/vertebra.py
--rw-r--r--   0        0        0     1190 2024-04-11 12:53:48.874194 spine_segmentation-0.3.1/spine_segmentation/trainer/learning_rate_finder.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.3.1/spine_segmentation/utils/__init__.py
--rw-r--r--   0        0        0      685 2024-04-10 12:31:20.207512 spine_segmentation-0.3.1/spine_segmentation/utils/fix_validations_step_bar.py
--rw-r--r--   0        0        0      218 2024-04-10 12:31:20.207512 spine_segmentation-0.3.1/spine_segmentation/utils/globals.py
--rw-r--r--   0        0        0      552 2024-04-10 12:31:20.207512 spine_segmentation-0.3.1/spine_segmentation/utils/log_dir.py
--rw-r--r--   0        0        0      690 2024-04-10 12:31:20.207512 spine_segmentation-0.3.1/spine_segmentation/utils/profiling.py
--rw-r--r--   0        0        0      930 2024-04-10 12:31:20.207512 spine_segmentation-0.3.1/spine_segmentation/utils/proxy_class.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.3.1/spine_segmentation/visualisation/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.3.1/spine_segmentation/visualisation/blender/__init__.py
--rw-r--r--   0        0        0    11971 2024-04-10 12:31:20.207512 spine_segmentation-0.3.1/spine_segmentation/visualisation/blender/blender_script.py
--rw-r--r--   0        0        0     9179 2024-04-11 12:53:48.830193 spine_segmentation-0.3.1/spine_segmentation/visualisation/blender/gen_obj.py
--rw-r--r--   0        0        0     8158 2024-04-11 12:53:48.822193 spine_segmentation-0.3.1/spine_segmentation/visualisation/blender/open_in_blender.py
--rw-r--r--   0        0        0    12036 2024-04-10 12:31:20.207512 spine_segmentation-0.3.1/spine_segmentation/visualisation/color.py
--rw-r--r--   0        0        0     1705 2024-04-11 12:53:48.794192 spine_segmentation-0.3.1/spine_segmentation/visualisation/color_palettes.py
--rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 spine_segmentation-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-11 11:32:29.446351 spine_segmentation-0.3.2/README.md
+-rw-r--r--   0        0        0     2380 2024-04-18 11:43:43.663300 spine_segmentation-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-04-11 12:53:48.914194 spine_segmentation-0.3.2/spine_segmentation/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.3.2/spine_segmentation/annotators/__init__.py
+-rw-r--r--   0        0        0    16308 2024-04-11 12:53:48.934194 spine_segmentation-0.3.2/spine_segmentation/annotators/annotator_base.py
+-rw-r--r--   0        0        0     8225 2024-04-11 12:53:48.814193 spine_segmentation-0.3.2/spine_segmentation/annotators/vector_annotator.py
+-rw-r--r--   0        0        0     2190 2024-04-11 12:53:48.766192 spine_segmentation-0.3.2/spine_segmentation/cli/cli.py
+-rw-r--r--   0        0        0    12072 2024-04-10 12:31:20.207512 spine_segmentation-0.3.2/spine_segmentation/dataloader/statistics.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.3.2/spine_segmentation/datasets/__init__.py
+-rw-r--r--   0        0        0     2870 2024-04-17 08:50:53.510931 spine_segmentation-0.3.2/spine_segmentation/datasets/augmentation.py
+-rw-r--r--   0        0        0     4312 2024-04-11 12:53:48.806193 spine_segmentation-0.3.2/spine_segmentation/datasets/feature_dataset.py
+-rw-r--r--   0        0        0     6696 2024-04-11 15:53:29.418496 spine_segmentation-0.3.2/spine_segmentation/datasets/metadata_prediction_dataset.py
+-rw-r--r--   0        0        0     6372 2024-04-11 15:53:29.430496 spine_segmentation-0.3.2/spine_segmentation/datasets/patch_segmentation_dataset.py
+-rw-r--r--   0        0        0     1360 2024-04-17 15:04:24.163586 spine_segmentation-0.3.2/spine_segmentation/datasets/path_helper.py
+-rw-r--r--   0        0        0    14744 2024-04-11 15:47:48.534212 spine_segmentation-0.3.2/spine_segmentation/datasets/sample.py
+-rw-r--r--   0        0        0    14989 2024-04-11 15:53:29.422496 spine_segmentation-0.3.2/spine_segmentation/datasets/segmentation_dataset.py
+-rw-r--r--   0        0        0     2037 2024-04-11 12:53:48.782192 spine_segmentation-0.3.2/spine_segmentation/datasets/vector_table_graphs_dataset.py
+-rw-r--r--   0        0        0     2581 2024-04-11 12:53:48.890194 spine_segmentation-0.3.2/spine_segmentation/evaluate/analyze_edge_cases.py
+-rw-r--r--   0        0        0     2520 2024-04-11 12:53:48.798193 spine_segmentation-0.3.2/spine_segmentation/evaluate/analyze_index_list.py
+-rw-r--r--   0        0        0     1659 2024-04-11 12:53:48.854193 spine_segmentation-0.3.2/spine_segmentation/evaluate/classic_ml.py
+-rw-r--r--   0        0        0     1108 2024-04-10 12:31:20.207512 spine_segmentation-0.3.2/spine_segmentation/evaluate/eval_created_stats.py
+-rw-r--r--   0        0        0    15527 2024-04-11 15:52:07.339228 spine_segmentation-0.3.2/spine_segmentation/evaluate/eval_instance_seg_model.py
+-rw-r--r--   0        0        0     8215 2024-04-11 12:53:48.746192 spine_segmentation-0.3.2/spine_segmentation/evaluate/eval_splitting.py
+-rw-r--r--   0        0        0     6109 2024-04-11 15:52:07.363228 spine_segmentation-0.3.2/spine_segmentation/evaluate/load_model.py
+-rw-r--r--   0        0        0     4885 2024-04-11 12:53:48.882194 spine_segmentation-0.3.2/spine_segmentation/evaluate/metadata.py
+-rw-r--r--   0        0        0     1627 2024-04-11 12:53:48.894194 spine_segmentation-0.3.2/spine_segmentation/evaluate/volume_size_in_gt.py
+-rw-r--r--   0        0        0     8409 2024-04-16 14:15:30.172895 spine_segmentation-0.3.2/spine_segmentation/inference/instance_segmentation.py
+-rw-r--r--   0        0        0     7109 2024-04-18 11:44:20.196025 spine_segmentation-0.3.2/spine_segmentation/inference/onnx_model.py
+-rw-r--r--   0        0        0     7515 2024-04-11 12:53:48.906194 spine_segmentation-0.3.2/spine_segmentation/instance_separation/instance_separation.py
+-rw-r--r--   0        0        0      304 2024-04-10 12:31:20.207512 spine_segmentation-0.3.2/spine_segmentation/losses/diffis1.py
+-rw-r--r--   0        0        0     2093 2024-04-16 12:12:21.446441 spine_segmentation-0.3.2/spine_segmentation/model_downloader/model_downloader.py
+-rw-r--r--   0        0        0      712 2024-04-11 12:53:48.850193 spine_segmentation-0.3.2/spine_segmentation/plotting/bmi.py
+-rw-r--r--   0        0        0     8132 2024-04-11 12:53:48.778192 spine_segmentation-0.3.2/spine_segmentation/plotting/classification_correlation.py
+-rw-r--r--   0        0        0     2566 2024-04-11 12:53:48.886194 spine_segmentation-0.3.2/spine_segmentation/plotting/patient_metadata.py
+-rw-r--r--   0        0        0    10404 2024-04-11 12:53:48.826193 spine_segmentation-0.3.2/spine_segmentation/plotting/plot_slice.py
+-rw-r--r--   0        0        0     1795 2024-04-11 12:53:48.938195 spine_segmentation-0.3.2/spine_segmentation/plotting/plot_statistics.py
+-rw-r--r--   0        0        0     5823 2024-04-11 12:53:48.834193 spine_segmentation-0.3.2/spine_segmentation/plotting/read_npz_eval_per_roi_accuracy.py
+-rw-r--r--   0        0        0     5767 2024-04-11 12:53:48.786192 spine_segmentation-0.3.2/spine_segmentation/plotting/show_plane_splitting_3d.py
+-rw-r--r--   0        0        0      266 2024-04-11 12:53:48.858193 spine_segmentation-0.3.2/spine_segmentation/plotting/ydata_profile_report.py
+-rw-r--r--   0        0        0      930 2024-04-11 15:55:12.773382 spine_segmentation-0.3.2/spine_segmentation/resources/paths.py
+-rw-r--r--   0        0        0      933 2024-04-11 12:53:48.842193 spine_segmentation-0.3.2/spine_segmentation/resources/preloaded.py
+-rw-r--r--   0        0        0       63 2024-04-11 09:34:14.336647 spine_segmentation-0.3.2/spine_segmentation/run.py
+-rw-r--r--   0        0        0     4575 2024-04-10 12:31:20.207512 spine_segmentation-0.3.2/spine_segmentation/scripts/format_results.py
+-rw-r--r--   0        0        0     4546 2024-04-11 12:53:48.866193 spine_segmentation-0.3.2/spine_segmentation/scripts/split_train_val_test.py
+-rw-r--r--   0        0        0      210 2024-04-10 12:31:20.207512 spine_segmentation-0.3.2/spine_segmentation/scripts/test_patient_ids.txt
+-rw-r--r--   0        0        0      112 2024-04-10 18:52:49.798849 spine_segmentation-0.3.2/spine_segmentation/spine_types/disc.py
+-rw-r--r--   0        0        0     1317 2024-04-16 11:21:51.078669 spine_segmentation-0.3.2/spine_segmentation/spine_types/labels.py
+-rw-r--r--   0        0        0      219 2024-04-10 12:31:20.207512 spine_segmentation-0.3.2/spine_segmentation/spine_types/line_segment.py
+-rw-r--r--   0        0        0     2409 2024-04-10 12:31:20.207512 spine_segmentation-0.3.2/spine_segmentation/spine_types/plane.py
+-rw-r--r--   0        0        0       67 2024-04-10 12:31:20.207512 spine_segmentation-0.3.2/spine_segmentation/spine_types/roi.py
+-rw-r--r--   0        0        0      246 2024-04-10 12:31:20.207512 spine_segmentation-0.3.2/spine_segmentation/spine_types/spine.py
+-rw-r--r--   0        0        0      116 2024-04-10 18:52:49.974852 spine_segmentation-0.3.2/spine_segmentation/spine_types/vertebra.py
+-rw-r--r--   0        0        0     1190 2024-04-11 12:53:48.874194 spine_segmentation-0.3.2/spine_segmentation/trainer/learning_rate_finder.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.3.2/spine_segmentation/utils/__init__.py
+-rw-r--r--   0        0        0      685 2024-04-10 12:31:20.207512 spine_segmentation-0.3.2/spine_segmentation/utils/fix_validations_step_bar.py
+-rw-r--r--   0        0        0      218 2024-04-10 12:31:20.207512 spine_segmentation-0.3.2/spine_segmentation/utils/globals.py
+-rw-r--r--   0        0        0      552 2024-04-10 12:31:20.207512 spine_segmentation-0.3.2/spine_segmentation/utils/log_dir.py
+-rw-r--r--   0        0        0      690 2024-04-10 12:31:20.207512 spine_segmentation-0.3.2/spine_segmentation/utils/profiling.py
+-rw-r--r--   0        0        0      930 2024-04-10 12:31:20.207512 spine_segmentation-0.3.2/spine_segmentation/utils/proxy_class.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.3.2/spine_segmentation/visualisation/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.3.2/spine_segmentation/visualisation/blender/__init__.py
+-rw-r--r--   0        0        0    11971 2024-04-10 12:31:20.207512 spine_segmentation-0.3.2/spine_segmentation/visualisation/blender/blender_script.py
+-rw-r--r--   0        0        0     9179 2024-04-11 12:53:48.830193 spine_segmentation-0.3.2/spine_segmentation/visualisation/blender/gen_obj.py
+-rw-r--r--   0        0        0     8158 2024-04-11 12:53:48.822193 spine_segmentation-0.3.2/spine_segmentation/visualisation/blender/open_in_blender.py
+-rw-r--r--   0        0        0    12036 2024-04-10 12:31:20.207512 spine_segmentation-0.3.2/spine_segmentation/visualisation/color.py
+-rw-r--r--   0        0        0     1705 2024-04-11 12:53:48.794192 spine_segmentation-0.3.2/spine_segmentation/visualisation/color_palettes.py
+-rw-r--r--   0        0        0     2588 1970-01-01 00:00:00.000000 spine_segmentation-0.3.2/PKG-INFO
```

### Comparing `spine_segmentation-0.3.1/README.md` & `spine_segmentation-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/pyproject.toml` & `spine_segmentation-0.3.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spine-segmentation"
-version = "0.3.1"
+version = "0.3.2"
 description = "Anatomical labeling of the spine in small field-of-view MRI scans"
 authors = [
     "Brutenis Gliwa <brutenis@gmail.com>",
 ]
 readme = "README.md"
 
 classifiers = [
@@ -22,16 +22,16 @@
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.13.0"
 numpy = "^1.23.0"                       # basic
 #torch = "^2.1.1"
 #torch-geometric = "^2.3.1"              # gnn in pytorch
 #lightning = "^2.2.1"
 # onnx = "^1.14.1"
-onnxruntime = "^1.15.1"
-onnxruntime-gpu = "^1.15.1"
+onnxruntime = "1.17.1"
+onnxruntime-gpu = "1.17.1"
 #torchvision = "^0.17.2"
 tqdm = "^4.66.2"
 requests = "^2.28.0"
 xxhash = "^3.4.1"
 connected-components-3d = "^3.12.1"     # algorithms for finding connected compoents
 pandas = "<2.0"
 scikit-learn = "^1.2.2"                 # ML
```

### Comparing `spine_segmentation-0.3.1/spine_segmentation/annotators/annotator_base.py` & `spine_segmentation-0.3.2/spine_segmentation/annotators/annotator_base.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/annotators/vector_annotator.py` & `spine_segmentation-0.3.2/spine_segmentation/annotators/vector_annotator.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/cli/cli.py` & `spine_segmentation-0.3.2/spine_segmentation/cli/cli.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/dataloader/statistics.py` & `spine_segmentation-0.3.2/spine_segmentation/dataloader/statistics.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/datasets/augmentation.py` & `spine_segmentation-0.3.2/spine_segmentation/datasets/augmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self.use_mask = use_mask
 
         # === GEOMETRIC ===
         geometric_augmentations = []
 
         if geometric_aug_type == "all":
             geometric_augmentations += [
-                K.RandomVerticalFlip(),  # Note that patient is lying on back, so this is actually a horizontal flip
+                # K.RandomVerticalFlip(),  # Note that patient is lying on back, so this is actually a horizontal flip
                 K.RandomAffine(degrees=20, translate=(0.1, 0.1), scale=(0.8, 1.2), p=0.50),
             ]
 
         if cropping_type == "same":
             geometric_augmentations += [
                 K.RandomCrop((320, 300), p=1.0),
                 K.PadTo((320, 896)),
```

### Comparing `spine_segmentation-0.3.1/spine_segmentation/datasets/feature_dataset.py` & `spine_segmentation-0.3.2/spine_segmentation/datasets/feature_dataset.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/datasets/metadata_prediction_dataset.py` & `spine_segmentation-0.3.2/spine_segmentation/datasets/metadata_prediction_dataset.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/datasets/patch_segmentation_dataset.py` & `spine_segmentation-0.3.2/spine_segmentation/datasets/patch_segmentation_dataset.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/datasets/path_helper.py` & `spine_segmentation-0.3.2/spine_segmentation/datasets/path_helper.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/datasets/sample.py` & `spine_segmentation-0.3.2/spine_segmentation/datasets/sample.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/datasets/segmentation_dataset.py` & `spine_segmentation-0.3.2/spine_segmentation/datasets/segmentation_dataset.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/datasets/vector_table_graphs_dataset.py` & `spine_segmentation-0.3.2/spine_segmentation/datasets/vector_table_graphs_dataset.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/evaluate/analyze_edge_cases.py` & `spine_segmentation-0.3.2/spine_segmentation/evaluate/analyze_edge_cases.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/evaluate/analyze_index_list.py` & `spine_segmentation-0.3.2/spine_segmentation/evaluate/analyze_index_list.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/evaluate/classic_ml.py` & `spine_segmentation-0.3.2/spine_segmentation/evaluate/classic_ml.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/evaluate/eval_created_stats.py` & `spine_segmentation-0.3.2/spine_segmentation/evaluate/eval_created_stats.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/evaluate/eval_instance_seg_model.py` & `spine_segmentation-0.3.2/spine_segmentation/evaluate/eval_instance_seg_model.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/evaluate/eval_splitting.py` & `spine_segmentation-0.3.2/spine_segmentation/evaluate/eval_splitting.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/evaluate/load_model.py` & `spine_segmentation-0.3.2/spine_segmentation/evaluate/load_model.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/evaluate/metadata.py` & `spine_segmentation-0.3.2/spine_segmentation/evaluate/metadata.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/evaluate/volume_size_in_gt.py` & `spine_segmentation-0.3.2/spine_segmentation/evaluate/volume_size_in_gt.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/inference/instance_segmentation.py` & `spine_segmentation-0.3.2/spine_segmentation/inference/instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/inference/onnx_model.py` & `spine_segmentation-0.3.2/spine_segmentation/inference/onnx_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,14 +52,18 @@
     @staticmethod
     def get_best_instance_segmentation_model(*args, **kwargs):
         # model_url = "https://github.com/LiquidFun/Spine/releases/download/onnx_models_1.0.0/2023-11-09_Seg25_Unet_resnet152_vert-only_896px_no-input-seg.onnx"
         model_url = "https://github.com/LiquidFun/Spine/releases/download/onnx_models_1.0.0/2023-11-06_Seg25_Unet_mitb5_vert-only_896px_no-input-seg.onnx"
         onnx_model_path = download_file_with_progress(model_url)
         return ONNXInferenceModel(onnx_model_path, *args, **kwargs, is_segmentation_model=False)
 
+
+
+
+
     def save_index_list(self):
         path = self.cache_path / "index_list.npz"
         np.savez_compressed(
             path,
             index_to_npz_path=self.index_to_npz_path,
             index_to_slice_index=self.index_to_slice_index,
             index_to_series_id=self.index_to_series_id,
```

### Comparing `spine_segmentation-0.3.1/spine_segmentation/instance_separation/instance_separation.py` & `spine_segmentation-0.3.2/spine_segmentation/instance_separation/instance_separation.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/model_downloader/model_downloader.py` & `spine_segmentation-0.3.2/spine_segmentation/model_downloader/model_downloader.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/plotting/bmi.py` & `spine_segmentation-0.3.2/spine_segmentation/plotting/bmi.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/plotting/classification_correlation.py` & `spine_segmentation-0.3.2/spine_segmentation/plotting/classification_correlation.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/plotting/patient_metadata.py` & `spine_segmentation-0.3.2/spine_segmentation/plotting/patient_metadata.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/plotting/plot_slice.py` & `spine_segmentation-0.3.2/spine_segmentation/plotting/plot_slice.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/plotting/plot_statistics.py` & `spine_segmentation-0.3.2/spine_segmentation/plotting/plot_statistics.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/plotting/read_npz_eval_per_roi_accuracy.py` & `spine_segmentation-0.3.2/spine_segmentation/plotting/read_npz_eval_per_roi_accuracy.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/plotting/show_plane_splitting_3d.py` & `spine_segmentation-0.3.2/spine_segmentation/plotting/show_plane_splitting_3d.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/resources/paths.py` & `spine_segmentation-0.3.2/spine_segmentation/resources/paths.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/resources/preloaded.py` & `spine_segmentation-0.3.2/spine_segmentation/resources/preloaded.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/scripts/format_results.py` & `spine_segmentation-0.3.2/spine_segmentation/scripts/format_results.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/scripts/split_train_val_test.py` & `spine_segmentation-0.3.2/spine_segmentation/scripts/split_train_val_test.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/spine_types/labels.py` & `spine_segmentation-0.3.2/spine_segmentation/spine_types/labels.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/spine_types/plane.py` & `spine_segmentation-0.3.2/spine_segmentation/spine_types/plane.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/trainer/learning_rate_finder.py` & `spine_segmentation-0.3.2/spine_segmentation/trainer/learning_rate_finder.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/utils/fix_validations_step_bar.py` & `spine_segmentation-0.3.2/spine_segmentation/utils/fix_validations_step_bar.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/utils/log_dir.py` & `spine_segmentation-0.3.2/spine_segmentation/utils/log_dir.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/utils/profiling.py` & `spine_segmentation-0.3.2/spine_segmentation/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/utils/proxy_class.py` & `spine_segmentation-0.3.2/spine_segmentation/utils/proxy_class.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/visualisation/blender/blender_script.py` & `spine_segmentation-0.3.2/spine_segmentation/visualisation/blender/blender_script.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/visualisation/blender/gen_obj.py` & `spine_segmentation-0.3.2/spine_segmentation/visualisation/blender/gen_obj.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/visualisation/blender/open_in_blender.py` & `spine_segmentation-0.3.2/spine_segmentation/visualisation/blender/open_in_blender.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/visualisation/color.py` & `spine_segmentation-0.3.2/spine_segmentation/visualisation/color.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/spine_segmentation/visualisation/color_palettes.py` & `spine_segmentation-0.3.2/spine_segmentation/visualisation/color_palettes.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.3.1/PKG-INFO` & `spine_segmentation-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spine-segmentation
-Version: 0.3.1
+Version: 0.3.2
 Summary: Anatomical labeling of the spine in small field-of-view MRI scans
 Author: Brutenis Gliwa
 Author-email: brutenis@gmail.com
 Requires-Python: >=3.8.1,<3.13.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -17,16 +17,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: connected-components-3d (>=3.12.1,<4.0.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: nibabel (>=5.1.0,<6.0.0)
 Requires-Dist: numpy (>=1.23.0,<2.0.0)
-Requires-Dist: onnxruntime (>=1.15.1,<2.0.0)
-Requires-Dist: onnxruntime-gpu (>=1.15.1,<2.0.0)
+Requires-Dist: onnxruntime (==1.17.1)
+Requires-Dist: onnxruntime-gpu (==1.17.1)
 Requires-Dist: pandas (<2.0)
 Requires-Dist: pydicom (>=2.4.3,<3.0.0)
 Requires-Dist: requests (>=2.28.0,<3.0.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: seaborn (>=0.13.0,<0.14.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: xxhash (>=3.4.1,<4.0.0)
```

