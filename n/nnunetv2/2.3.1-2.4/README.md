# Comparing `tmp/nnunetv2-2.3.1.tar.gz` & `tmp/nnunetv2-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnunetv2-2.3.1.tar", last modified: Wed Feb 21 20:50:40 2024, max compression
+gzip compressed data, was "nnunetv2-2.4.tar", last modified: Thu Apr 18 09:20:23 2024, max compression
```

## Comparing `nnunetv2-2.3.1.tar` & `nnunetv2-2.4.tar`

### file list

```diff
@@ -1,223 +1,226 @@
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.675083 nnunetv2-2.3.1/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    11427 2023-03-17 08:55:29.000000 nnunetv2-2.3.1/LICENSE
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    24140 2024-02-21 20:50:40.675083 nnunetv2-2.3.1/PKG-INFO
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.659083 nnunetv2-2.3.1/nnunetv2/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/__init__.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.659083 nnunetv2-2.3.1/nnunetv2/batch_running/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/batch_running/__init__.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.659083 nnunetv2-2.3.1/nnunetv2/batch_running/benchmarking/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/batch_running/benchmarking/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2041 2023-10-27 11:39:44.000000 nnunetv2-2.3.1/nnunetv2/batch_running/benchmarking/generate_benchmarking_commands.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3272 2023-10-27 11:39:44.000000 nnunetv2-2.3.1/nnunetv2/batch_running/benchmarking/summarize_benchmark_results.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     5798 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/batch_running/collect_results_custom_Decathlon.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      708 2024-02-19 15:41:35.000000 nnunetv2-2.3.1/nnunetv2/batch_running/collect_results_custom_Decathlon_2d.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3300 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/batch_running/generate_lsf_runs_customDecathlon.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.659083 nnunetv2-2.3.1/nnunetv2/batch_running/release_trainings/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/batch_running/release_trainings/__init__.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.659083 nnunetv2-2.3.1/nnunetv2/batch_running/release_trainings/nnunetv2_v1/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/batch_running/release_trainings/nnunetv2_v1/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     5662 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/batch_running/release_trainings/nnunetv2_v1/collect_results.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3833 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/batch_running/release_trainings/nnunetv2_v1/generate_lsf_commands.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      416 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/configuration.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.663082 nnunetv2-2.3.1/nnunetv2/dataset_conversion/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     4545 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/dataset_conversion/Dataset027_ACDC.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     4162 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/dataset_conversion/Dataset073_Fluo_C3DH_A549_SIM.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     9018 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/dataset_conversion/Dataset114_MNMs.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2406 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/dataset_conversion/Dataset115_EMIDEC.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3430 2023-10-27 11:39:44.000000 nnunetv2-2.3.1/nnunetv2/dataset_conversion/Dataset120_RoadSegmentation.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3994 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/dataset_conversion/Dataset137_BraTS21.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3742 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/dataset_conversion/Dataset218_Amos2022_task1.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3555 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/dataset_conversion/Dataset219_Amos2022_task2.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2080 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/dataset_conversion/Dataset220_KiTS2023.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3167 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/dataset_conversion/Dataset221_AutoPETII_2023.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2653 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/dataset_conversion/Dataset223_AMOS2022postChallenge.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1369 2023-10-27 11:39:44.000000 nnunetv2-2.3.1/nnunetv2/dataset_conversion/Dataset988_dummyDataset4.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/dataset_conversion/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     6074 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/dataset_conversion/convert_MSD_dataset.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2930 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/dataset_conversion/convert_raw_dataset_from_old_nnunet_format.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.663082 nnunetv2-2.3.1/nnunetv2/dataset_conversion/datasets_for_integration_tests/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3250 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset996_IntegrationTest_Hippocampus_regions_ignore.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1468 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset997_IntegrationTest_Hippocampus_regions.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1364 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset998_IntegrationTest_Hippocampus_ignore.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1085 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset999_IntegrationTest_Hippocampus.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/dataset_conversion/datasets_for_integration_tests/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     4045 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/dataset_conversion/generate_dataset_json.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.663082 nnunetv2-2.3.1/nnunetv2/ensembling/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/ensembling/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    10027 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/ensembling/ensemble.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.663082 nnunetv2-2.3.1/nnunetv2/evaluation/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/evaluation/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3273 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/evaluation/accumulate_cv_results.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    12556 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/evaluation/evaluate_predictions.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    18653 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/evaluation/find_best_configuration.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.663082 nnunetv2-2.3.1/nnunetv2/experiment_planning/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/experiment_planning/__init__.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.663082 nnunetv2-2.3.1/nnunetv2/experiment_planning/dataset_fingerprint/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/experiment_planning/dataset_fingerprint/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    11563 2023-12-15 15:04:30.000000 nnunetv2-2.3.1/nnunetv2/experiment_planning/dataset_fingerprint/fingerprint_extractor.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.663082 nnunetv2-2.3.1/nnunetv2/experiment_planning/experiment_planners/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/experiment_planning/experiment_planners/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    33587 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/experiment_planning/experiment_planners/default_experiment_planner.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3928 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/experiment_planning/experiment_planners/network_topology.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    14327 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/experiment_planning/experiment_planners/resencUNet_planner.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     8088 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/experiment_planning/plan_and_preprocess_api.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    16464 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/experiment_planning/plan_and_preprocess_entrypoints.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.663082 nnunetv2-2.3.1/nnunetv2/experiment_planning/plans_for_pretraining/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/experiment_planning/plans_for_pretraining/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     4469 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/experiment_planning/plans_for_pretraining/move_plans_between_datasets.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    12232 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/experiment_planning/verify_dataset_integrity.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.667083 nnunetv2-2.3.1/nnunetv2/imageio/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/imageio/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     5626 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/imageio/base_reader_writer.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3344 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/imageio/natural_image_reader_writer.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     8631 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/imageio/nibabel_reader_writer.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3865 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/imageio/reader_writer_registry.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     5661 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/imageio/simpleitk_reader_writer.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     4731 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/imageio/tif_reader_writer.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.667083 nnunetv2-2.3.1/nnunetv2/inference/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/inference/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    16275 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/inference/data_iterators.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     6488 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/inference/examples.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     8259 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/inference/export_prediction.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    55889 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/inference/predict_from_raw_data.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2928 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/inference/sliding_window_prediction.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.667083 nnunetv2-2.3.1/nnunetv2/model_sharing/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/model_sharing/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3528 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/model_sharing/entry_points.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1856 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/model_sharing/model_download.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     6830 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/model_sharing/model_export.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      202 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/model_sharing/model_import.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1865 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/paths.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.667083 nnunetv2-2.3.1/nnunetv2/postprocessing/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/postprocessing/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    20662 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/postprocessing/remove_connected_components.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.667083 nnunetv2-2.3.1/nnunetv2/preprocessing/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/preprocessing/__init__.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.667083 nnunetv2-2.3.1/nnunetv2/preprocessing/cropping/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/preprocessing/cropping/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1511 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/preprocessing/cropping/cropping.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.667083 nnunetv2-2.3.1/nnunetv2/preprocessing/normalization/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/preprocessing/normalization/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     4145 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/preprocessing/normalization/default_normalization_schemes.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      965 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/preprocessing/normalization/map_channel_name_to_normalization.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.667083 nnunetv2-2.3.1/nnunetv2/preprocessing/preprocessors/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/preprocessing/preprocessors/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    16203 2024-02-19 15:41:35.000000 nnunetv2-2.3.1/nnunetv2/preprocessing/preprocessors/default_preprocessor.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.667083 nnunetv2-2.3.1/nnunetv2/preprocessing/resampling/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/preprocessing/resampling/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     9602 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/preprocessing/resampling/default_resampling.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      713 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/preprocessing/resampling/utils.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.667083 nnunetv2-2.3.1/nnunetv2/run/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/run/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3176 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/run/load_pretrained_weights.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    13994 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/run/run_training.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.667083 nnunetv2-2.3.1/nnunetv2/tests/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/tests/__init__.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.667083 nnunetv2-2.3.1/nnunetv2/tests/integration_tests/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/tests/integration_tests/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1550 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/tests/integration_tests/add_lowres_and_cascade.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      659 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/tests/integration_tests/cleanup_integration_test.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     4244 2023-10-27 11:39:44.000000 nnunetv2-2.3.1/nnunetv2/tests/integration_tests/run_integration_test_bestconfig_inference.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.667083 nnunetv2-2.3.1/nnunetv2/training/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/__init__.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.667083 nnunetv2-2.3.1/nnunetv2/training/data_augmentation/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/data_augmentation/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1157 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/data_augmentation/compute_initial_patch_size.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.671083 nnunetv2-2.3.1/nnunetv2/training/data_augmentation/custom_transforms/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/data_augmentation/custom_transforms/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     7310 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/data_augmentation/custom_transforms/cascade_transforms.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2601 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/training/data_augmentation/custom_transforms/deep_supervision_donwsampling.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      349 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/data_augmentation/custom_transforms/limited_length_multithreaded_augmenter.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      326 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/data_augmentation/custom_transforms/manipulating_data_dict.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      893 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/data_augmentation/custom_transforms/masking.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1665 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/data_augmentation/custom_transforms/region_based_training.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2455 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/data_augmentation/custom_transforms/transforms_for_dummy_2d.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.671083 nnunetv2-2.3.1/nnunetv2/training/dataloading/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/dataloading/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     8320 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/dataloading/base_data_loader.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     5638 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/training/dataloading/data_loader_2d.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3147 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/training/dataloading/data_loader_3d.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     6510 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/training/dataloading/nnunet_dataset.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     5774 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/training/dataloading/utils.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.671083 nnunetv2-2.3.1/nnunetv2/training/logging/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/logging/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     4718 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/logging/nnunet_logger.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.671083 nnunetv2-2.3.1/nnunetv2/training/loss/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/loss/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     5924 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/training/loss/compound_losses.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1398 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/training/loss/deep_supervision.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     6681 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/training/loss/dice.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1153 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/training/loss/robust_ce_loss.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.671083 nnunetv2-2.3.1/nnunetv2/training/lr_scheduler/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/lr_scheduler/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      803 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/lr_scheduler/polylr.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.671083 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    70405 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/nnUNetTrainer.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.671083 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/__init__.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.671083 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/benchmarking/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/benchmarking/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2858 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/benchmarking/nnUNetTrainerBenchmark_5epochs.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2566 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/benchmarking/nnUNetTrainerBenchmark_5epochs_noDataLoading.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.671083 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    20171 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerDA5.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     8889 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerDAOrd0.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2105 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerNoDA.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1230 2024-02-19 15:41:35.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerNoMirroring.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.671083 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/loss/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/loss/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1690 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/loss/nnUNetTrainerCELoss.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3051 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/loss/nnUNetTrainerDiceLoss.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3473 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/loss/nnUNetTrainerTopkLoss.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.675083 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/lr_schedule/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/lr_schedule/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      517 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/lr_schedule/nnUNetTrainerCosAnneal.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.675083 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/network_architecture/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/network_architecture/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1710 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/network_architecture/nnUNetTrainerBN.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      501 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/network_architecture/nnUNetTrainerNoDeepSupervision.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.675083 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/optimizer/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/optimizer/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2882 2024-02-19 15:41:35.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/optimizer/nnUNetTrainerAdam.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3259 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/optimizer/nnUNetTrainerAdan.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.675083 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/sampling/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/sampling/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     5088 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/sampling/nnUNetTrainer_probabilisticOversampling.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.675083 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/training_length/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/training_length/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3690 2024-02-19 15:41:35.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/training_length/nnUNetTrainer_Xepochs.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3157 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/training_length/nnUNetTrainer_Xepochs_NoMirroring.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.675083 nnunetv2-2.3.1/nnunetv2/utilities/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/utilities/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      906 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/utilities/collate_outputs.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      619 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/utilities/crossval_split.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3925 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/utilities/dataset_name_id_conversion.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1748 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/utilities/ddp_allgather.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1854 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/utilities/default_n_proc_DA.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     5545 2024-02-19 15:41:35.000000 nnunetv2-2.3.1/nnunetv2/utilities/file_path_utilities.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      868 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/utilities/find_class_by_name.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1910 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/utilities/get_network_from_plans.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      543 2024-02-19 15:41:35.000000 nnunetv2-2.3.1/nnunetv2/utilities/helpers.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2420 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/utilities/json_export.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.675083 nnunetv2-2.3.1/nnunetv2/utilities/label_handling/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/utilities/label_handling/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    14925 2024-02-19 15:41:35.000000 nnunetv2-2.3.1/nnunetv2/utilities/label_handling/label_handling.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      509 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/utilities/network_initialization.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    11953 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/nnunetv2/utilities/overlay_plots.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.675083 nnunetv2-2.3.1/nnunetv2/utilities/plans_handling/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2023-10-06 14:24:16.000000 nnunetv2-2.3.1/nnunetv2/utilities/plans_handling/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    15055 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/nnunetv2/utilities/plans_handling/plans_handler.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3139 2023-10-27 11:39:44.000000 nnunetv2-2.3.1/nnunetv2/utilities/utils.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-02-21 20:50:40.659083 nnunetv2-2.3.1/nnunetv2.egg-info/
--rw-r--r--   0 isensee   (1000) isensee   (1000)    24140 2024-02-21 20:50:40.000000 nnunetv2-2.3.1/nnunetv2.egg-info/PKG-INFO
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     9295 2024-02-21 20:50:40.000000 nnunetv2-2.3.1/nnunetv2.egg-info/SOURCES.txt
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        1 2024-02-21 20:50:40.000000 nnunetv2-2.3.1/nnunetv2.egg-info/dependency_links.txt
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2244 2024-02-21 20:50:40.000000 nnunetv2-2.3.1/nnunetv2.egg-info/entry_points.txt
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      283 2024-02-21 20:50:40.000000 nnunetv2-2.3.1/nnunetv2.egg-info/requires.txt
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        9 2024-02-21 20:50:40.000000 nnunetv2-2.3.1/nnunetv2.egg-info/top_level.txt
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     4126 2024-02-21 20:50:17.000000 nnunetv2-2.3.1/pyproject.toml
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     9993 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/readme.md
--rw-rw-r--   0 isensee   (1000) isensee   (1000)       38 2024-02-21 20:50:40.675083 nnunetv2-2.3.1/setup.cfg
--rwxrwxr-x   0 isensee   (1000) isensee   (1000)       69 2023-12-12 12:27:04.000000 nnunetv2-2.3.1/setup.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.668660 nnunetv2-2.4/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    11427 2023-03-17 08:55:29.000000 nnunetv2-2.4/LICENSE
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    24711 2024-04-18 09:20:23.668660 nnunetv2-2.4/PKG-INFO
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.648660 nnunetv2-2.4/nnunetv2/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/__init__.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.648660 nnunetv2-2.4/nnunetv2/batch_running/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/batch_running/__init__.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.648660 nnunetv2-2.4/nnunetv2/batch_running/benchmarking/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/batch_running/benchmarking/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2041 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/batch_running/benchmarking/generate_benchmarking_commands.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3272 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/batch_running/benchmarking/summarize_benchmark_results.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     5798 2024-04-18 09:18:23.000000 nnunetv2-2.4/nnunetv2/batch_running/collect_results_custom_Decathlon.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      708 2024-04-18 09:18:23.000000 nnunetv2-2.4/nnunetv2/batch_running/collect_results_custom_Decathlon_2d.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3300 2024-04-18 09:18:23.000000 nnunetv2-2.4/nnunetv2/batch_running/generate_lsf_runs_customDecathlon.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.648660 nnunetv2-2.4/nnunetv2/batch_running/release_trainings/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/batch_running/release_trainings/__init__.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.648660 nnunetv2-2.4/nnunetv2/batch_running/release_trainings/nnunetv2_v1/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/batch_running/release_trainings/nnunetv2_v1/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     5662 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/batch_running/release_trainings/nnunetv2_v1/collect_results.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3833 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/batch_running/release_trainings/nnunetv2_v1/generate_lsf_commands.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      416 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/configuration.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.652660 nnunetv2-2.4/nnunetv2/dataset_conversion/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     4545 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/dataset_conversion/Dataset027_ACDC.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     4162 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/dataset_conversion/Dataset073_Fluo_C3DH_A549_SIM.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     9018 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/dataset_conversion/Dataset114_MNMs.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2406 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/dataset_conversion/Dataset115_EMIDEC.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3430 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/dataset_conversion/Dataset120_RoadSegmentation.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3994 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/dataset_conversion/Dataset137_BraTS21.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3742 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/dataset_conversion/Dataset218_Amos2022_task1.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3555 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/dataset_conversion/Dataset219_Amos2022_task2.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2080 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/dataset_conversion/Dataset220_KiTS2023.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3167 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/dataset_conversion/Dataset221_AutoPETII_2023.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2653 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/dataset_conversion/Dataset223_AMOS2022postChallenge.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1369 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/dataset_conversion/Dataset988_dummyDataset4.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/dataset_conversion/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     6074 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/dataset_conversion/convert_MSD_dataset.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2930 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/dataset_conversion/convert_raw_dataset_from_old_nnunet_format.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.652660 nnunetv2-2.4/nnunetv2/dataset_conversion/datasets_for_integration_tests/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3250 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset996_IntegrationTest_Hippocampus_regions_ignore.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1468 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset997_IntegrationTest_Hippocampus_regions.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1364 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset998_IntegrationTest_Hippocampus_ignore.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1085 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset999_IntegrationTest_Hippocampus.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/dataset_conversion/datasets_for_integration_tests/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     4045 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/dataset_conversion/generate_dataset_json.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.652660 nnunetv2-2.4/nnunetv2/ensembling/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/ensembling/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    10027 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/ensembling/ensemble.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.652660 nnunetv2-2.4/nnunetv2/evaluation/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/evaluation/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3273 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/evaluation/accumulate_cv_results.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    12556 2024-04-18 09:18:23.000000 nnunetv2-2.4/nnunetv2/evaluation/evaluate_predictions.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    18653 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/evaluation/find_best_configuration.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.652660 nnunetv2-2.4/nnunetv2/experiment_planning/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/experiment_planning/__init__.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.652660 nnunetv2-2.4/nnunetv2/experiment_planning/dataset_fingerprint/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/experiment_planning/dataset_fingerprint/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    11935 2024-04-18 08:44:04.000000 nnunetv2-2.4/nnunetv2/experiment_planning/dataset_fingerprint/fingerprint_extractor.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.652660 nnunetv2-2.4/nnunetv2/experiment_planning/experiment_planners/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/experiment_planning/experiment_planners/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    33576 2024-04-18 09:18:23.000000 nnunetv2-2.4/nnunetv2/experiment_planning/experiment_planners/default_experiment_planner.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3928 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/experiment_planning/experiment_planners/network_topology.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    14292 2024-04-18 08:44:04.000000 nnunetv2-2.4/nnunetv2/experiment_planning/experiment_planners/resencUNet_planner.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.656660 nnunetv2-2.4/nnunetv2/experiment_planning/experiment_planners/residual_unets/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-18 08:44:04.000000 nnunetv2-2.4/nnunetv2/experiment_planning/experiment_planners/residual_unets/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    18309 2024-04-18 08:44:04.000000 nnunetv2-2.4/nnunetv2/experiment_planning/experiment_planners/residual_unets/residual_encoder_unet_planners.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     8566 2024-04-18 08:44:04.000000 nnunetv2-2.4/nnunetv2/experiment_planning/plan_and_preprocess_api.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    16650 2024-04-18 08:44:04.000000 nnunetv2-2.4/nnunetv2/experiment_planning/plan_and_preprocess_entrypoints.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.656660 nnunetv2-2.4/nnunetv2/experiment_planning/plans_for_pretraining/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/experiment_planning/plans_for_pretraining/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     4469 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/experiment_planning/plans_for_pretraining/move_plans_between_datasets.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    12234 2024-04-18 08:44:04.000000 nnunetv2-2.4/nnunetv2/experiment_planning/verify_dataset_integrity.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.656660 nnunetv2-2.4/nnunetv2/imageio/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/imageio/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     5626 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/imageio/base_reader_writer.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3344 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/imageio/natural_image_reader_writer.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     8639 2024-04-18 08:44:04.000000 nnunetv2-2.4/nnunetv2/imageio/nibabel_reader_writer.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3865 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/imageio/reader_writer_registry.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     5665 2024-04-18 08:44:04.000000 nnunetv2-2.4/nnunetv2/imageio/simpleitk_reader_writer.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     4731 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/imageio/tif_reader_writer.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.656660 nnunetv2-2.4/nnunetv2/inference/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/inference/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    16219 2024-04-18 08:44:04.000000 nnunetv2-2.4/nnunetv2/inference/data_iterators.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     6488 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/inference/examples.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     8259 2024-04-12 14:38:44.000000 nnunetv2-2.4/nnunetv2/inference/export_prediction.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    56414 2024-04-18 09:18:23.000000 nnunetv2-2.4/nnunetv2/inference/predict_from_raw_data.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2895 2024-04-18 08:44:04.000000 nnunetv2-2.4/nnunetv2/inference/sliding_window_prediction.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.656660 nnunetv2-2.4/nnunetv2/model_sharing/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/model_sharing/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3528 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/model_sharing/entry_points.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1856 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/model_sharing/model_download.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     6830 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/model_sharing/model_export.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      202 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/model_sharing/model_import.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1865 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/paths.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.656660 nnunetv2-2.4/nnunetv2/postprocessing/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/postprocessing/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    20662 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/postprocessing/remove_connected_components.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.656660 nnunetv2-2.4/nnunetv2/preprocessing/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/preprocessing/__init__.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.656660 nnunetv2-2.4/nnunetv2/preprocessing/cropping/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/preprocessing/cropping/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1274 2024-04-18 08:44:04.000000 nnunetv2-2.4/nnunetv2/preprocessing/cropping/cropping.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.656660 nnunetv2-2.4/nnunetv2/preprocessing/normalization/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/preprocessing/normalization/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     4145 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/preprocessing/normalization/default_normalization_schemes.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      976 2024-04-18 08:44:04.000000 nnunetv2-2.4/nnunetv2/preprocessing/normalization/map_channel_name_to_normalization.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.656660 nnunetv2-2.4/nnunetv2/preprocessing/preprocessors/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/preprocessing/preprocessors/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    16203 2024-04-18 09:18:23.000000 nnunetv2-2.4/nnunetv2/preprocessing/preprocessors/default_preprocessor.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.660660 nnunetv2-2.4/nnunetv2/preprocessing/resampling/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/preprocessing/resampling/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     9599 2024-04-18 09:18:23.000000 nnunetv2-2.4/nnunetv2/preprocessing/resampling/default_resampling.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      713 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/preprocessing/resampling/utils.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.660660 nnunetv2-2.4/nnunetv2/run/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/run/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3345 2024-04-18 08:44:04.000000 nnunetv2-2.4/nnunetv2/run/load_pretrained_weights.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    14405 2024-04-18 09:18:23.000000 nnunetv2-2.4/nnunetv2/run/run_training.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.660660 nnunetv2-2.4/nnunetv2/tests/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/tests/__init__.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.660660 nnunetv2-2.4/nnunetv2/tests/integration_tests/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/tests/integration_tests/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1550 2024-04-12 14:38:44.000000 nnunetv2-2.4/nnunetv2/tests/integration_tests/add_lowres_and_cascade.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      659 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/tests/integration_tests/cleanup_integration_test.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     4244 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/tests/integration_tests/run_integration_test_bestconfig_inference.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.660660 nnunetv2-2.4/nnunetv2/training/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/__init__.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.660660 nnunetv2-2.4/nnunetv2/training/data_augmentation/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/data_augmentation/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1157 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/data_augmentation/compute_initial_patch_size.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.660660 nnunetv2-2.4/nnunetv2/training/data_augmentation/custom_transforms/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/data_augmentation/custom_transforms/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     7310 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/data_augmentation/custom_transforms/cascade_transforms.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2601 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/data_augmentation/custom_transforms/deep_supervision_donwsampling.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      349 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/data_augmentation/custom_transforms/limited_length_multithreaded_augmenter.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      326 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/data_augmentation/custom_transforms/manipulating_data_dict.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      893 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/data_augmentation/custom_transforms/masking.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1665 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/data_augmentation/custom_transforms/region_based_training.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2455 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/data_augmentation/custom_transforms/transforms_for_dummy_2d.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.660660 nnunetv2-2.4/nnunetv2/training/dataloading/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/dataloading/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     8214 2024-04-18 09:18:23.000000 nnunetv2-2.4/nnunetv2/training/dataloading/base_data_loader.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     5638 2024-04-18 09:18:23.000000 nnunetv2-2.4/nnunetv2/training/dataloading/data_loader_2d.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3142 2024-04-18 09:18:23.000000 nnunetv2-2.4/nnunetv2/training/dataloading/data_loader_3d.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     6510 2024-04-12 14:38:44.000000 nnunetv2-2.4/nnunetv2/training/dataloading/nnunet_dataset.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3393 2024-04-18 08:44:04.000000 nnunetv2-2.4/nnunetv2/training/dataloading/utils.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.660660 nnunetv2-2.4/nnunetv2/training/logging/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/logging/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     4718 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/logging/nnunet_logger.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.664660 nnunetv2-2.4/nnunetv2/training/loss/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/loss/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     5924 2024-04-18 09:18:23.000000 nnunetv2-2.4/nnunetv2/training/loss/compound_losses.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1398 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/loss/deep_supervision.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     6681 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/loss/dice.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1153 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/loss/robust_ce_loss.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.664660 nnunetv2-2.4/nnunetv2/training/lr_scheduler/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/lr_scheduler/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      803 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/lr_scheduler/polylr.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.664660 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    70783 2024-04-18 09:18:23.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/nnUNetTrainer.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.664660 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/__init__.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.664660 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/benchmarking/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/benchmarking/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2858 2024-04-12 14:38:44.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/benchmarking/nnUNetTrainerBenchmark_5epochs.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2566 2024-04-12 14:38:44.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/benchmarking/nnUNetTrainerBenchmark_5epochs_noDataLoading.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.664660 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    20171 2024-04-18 09:18:23.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerDA5.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     8889 2024-04-18 09:18:23.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerDAOrd0.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2105 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerNoDA.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1230 2024-04-18 09:18:23.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerNoMirroring.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.664660 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/loss/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/loss/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1690 2024-04-18 09:18:23.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/loss/nnUNetTrainerCELoss.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3051 2024-04-18 09:18:23.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/loss/nnUNetTrainerDiceLoss.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3473 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/loss/nnUNetTrainerTopkLoss.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.664660 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/lr_schedule/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/lr_schedule/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      517 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/lr_schedule/nnUNetTrainerCosAnneal.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.664660 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/network_architecture/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/network_architecture/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1710 2024-04-18 08:44:04.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/network_architecture/nnUNetTrainerBN.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      501 2024-04-12 14:38:44.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/network_architecture/nnUNetTrainerNoDeepSupervision.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.664660 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/optimizer/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/optimizer/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2882 2024-04-18 09:18:23.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/optimizer/nnUNetTrainerAdam.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3259 2024-04-12 14:38:44.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/optimizer/nnUNetTrainerAdan.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.664660 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/sampling/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/sampling/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     5088 2024-04-12 14:38:44.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/sampling/nnUNetTrainer_probabilisticOversampling.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.664660 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/training_length/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/training_length/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3690 2024-04-18 09:18:23.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/training_length/nnUNetTrainer_Xepochs.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3157 2024-04-12 14:38:44.000000 nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/training_length/nnUNetTrainer_Xepochs_NoMirroring.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.668660 nnunetv2-2.4/nnunetv2/utilities/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/utilities/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      906 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/utilities/collate_outputs.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      619 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/utilities/crossval_split.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3925 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/utilities/dataset_name_id_conversion.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1748 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/utilities/ddp_allgather.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1854 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/utilities/default_n_proc_DA.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     5545 2024-04-18 09:18:23.000000 nnunetv2-2.4/nnunetv2/utilities/file_path_utilities.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      868 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/utilities/find_class_by_name.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1910 2024-04-18 08:44:04.000000 nnunetv2-2.4/nnunetv2/utilities/get_network_from_plans.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      543 2024-04-18 09:18:23.000000 nnunetv2-2.4/nnunetv2/utilities/helpers.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2420 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/utilities/json_export.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.668660 nnunetv2-2.4/nnunetv2/utilities/label_handling/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/utilities/label_handling/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    14925 2024-04-18 09:18:23.000000 nnunetv2-2.4/nnunetv2/utilities/label_handling/label_handling.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      509 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/utilities/network_initialization.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    11953 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/utilities/overlay_plots.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.668660 nnunetv2-2.4/nnunetv2/utilities/plans_handling/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/utilities/plans_handling/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    15055 2024-04-18 09:18:23.000000 nnunetv2-2.4/nnunetv2/utilities/plans_handling/plans_handler.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3139 2024-04-09 18:40:42.000000 nnunetv2-2.4/nnunetv2/utilities/utils.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:20:23.648660 nnunetv2-2.4/nnunetv2.egg-info/
+-rw-r--r--   0 isensee   (1000) isensee   (1000)    24711 2024-04-18 09:20:23.000000 nnunetv2-2.4/nnunetv2.egg-info/PKG-INFO
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     9469 2024-04-18 09:20:23.000000 nnunetv2-2.4/nnunetv2.egg-info/SOURCES.txt
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        1 2024-04-18 09:20:23.000000 nnunetv2-2.4/nnunetv2.egg-info/dependency_links.txt
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2244 2024-04-18 09:20:23.000000 nnunetv2-2.4/nnunetv2.egg-info/entry_points.txt
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      285 2024-04-18 09:20:23.000000 nnunetv2-2.4/nnunetv2.egg-info/requires.txt
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        9 2024-04-18 09:20:23.000000 nnunetv2-2.4/nnunetv2.egg-info/top_level.txt
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     4216 2024-04-18 08:44:04.000000 nnunetv2-2.4/pyproject.toml
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    10566 2024-04-18 08:44:04.000000 nnunetv2-2.4/readme.md
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)       38 2024-04-18 09:20:23.668660 nnunetv2-2.4/setup.cfg
+-rwxrwxr-x   0 isensee   (1000) isensee   (1000)       69 2024-04-09 18:40:42.000000 nnunetv2-2.4/setup.py
```

### Comparing `nnunetv2-2.3.1/LICENSE` & `nnunetv2-2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/PKG-INFO` & `nnunetv2-2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nnunetv2
-Version: 2.3.1
+Version: 2.4
 Summary: nnU-Net is a framework for out-of-the box image segmentation.
 Author: Helmholtz Imaging Applied Computer Vision Lab
 Author-email: Fabian Isensee <f.isensee@dkfz-heidelberg.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -224,14 +224,21 @@
 
 # Welcome to the new nnU-Net!
 
 Click [here](https://github.com/MIC-DKFZ/nnUNet/tree/nnunetv1) if you were looking for the old one instead.
 
 Coming from V1? Check out the [TLDR Migration Guide](documentation/tldr_migration_guide_from_v1.md). Reading the rest of the documentation is still strongly recommended ;-)
 
+## **2024-04-18 UPDATE: New residual encoder UNet presets available!**
+Residual encoder UNet presets substantially improve segmentation performance.
+They ship for a variety of GPU memory targets. It's all awesome stuff, promised! 
+Read more :point_right: [here](documentation/resenc_presets.md) :point_left:
+
+Also check out our [new paper](https://arxiv.org/pdf/2404.09556.pdf) on systematically benchmarking recent developments in medical image segmentation. You might be surprised!
+
 # What is nnU-Net?
 Image datasets are enormously diverse: image dimensionality (2D, 3D), modalities/input channels (RGB image, CT, MRI, microscopy, ...), 
 image sizes, voxel sizes, class ratio, target structure properties and more change substantially between datasets. 
 Traditionally, given a new problem, a tailored solution needs to be manually designed and optimized  - a process that 
 is prone to errors, not scalable and where success is overwhelmingly determined by the skill of the experimenter. Even 
 for experts, this process is anything but simple: there are not only many design choices and data properties that need to 
 be considered, but they are also tightly interconnected, rendering reliable manual pipeline optimization all but impossible! 
@@ -308,14 +315,15 @@
 ## How to get started?
 Read these:
 - [Installation instructions](documentation/installation_instructions.md)
 - [Dataset conversion](documentation/dataset_format.md)
 - [Usage instructions](documentation/how_to_use_nnunet.md)
 
 Additional information:
+- [Learning from sparse annotations (scribbles, slices)](documentation/ignore_label.md)
 - [Region-based training](documentation/region_based_training.md)
 - [Manual data splits](documentation/manual_data_splits.md)
 - [Pretraining and finetuning](documentation/pretraining_and_finetuning.md)
 - [Intensity Normalization in nnU-Net](documentation/explanation_normalization.md)
 - [Manually editing nnU-Net configurations](documentation/explanation_plans_files.md)
 - [Extending nnU-Net](documentation/extending_nnunet.md)
 - [What is different in V2?](documentation/changelog.md)
```

### Comparing `nnunetv2-2.3.1/nnunetv2/batch_running/benchmarking/generate_benchmarking_commands.py` & `nnunetv2-2.4/nnunetv2/batch_running/benchmarking/generate_benchmarking_commands.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/batch_running/benchmarking/summarize_benchmark_results.py` & `nnunetv2-2.4/nnunetv2/batch_running/benchmarking/summarize_benchmark_results.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/batch_running/collect_results_custom_Decathlon.py` & `nnunetv2-2.4/nnunetv2/batch_running/collect_results_custom_Decathlon.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/batch_running/collect_results_custom_Decathlon_2d.py` & `nnunetv2-2.4/nnunetv2/batch_running/collect_results_custom_Decathlon_2d.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/batch_running/generate_lsf_runs_customDecathlon.py` & `nnunetv2-2.4/nnunetv2/batch_running/generate_lsf_runs_customDecathlon.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/batch_running/release_trainings/nnunetv2_v1/collect_results.py` & `nnunetv2-2.4/nnunetv2/batch_running/release_trainings/nnunetv2_v1/collect_results.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/batch_running/release_trainings/nnunetv2_v1/generate_lsf_commands.py` & `nnunetv2-2.4/nnunetv2/batch_running/release_trainings/nnunetv2_v1/generate_lsf_commands.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/dataset_conversion/Dataset027_ACDC.py` & `nnunetv2-2.4/nnunetv2/dataset_conversion/Dataset027_ACDC.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/dataset_conversion/Dataset073_Fluo_C3DH_A549_SIM.py` & `nnunetv2-2.4/nnunetv2/dataset_conversion/Dataset073_Fluo_C3DH_A549_SIM.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/dataset_conversion/Dataset114_MNMs.py` & `nnunetv2-2.4/nnunetv2/dataset_conversion/Dataset114_MNMs.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/dataset_conversion/Dataset115_EMIDEC.py` & `nnunetv2-2.4/nnunetv2/dataset_conversion/Dataset115_EMIDEC.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/dataset_conversion/Dataset120_RoadSegmentation.py` & `nnunetv2-2.4/nnunetv2/dataset_conversion/Dataset120_RoadSegmentation.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/dataset_conversion/Dataset137_BraTS21.py` & `nnunetv2-2.4/nnunetv2/dataset_conversion/Dataset137_BraTS21.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/dataset_conversion/Dataset218_Amos2022_task1.py` & `nnunetv2-2.4/nnunetv2/dataset_conversion/Dataset218_Amos2022_task1.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/dataset_conversion/Dataset219_Amos2022_task2.py` & `nnunetv2-2.4/nnunetv2/dataset_conversion/Dataset219_Amos2022_task2.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/dataset_conversion/Dataset220_KiTS2023.py` & `nnunetv2-2.4/nnunetv2/dataset_conversion/Dataset220_KiTS2023.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/dataset_conversion/Dataset221_AutoPETII_2023.py` & `nnunetv2-2.4/nnunetv2/dataset_conversion/Dataset221_AutoPETII_2023.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/dataset_conversion/Dataset223_AMOS2022postChallenge.py` & `nnunetv2-2.4/nnunetv2/dataset_conversion/Dataset223_AMOS2022postChallenge.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/dataset_conversion/Dataset988_dummyDataset4.py` & `nnunetv2-2.4/nnunetv2/dataset_conversion/Dataset988_dummyDataset4.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/dataset_conversion/convert_MSD_dataset.py` & `nnunetv2-2.4/nnunetv2/dataset_conversion/convert_MSD_dataset.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/dataset_conversion/convert_raw_dataset_from_old_nnunet_format.py` & `nnunetv2-2.4/nnunetv2/dataset_conversion/convert_raw_dataset_from_old_nnunet_format.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset996_IntegrationTest_Hippocampus_regions_ignore.py` & `nnunetv2-2.4/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset996_IntegrationTest_Hippocampus_regions_ignore.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset997_IntegrationTest_Hippocampus_regions.py` & `nnunetv2-2.4/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset997_IntegrationTest_Hippocampus_regions.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset998_IntegrationTest_Hippocampus_ignore.py` & `nnunetv2-2.4/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset998_IntegrationTest_Hippocampus_ignore.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset999_IntegrationTest_Hippocampus.py` & `nnunetv2-2.4/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset999_IntegrationTest_Hippocampus.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/dataset_conversion/generate_dataset_json.py` & `nnunetv2-2.4/nnunetv2/dataset_conversion/generate_dataset_json.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/ensembling/ensemble.py` & `nnunetv2-2.4/nnunetv2/ensembling/ensemble.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/evaluation/accumulate_cv_results.py` & `nnunetv2-2.4/nnunetv2/evaluation/accumulate_cv_results.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/evaluation/evaluate_predictions.py` & `nnunetv2-2.4/nnunetv2/evaluation/evaluate_predictions.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
     """
     if output_file is not None:
         assert output_file.endswith('.json'), 'output_file should end with .json'
     files_pred = subfiles(folder_pred, suffix=file_ending, join=False)
     files_ref = subfiles(folder_ref, suffix=file_ending, join=False)
     if not chill:
         present = [isfile(join(folder_pred, i)) for i in files_ref]
-        assert all(present), "Not all files in folder_pred exist in folder_ref"
+        assert all(present), "Not all files in folder_ref exist in folder_pred"
     files_ref = [join(folder_ref, i) for i in files_pred]
     files_pred = [join(folder_pred, i) for i in files_pred]
     with multiprocessing.get_context("spawn").Pool(num_processes) as pool:
         # for i in list(zip(files_ref, files_pred, [image_reader_writer] * len(files_pred), [regions_or_labels] * len(files_pred), [ignore_label] * len(files_pred))):
         #     compute_metrics(*i)
         results = pool.starmap(
             compute_metrics,
```

### Comparing `nnunetv2-2.3.1/nnunetv2/evaluation/find_best_configuration.py` & `nnunetv2-2.4/nnunetv2/evaluation/find_best_configuration.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/experiment_planning/dataset_fingerprint/fingerprint_extractor.py` & `nnunetv2-2.4/nnunetv2/experiment_planning/dataset_fingerprint/fingerprint_extractor.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,44 +40,51 @@
 
     @staticmethod
     def collect_foreground_intensities(segmentation: np.ndarray, images: np.ndarray, seed: int = 1234,
                                        num_samples: int = 10000):
         """
         images=image with multiple channels = shape (c, x, y(, z))
         """
-        assert images.ndim == 4
-        assert segmentation.ndim == 4
-
+        assert images.ndim == 4 and segmentation.ndim == 4
         assert not np.any(np.isnan(segmentation)), "Segmentation contains NaN values. grrrr.... :-("
         assert not np.any(np.isnan(images)), "Images contains NaN values. grrrr.... :-("
 
         rs = np.random.RandomState(seed)
 
         intensities_per_channel = []
         # we don't use the intensity_statistics_per_channel at all, it's just something that might be nice to have
         intensity_statistics_per_channel = []
 
         # segmentation is 4d: 1,x,y,z. We need to remove the empty dimension for the following code to work
         foreground_mask = segmentation[0] > 0
+        percentiles = np.array((0.5, 50.0, 99.5))
 
         for i in range(len(images)):
             foreground_pixels = images[i][foreground_mask]
             num_fg = len(foreground_pixels)
             # sample with replacement so that we don't get issues with cases that have less than num_samples
             # foreground_pixels. We could also just sample less in those cases but that would than cause these
             # training cases to be underrepresented
             intensities_per_channel.append(
                 rs.choice(foreground_pixels, num_samples, replace=True) if num_fg > 0 else [])
+
+            mean, median, mini, maxi, percentile_99_5, percentile_00_5 = np.nan, np.nan, np.nan, np.nan, np.nan, np.nan
+            if num_fg > 0:
+                percentile_00_5, median, percentile_99_5 = np.percentile(foreground_pixels, percentiles)
+                mean = np.mean(foreground_pixels)
+                mini = np.min(foreground_pixels)
+                maxi = np.max(foreground_pixels)
+
             intensity_statistics_per_channel.append({
-                'mean': np.mean(foreground_pixels) if num_fg > 0 else np.nan,
-                'median': np.median(foreground_pixels) if num_fg > 0 else np.nan,
-                'min': np.min(foreground_pixels) if num_fg > 0 else np.nan,
-                'max': np.max(foreground_pixels) if num_fg > 0 else np.nan,
-                'percentile_99_5': np.percentile(foreground_pixels, 99.5) if num_fg > 0 else np.nan,
-                'percentile_00_5': np.percentile(foreground_pixels, 0.5) if num_fg > 0 else np.nan,
+                'mean': mean,
+                'median': median,
+                'min': mini,
+                'max': maxi,
+                'percentile_99_5': percentile_99_5,
+                'percentile_00_5': percentile_00_5,
 
             })
 
         return intensities_per_channel, intensity_statistics_per_channel
 
     @staticmethod
     def analyze_case(image_files: List[str], segmentation_file: str, reader_writer_class: Type[BaseReaderWriter],
@@ -153,31 +160,35 @@
             #                 num_samples=num_foreground_samples_per_case, disable=self.verbose)
             results = [i.get()[0] for i in r]
 
             shapes_after_crop = [r[0] for r in results]
             spacings = [r[1] for r in results]
             foreground_intensities_per_channel = [np.concatenate([r[2][i] for r in results]) for i in
                                                   range(len(results[0][2]))]
+            foreground_intensities_per_channel = np.array(foreground_intensities_per_channel)
             # we drop this so that the json file is somewhat human readable
             # foreground_intensity_stats_by_case_and_modality = [r[3] for r in results]
             median_relative_size_after_cropping = np.median([r[4] for r in results], 0)
 
             num_channels = len(self.dataset_json['channel_names'].keys()
                                  if 'channel_names' in self.dataset_json.keys()
                                  else self.dataset_json['modality'].keys())
             intensity_statistics_per_channel = {}
+            percentiles = np.array((0.5, 50.0, 99.5))
             for i in range(num_channels):
+                percentile_00_5, median, percentile_99_5 = np.percentile(foreground_intensities_per_channel[i],
+                                                                         percentiles)
                 intensity_statistics_per_channel[i] = {
                     'mean': float(np.mean(foreground_intensities_per_channel[i])),
-                    'median': float(np.median(foreground_intensities_per_channel[i])),
+                    'median': float(median),
                     'std': float(np.std(foreground_intensities_per_channel[i])),
                     'min': float(np.min(foreground_intensities_per_channel[i])),
                     'max': float(np.max(foreground_intensities_per_channel[i])),
-                    'percentile_99_5': float(np.percentile(foreground_intensities_per_channel[i], 99.5)),
-                    'percentile_00_5': float(np.percentile(foreground_intensities_per_channel[i], 0.5)),
+                    'percentile_99_5': float(percentile_99_5),
+                    'percentile_00_5': float(percentile_00_5),
                 }
 
             fingerprint = {
                     "spacings": spacings,
                     "shapes_after_crop": shapes_after_crop,
                     'foreground_intensity_properties_per_channel': intensity_statistics_per_channel,
                     "median_relative_size_after_cropping": median_relative_size_after_cropping
```

### Comparing `nnunetv2-2.3.1/nnunetv2/experiment_planning/experiment_planners/default_experiment_planner.py` & `nnunetv2-2.4/nnunetv2/experiment_planning/experiment_planners/default_experiment_planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,18 +161,18 @@
         (for example ACDC with (10, 1.5, 1.5)). These datasets still have examples with a spacing of 5 or 6 mm in the low
         resolution axis. Choosing the median here will result in bad interpolation artifacts that can substantially
         impact performance (due to the low number of slices).
         """
         if self.overwrite_target_spacing is not None:
             return np.array(self.overwrite_target_spacing)
 
-        spacings = self.dataset_fingerprint['spacings']
+        spacings = np.vstack(self.dataset_fingerprint['spacings'])
         sizes = self.dataset_fingerprint['shapes_after_crop']
 
-        target = np.percentile(np.vstack(spacings), 50, 0)
+        target = np.percentile(spacings, 50, 0)
 
         # todo sizes_after_resampling = [compute_new_shape(j, i, target) for i, j in zip(spacings, sizes)]
 
         target_size = np.percentile(np.vstack(sizes), 50, 0)
         # we need to identify datasets for which a different target spacing could be beneficial. These datasets have
         # the following properties:
         # - one axis which much lower resolution than the others
@@ -183,15 +183,15 @@
         other_spacings = [target[i] for i in other_axes]
         other_sizes = [target_size[i] for i in other_axes]
 
         has_aniso_spacing = target[worst_spacing_axis] > (self.anisotropy_threshold * max(other_spacings))
         has_aniso_voxels = target_size[worst_spacing_axis] * self.anisotropy_threshold < min(other_sizes)
 
         if has_aniso_spacing and has_aniso_voxels:
-            spacings_of_that_axis = np.vstack(spacings)[:, worst_spacing_axis]
+            spacings_of_that_axis = spacings[:, worst_spacing_axis]
             target_spacing_of_that_axis = np.percentile(spacings_of_that_axis, 10)
             # don't let the spacing of that axis get higher than the other axes
             if target_spacing_of_that_axis < max(other_spacings):
                 target_spacing_of_that_axis = max(max(other_spacings), target_spacing_of_that_axis) + 1e-5
             target[worst_spacing_axis] = target_spacing_of_that_axis
         return target
```

### Comparing `nnunetv2-2.3.1/nnunetv2/experiment_planning/experiment_planners/network_topology.py` & `nnunetv2-2.4/nnunetv2/experiment_planning/experiment_planners/network_topology.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/experiment_planning/experiment_planners/resencUNet_planner.py` & `nnunetv2-2.4/nnunetv2/experiment_planning/experiment_planners/resencUNet_planner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from copy import deepcopy
 from typing import Union, List, Tuple
 
-from dynamic_network_architectures.architectures.residual_unet import ResidualEncoderUNet
+from dynamic_network_architectures.architectures.unet import ResidualEncoderUNet
 from dynamic_network_architectures.building_blocks.helper import convert_dim_to_conv_op, get_matching_instancenorm
 from torch import nn
 
 from nnunetv2.experiment_planning.experiment_planners.default_experiment_planner import ExperimentPlanner
 
 from nnunetv2.experiment_planning.experiment_planners.network_topology import get_pool_and_conv_props
 
@@ -75,15 +75,15 @@
             initial_patch_size = [round(i) for i in tmp * (2048 ** 2 / np.prod(tmp)) ** (1 / 2)]
         else:
             raise RuntimeError()
 
         # clip initial patch size to median_shape. It makes little sense to have it be larger than that. Note that
         # this is different from how nnU-Net v1 does it!
         # todo patch size can still get too large because we pad the patch size to a multiple of 2**n
-        initial_patch_size = np.array([min(i, j) for i, j in zip(initial_patch_size, median_shape[:len(spacing)])])
+        initial_patch_size = np.minimum(initial_patch_size, median_shape[:len(spacing)])
 
         # use that to get the network topology. Note that this changes the patch_size depending on the number of
         # pooling operations (must be divisible by 2**num_pool in each axis)
         network_num_pool_per_axis, pool_op_kernel_sizes, conv_kernel_sizes, patch_size, \
         shape_must_be_divisible_by = get_pool_and_conv_props(spacing, initial_patch_size,
                                                              self.UNet_featuremap_min_edge_length,
                                                              999999)
@@ -228,8 +228,8 @@
 
     net = ResidualEncoderUNet(input_channels=1, n_stages=7, features_per_stage=(32, 64, 128, 256, 512, 512, 512),
                               conv_op=nn.Conv2d, kernel_sizes=3, strides=(1, 2, 2, 2, 2, 2, 2),
                               n_blocks_per_stage=(1, 3, 4, 6, 6, 6, 6), num_classes=3,
                               n_conv_per_stage_decoder=(1, 1, 1, 1, 1, 1),
                               conv_bias=True, norm_op=nn.InstanceNorm2d, norm_op_kwargs={}, dropout_op=None,
                               nonlin=nn.LeakyReLU, nonlin_kwargs={'inplace': True}, deep_supervision=True)
-    print(net.compute_conv_feature_map_size((512, 512)))  # -> 129793792
+    print(net.compute_conv_feature_map_size((512, 512)))  # -> 129793792
```

### Comparing `nnunetv2-2.3.1/nnunetv2/experiment_planning/plan_and_preprocess_api.py` & `nnunetv2-2.4/nnunetv2/experiment_planning/plan_and_preprocess_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from typing import List, Type, Optional, Tuple, Union
 
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, load_json
 
 import nnunetv2
 from nnunetv2.configuration import default_num_processes
 from nnunetv2.experiment_planning.dataset_fingerprint.fingerprint_extractor import DatasetFingerprintExtractor
@@ -45,43 +46,50 @@
     for d in dataset_ids:
         extract_fingerprint_dataset(d, fingerprint_extractor_class, num_processes, check_dataset_integrity, clean,
                                     verbose)
 
 
 def plan_experiment_dataset(dataset_id: int,
                             experiment_planner_class: Type[ExperimentPlanner] = ExperimentPlanner,
-                            gpu_memory_target_in_gb: float = 8, preprocess_class_name: str = 'DefaultPreprocessor',
+                            gpu_memory_target_in_gb: float = None, preprocess_class_name: str = 'DefaultPreprocessor',
                             overwrite_target_spacing: Optional[Tuple[float, ...]] = None,
                             overwrite_plans_name: Optional[str] = None) -> Tuple[dict, str]:
     """
     overwrite_target_spacing ONLY applies to 3d_fullres and 3d_cascade fullres!
     """
     kwargs = {}
     if overwrite_plans_name is not None:
         kwargs['plans_name'] = overwrite_plans_name
+    if gpu_memory_target_in_gb is not None:
+        kwargs['gpu_memory_target_in_gb'] = gpu_memory_target_in_gb
 
     planner = experiment_planner_class(dataset_id,
-                                       gpu_memory_target_in_gb=gpu_memory_target_in_gb,
                                        preprocessor_name=preprocess_class_name,
                                        overwrite_target_spacing=[float(i) for i in overwrite_target_spacing] if
                                        overwrite_target_spacing is not None else overwrite_target_spacing,
                                        suppress_transpose=False,  # might expose this later,
                                        **kwargs
                                        )
     ret = planner.plan_experiment()
     return ret, planner.plans_identifier
 
 
 def plan_experiments(dataset_ids: List[int], experiment_planner_class_name: str = 'ExperimentPlanner',
-                     gpu_memory_target_in_gb: float = 8, preprocess_class_name: str = 'DefaultPreprocessor',
+                     gpu_memory_target_in_gb: float = None, preprocess_class_name: str = 'DefaultPreprocessor',
                      overwrite_target_spacing: Optional[Tuple[float, ...]] = None,
                      overwrite_plans_name: Optional[str] = None):
     """
     overwrite_target_spacing ONLY applies to 3d_fullres and 3d_cascade fullres!
     """
+    if experiment_planner_class_name == 'ExperimentPlanner':
+        print("\n############################\n"
+              "INFO: You are using the old nnU-Net default planner. We have updated our recommendations. "
+              "Please consider using those instead! "
+              "Read more here: https://github.com/MIC-DKFZ/nnUNet/blob/master/documentation/resenc_presets.md"
+              "\n############################\n")
     experiment_planner = recursive_find_python_class(join(nnunetv2.__path__[0], "experiment_planning"),
                                                      experiment_planner_class_name,
                                                      current_module="nnunetv2.experiment_planning")
     plans_identifier = None
     for d in dataset_ids:
         _, plans_identifier = plan_experiment_dataset(d, experiment_planner, gpu_memory_target_in_gb,
                                                       preprocess_class_name,
```

### Comparing `nnunetv2-2.3.1/nnunetv2/experiment_planning/plan_and_preprocess_entrypoints.py` & `nnunetv2-2.4/nnunetv2/experiment_planning/plan_and_preprocess_entrypoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,19 +33,20 @@
     parser.add_argument('-d', nargs='+', type=int,
                         help="[REQUIRED] List of dataset IDs. Example: 2 4 5. This will run fingerprint extraction, experiment "
                              "planning and preprocessing for these datasets. Can of course also be just one dataset")
     parser.add_argument('-pl', type=str, default='ExperimentPlanner', required=False,
                         help='[OPTIONAL] Name of the Experiment Planner class that should be used. Default is '
                              '\'ExperimentPlanner\'. Note: There is no longer a distinction between 2d and 3d planner. '
                              'It\'s an all in one solution now. Wuch. Such amazing.')
-    parser.add_argument('-gpu_memory_target', default=8, type=float, required=False,
-                        help='[OPTIONAL] DANGER ZONE! Sets a custom GPU memory target. Default: 8 [GB]. Changing this will '
+    parser.add_argument('-gpu_memory_target', default=None, type=float, required=False,
+                        help='[OPTIONAL] DANGER ZONE! Sets a custom GPU memory target (in GB). Default: None (=Planner '
+                             'class default is used). Changing this will '
                              'affect patch and batch size and will '
                              'definitely affect your models performance! Only use this if you really know what you '
-                             'are doing and NEVER use this without running the default nnU-Net first (as a baseline).')
+                             'are doing and NEVER use this without running the default nnU-Net first as a baseline.')
     parser.add_argument('-preprocessor_name', default='DefaultPreprocessor', type=str, required=False,
                         help='[OPTIONAL] DANGER ZONE! Sets a custom preprocessor class. This class must be located in '
                              'nnunetv2.preprocessing. Default: \'DefaultPreprocessor\'. Changing this may affect your '
                              'models performance! Only use this if you really know what you '
                              'are doing and NEVER use this without running the default nnU-Net first (as a baseline).')
     parser.add_argument('-overwrite_target_spacing', default=None, nargs='+', required=False,
                         help='[OPTIONAL] DANGER ZONE! Sets a custom target spacing for the 3d_fullres and 3d_cascade_fullres '
@@ -127,19 +128,20 @@
                         help='[OPTIONAL] Set this flag to overwrite existing fingerprints. If this flag is not set and a '
                              'fingerprint already exists, the fingerprint extractor will not run. REQUIRED IF YOU '
                              'CHANGE THE DATASET FINGERPRINT EXTRACTOR OR MAKE CHANGES TO THE DATASET!')
     parser.add_argument('-pl', type=str, default='ExperimentPlanner', required=False,
                         help='[OPTIONAL] Name of the Experiment Planner class that should be used. Default is '
                              '\'ExperimentPlanner\'. Note: There is no longer a distinction between 2d and 3d planner. '
                              'It\'s an all in one solution now. Wuch. Such amazing.')
-    parser.add_argument('-gpu_memory_target', default=8, type=int, required=False,
-                        help='[OPTIONAL] DANGER ZONE! Sets a custom GPU memory target. Default: 8 [GB]. Changing this will '
+    parser.add_argument('-gpu_memory_target', default=None, type=float, required=False,
+                        help='[OPTIONAL] DANGER ZONE! Sets a custom GPU memory target (in GB). Default: None (=Planner '
+                             'class default is used). Changing this will '
                              'affect patch and batch size and will '
                              'definitely affect your models performance! Only use this if you really know what you '
-                             'are doing and NEVER use this without running the default nnU-Net first (as a baseline).')
+                             'are doing and NEVER use this without running the default nnU-Net first as a baseline.')
     parser.add_argument('-preprocessor_name', default='DefaultPreprocessor', type=str, required=False,
                         help='[OPTIONAL] DANGER ZONE! Sets a custom preprocessor class. This class must be located in '
                              'nnunetv2.preprocessing. Default: \'DefaultPreprocessor\'. Changing this may affect your '
                              'models performance! Only use this if you really know what you '
                              'are doing and NEVER use this without running the default nnU-Net first (as a baseline).')
     parser.add_argument('-overwrite_target_spacing', default=None, nargs='+', required=False,
                         help='[OPTIONAL] DANGER ZONE! Sets a custom target spacing for the 3d_fullres and 3d_cascade_fullres '
@@ -179,15 +181,16 @@
 
     # fingerprint extraction
     print("Fingerprint extraction...")
     extract_fingerprints(args.d, args.fpe, args.npfp, args.verify_dataset_integrity, args.clean, args.verbose)
 
     # experiment planning
     print('Experiment planning...')
-    plans_identifier = plan_experiments(args.d, args.pl, args.gpu_memory_target, args.preprocessor_name, args.overwrite_target_spacing, args.overwrite_plans_name)
+    plans_identifier = plan_experiments(args.d, args.pl, args.gpu_memory_target, args.preprocessor_name,
+                                        args.overwrite_target_spacing, args.overwrite_plans_name)
 
     # manage default np
     if args.np is None:
         default_np = {"2d": 8, "3d_fullres": 4, "3d_lowres": 8}
         np = [default_np[c] if c in default_np.keys() else 4 for c in args.c]
     else:
         np = args.np
```

### Comparing `nnunetv2-2.3.1/nnunetv2/experiment_planning/plans_for_pretraining/move_plans_between_datasets.py` & `nnunetv2-2.4/nnunetv2/experiment_planning/plans_for_pretraining/move_plans_between_datasets.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/experiment_planning/verify_dataset_integrity.py` & `nnunetv2-2.4/nnunetv2/experiment_planning/verify_dataset_integrity.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     if 'nibabel_stuff' in properties_image.keys():
         # this image was read with NibabelIO
         affine_image = properties_image['nibabel_stuff']['original_affine']
         affine_seg = properties_seg['nibabel_stuff']['original_affine']
         if not np.allclose(affine_image, affine_seg):
             print('WARNING: Affine is not the same for image and seg! \nAffine image: %s \nAffine seg: %s\n'
                   'Image files: %s. \nSeg file: %s.\nThis can be a problem but doesn\'t have to be. Please run '
-                  'nnUNet_plot_dataset_pngs to verify if everything is OK!\n'
+                  'nnUNetv2_plot_overlay_pngs to verify if everything is OK!\n'
                   % (affine_image, affine_seg, image_files, label_file))
 
     # sitk checks
     if 'sitk_stuff' in properties_image.keys():
         # this image was read with SimpleITKIO
         # spacing has already been checked, only check direction and origin
         origin_image = properties_image['sitk_stuff']['origin']
```

### Comparing `nnunetv2-2.3.1/nnunetv2/imageio/base_reader_writer.py` & `nnunetv2-2.4/nnunetv2/imageio/base_reader_writer.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/imageio/natural_image_reader_writer.py` & `nnunetv2-2.4/nnunetv2/imageio/natural_image_reader_writer.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/imageio/nibabel_reader_writer.py` & `nnunetv2-2.4/nnunetv2/imageio/nibabel_reader_writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 class NibabelIO(BaseReaderWriter):
     """
     Nibabel loads the images in a different order than sitk. We convert the axes to the sitk order to be
     consistent. This is of course considered properly in segmentation export as well.
 
-    IMPORTANT: Run nnUNet_plot_dataset_pngs to verify that this did not destroy the alignment of data and seg!
+    IMPORTANT: Run nnUNetv2_plot_overlay_pngs to verify that this did not destroy the alignment of data and seg!
     """
     supported_file_endings = [
         '.nii.gz',
         '.nrrd',
         '.mha'
     ]
 
@@ -63,15 +63,15 @@
             raise RuntimeError()
         if not self._check_all_same_array(original_affines):
             print('WARNING! Not all input images have the same original_affines!')
             print('Affines:')
             print(original_affines)
             print('Image files:')
             print(image_fnames)
-            print('It is up to you to decide whether that\'s a problem. You should run nnUNet_plot_dataset_pngs to verify '
+            print('It is up to you to decide whether that\'s a problem. You should run nnUNetv2_plot_overlay_pngs to verify '
                   'that segmentations and data overlap.')
         if not self._check_all_same(spacings_for_nnunet):
             print('ERROR! Not all input images have the same spacing_for_nnunet! This might be caused by them not '
                   'having the same affine')
             print('spacings_for_nnunet:')
             print(spacings_for_nnunet)
             print('Image files:')
@@ -100,15 +100,15 @@
 class NibabelIOWithReorient(BaseReaderWriter):
     """
     Reorients images to RAS
 
     Nibabel loads the images in a different order than sitk. We convert the axes to the sitk order to be
     consistent. This is of course considered properly in segmentation export as well.
 
-    IMPORTANT: Run nnUNet_plot_dataset_pngs to verify that this did not destroy the alignment of data and seg!
+    IMPORTANT: Run nnUNetv2_plot_overlay_pngs to verify that this did not destroy the alignment of data and seg!
     """
     supported_file_endings = [
         '.nii.gz',
         '.nrrd',
         '.mha'
     ]
 
@@ -145,15 +145,15 @@
             raise RuntimeError()
         if not self._check_all_same_array(reoriented_affines):
             print('WARNING! Not all input images have the same reoriented_affines!')
             print('Affines:')
             print(reoriented_affines)
             print('Image files:')
             print(image_fnames)
-            print('It is up to you to decide whether that\'s a problem. You should run nnUNet_plot_dataset_pngs to verify '
+            print('It is up to you to decide whether that\'s a problem. You should run nnUNetv2_plot_overlay_pngs to verify '
                   'that segmentations and data overlap.')
         if not self._check_all_same(spacings_for_nnunet):
             print('ERROR! Not all input images have the same spacing_for_nnunet! This might be caused by them not '
                   'having the same affine')
             print('spacings_for_nnunet:')
             print(spacings_for_nnunet)
             print('Image files:')
```

### Comparing `nnunetv2-2.3.1/nnunetv2/imageio/reader_writer_registry.py` & `nnunetv2-2.4/nnunetv2/imageio/reader_writer_registry.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/imageio/simpleitk_reader_writer.py` & `nnunetv2-2.4/nnunetv2/imageio/simpleitk_reader_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,23 +74,23 @@
             raise RuntimeError()
         if not self._check_all_same(origins):
             print('WARNING! Not all input images have the same origin!')
             print('Origins:')
             print(origins)
             print('Image files:')
             print(image_fnames)
-            print('It is up to you to decide whether that\'s a problem. You should run nnUNet_plot_dataset_pngs to verify '
+            print('It is up to you to decide whether that\'s a problem. You should run nnUNetv2_plot_overlay_pngs to verify '
                   'that segmentations and data overlap.')
         if not self._check_all_same(directions):
             print('WARNING! Not all input images have the same direction!')
             print('Directions:')
             print(directions)
             print('Image files:')
             print(image_fnames)
-            print('It is up to you to decide whether that\'s a problem. You should run nnUNet_plot_dataset_pngs to verify '
+            print('It is up to you to decide whether that\'s a problem. You should run nnUNetv2_plot_overlay_pngs to verify '
                   'that segmentations and data overlap.')
         if not self._check_all_same(spacings_for_nnunet):
             print('ERROR! Not all input images have the same spacing_for_nnunet! (This should not happen and must be a '
                   'bug. Please report!')
             print('spacings_for_nnunet:')
             print(spacings_for_nnunet)
             print('Image files:')
```

### Comparing `nnunetv2-2.3.1/nnunetv2/imageio/tif_reader_writer.py` & `nnunetv2-2.4/nnunetv2/imageio/tif_reader_writer.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/inference/data_iterators.py` & `nnunetv2-2.4/nnunetv2/inference/data_iterators.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
                                                                plans_manager,
                                                                configuration_manager,
                                                                dataset_json)
             if list_of_segs_from_prev_stage_files is not None and list_of_segs_from_prev_stage_files[idx] is not None:
                 seg_onehot = convert_labelmap_to_one_hot(seg[0], label_manager.foreground_labels, data.dtype)
                 data = np.vstack((data, seg_onehot))
 
-            data = torch.from_numpy(data).contiguous().float()
+            data = torch.from_numpy(data).to(dtype=torch.float32, memory_format=torch.contiguous_format)
 
             item = {'data': data, 'data_properties': data_properties,
                     'ofile': output_filenames_truncated[idx] if output_filenames_truncated is not None else None}
             success = False
             while not success:
                 try:
                     if abort_event.is_set():
@@ -142,17 +142,15 @@
                          seed_for_shuffle=1, return_incomplete=True,
                          shuffle=False, infinite=False, sampling_probabilities=None)
 
         self.indices = list(range(len(list_of_lists)))
 
     def generate_train_batch(self):
         idx = self.get_indices()[0]
-        files = self._data[idx][0]
-        seg_prev_stage = self._data[idx][1]
-        ofile = self._data[idx][2]
+        files, seg_prev_stage, ofile = self._data[idx][0]
         # if we have a segmentation from the previous stage we have to process it together with the images so that we
         # can crop it appropriately (if needed). Otherwise it would just be resized to the shape of the data after
         # preprocessing and then there might be misalignments
         data, seg, data_properties = self.preprocessor.run_case(files, seg_prev_stage, self.plans_manager,
                                                                 self.configuration_manager,
                                                                 self.dataset_json)
         if seg_prev_stage is not None:
@@ -188,18 +186,15 @@
             seed_for_shuffle=1, return_incomplete=True,
             shuffle=False, infinite=False, sampling_probabilities=None)
 
         self.indices = list(range(len(list_of_images)))
 
     def generate_train_batch(self):
         idx = self.get_indices()[0]
-        image = self._data[idx][0]
-        seg_prev_stage = self._data[idx][1]
-        props = self._data[idx][2]
-        ofname = self._data[idx][3]
+        image, seg_prev_stage, props, ofname = self._data[idx][0]
         # if we have a segmentation from the previous stage we have to process it together with the images so that we
         # can crop it appropriately (if needed). Otherwise it would just be resized to the shape of the data after
         # preprocessing and then there might be misalignments
         data, seg = self.preprocessor.run_case_npy(image, seg_prev_stage, props,
                                                    self.plans_manager,
                                                    self.configuration_manager,
                                                    self.dataset_json)
@@ -234,15 +229,15 @@
                                                   plans_manager,
                                                   configuration_manager,
                                                   dataset_json)
             if list_of_segs_from_prev_stage is not None and list_of_segs_from_prev_stage[idx] is not None:
                 seg_onehot = convert_labelmap_to_one_hot(seg[0], label_manager.foreground_labels, data.dtype)
                 data = np.vstack((data, seg_onehot))
 
-            data = torch.from_numpy(data).contiguous().float()
+            data = torch.from_numpy(data).to(dtype=torch.float32, memory_format=torch.contiguous_format)
 
             item = {'data': data, 'data_properties': list_of_image_properties[idx],
                     'ofile': truncated_ofnames[idx] if truncated_ofnames is not None else None}
             success = False
             while not success:
                 try:
                     if abort_event.is_set():
```

### Comparing `nnunetv2-2.3.1/nnunetv2/inference/examples.py` & `nnunetv2-2.4/nnunetv2/inference/examples.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/inference/export_prediction.py` & `nnunetv2-2.4/nnunetv2/inference/export_prediction.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/inference/predict_from_raw_data.py` & `nnunetv2-2.4/nnunetv2/inference/predict_from_raw_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,17 +51,16 @@
         self.plans_manager, self.configuration_manager, self.list_of_parameters, self.network, self.dataset_json, \
         self.trainer_name, self.allowed_mirroring_axes, self.label_manager = None, None, None, None, None, None, None, None
 
         self.tile_step_size = tile_step_size
         self.use_gaussian = use_gaussian
         self.use_mirroring = use_mirroring
         if device.type == 'cuda':
-            # device = torch.device(type='cuda', index=0)  # set the desired GPU with CUDA_VISIBLE_DEVICES!
-            pass
-        if device.type != 'cuda':
+            torch.backends.cudnn.benchmark = True
+        else:
             print(f'perform_everything_on_device=True is only supported for cuda devices! Setting this to False')
             perform_everything_on_device = False
         self.device = device
         self.perform_everything_on_device = perform_everything_on_device
 
     def initialize_from_trained_model_folder(self, model_training_output_dir: str,
                                              use_folds: Union[Tuple[Union[int, str]], None],
@@ -418,14 +417,24 @@
         return ret
 
     def predict_single_npy_array(self, input_image: np.ndarray, image_properties: dict,
                                  segmentation_previous_stage: np.ndarray = None,
                                  output_file_truncated: str = None,
                                  save_or_return_probabilities: bool = False):
         """
+        WARNING: SLOW. ONLY USE THIS IF YOU CANNOT GIVE NNUNET MULTIPLE IMAGES AT ONCE FOR SOME REASON.
+
+
+        input_image: Make sure to load the image in the way nnU-Net expects! nnU-Net is trained on a certain axis
+                     ordering which cannot be disturbed in inference,
+                     otherwise you will get bad results. The easiest way to achieve that is to use the same I/O class
+                     for loading images as was used during nnU-Net preprocessing! You can find that class in your
+                     plans.json file under the key "image_reader_writer". If you decide to freestyle, know that the
+                     default axis ordering for medical images is the one from SimpleITK. If you load with nibabel,
+                     you need to transpose your axes AND your spacing from [x,y,z] to [z,y,x]!
         image_properties must only have a 'spacing' key!
         """
         ppa = PreprocessAdapterFromNpy([input_image], [segmentation_previous_stage], [image_properties],
                                        [output_file_truncated],
                                        self.plans_manager, self.dataset_json, self.configuration_manager,
                                        num_threads_in_multithreaded=1, verbose=self.verbose)
         if self.verbose:
@@ -460,38 +469,36 @@
         TOP OF THE IMAGE AS ONE-HOT REPRESENTATION! SEE PreprocessAdapter ON HOW THIS SHOULD BE DONE!
 
         RETURNED LOGITS HAVE THE SHAPE OF THE INPUT. THEY MUST BE CONVERTED BACK TO THE ORIGINAL IMAGE SIZE.
         SEE convert_predicted_logits_to_segmentation_with_correct_shape
         """
         n_threads = torch.get_num_threads()
         torch.set_num_threads(default_num_processes if default_num_processes < n_threads else n_threads)
-        with torch.no_grad():
-            prediction = None
+        prediction = None
 
-            for params in self.list_of_parameters:
+        for params in self.list_of_parameters:
 
-                # messing with state dict names...
-                if not isinstance(self.network, OptimizedModule):
-                    self.network.load_state_dict(params)
-                else:
-                    self.network._orig_mod.load_state_dict(params)
+            # messing with state dict names...
+            if not isinstance(self.network, OptimizedModule):
+                self.network.load_state_dict(params)
+            else:
+                self.network._orig_mod.load_state_dict(params)
 
-                # why not leave prediction on device if perform_everything_on_device? Because this may cause the
-                # second iteration to crash due to OOM. Grabbing that with try except cause way more bloated code than
-                # this actually saves computation time
-                if prediction is None:
-                    prediction = self.predict_sliding_window_return_logits(data).to('cpu')
-                else:
-                    prediction += self.predict_sliding_window_return_logits(data).to('cpu')
+            # why not leave prediction on device if perform_everything_on_device? Because this may cause the
+            # second iteration to crash due to OOM. Grabbing that with try except cause way more bloated code than
+            # this actually saves computation time
+            if prediction is None:
+                prediction = self.predict_sliding_window_return_logits(data).to('cpu')
+            else:
+                prediction += self.predict_sliding_window_return_logits(data).to('cpu')
 
-            if len(self.list_of_parameters) > 1:
-                prediction /= len(self.list_of_parameters)
+        if len(self.list_of_parameters) > 1:
+            prediction /= len(self.list_of_parameters)
 
-            if self.verbose: print('Prediction done')
-            prediction = prediction.to('cpu')
+        if self.verbose: print('Prediction done')
         torch.set_num_threads(n_threads)
         return prediction
 
     def _internal_get_sliding_window_slicers(self, image_size: Tuple[int, ...]):
         slicers = []
         if len(self.configuration_manager.patch_size) < len(image_size):
             assert len(self.configuration_manager.patch_size) == len(
@@ -530,19 +537,20 @@
         prediction = self.network(x)
 
         if mirror_axes is not None:
             # check for invalid numbers in mirror_axes
             # x should be 5d for 3d images and 4d for 2d. so the max value of mirror_axes cannot exceed len(x.shape) - 3
             assert max(mirror_axes) <= x.ndim - 3, 'mirror_axes does not match the dimension of the input!'
 
+            mirror_axes = [m + 2 for m in mirror_axes]
             axes_combinations = [
-                c for i in range(len(mirror_axes)) for c in itertools.combinations([m + 2 for m in mirror_axes], i + 1)
+                c for i in range(len(mirror_axes)) for c in itertools.combinations(mirror_axes, i + 1)
             ]
             for axes in axes_combinations:
-                prediction += torch.flip(self.network(torch.flip(x, (*axes,))), (*axes,))
+                prediction += torch.flip(self.network(torch.flip(x, axes)), axes)
             prediction /= (len(axes_combinations) + 1)
         return prediction
 
     def _internal_predict_sliding_window_return_logits(self,
                                                        data: torch.Tensor,
                                                        slicers,
                                                        do_on_device: bool = True,
@@ -561,89 +569,95 @@
             # preallocate arrays
             if self.verbose:
                 print(f'preallocating results arrays on device {results_device}')
             predicted_logits = torch.zeros((self.label_manager.num_segmentation_heads, *data.shape[1:]),
                                            dtype=torch.half,
                                            device=results_device)
             n_predictions = torch.zeros(data.shape[1:], dtype=torch.half, device=results_device)
+
             if self.use_gaussian:
                 gaussian = compute_gaussian(tuple(self.configuration_manager.patch_size), sigma_scale=1. / 8,
                                             value_scaling_factor=10,
                                             device=results_device)
+            else:
+                gaussian = 1
 
-            if self.verbose: print('running prediction')
-            if not self.allow_tqdm and self.verbose: print(f'{len(slicers)} steps')
+            if not self.allow_tqdm and self.verbose:
+                print(f'running prediction: {len(slicers)} steps')
             for sl in tqdm(slicers, disable=not self.allow_tqdm):
                 workon = data[sl][None]
-                workon = workon.to(self.device, non_blocking=False)
+                workon = workon.to(self.device)
 
                 prediction = self._internal_maybe_mirror_and_predict(workon)[0].to(results_device)
 
-                predicted_logits[sl] += (prediction * gaussian if self.use_gaussian else prediction)
-                n_predictions[sl[1:]] += (gaussian if self.use_gaussian else 1)
+                if self.use_gaussian:
+                    prediction *= gaussian
+                predicted_logits[sl] += prediction
+                n_predictions[sl[1:]] += gaussian
 
             predicted_logits /= n_predictions
             # check for infs
             if torch.any(torch.isinf(predicted_logits)):
                 raise RuntimeError('Encountered inf in predicted array. Aborting... If this problem persists, '
                                    'reduce value_scaling_factor in compute_gaussian or increase the dtype of '
                                    'predicted_logits to fp32')
         except Exception as e:
             del predicted_logits, n_predictions, prediction, gaussian, workon
             empty_cache(self.device)
             empty_cache(results_device)
             raise e
         return predicted_logits
 
+    @torch.inference_mode()
     def predict_sliding_window_return_logits(self, input_image: torch.Tensor) \
             -> Union[np.ndarray, torch.Tensor]:
         assert isinstance(input_image, torch.Tensor)
         self.network = self.network.to(self.device)
         self.network.eval()
 
         empty_cache(self.device)
 
         # Autocast can be annoying
         # If the device_type is 'cpu' then it's slow as heck on some CPUs (no auto bfloat16 support detection)
         # and needs to be disabled.
         # If the device_type is 'mps' then it will complain that mps is not implemented, even if enabled=False
         # is set. Whyyyyyyy. (this is why we don't make use of enabled=False)
         # So autocast will only be active if we have a cuda device.
-        with torch.no_grad():
-            with torch.autocast(self.device.type, enabled=True) if self.device.type == 'cuda' else dummy_context():
-                assert input_image.ndim == 4, 'input_image must be a 4D np.ndarray or torch.Tensor (c, x, y, z)'
-
-                if self.verbose: print(f'Input shape: {input_image.shape}')
-                if self.verbose: print("step_size:", self.tile_step_size)
-                if self.verbose: print("mirror_axes:", self.allowed_mirroring_axes if self.use_mirroring else None)
-
-                # if input_image is smaller than tile_size we need to pad it to tile_size.
-                data, slicer_revert_padding = pad_nd_image(input_image, self.configuration_manager.patch_size,
-                                                           'constant', {'value': 0}, True,
-                                                           None)
-
-                slicers = self._internal_get_sliding_window_slicers(data.shape[1:])
-
-                if self.perform_everything_on_device and self.device != 'cpu':
-                    # we need to try except here because we can run OOM in which case we need to fall back to CPU as a results device
-                    try:
-                        predicted_logits = self._internal_predict_sliding_window_return_logits(data, slicers,
-                                                                                               self.perform_everything_on_device)
-                    except RuntimeError:
-                        print(
-                            'Prediction on device was unsuccessful, probably due to a lack of memory. Moving results arrays to CPU')
-                        empty_cache(self.device)
-                        predicted_logits = self._internal_predict_sliding_window_return_logits(data, slicers, False)
-                else:
+        with torch.autocast(self.device.type, enabled=True) if self.device.type == 'cuda' else dummy_context():
+            assert input_image.ndim == 4, 'input_image must be a 4D np.ndarray or torch.Tensor (c, x, y, z)'
+
+            if self.verbose: 
+                print(f'Input shape: {input_image.shape}')
+                print("step_size:", self.tile_step_size)
+                print("mirror_axes:", self.allowed_mirroring_axes if self.use_mirroring else None)
+
+            # if input_image is smaller than tile_size we need to pad it to tile_size.
+            data, slicer_revert_padding = pad_nd_image(input_image, self.configuration_manager.patch_size,
+                                                       'constant', {'value': 0}, True,
+                                                       None)
+
+            slicers = self._internal_get_sliding_window_slicers(data.shape[1:])
+
+            if self.perform_everything_on_device and self.device != 'cpu':
+                # we need to try except here because we can run OOM in which case we need to fall back to CPU as a results device
+                try:
                     predicted_logits = self._internal_predict_sliding_window_return_logits(data, slicers,
                                                                                            self.perform_everything_on_device)
+                except RuntimeError:
+                    print(
+                        'Prediction on device was unsuccessful, probably due to a lack of memory. Moving results arrays to CPU')
+                    empty_cache(self.device)
+                    predicted_logits = self._internal_predict_sliding_window_return_logits(data, slicers, False)
+            else:
+                predicted_logits = self._internal_predict_sliding_window_return_logits(data, slicers,
+                                                                                       self.perform_everything_on_device)
 
-                empty_cache(self.device)
-                # revert padding
-                predicted_logits = predicted_logits[tuple([slice(None), *slicer_revert_padding[1:]])]
+            empty_cache(self.device)
+            # revert padding
+            predicted_logits = predicted_logits[(slice(None), *slicer_revert_padding[1:])]
         return predicted_logits
 
 
 def predict_entry_point_modelfolder():
     import argparse
     parser = argparse.ArgumentParser(description='Use this to run inference with nnU-Net. This function is used when '
                                                  'you want to manually specify a folder containing a trained nnU-Net '
```

### Comparing `nnunetv2-2.3.1/nnunetv2/inference/sliding_window_prediction.py` & `nnunetv2-2.4/nnunetv2/inference/sliding_window_prediction.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,21 +15,19 @@
     center_coords = [i // 2 for i in tile_size]
     sigmas = [i * sigma_scale for i in tile_size]
     tmp[tuple(center_coords)] = 1
     gaussian_importance_map = gaussian_filter(tmp, sigmas, 0, mode='constant', cval=0)
 
     gaussian_importance_map = torch.from_numpy(gaussian_importance_map)
 
-    gaussian_importance_map = gaussian_importance_map / torch.max(gaussian_importance_map) * value_scaling_factor
-    gaussian_importance_map = gaussian_importance_map.type(dtype).to(device)
-
+    gaussian_importance_map /= (torch.max(gaussian_importance_map) / value_scaling_factor)
+    gaussian_importance_map = gaussian_importance_map.to(device=device, dtype=dtype)
     # gaussian_importance_map cannot be 0, otherwise we may end up with nans!
-    gaussian_importance_map[gaussian_importance_map == 0] = torch.min(
-        gaussian_importance_map[gaussian_importance_map != 0])
-
+    mask = gaussian_importance_map == 0
+    gaussian_importance_map[mask] = torch.min(gaussian_importance_map[~mask])
     return gaussian_importance_map
 
 
 def compute_steps_for_sliding_window(image_size: Tuple[int, ...], tile_size: Tuple[int, ...], tile_step_size: float) -> \
         List[List[int]]:
     assert [i >= j for i, j in zip(image_size, tile_size)], "image size must be as large or larger than patch_size"
     assert 0 < tile_step_size <= 1, 'step_size must be larger than 0 and smaller or equal to 1'
```

### Comparing `nnunetv2-2.3.1/nnunetv2/model_sharing/entry_points.py` & `nnunetv2-2.4/nnunetv2/model_sharing/entry_points.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/model_sharing/model_download.py` & `nnunetv2-2.4/nnunetv2/model_sharing/model_download.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/model_sharing/model_export.py` & `nnunetv2-2.4/nnunetv2/model_sharing/model_export.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/paths.py` & `nnunetv2-2.4/nnunetv2/paths.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/postprocessing/remove_connected_components.py` & `nnunetv2-2.4/nnunetv2/postprocessing/remove_connected_components.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/preprocessing/normalization/default_normalization_schemes.py` & `nnunetv2-2.4/nnunetv2/preprocessing/normalization/default_normalization_schemes.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/preprocessing/normalization/map_channel_name_to_normalization.py` & `nnunetv2-2.4/nnunetv2/preprocessing/normalization/map_channel_name_to_normalization.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import Type
 
 from nnunetv2.preprocessing.normalization.default_normalization_schemes import CTNormalization, NoNormalization, \
     ZScoreNormalization, RescaleTo01Normalization, RGBTo01Normalization, ImageNormalization
 
 channel_name_to_normalization_mapping = {
-    'CT': CTNormalization,
-    'noNorm': NoNormalization,
+    'ct': CTNormalization,
+    'nonorm': NoNormalization,
     'zscore': ZScoreNormalization,
     'rescale_to_0_1': RescaleTo01Normalization,
     'rgb_to_0_1': RGBTo01Normalization
 }
 
 
 def get_normalization_scheme(channel_name: str) -> Type[ImageNormalization]:
     """
     If we find the channel_name in channel_name_to_normalization_mapping return the corresponding normalization. If it is
     not found, use the default (ZScoreNormalization)
     """
-    norm_scheme = channel_name_to_normalization_mapping.get(channel_name)
+    norm_scheme = channel_name_to_normalization_mapping.get(channel_name.casefold())
     if norm_scheme is None:
         norm_scheme = ZScoreNormalization
     # print('Using %s for image normalization' % norm_scheme.__name__)
     return norm_scheme
```

### Comparing `nnunetv2-2.3.1/nnunetv2/preprocessing/preprocessors/default_preprocessor.py` & `nnunetv2-2.4/nnunetv2/preprocessing/preprocessors/default_preprocessor.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/preprocessing/resampling/default_resampling.py` & `nnunetv2-2.4/nnunetv2/preprocessing/resampling/default_resampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             do_separate_z = False
         else:
             pass
 
     if data is not None:
         assert data.ndim == 4, "data must be c x y z"
 
-    shape = np.array(data[0].shape)
+    shape = np.array(data.shape)
     new_shape = compute_new_shape(shape[1:], current_spacing, new_spacing)
 
     data_reshaped = resample_data_or_seg(data, new_shape, is_seg, axis, order, do_separate_z, order_z=order_z)
     return data_reshaped
 
 
 def resample_data_or_seg_to_shape(data: Union[torch.Tensor, np.ndarray],
```

### Comparing `nnunetv2-2.3.1/nnunetv2/preprocessing/resampling/utils.py` & `nnunetv2-2.4/nnunetv2/preprocessing/resampling/utils.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/run/load_pretrained_weights.py` & `nnunetv2-2.4/nnunetv2/run/load_pretrained_weights.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import torch
 from torch._dynamo import OptimizedModule
 from torch.nn.parallel import DistributedDataParallel as DDP
+import torch.distributed as dist
 
 
 def load_pretrained_weights(network, fname, verbose=False):
     """
     Transfers all weights between matching keys in state_dicts. matching is done by name and we only transfer if the
     shape is also the same. Segmentation layers (the 1x1(x1) layers that produce the segmentation maps)
     identified by keys ending with '.seg_layers') are not transferred!
 
     If the pretrained weights were obtained with a training outside nnU-Net and DDP or torch.optimize was used,
     you need to change the keys of the pretrained state_dict. DDP adds a 'module.' prefix and torch.optim adds
     '_orig_mod'. You DO NOT need to worry about this if pretraining was done with nnU-Net as
     nnUNetTrainer.save_checkpoint takes care of that!
 
     """
-    saved_model = torch.load(fname)
+    if dist.is_initialized():
+        saved_model = torch.load(fname, map_location=torch.device('cuda', dist.get_rank()))
+    else:
+        saved_model = torch.load(fname)
     pretrained_dict = saved_model['network_weights']
 
     skip_strings_in_pretrained = [
         '.seg_layers.',
     ]
 
     if isinstance(network, DDP):
```

### Comparing `nnunetv2-2.3.1/nnunetv2/run/run_training.py` & `nnunetv2-2.4/nnunetv2/run/run_training.py`

 * *Files 3% similar despite different names*

```diff
@@ -144,14 +144,20 @@
                  use_compressed_data: bool = False,
                  export_validation_probabilities: bool = False,
                  continue_training: bool = False,
                  only_run_validation: bool = False,
                  disable_checkpointing: bool = False,
                  val_with_best: bool = False,
                  device: torch.device = torch.device('cuda')):
+    if plans_identifier == 'nnUNetPlans':
+        print("\n############################\n"
+              "INFO: You are using the old nnU-Net default plans. We have updated our recommendations. "
+              "Please consider using those instead! "
+              "Read more here: https://github.com/MIC-DKFZ/nnUNet/blob/master/documentation/resenc_presets.md"
+              "\n############################\n")
     if isinstance(fold, str):
         if fold != 'all':
             try:
                 fold = int(fold)
             except ValueError as e:
                 print(f'Unable to convert given value for fold to int: {fold}. fold must bei either "all" or an integer!')
                 raise e
```

### Comparing `nnunetv2-2.3.1/nnunetv2/tests/integration_tests/add_lowres_and_cascade.py` & `nnunetv2-2.4/nnunetv2/tests/integration_tests/add_lowres_and_cascade.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/tests/integration_tests/cleanup_integration_test.py` & `nnunetv2-2.4/nnunetv2/tests/integration_tests/cleanup_integration_test.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/tests/integration_tests/run_integration_test_bestconfig_inference.py` & `nnunetv2-2.4/nnunetv2/tests/integration_tests/run_integration_test_bestconfig_inference.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/data_augmentation/compute_initial_patch_size.py` & `nnunetv2-2.4/nnunetv2/training/data_augmentation/compute_initial_patch_size.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/data_augmentation/custom_transforms/cascade_transforms.py` & `nnunetv2-2.4/nnunetv2/training/data_augmentation/custom_transforms/cascade_transforms.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/data_augmentation/custom_transforms/deep_supervision_donwsampling.py` & `nnunetv2-2.4/nnunetv2/training/data_augmentation/custom_transforms/deep_supervision_donwsampling.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/data_augmentation/custom_transforms/masking.py` & `nnunetv2-2.4/nnunetv2/training/data_augmentation/custom_transforms/masking.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/data_augmentation/custom_transforms/region_based_training.py` & `nnunetv2-2.4/nnunetv2/training/data_augmentation/custom_transforms/region_based_training.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/data_augmentation/custom_transforms/transforms_for_dummy_2d.py` & `nnunetv2-2.4/nnunetv2/training/data_augmentation/custom_transforms/transforms_for_dummy_2d.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/dataloading/base_data_loader.py` & `nnunetv2-2.4/nnunetv2/training/dataloading/base_data_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,14 @@
                  final_patch_size: Union[List[int], Tuple[int, ...], np.ndarray],
                  label_manager: LabelManager,
                  oversample_foreground_percent: float = 0.0,
                  sampling_probabilities: Union[List[int], Tuple[int, ...], np.ndarray] = None,
                  pad_sides: Union[List[int], Tuple[int, ...], np.ndarray] = None,
                  probabilistic_oversampling: bool = False):
         super().__init__(data, batch_size, 1, None, True, False, True, sampling_probabilities)
-        assert isinstance(data, nnUNetDataset), 'nnUNetDataLoaderBase only supports dictionaries as data'
         self.indices = list(data.keys())
 
         self.oversample_foreground_percent = oversample_foreground_percent
         self.final_patch_size = final_patch_size
         self.patch_size = patch_size
         self.list_of_keys = list(self._data.keys())
         # need_to_pad denotes by how much we need to pad the data so that if we sample a patch of size final_patch_size
```

### Comparing `nnunetv2-2.3.1/nnunetv2/training/dataloading/data_loader_2d.py` & `nnunetv2-2.4/nnunetv2/training/dataloading/data_loader_2d.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/dataloading/data_loader_3d.py` & `nnunetv2-2.4/nnunetv2/training/dataloading/data_loader_3d.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,30 +25,31 @@
             dim = len(shape)
             bbox_lbs, bbox_ubs = self.get_bbox(shape, force_fg, properties['class_locations'])
 
             # whoever wrote this knew what he was doing (hint: it was me). We first crop the data to the region of the
             # bbox that actually lies within the data. This will result in a smaller array which is then faster to pad.
             # valid_bbox is just the coord that lied within the data cube. It will be padded to match the patch size
             # later
-            valid_bbox_lbs = [max(0, bbox_lbs[i]) for i in range(dim)]
-            valid_bbox_ubs = [min(shape[i], bbox_ubs[i]) for i in range(dim)]
+            valid_bbox_lbs = np.clip(bbox_lbs, a_min=0, a_max=None)
+            valid_bbox_ubs = np.minimum(shape, bbox_ubs)
 
             # At this point you might ask yourself why we would treat seg differently from seg_from_previous_stage.
             # Why not just concatenate them here and forget about the if statements? Well that's because segneeds to
             # be padded with -1 constant whereas seg_from_previous_stage needs to be padded with 0s (we could also
             # remove label -1 in the data augmentation but this way it is less error prone)
             this_slice = tuple([slice(0, data.shape[0])] + [slice(i, j) for i, j in zip(valid_bbox_lbs, valid_bbox_ubs)])
             data = data[this_slice]
 
             this_slice = tuple([slice(0, seg.shape[0])] + [slice(i, j) for i, j in zip(valid_bbox_lbs, valid_bbox_ubs)])
             seg = seg[this_slice]
 
             padding = [(-min(0, bbox_lbs[i]), max(bbox_ubs[i] - shape[i], 0)) for i in range(dim)]
-            data_all[j] = np.pad(data, ((0, 0), *padding), 'constant', constant_values=0)
-            seg_all[j] = np.pad(seg, ((0, 0), *padding), 'constant', constant_values=-1)
+            padding = ((0, 0), *padding)
+            data_all[j] = np.pad(data, padding, 'constant', constant_values=0)
+            seg_all[j] = np.pad(seg, padding, 'constant', constant_values=-1)
 
         return {'data': data_all, 'seg': seg_all, 'properties': case_properties, 'keys': selected_keys}
 
 
 if __name__ == '__main__':
     folder = '/media/fabian/data/nnUNet_preprocessed/Dataset002_Heart/3d_fullres'
     ds = nnUNetDataset(folder, 0)  # this should not load the properties!
```

### Comparing `nnunetv2-2.3.1/nnunetv2/training/dataloading/nnunet_dataset.py` & `nnunetv2-2.4/nnunetv2/training/dataloading/nnunet_dataset.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/logging/nnunet_logger.py` & `nnunetv2-2.4/nnunetv2/training/logging/nnunet_logger.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/loss/compound_losses.py` & `nnunetv2-2.4/nnunetv2/training/loss/compound_losses.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/loss/deep_supervision.py` & `nnunetv2-2.4/nnunetv2/training/loss/deep_supervision.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/loss/dice.py` & `nnunetv2-2.4/nnunetv2/training/loss/dice.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/loss/robust_ce_loss.py` & `nnunetv2-2.4/nnunetv2/training/loss/robust_ce_loss.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/lr_scheduler/polylr.py` & `nnunetv2-2.4/nnunetv2/training/lr_scheduler/polylr.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/nnUNetTrainer.py` & `nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/nnUNetTrainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,19 @@
             self.loss = self._build_loss()
             self.was_initialized = True
         else:
             raise RuntimeError("You have called self.initialize even though the trainer was already initialized. "
                                "That should not happen.")
 
     def _do_i_compile(self):
-        return ('nnUNet_compile' in os.environ.keys()) and (os.environ['nnUNet_compile'].lower() in ('true', '1', 't'))
+        # new default: compile is enabled!
+        if 'nnUNet_compile' not in os.environ.keys():
+            return True
+        else:
+            return os.environ['nnUNet_compile'].lower() in ('true', '1', 't')
 
     def _save_debug_information(self):
         # saving some debug information
         if self.local_rank == 0:
             dct = {}
             for k in self.__dir__():
                 if not k.startswith("__"):
@@ -643,14 +647,17 @@
             mt_gen_train = LimitedLenWrapper(self.num_iterations_per_epoch, data_loader=dl_tr, transform=tr_transforms,
                                              num_processes=allowed_num_processes, num_cached=6, seeds=None,
                                              pin_memory=self.device.type == 'cuda', wait_time=0.02)
             mt_gen_val = LimitedLenWrapper(self.num_val_iterations_per_epoch, data_loader=dl_val,
                                            transform=val_transforms, num_processes=max(1, allowed_num_processes // 2),
                                            num_cached=3, seeds=None, pin_memory=self.device.type == 'cuda',
                                            wait_time=0.02)
+        # # let's get this party started
+        _ = next(mt_gen_train)
+        _ = next(mt_gen_val)
         return mt_gen_train, mt_gen_val
 
     def get_plain_dataloaders(self, initial_patch_size: Tuple[int, ...], dim: int):
         dataset_tr, dataset_val = self.get_tr_and_val_datasets()
 
         if dim == 2:
             dl_tr = nnUNetDataLoader2D(dataset_tr, self.batch_size,
@@ -815,14 +822,18 @@
             mod = self.network
         if isinstance(mod, OptimizedModule):
             mod = mod._orig_mod
 
         mod.decoder.deep_supervision = enabled
 
     def on_train_start(self):
+        # dataloaders must be instantiated here (instead of __init__) because they need access to the training data
+        # which may not be present  when doing inference
+        self.dataloader_train, self.dataloader_val = self.get_dataloaders()
+
         if not self.was_initialized:
             self.initialize()
 
         maybe_mkdir_p(self.output_folder)
 
         # make sure deep supervision is on in the network
         self.set_deep_supervision_enabled(self.enable_deep_supervision)
@@ -830,24 +841,20 @@
         self.print_plans()
         empty_cache(self.device)
 
         # maybe unpack
         if self.unpack_dataset and self.local_rank == 0:
             self.print_to_log_file('unpacking dataset...')
             unpack_dataset(self.preprocessed_dataset_folder, unpack_segmentation=True, overwrite_existing=False,
-                           num_processes=max(1, round(get_allowed_n_proc_DA() // 2)))
+                           num_processes=max(1, round(get_allowed_n_proc_DA() // 2)), verify_npy=True)
             self.print_to_log_file('unpacking done...')
 
         if self.is_ddp:
             dist.barrier()
 
-        # dataloaders must be instantiated here because they need access to the training data which may not be present
-        # when doing inference
-        self.dataloader_train, self.dataloader_val = self.get_dataloaders()
-
         # copy plans and dataset.json so that they can be used for restoring everything we need for inference
         save_json(self.plans_manager.plans, join(self.output_folder_base, 'plans.json'), sort_keys=False)
         save_json(self.dataset_json, join(self.output_folder_base, 'dataset.json'), sort_keys=False)
 
         # we don't really need the fingerprint but its still handy to have it with the others
         shutil.copy(join(self.preprocessed_dataset_folder_base, 'dataset_fingerprint.json'),
                     join(self.output_folder_base, 'dataset_fingerprint.json'))
@@ -1280,21 +1287,25 @@
         self.on_train_start()
 
         for epoch in range(self.current_epoch, self.num_epochs):
             self.on_epoch_start()
 
             self.on_train_epoch_start()
             train_outputs = []
+            st = time()
             for batch_id in range(self.num_iterations_per_epoch):
                 train_outputs.append(self.train_step(next(self.dataloader_train)))
+            print('train time', time() - st)
             self.on_train_epoch_end(train_outputs)
 
             with torch.no_grad():
                 self.on_validation_epoch_start()
                 val_outputs = []
+                st = time()
                 for batch_id in range(self.num_val_iterations_per_epoch):
                     val_outputs.append(self.validation_step(next(self.dataloader_val)))
+                print('val time', time() - st)
                 self.on_validation_epoch_end(val_outputs)
 
             self.on_epoch_end()
 
         self.on_train_end()
```

### Comparing `nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/benchmarking/nnUNetTrainerBenchmark_5epochs.py` & `nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/benchmarking/nnUNetTrainerBenchmark_5epochs.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/benchmarking/nnUNetTrainerBenchmark_5epochs_noDataLoading.py` & `nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/benchmarking/nnUNetTrainerBenchmark_5epochs_noDataLoading.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerDA5.py` & `nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerDA5.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerDAOrd0.py` & `nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerDAOrd0.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerNoDA.py` & `nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerNoDA.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerNoMirroring.py` & `nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerNoMirroring.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/loss/nnUNetTrainerCELoss.py` & `nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/loss/nnUNetTrainerCELoss.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/loss/nnUNetTrainerDiceLoss.py` & `nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/loss/nnUNetTrainerDiceLoss.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/loss/nnUNetTrainerTopkLoss.py` & `nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/loss/nnUNetTrainerTopkLoss.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/lr_schedule/nnUNetTrainerCosAnneal.py` & `nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/lr_schedule/nnUNetTrainerCosAnneal.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/network_architecture/nnUNetTrainerBN.py` & `nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/network_architecture/nnUNetTrainerBN.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/optimizer/nnUNetTrainerAdam.py` & `nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/optimizer/nnUNetTrainerAdam.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/optimizer/nnUNetTrainerAdan.py` & `nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/optimizer/nnUNetTrainerAdan.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/sampling/nnUNetTrainer_probabilisticOversampling.py` & `nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/sampling/nnUNetTrainer_probabilisticOversampling.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/training_length/nnUNetTrainer_Xepochs.py` & `nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/training_length/nnUNetTrainer_Xepochs.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/training/nnUNetTrainer/variants/training_length/nnUNetTrainer_Xepochs_NoMirroring.py` & `nnunetv2-2.4/nnunetv2/training/nnUNetTrainer/variants/training_length/nnUNetTrainer_Xepochs_NoMirroring.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/utilities/collate_outputs.py` & `nnunetv2-2.4/nnunetv2/utilities/collate_outputs.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/utilities/crossval_split.py` & `nnunetv2-2.4/nnunetv2/utilities/crossval_split.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/utilities/dataset_name_id_conversion.py` & `nnunetv2-2.4/nnunetv2/utilities/dataset_name_id_conversion.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/utilities/ddp_allgather.py` & `nnunetv2-2.4/nnunetv2/utilities/ddp_allgather.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/utilities/default_n_proc_DA.py` & `nnunetv2-2.4/nnunetv2/utilities/default_n_proc_DA.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/utilities/file_path_utilities.py` & `nnunetv2-2.4/nnunetv2/utilities/file_path_utilities.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/utilities/find_class_by_name.py` & `nnunetv2-2.4/nnunetv2/utilities/find_class_by_name.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/utilities/get_network_from_plans.py` & `nnunetv2-2.4/nnunetv2/utilities/get_network_from_plans.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/utilities/helpers.py` & `nnunetv2-2.4/nnunetv2/utilities/helpers.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/utilities/json_export.py` & `nnunetv2-2.4/nnunetv2/utilities/json_export.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/utilities/label_handling/label_handling.py` & `nnunetv2-2.4/nnunetv2/utilities/label_handling/label_handling.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/utilities/overlay_plots.py` & `nnunetv2-2.4/nnunetv2/utilities/overlay_plots.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/utilities/plans_handling/plans_handler.py` & `nnunetv2-2.4/nnunetv2/utilities/plans_handling/plans_handler.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2/utilities/utils.py` & `nnunetv2-2.4/nnunetv2/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/nnunetv2.egg-info/PKG-INFO` & `nnunetv2-2.4/nnunetv2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nnunetv2
-Version: 2.3.1
+Version: 2.4
 Summary: nnU-Net is a framework for out-of-the box image segmentation.
 Author: Helmholtz Imaging Applied Computer Vision Lab
 Author-email: Fabian Isensee <f.isensee@dkfz-heidelberg.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -224,14 +224,21 @@
 
 # Welcome to the new nnU-Net!
 
 Click [here](https://github.com/MIC-DKFZ/nnUNet/tree/nnunetv1) if you were looking for the old one instead.
 
 Coming from V1? Check out the [TLDR Migration Guide](documentation/tldr_migration_guide_from_v1.md). Reading the rest of the documentation is still strongly recommended ;-)
 
+## **2024-04-18 UPDATE: New residual encoder UNet presets available!**
+Residual encoder UNet presets substantially improve segmentation performance.
+They ship for a variety of GPU memory targets. It's all awesome stuff, promised! 
+Read more :point_right: [here](documentation/resenc_presets.md) :point_left:
+
+Also check out our [new paper](https://arxiv.org/pdf/2404.09556.pdf) on systematically benchmarking recent developments in medical image segmentation. You might be surprised!
+
 # What is nnU-Net?
 Image datasets are enormously diverse: image dimensionality (2D, 3D), modalities/input channels (RGB image, CT, MRI, microscopy, ...), 
 image sizes, voxel sizes, class ratio, target structure properties and more change substantially between datasets. 
 Traditionally, given a new problem, a tailored solution needs to be manually designed and optimized  - a process that 
 is prone to errors, not scalable and where success is overwhelmingly determined by the skill of the experimenter. Even 
 for experts, this process is anything but simple: there are not only many design choices and data properties that need to 
 be considered, but they are also tightly interconnected, rendering reliable manual pipeline optimization all but impossible! 
@@ -308,14 +315,15 @@
 ## How to get started?
 Read these:
 - [Installation instructions](documentation/installation_instructions.md)
 - [Dataset conversion](documentation/dataset_format.md)
 - [Usage instructions](documentation/how_to_use_nnunet.md)
 
 Additional information:
+- [Learning from sparse annotations (scribbles, slices)](documentation/ignore_label.md)
 - [Region-based training](documentation/region_based_training.md)
 - [Manual data splits](documentation/manual_data_splits.md)
 - [Pretraining and finetuning](documentation/pretraining_and_finetuning.md)
 - [Intensity Normalization in nnU-Net](documentation/explanation_normalization.md)
 - [Manually editing nnU-Net configurations](documentation/explanation_plans_files.md)
 - [Extending nnU-Net](documentation/extending_nnunet.md)
 - [What is different in V2?](documentation/changelog.md)
```

### Comparing `nnunetv2-2.3.1/nnunetv2.egg-info/SOURCES.txt` & `nnunetv2-2.4/nnunetv2.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,16 @@
 nnunetv2/experiment_planning/verify_dataset_integrity.py
 nnunetv2/experiment_planning/dataset_fingerprint/__init__.py
 nnunetv2/experiment_planning/dataset_fingerprint/fingerprint_extractor.py
 nnunetv2/experiment_planning/experiment_planners/__init__.py
 nnunetv2/experiment_planning/experiment_planners/default_experiment_planner.py
 nnunetv2/experiment_planning/experiment_planners/network_topology.py
 nnunetv2/experiment_planning/experiment_planners/resencUNet_planner.py
+nnunetv2/experiment_planning/experiment_planners/residual_unets/__init__.py
+nnunetv2/experiment_planning/experiment_planners/residual_unets/residual_encoder_unet_planners.py
 nnunetv2/experiment_planning/plans_for_pretraining/__init__.py
 nnunetv2/experiment_planning/plans_for_pretraining/move_plans_between_datasets.py
 nnunetv2/imageio/__init__.py
 nnunetv2/imageio/base_reader_writer.py
 nnunetv2/imageio/natural_image_reader_writer.py
 nnunetv2/imageio/nibabel_reader_writer.py
 nnunetv2/imageio/reader_writer_registry.py
```

### Comparing `nnunetv2-2.3.1/nnunetv2.egg-info/entry_points.txt` & `nnunetv2-2.4/nnunetv2.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.3.1/pyproject.toml` & `nnunetv2-2.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nnunetv2"
-version = "2.3.1"
+version = "2.4"
 requires-python = ">=3.9"
 description = "nnU-Net is a framework for out-of-the box image segmentation."
 readme = "readme.md"
 license = { file = "LICENSE" }
 authors = [
     { name = "Fabian Isensee", email = "f.isensee@dkfz-heidelberg.de"},
     { name = "Helmholtz Imaging Applied Computer Vision Lab" }
@@ -26,17 +26,17 @@
     'semantic segmentation',
     'medical image analysis',
     'medical image segmentation',
     'nnU-Net',
     'nnunet'
 ]
 dependencies = [
-    "torch>=2.0.0",
+    "torch>=2.1.2",
     "acvl-utils>=0.2,<0.3",  # 0.3 may bring breaking changes. Careful!
-    "dynamic-network-architectures>=0.2,<0.4",  # 0.3.1 and lower are supported, 0.4 may have breaking changes. Let's be careful here
+    "dynamic-network-architectures>=0.3.1,<0.4",  # 0.3.1 and lower are supported, 0.4 may have breaking changes. Let's be careful here
     "tqdm",
     "dicom2nifti",
     "scipy",
     "batchgenerators>=0.25",
     "numpy",
     "scikit-learn",
     "scikit-image>=0.19.3",
@@ -82,11 +82,15 @@
 [project.optional-dependencies]
 dev = [
     "black",
     "ruff",
     "pre-commit"
 ]
 
+[build-system]
+requires = ["setuptools>=67.8.0"]
+build-backend = "setuptools.build_meta"
+
 [tool.codespell]
 skip = '.git,*.pdf,*.svg'
 #
 # ignore-words-list = ''
```

### Comparing `nnunetv2-2.3.1/readme.md` & `nnunetv2-2.4/readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 # Welcome to the new nnU-Net!
 
 Click [here](https://github.com/MIC-DKFZ/nnUNet/tree/nnunetv1) if you were looking for the old one instead.
 
 Coming from V1? Check out the [TLDR Migration Guide](documentation/tldr_migration_guide_from_v1.md). Reading the rest of the documentation is still strongly recommended ;-)
 
+## **2024-04-18 UPDATE: New residual encoder UNet presets available!**
+Residual encoder UNet presets substantially improve segmentation performance.
+They ship for a variety of GPU memory targets. It's all awesome stuff, promised! 
+Read more :point_right: [here](documentation/resenc_presets.md) :point_left:
+
+Also check out our [new paper](https://arxiv.org/pdf/2404.09556.pdf) on systematically benchmarking recent developments in medical image segmentation. You might be surprised!
+
 # What is nnU-Net?
 Image datasets are enormously diverse: image dimensionality (2D, 3D), modalities/input channels (RGB image, CT, MRI, microscopy, ...), 
 image sizes, voxel sizes, class ratio, target structure properties and more change substantially between datasets. 
 Traditionally, given a new problem, a tailored solution needs to be manually designed and optimized  - a process that 
 is prone to errors, not scalable and where success is overwhelmingly determined by the skill of the experimenter. Even 
 for experts, this process is anything but simple: there are not only many design choices and data properties that need to 
 be considered, but they are also tightly interconnected, rendering reliable manual pipeline optimization all but impossible! 
@@ -84,14 +91,15 @@
 ## How to get started?
 Read these:
 - [Installation instructions](documentation/installation_instructions.md)
 - [Dataset conversion](documentation/dataset_format.md)
 - [Usage instructions](documentation/how_to_use_nnunet.md)
 
 Additional information:
+- [Learning from sparse annotations (scribbles, slices)](documentation/ignore_label.md)
 - [Region-based training](documentation/region_based_training.md)
 - [Manual data splits](documentation/manual_data_splits.md)
 - [Pretraining and finetuning](documentation/pretraining_and_finetuning.md)
 - [Intensity Normalization in nnU-Net](documentation/explanation_normalization.md)
 - [Manually editing nnU-Net configurations](documentation/explanation_plans_files.md)
 - [Extending nnU-Net](documentation/extending_nnunet.md)
 - [What is different in V2?](documentation/changelog.md)
```

