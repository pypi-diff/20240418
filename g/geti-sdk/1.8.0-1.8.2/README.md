# Comparing `tmp/geti-sdk-1.8.0.tar.gz` & `tmp/geti-sdk-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geti-sdk-1.8.0.tar", last modified: Fri Oct 20 11:29:46 2023, max compression
+gzip compressed data, was "geti-sdk-1.8.2.tar", last modified: Mon Feb 26 08:14:10 2024, max compression
```

## Comparing `geti-sdk-1.8.0.tar` & `geti-sdk-1.8.2.tar`

### file list

```diff
@@ -1,177 +1,180 @@
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.605953 geti-sdk-1.8.0/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10174 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/LICENSE
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      178 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/MANIFEST.in
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    19019 2023-10-20 11:29:46.605953 geti-sdk-1.8.0/PKG-INFO
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16457 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/README.md
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.585953 geti-sdk-1.8.0/geti_sdk/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2231 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/__init__.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.585953 geti-sdk-1.8.0/geti_sdk/annotation_readers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1948 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/annotation_readers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4239 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/annotation_readers/base_annotation_reader.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.585953 geti-sdk-1.8.0/geti_sdk/annotation_readers/datumaro_annotation_reader/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      695 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    12680 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    11868 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10558 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/annotation_readers/directory_tree_annotation_reader.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9911 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/annotation_readers/geti_annotation_reader.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.589953 geti-sdk-1.8.0/geti_sdk/data_models/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5142 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1890 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/algorithms.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14951 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/annotation_scene.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6286 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/annotations.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2564 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/code_deployment_info.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6173 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/configurable_parameter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10440 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/configurable_parameter_group.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14304 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/configuration.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3358 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/configuration_identifiers.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.589953 geti-sdk-1.8.0/geti_sdk/data_models/containers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/containers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5250 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/containers/algorithm_list.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3608 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/containers/media_list.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.593953 geti-sdk-1.8.0/geti_sdk/data_models/enums/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1382 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/enums/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/enums/annotation_kind.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1035 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/enums/annotation_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2192 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/enums/configuration_enums.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      987 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/enums/deployment_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1587 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/enums/domain.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1735 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/enums/job_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1061 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/enums/job_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1062 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/enums/media_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1031 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/enums/model_status.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      979 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/enums/optimization_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/enums/prediction_mode.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1013 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/enums/shape_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4225 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/enums/task_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10270 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/job.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5736 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/label.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16509 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/media.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2520 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/media_identifiers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8547 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/model.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     7302 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/model_group.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2086 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/performance.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9330 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/predictions.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    12132 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/project.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    31421 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/shapes.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6635 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/status.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5705 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/task.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1019 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/task_annotation_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3082 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/test_result.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      789 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/user.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9823 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/data_models/utils.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.593953 geti-sdk-1.8.0/geti_sdk/demos/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2015 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/demos/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      909 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/demos/constants.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.585953 geti-sdk-1.8.0/geti_sdk/demos/data/
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.593953 geti-sdk-1.8.0/geti_sdk/demos/data/example/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)   724731 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/demos/data/example/dogs.png
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.593953 geti-sdk-1.8.0/geti_sdk/demos/data_helpers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      925 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/demos/data_helpers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6177 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/demos/data_helpers/anomaly_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9179 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/demos/data_helpers/coco_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5727 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/demos/data_helpers/download_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1945 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/demos/data_helpers/video_helpers.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.593953 geti-sdk-1.8.0/geti_sdk/demos/demo_projects/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1438 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/demos/demo_projects/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5247 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/demos/demo_projects/anomaly_demos.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16855 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/demos/demo_projects/coco_demos.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3058 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/demos/demo_projects/utils.py
--rwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)     7414 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/demos/predict_video.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.597953 geti-sdk-1.8.0/geti_sdk/deployment/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2684 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/deployment/__init__.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.597953 geti-sdk-1.8.0/geti_sdk/deployment/data_models/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      753 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/deployment/data_models/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4715 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/deployment/data_models/intermediate_inference_result.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2064 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/deployment/data_models/region_of_interest.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    26665 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/deployment/deployed_model.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    24438 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/deployment/deployment.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.597953 geti-sdk-1.8.0/geti_sdk/deployment/resources/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2669 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/deployment/resources/OVMS_README.md
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      653 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/deployment/resources/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3306 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/deployment/utils.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    55582 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/geti.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.597953 geti-sdk-1.8.0/geti_sdk/http_session/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2120 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/http_session/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2504 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/http_session/exception.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18822 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/http_session/geti_session.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4421 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/http_session/server_config.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6348 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/platform_versions.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.597953 geti-sdk-1.8.0/geti_sdk/rest_clients/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3723 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_clients/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2203 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_clients/active_learning_client.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.597953 geti-sdk-1.8.0/geti_sdk/rest_clients/annotation_clients/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      676 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_clients/annotation_clients/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14474 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_clients/annotation_clients/annotation_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    19255 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16462 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_clients/configuration_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4949 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_clients/dataset_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18377 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_clients/deployment_client.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.597953 geti-sdk-1.8.0/geti_sdk/rest_clients/media_client/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_clients/media_client/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8828 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_clients/media_client/image_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16826 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_clients/media_client/media_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6260 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_clients/media_client/video_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17521 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_clients/model_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    24590 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_clients/prediction_client.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.601953 geti-sdk-1.8.0/geti_sdk/rest_clients/project_client/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      667 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_clients/project_client/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    26172 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_clients/project_client/project_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2045 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_clients/project_client/task_templates.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4808 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_clients/testing_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    12260 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_clients/training_client.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.601953 geti-sdk-1.8.0/geti_sdk/rest_converters/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2163 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_converters/__init__.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.601953 geti-sdk-1.8.0/geti_sdk/rest_converters/annotation_rest_converter/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_converters/annotation_rest_converter/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6393 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6909 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10877 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_converters/configuration_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1722 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_converters/job_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1554 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_converters/media_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2411 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_converters/model_rest_converter.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.601953 geti-sdk-1.8.0/geti_sdk/rest_converters/prediction_rest_converter/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_converters/prediction_rest_converter/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3977 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3471 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2292 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_converters/project_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1400 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_converters/status_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1545 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/rest_converters/test_result_rest_converter.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.601953 geti-sdk-1.8.0/geti_sdk/utils/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1784 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/utils/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2007 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/utils/algorithm_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6398 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/utils/credentials_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1259 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/utils/dictionary_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5753 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/utils/job_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3839 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/utils/label_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6661 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/utils/plot_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1408 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/utils/project_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3455 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/utils/serialization_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1669 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/geti_sdk/utils/workspace_helpers.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.585953 geti-sdk-1.8.0/geti_sdk.egg-info/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    19019 2023-10-20 11:29:46.000000 geti-sdk-1.8.0/geti_sdk.egg-info/PKG-INFO
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5988 2023-10-20 11:29:46.000000 geti-sdk-1.8.0/geti_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)        1 2023-10-20 11:29:46.000000 geti-sdk-1.8.0/geti_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      748 2023-10-20 11:29:46.000000 geti-sdk-1.8.0/geti_sdk.egg-info/requires.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       15 2023-10-20 11:29:46.000000 geti-sdk-1.8.0/geti_sdk.egg-info/top_level.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       94 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/pyproject.toml
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.601953 geti-sdk-1.8.0/requirements/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      249 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/requirements/requirements-dev.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       98 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/requirements/requirements-docs.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      121 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/requirements/requirements-notebooks.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      404 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/requirements/requirements.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       38 2023-10-20 11:29:46.605953 geti-sdk-1.8.0/setup.cfg
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2844 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/setup.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.601953 geti-sdk-1.8.0/tests/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      581 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/tests/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8562 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/tests/conftest.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-10-20 11:29:46.605953 geti-sdk-1.8.0/tests/helpers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1351 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/tests/helpers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1002 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/tests/helpers/constants.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1709 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/tests/helpers/enums.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2326 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/tests/helpers/finalizers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2412 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/tests/helpers/fixtures.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2761 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/tests/helpers/plotting.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4417 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/tests/helpers/project_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18968 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/tests/helpers/project_service.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1866 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/tests/helpers/training.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3068 2023-10-16 11:58:54.000000 geti-sdk-1.8.0/tests/helpers/vcr_helpers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.143622 geti-sdk-1.8.2/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10174 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/LICENSE
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      178 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/MANIFEST.in
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    19043 2024-02-26 08:14:10.143622 geti-sdk-1.8.2/PKG-INFO
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16457 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/README.md
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.123623 geti-sdk-1.8.2/geti_sdk/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2231 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/__init__.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.123623 geti-sdk-1.8.2/geti_sdk/annotation_readers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1948 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/annotation_readers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4239 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/annotation_readers/base_annotation_reader.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.123623 geti-sdk-1.8.2/geti_sdk/annotation_readers/datumaro_annotation_reader/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      695 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    12680 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    11868 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10558 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/annotation_readers/directory_tree_annotation_reader.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9911 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/annotation_readers/geti_annotation_reader.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.127623 geti-sdk-1.8.2/geti_sdk/data_models/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5142 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1890 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/data_models/algorithms.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14951 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/data_models/annotation_scene.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6286 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/annotations.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2564 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/code_deployment_info.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6173 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/configurable_parameter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10440 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/data_models/configurable_parameter_group.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14304 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/configuration.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3358 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/configuration_identifiers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.127623 geti-sdk-1.8.2/geti_sdk/data_models/containers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/containers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5250 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/data_models/containers/algorithm_list.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3608 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/containers/media_list.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.127623 geti-sdk-1.8.2/geti_sdk/data_models/enums/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1382 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/enums/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/enums/annotation_kind.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1035 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/enums/annotation_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2192 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/enums/configuration_enums.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      987 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/enums/deployment_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1587 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/enums/domain.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1735 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/enums/job_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1061 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/data_models/enums/job_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1062 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/enums/media_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1031 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/enums/model_status.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      979 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/enums/optimization_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/enums/prediction_mode.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1013 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/enums/shape_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4225 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/enums/task_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10270 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/data_models/job.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5736 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/label.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16509 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/media.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2520 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/media_identifiers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8547 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/data_models/model.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     7302 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/data_models/model_group.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2086 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/performance.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9330 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/data_models/predictions.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    12132 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/project.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    31421 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/shapes.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6635 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/status.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5705 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/task.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1019 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/data_models/task_annotation_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3082 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/test_result.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      789 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/data_models/user.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9823 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/data_models/utils.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.127623 geti-sdk-1.8.2/geti_sdk/demos/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2015 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/demos/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      909 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/demos/constants.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.119623 geti-sdk-1.8.2/geti_sdk/demos/data/
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.127623 geti-sdk-1.8.2/geti_sdk/demos/data/example/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)   724731 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/demos/data/example/dogs.png
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.131623 geti-sdk-1.8.2/geti_sdk/demos/data_helpers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      925 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/demos/data_helpers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6177 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/demos/data_helpers/anomaly_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9179 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/demos/data_helpers/coco_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5727 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/demos/data_helpers/download_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1945 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/demos/data_helpers/video_helpers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.131623 geti-sdk-1.8.2/geti_sdk/demos/demo_projects/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1438 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/demos/demo_projects/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5247 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/demos/demo_projects/anomaly_demos.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16855 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/demos/demo_projects/coco_demos.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3058 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/demos/demo_projects/utils.py
+-rwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)     7414 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/demos/predict_video.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.131623 geti-sdk-1.8.2/geti_sdk/deployment/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2684 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/deployment/__init__.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.131623 geti-sdk-1.8.2/geti_sdk/deployment/data_models/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      753 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/deployment/data_models/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4715 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/deployment/data_models/intermediate_inference_result.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2064 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/deployment/data_models/region_of_interest.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    26859 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/deployment/deployed_model.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    25630 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/deployment/deployment.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.131623 geti-sdk-1.8.2/geti_sdk/deployment/legacy_converters/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      862 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/deployment/legacy_converters/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2516 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/deployment/legacy_converters/legacy_anomaly_converter.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.131623 geti-sdk-1.8.2/geti_sdk/deployment/resources/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2669 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/deployment/resources/OVMS_README.md
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      653 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/deployment/resources/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3306 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/deployment/utils.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    55582 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/geti.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.131623 geti-sdk-1.8.2/geti_sdk/http_session/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2120 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/http_session/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2504 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/http_session/exception.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18822 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/http_session/geti_session.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4421 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/http_session/server_config.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6348 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/platform_versions.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.135623 geti-sdk-1.8.2/geti_sdk/rest_clients/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3723 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/rest_clients/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2203 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/rest_clients/active_learning_client.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.135623 geti-sdk-1.8.2/geti_sdk/rest_clients/annotation_clients/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      676 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/rest_clients/annotation_clients/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14474 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/rest_clients/annotation_clients/annotation_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    19255 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16462 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/rest_clients/configuration_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4949 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/rest_clients/dataset_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18377 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/rest_clients/deployment_client.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.135623 geti-sdk-1.8.2/geti_sdk/rest_clients/media_client/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/rest_clients/media_client/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8828 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/rest_clients/media_client/image_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16826 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/rest_clients/media_client/media_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6260 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/rest_clients/media_client/video_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17521 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/rest_clients/model_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    24590 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/rest_clients/prediction_client.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.135623 geti-sdk-1.8.2/geti_sdk/rest_clients/project_client/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      667 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/rest_clients/project_client/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    26172 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/rest_clients/project_client/project_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2045 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/rest_clients/project_client/task_templates.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4808 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/rest_clients/testing_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    12260 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/rest_clients/training_client.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.135623 geti-sdk-1.8.2/geti_sdk/rest_converters/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2163 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/rest_converters/__init__.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.135623 geti-sdk-1.8.2/geti_sdk/rest_converters/annotation_rest_converter/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/rest_converters/annotation_rest_converter/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6393 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6909 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10877 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/rest_converters/configuration_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1722 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/rest_converters/job_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1554 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/rest_converters/media_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2411 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/rest_converters/model_rest_converter.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.139623 geti-sdk-1.8.2/geti_sdk/rest_converters/prediction_rest_converter/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/rest_converters/prediction_rest_converter/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3977 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3471 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2292 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/rest_converters/project_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1400 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/rest_converters/status_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1545 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/rest_converters/test_result_rest_converter.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.139623 geti-sdk-1.8.2/geti_sdk/utils/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1784 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/utils/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2007 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/utils/algorithm_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6398 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/utils/credentials_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1259 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/utils/dictionary_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5753 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/utils/job_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3839 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/utils/label_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6661 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/utils/plot_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1408 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/utils/project_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3455 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/geti_sdk/utils/serialization_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1669 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/geti_sdk/utils/workspace_helpers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.139623 geti-sdk-1.8.2/geti_sdk.egg-info/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    19043 2024-02-26 08:14:10.000000 geti-sdk-1.8.2/geti_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6104 2024-02-26 08:14:10.000000 geti-sdk-1.8.2/geti_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)        1 2024-02-26 08:14:10.000000 geti-sdk-1.8.2/geti_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      757 2024-02-26 08:14:10.000000 geti-sdk-1.8.2/geti_sdk.egg-info/requires.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       15 2024-02-26 08:14:10.000000 geti-sdk-1.8.2/geti_sdk.egg-info/top_level.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       94 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/pyproject.toml
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.139623 geti-sdk-1.8.2/requirements/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      246 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/requirements/requirements-dev.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       97 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/requirements/requirements-docs.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      117 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/requirements/requirements-notebooks.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      421 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/requirements/requirements.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       38 2024-02-26 08:14:10.143622 geti-sdk-1.8.2/setup.cfg
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2844 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/setup.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.139623 geti-sdk-1.8.2/tests/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      581 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/tests/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8562 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/tests/conftest.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2024-02-26 08:14:10.139623 geti-sdk-1.8.2/tests/helpers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1351 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/tests/helpers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1002 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/tests/helpers/constants.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1709 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/tests/helpers/enums.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2326 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/tests/helpers/finalizers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2412 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/tests/helpers/fixtures.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2761 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/tests/helpers/plotting.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4417 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/tests/helpers/project_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18968 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/tests/helpers/project_service.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1866 2024-02-26 08:13:45.000000 geti-sdk-1.8.2/tests/helpers/training.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3068 2024-02-23 00:09:15.000000 geti-sdk-1.8.2/tests/helpers/vcr_helpers.py
```

### Comparing `geti-sdk-1.8.0/LICENSE` & `geti-sdk-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/PKG-INFO` & `geti-sdk-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geti-sdk
-Version: 1.8.0
+Version: 1.8.2
 Summary: Software Development Kit for the Intel® Geti™ platform
 Home-page: https://github.com/openvinotoolkit/geti-sdk
 Author: Intel OpenVINO
 Author-email: ludo.cornelissen@intel.com
 License: Copyright (C) 2022 Intel Corporation - All Rights Reserved. Licensed under the Apache License, Version 2.0 (the 'License'). See LICENSE file for more details.
 Project-URL: Documentation, https://openvinotoolkit.github.io/geti-sdk
 Project-URL: Bug Tracker, https://github.com/openvinotoolkit/geti-sdk/issues
@@ -12,56 +12,57 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: datumaro==1.4.*
 Requires-Dist: requests==2.31.*
-Requires-Dist: numpy==1.22.*
+Requires-Dist: numpy==1.23.*
 Requires-Dist: omegaconf==2.3.*
-Requires-Dist: opencv-python==4.8.*
+Requires-Dist: opencv-python==4.9.*
 Requires-Dist: python-dotenv==1.0.*
 Requires-Dist: tqdm==4.65.*
-Requires-Dist: Pillow==9.5.*
+Requires-Dist: Pillow==10.2.*
 Requires-Dist: pathvalidate>=2.5.0
 Requires-Dist: simplejson==3.19.*
 Requires-Dist: ipython==8.12.*
-Requires-Dist: otx==1.4.*
+Requires-Dist: otx==1.4.4
 Requires-Dist: openvino==2023.0.*
 Requires-Dist: openvino-model-api==0.1.5
 Requires-Dist: certifi>=2022.12.7
 Requires-Dist: joblib>=1.1.1
 Requires-Dist: protobuf>=3.20.2
 Requires-Dist: ovmsclient>=2022.3
 Requires-Dist: orjson==3.9.2
 Requires-Dist: imageio-ffmpeg==0.4.8
 Requires-Dist: cryptography>=41.0.2
 Requires-Dist: semver>=3.0.1
+Requires-Dist: urllib3==1.26.*
 Provides-Extra: dev
-Requires-Dist: vcrpy==4.3.*; extra == "dev"
-Requires-Dist: pytest==7.3.*; extra == "dev"
+Requires-Dist: vcrpy==4.4.*; extra == "dev"
+Requires-Dist: pytest==7.4.*; extra == "dev"
 Requires-Dist: pytest-recording==0.12.*; extra == "dev"
 Requires-Dist: pytest-cov==4.1.*; extra == "dev"
-Requires-Dist: pytest-env==0.8.*; extra == "dev"
+Requires-Dist: pytest-env==1.0.*; extra == "dev"
 Requires-Dist: pytest-html==3.2.*; extra == "dev"
 Requires-Dist: flake8==6.0.*; extra == "dev"
 Requires-Dist: pydocstyle>=6.1; extra == "dev"
 Requires-Dist: black>=22.6; extra == "dev"
 Requires-Dist: isort>=5.12; extra == "dev"
-Requires-Dist: pre-commit>=2.20.0; extra == "dev"
-Requires-Dist: nbqa>=1.4.0; extra == "dev"
+Requires-Dist: pre-commit>=3.5; extra == "dev"
+Requires-Dist: nbqa>=1.7.0; extra == "dev"
 Requires-Dist: pytest-mock>=3.10.0; extra == "dev"
 Provides-Extra: docs
-Requires-Dist: sphinx>=4.5; extra == "docs"
-Requires-Dist: sphinx-rtd-theme>=1.0; extra == "docs"
-Requires-Dist: myst-parser>=0.18; extra == "docs"
+Requires-Dist: sphinx>=7.2; extra == "docs"
+Requires-Dist: sphinx-rtd-theme>=1.3; extra == "docs"
+Requires-Dist: myst-parser>=2.0; extra == "docs"
 Provides-Extra: notebooks
-Requires-Dist: jupyterlab>=3.5.3; extra == "notebooks"
+Requires-Dist: jupyterlab>=4.0; extra == "notebooks"
 Requires-Dist: jupyter-core>=4.11.2; extra == "notebooks"
-Requires-Dist: ipywidgets>=8.0.0; extra == "notebooks"
+Requires-Dist: ipywidgets>=8.1; extra == "notebooks"
 Requires-Dist: mistune>=2.0.3; extra == "notebooks"
 
 # Introduction
 
 Welcome to the Intel® Geti™ SDK! The [Intel® Geti™ platform](https://geti.intel.com) enables
 teams to rapidly develop AI models. The platform reduces the time needed to build
 models by easing the complexities of model development and harnessing greater
```

### Comparing `geti-sdk-1.8.0/README.md` & `geti-sdk-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/__init__.py` & `geti-sdk-1.8.2/geti_sdk/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,10 +74,10 @@
 
    .. automethod:: upload_and_predict_media_folder
 
 """
 
 from .geti import Geti
 
-__version__ = "1.8.0"
+__version__ = "1.8.2"
 
 __all__ = ["Geti"]
```

### Comparing `geti-sdk-1.8.0/geti_sdk/annotation_readers/__init__.py` & `geti-sdk-1.8.2/geti_sdk/annotation_readers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/annotation_readers/base_annotation_reader.py` & `geti-sdk-1.8.2/geti_sdk/annotation_readers/base_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py` & `geti-sdk-1.8.2/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py` & `geti-sdk-1.8.2/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py` & `geti-sdk-1.8.2/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/annotation_readers/directory_tree_annotation_reader.py` & `geti-sdk-1.8.2/geti_sdk/annotation_readers/directory_tree_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/annotation_readers/geti_annotation_reader.py` & `geti-sdk-1.8.2/geti_sdk/annotation_readers/geti_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/__init__.py` & `geti-sdk-1.8.2/geti_sdk/data_models/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/algorithms.py` & `geti-sdk-1.8.2/geti_sdk/data_models/algorithms.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/annotation_scene.py` & `geti-sdk-1.8.2/geti_sdk/data_models/annotation_scene.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/annotations.py` & `geti-sdk-1.8.2/geti_sdk/data_models/annotations.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/code_deployment_info.py` & `geti-sdk-1.8.2/geti_sdk/data_models/code_deployment_info.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/configurable_parameter.py` & `geti-sdk-1.8.2/geti_sdk/data_models/configurable_parameter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/configurable_parameter_group.py` & `geti-sdk-1.8.2/geti_sdk/data_models/configurable_parameter_group.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/configuration.py` & `geti-sdk-1.8.2/geti_sdk/data_models/configuration.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/configuration_identifiers.py` & `geti-sdk-1.8.2/geti_sdk/data_models/configuration_identifiers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/containers/__init__.py` & `geti-sdk-1.8.2/geti_sdk/data_models/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/containers/algorithm_list.py` & `geti-sdk-1.8.2/geti_sdk/data_models/containers/algorithm_list.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/containers/media_list.py` & `geti-sdk-1.8.2/geti_sdk/data_models/containers/media_list.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/enums/__init__.py` & `geti-sdk-1.8.2/geti_sdk/data_models/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/enums/annotation_kind.py` & `geti-sdk-1.8.2/geti_sdk/data_models/enums/annotation_kind.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/enums/annotation_state.py` & `geti-sdk-1.8.2/geti_sdk/data_models/enums/annotation_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/enums/configuration_enums.py` & `geti-sdk-1.8.2/geti_sdk/data_models/enums/configuration_enums.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/enums/deployment_state.py` & `geti-sdk-1.8.2/geti_sdk/data_models/enums/deployment_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/enums/domain.py` & `geti-sdk-1.8.2/geti_sdk/data_models/enums/domain.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/enums/job_state.py` & `geti-sdk-1.8.2/geti_sdk/data_models/enums/job_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/enums/job_type.py` & `geti-sdk-1.8.2/geti_sdk/data_models/enums/job_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/enums/media_type.py` & `geti-sdk-1.8.2/geti_sdk/data_models/enums/media_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/enums/model_status.py` & `geti-sdk-1.8.2/geti_sdk/data_models/enums/model_status.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/enums/optimization_type.py` & `geti-sdk-1.8.2/geti_sdk/data_models/enums/optimization_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/enums/prediction_mode.py` & `geti-sdk-1.8.2/geti_sdk/data_models/enums/prediction_mode.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/enums/shape_type.py` & `geti-sdk-1.8.2/geti_sdk/data_models/enums/shape_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/enums/task_type.py` & `geti-sdk-1.8.2/geti_sdk/data_models/enums/task_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/job.py` & `geti-sdk-1.8.2/geti_sdk/data_models/job.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/label.py` & `geti-sdk-1.8.2/geti_sdk/data_models/label.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/media.py` & `geti-sdk-1.8.2/geti_sdk/data_models/media.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/media_identifiers.py` & `geti-sdk-1.8.2/geti_sdk/data_models/media_identifiers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/model.py` & `geti-sdk-1.8.2/geti_sdk/data_models/model.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/model_group.py` & `geti-sdk-1.8.2/geti_sdk/data_models/model_group.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/performance.py` & `geti-sdk-1.8.2/geti_sdk/data_models/performance.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/predictions.py` & `geti-sdk-1.8.2/geti_sdk/data_models/predictions.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/project.py` & `geti-sdk-1.8.2/geti_sdk/data_models/project.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/shapes.py` & `geti-sdk-1.8.2/geti_sdk/data_models/shapes.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/status.py` & `geti-sdk-1.8.2/geti_sdk/data_models/status.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/task.py` & `geti-sdk-1.8.2/geti_sdk/data_models/task.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/task_annotation_state.py` & `geti-sdk-1.8.2/geti_sdk/data_models/task_annotation_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/test_result.py` & `geti-sdk-1.8.2/geti_sdk/data_models/test_result.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/user.py` & `geti-sdk-1.8.2/geti_sdk/data_models/user.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/data_models/utils.py` & `geti-sdk-1.8.2/geti_sdk/data_models/utils.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/demos/__init__.py` & `geti-sdk-1.8.2/geti_sdk/demos/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/demos/constants.py` & `geti-sdk-1.8.2/geti_sdk/demos/constants.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/demos/data/example/dogs.png` & `geti-sdk-1.8.2/geti_sdk/demos/data/example/dogs.png`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/demos/data_helpers/__init__.py` & `geti-sdk-1.8.2/geti_sdk/demos/data_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/demos/data_helpers/anomaly_helpers.py` & `geti-sdk-1.8.2/geti_sdk/demos/data_helpers/anomaly_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/demos/data_helpers/coco_helpers.py` & `geti-sdk-1.8.2/geti_sdk/demos/data_helpers/coco_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/demos/data_helpers/download_helpers.py` & `geti-sdk-1.8.2/geti_sdk/demos/data_helpers/download_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/demos/data_helpers/video_helpers.py` & `geti-sdk-1.8.2/geti_sdk/demos/data_helpers/video_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/demos/demo_projects/__init__.py` & `geti-sdk-1.8.2/geti_sdk/demos/demo_projects/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/demos/demo_projects/anomaly_demos.py` & `geti-sdk-1.8.2/geti_sdk/demos/demo_projects/anomaly_demos.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/demos/demo_projects/coco_demos.py` & `geti-sdk-1.8.2/geti_sdk/demos/demo_projects/coco_demos.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/demos/demo_projects/utils.py` & `geti-sdk-1.8.2/geti_sdk/demos/demo_projects/utils.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/demos/predict_video.py` & `geti-sdk-1.8.2/geti_sdk/demos/predict_video.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/deployment/__init__.py` & `geti-sdk-1.8.2/geti_sdk/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/deployment/data_models/__init__.py` & `geti-sdk-1.8.2/geti_sdk/deployment/data_models/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/deployment/data_models/intermediate_inference_result.py` & `geti-sdk-1.8.2/geti_sdk/deployment/data_models/intermediate_inference_result.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/deployment/data_models/region_of_interest.py` & `geti-sdk-1.8.2/geti_sdk/deployment/data_models/region_of_interest.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/deployment/deployed_model.py` & `geti-sdk-1.8.2/geti_sdk/deployment/deployed_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,18 +160,23 @@
                     )
                 if PYTHON_DIR_NAME in source_contents:
                     model_python_path = os.path.join(source, PYTHON_DIR_NAME)
                 else:
                     model_python_path = os.path.join(
                         os.path.dirname(source), PYTHON_DIR_NAME
                     )
-                python_dir_contents = os.listdir(model_python_path)
+                python_dir_contents = (
+                    os.listdir(model_python_path)
+                    if os.path.exists(model_python_path)
+                    else []
+                )
                 if WRAPPER_DIR_NAME in python_dir_contents:
                     self._has_custom_model_wrappers = True
-                    self._model_python_path = os.path.join(source, PYTHON_DIR_NAME)
+
+                self._model_python_path = os.path.join(source, PYTHON_DIR_NAME)
 
         elif isinstance(source, GetiSession):
             if self.base_url is None:
                 raise ValueError(
                     f"Insufficient data to retrieve data for model {self}. Please set "
                     f"a base_url for the model first."
                 )
@@ -407,22 +412,23 @@
             return False
 
         shutil.copytree(
             src=self._model_data_path,
             dst=new_model_data_path,
             dirs_exist_ok=True,
         )
-        shutil.copytree(
-            src=self._model_python_path,
-            dst=new_model_python_path,
-            dirs_exist_ok=True,
-        )
+        if self._model_python_path is not None:
+            shutil.copytree(
+                src=self._model_python_path,
+                dst=new_model_python_path,
+                dirs_exist_ok=True,
+            )
+            self._model_python_path = new_model_python_path
 
         self._model_data_path = new_model_data_path
-        self._model_python_path = new_model_python_path
 
         config_dict = ConfigurationRESTConverter.configuration_to_minimal_dict(
             self.hyper_parameters
         )
         config_filepath = os.path.join(path_to_folder, "hyper_parameters.json")
         with open(config_filepath, "w") as config_file:
             json.dump(config_dict, config_file, indent=4)
```

### Comparing `geti-sdk-1.8.0/geti_sdk/deployment/deployment.py` & `geti-sdk-1.8.2/geti_sdk/deployment/deployment.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,17 @@
     ScoredLabel,
     Task,
     TaskType,
 )
 from geti_sdk.data_models.predictions import ResultMedium
 from geti_sdk.data_models.shapes import Polygon, Rectangle, RotatedRectangle
 from geti_sdk.deployment.data_models import ROI, IntermediateInferenceResult
+from geti_sdk.deployment.legacy_converters import (
+    AnomalyClassificationToAnnotationConverter,
+)
 from geti_sdk.rest_converters import ProjectRESTConverter
 
 from .deployed_model import DeployedModel
 from .utils import OVMS_README_PATH, generate_ovms_model_name
 
 
 @attr.define(slots=False)
@@ -321,17 +324,29 @@
             else:
                 raise ValueError(
                     f"Unknown postprocessing output of type "
                     f"`{type(postprocessing_results)}` for task `{task.title}`."
                 )
 
         if n_outputs != 0:
-            annotation_scene_entity = converter.convert_to_annotation(
-                predictions=postprocessing_results, metadata=metadata
-            )
+            try:
+                annotation_scene_entity = converter.convert_to_annotation(
+                    predictions=postprocessing_results, metadata=metadata
+                )
+            except AttributeError:
+                # Add backwards compatibility for anomaly models created in Geti v1.8 and below
+                if task.type.is_anomaly:
+                    legacy_converter = AnomalyClassificationToAnnotationConverter(
+                        label_schema=model.ote_label_schema
+                    )
+                    annotation_scene_entity = legacy_converter.convert_to_annotation(
+                        predictions=postprocessing_results, metadata=metadata
+                    )
+                    self._inference_converters[task.type] = legacy_converter
+
             prediction = Prediction.from_ote(
                 annotation_scene_entity, image_width=width, image_height=height
             )
         else:
             prediction = Prediction(annotations=[])
 
         # Empty label is not generated by OTE correctly, append it here if there are
@@ -459,28 +474,40 @@
         except ValueError as error:
             raise ValueError(
                 f"Task {task.title} is not in the list of trainable tasks for project "
                 f"{self.project.name}."
             ) from error
         return self.models[task_index]
 
-    def _remove_temporary_resources(self) -> None:
+    def _remove_temporary_resources(self) -> bool:
         """
         If necessary, clean up any temporary resources associated with the deployment.
+
+        :return: True if temp files have been deleted successfully
         """
         if self._path_to_temp_resources is not None and os.path.isdir(
             self._path_to_temp_resources
         ):
-            shutil.rmtree(self._path_to_temp_resources)
+            try:
+                shutil.rmtree(self._path_to_temp_resources)
+            except PermissionError:
+                logging.warning(
+                    f"Unable to remove temporary files for deployment at path "
+                    f"`{self._path_to_temp_resources}` because the files are in "
+                    f"use by another process. "
+                )
+                return False
         else:
             logging.debug(
                 f"Unable to clean up temporary resources for deployment {self}, "
                 f"because the resources were not found on the system. Possibly "
                 f"they were already deleted."
             )
+            return False
+        return True
 
     def __del__(self):
         """
         If necessary, clean up any temporary resources associated with the deployment.
         This method is called when the Deployment instance is deleted.
         """
         if self._requires_resource_cleanup:
```

### Comparing `geti-sdk-1.8.0/geti_sdk/deployment/resources/OVMS_README.md` & `geti-sdk-1.8.2/geti_sdk/deployment/resources/OVMS_README.md`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/deployment/resources/__init__.py` & `geti-sdk-1.8.2/geti_sdk/deployment/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/deployment/utils.py` & `geti-sdk-1.8.2/geti_sdk/deployment/utils.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/geti.py` & `geti-sdk-1.8.2/geti_sdk/geti.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/http_session/__init__.py` & `geti-sdk-1.8.2/geti_sdk/http_session/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/http_session/exception.py` & `geti-sdk-1.8.2/geti_sdk/http_session/exception.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/http_session/geti_session.py` & `geti-sdk-1.8.2/geti_sdk/http_session/geti_session.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/http_session/server_config.py` & `geti-sdk-1.8.2/geti_sdk/http_session/server_config.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/platform_versions.py` & `geti-sdk-1.8.2/geti_sdk/platform_versions.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_clients/__init__.py` & `geti-sdk-1.8.2/geti_sdk/rest_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_clients/active_learning_client.py` & `geti-sdk-1.8.2/geti_sdk/rest_clients/active_learning_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_clients/annotation_clients/__init__.py` & `geti-sdk-1.8.2/geti_sdk/rest_clients/annotation_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_clients/annotation_clients/annotation_client.py` & `geti-sdk-1.8.2/geti_sdk/rest_clients/annotation_clients/annotation_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py` & `geti-sdk-1.8.2/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_clients/configuration_client.py` & `geti-sdk-1.8.2/geti_sdk/rest_clients/configuration_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_clients/dataset_client.py` & `geti-sdk-1.8.2/geti_sdk/rest_clients/dataset_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_clients/deployment_client.py` & `geti-sdk-1.8.2/geti_sdk/rest_clients/deployment_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_clients/media_client/__init__.py` & `geti-sdk-1.8.2/geti_sdk/rest_clients/media_client/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_clients/media_client/image_client.py` & `geti-sdk-1.8.2/geti_sdk/rest_clients/media_client/image_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_clients/media_client/media_client.py` & `geti-sdk-1.8.2/geti_sdk/rest_clients/media_client/media_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_clients/media_client/video_client.py` & `geti-sdk-1.8.2/geti_sdk/rest_clients/media_client/video_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_clients/model_client.py` & `geti-sdk-1.8.2/geti_sdk/rest_clients/model_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_clients/prediction_client.py` & `geti-sdk-1.8.2/geti_sdk/rest_clients/prediction_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_clients/project_client/__init__.py` & `geti-sdk-1.8.2/geti_sdk/rest_clients/project_client/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_clients/project_client/project_client.py` & `geti-sdk-1.8.2/geti_sdk/rest_clients/project_client/project_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_clients/project_client/task_templates.py` & `geti-sdk-1.8.2/geti_sdk/rest_clients/project_client/task_templates.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_clients/testing_client.py` & `geti-sdk-1.8.2/geti_sdk/rest_clients/testing_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_clients/training_client.py` & `geti-sdk-1.8.2/geti_sdk/rest_clients/training_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_converters/__init__.py` & `geti-sdk-1.8.2/geti_sdk/rest_converters/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_converters/annotation_rest_converter/__init__.py` & `geti-sdk-1.8.2/geti_sdk/rest_converters/annotation_rest_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py` & `geti-sdk-1.8.2/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py` & `geti-sdk-1.8.2/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_converters/configuration_rest_converter.py` & `geti-sdk-1.8.2/geti_sdk/rest_converters/configuration_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_converters/job_rest_converter.py` & `geti-sdk-1.8.2/geti_sdk/rest_converters/job_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_converters/media_rest_converter.py` & `geti-sdk-1.8.2/geti_sdk/rest_converters/media_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_converters/model_rest_converter.py` & `geti-sdk-1.8.2/geti_sdk/rest_converters/model_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_converters/prediction_rest_converter/__init__.py` & `geti-sdk-1.8.2/geti_sdk/rest_converters/prediction_rest_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py` & `geti-sdk-1.8.2/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py` & `geti-sdk-1.8.2/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_converters/project_rest_converter.py` & `geti-sdk-1.8.2/geti_sdk/rest_converters/project_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_converters/status_rest_converter.py` & `geti-sdk-1.8.2/geti_sdk/rest_converters/status_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/rest_converters/test_result_rest_converter.py` & `geti-sdk-1.8.2/geti_sdk/rest_converters/test_result_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/utils/__init__.py` & `geti-sdk-1.8.2/geti_sdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/utils/algorithm_helpers.py` & `geti-sdk-1.8.2/geti_sdk/utils/algorithm_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/utils/credentials_helpers.py` & `geti-sdk-1.8.2/geti_sdk/utils/credentials_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/utils/dictionary_helpers.py` & `geti-sdk-1.8.2/geti_sdk/utils/dictionary_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/utils/job_helpers.py` & `geti-sdk-1.8.2/geti_sdk/utils/job_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/utils/label_helpers.py` & `geti-sdk-1.8.2/geti_sdk/utils/label_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/utils/plot_helpers.py` & `geti-sdk-1.8.2/geti_sdk/utils/plot_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/utils/project_helpers.py` & `geti-sdk-1.8.2/geti_sdk/utils/project_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/utils/serialization_helpers.py` & `geti-sdk-1.8.2/geti_sdk/utils/serialization_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk/utils/workspace_helpers.py` & `geti-sdk-1.8.2/geti_sdk/utils/workspace_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/geti_sdk.egg-info/PKG-INFO` & `geti-sdk-1.8.2/geti_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geti-sdk
-Version: 1.8.0
+Version: 1.8.2
 Summary: Software Development Kit for the Intel® Geti™ platform
 Home-page: https://github.com/openvinotoolkit/geti-sdk
 Author: Intel OpenVINO
 Author-email: ludo.cornelissen@intel.com
 License: Copyright (C) 2022 Intel Corporation - All Rights Reserved. Licensed under the Apache License, Version 2.0 (the 'License'). See LICENSE file for more details.
 Project-URL: Documentation, https://openvinotoolkit.github.io/geti-sdk
 Project-URL: Bug Tracker, https://github.com/openvinotoolkit/geti-sdk/issues
@@ -12,56 +12,57 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: datumaro==1.4.*
 Requires-Dist: requests==2.31.*
-Requires-Dist: numpy==1.22.*
+Requires-Dist: numpy==1.23.*
 Requires-Dist: omegaconf==2.3.*
-Requires-Dist: opencv-python==4.8.*
+Requires-Dist: opencv-python==4.9.*
 Requires-Dist: python-dotenv==1.0.*
 Requires-Dist: tqdm==4.65.*
-Requires-Dist: Pillow==9.5.*
+Requires-Dist: Pillow==10.2.*
 Requires-Dist: pathvalidate>=2.5.0
 Requires-Dist: simplejson==3.19.*
 Requires-Dist: ipython==8.12.*
-Requires-Dist: otx==1.4.*
+Requires-Dist: otx==1.4.4
 Requires-Dist: openvino==2023.0.*
 Requires-Dist: openvino-model-api==0.1.5
 Requires-Dist: certifi>=2022.12.7
 Requires-Dist: joblib>=1.1.1
 Requires-Dist: protobuf>=3.20.2
 Requires-Dist: ovmsclient>=2022.3
 Requires-Dist: orjson==3.9.2
 Requires-Dist: imageio-ffmpeg==0.4.8
 Requires-Dist: cryptography>=41.0.2
 Requires-Dist: semver>=3.0.1
+Requires-Dist: urllib3==1.26.*
 Provides-Extra: dev
-Requires-Dist: vcrpy==4.3.*; extra == "dev"
-Requires-Dist: pytest==7.3.*; extra == "dev"
+Requires-Dist: vcrpy==4.4.*; extra == "dev"
+Requires-Dist: pytest==7.4.*; extra == "dev"
 Requires-Dist: pytest-recording==0.12.*; extra == "dev"
 Requires-Dist: pytest-cov==4.1.*; extra == "dev"
-Requires-Dist: pytest-env==0.8.*; extra == "dev"
+Requires-Dist: pytest-env==1.0.*; extra == "dev"
 Requires-Dist: pytest-html==3.2.*; extra == "dev"
 Requires-Dist: flake8==6.0.*; extra == "dev"
 Requires-Dist: pydocstyle>=6.1; extra == "dev"
 Requires-Dist: black>=22.6; extra == "dev"
 Requires-Dist: isort>=5.12; extra == "dev"
-Requires-Dist: pre-commit>=2.20.0; extra == "dev"
-Requires-Dist: nbqa>=1.4.0; extra == "dev"
+Requires-Dist: pre-commit>=3.5; extra == "dev"
+Requires-Dist: nbqa>=1.7.0; extra == "dev"
 Requires-Dist: pytest-mock>=3.10.0; extra == "dev"
 Provides-Extra: docs
-Requires-Dist: sphinx>=4.5; extra == "docs"
-Requires-Dist: sphinx-rtd-theme>=1.0; extra == "docs"
-Requires-Dist: myst-parser>=0.18; extra == "docs"
+Requires-Dist: sphinx>=7.2; extra == "docs"
+Requires-Dist: sphinx-rtd-theme>=1.3; extra == "docs"
+Requires-Dist: myst-parser>=2.0; extra == "docs"
 Provides-Extra: notebooks
-Requires-Dist: jupyterlab>=3.5.3; extra == "notebooks"
+Requires-Dist: jupyterlab>=4.0; extra == "notebooks"
 Requires-Dist: jupyter-core>=4.11.2; extra == "notebooks"
-Requires-Dist: ipywidgets>=8.0.0; extra == "notebooks"
+Requires-Dist: ipywidgets>=8.1; extra == "notebooks"
 Requires-Dist: mistune>=2.0.3; extra == "notebooks"
 
 # Introduction
 
 Welcome to the Intel® Geti™ SDK! The [Intel® Geti™ platform](https://geti.intel.com) enables
 teams to rapidly develop AI models. The platform reduces the time needed to build
 models by easing the complexities of model development and harnessing greater
```

### Comparing `geti-sdk-1.8.0/geti_sdk.egg-info/SOURCES.txt` & `geti-sdk-1.8.2/geti_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,16 @@
 geti_sdk/deployment/__init__.py
 geti_sdk/deployment/deployed_model.py
 geti_sdk/deployment/deployment.py
 geti_sdk/deployment/utils.py
 geti_sdk/deployment/data_models/__init__.py
 geti_sdk/deployment/data_models/intermediate_inference_result.py
 geti_sdk/deployment/data_models/region_of_interest.py
+geti_sdk/deployment/legacy_converters/__init__.py
+geti_sdk/deployment/legacy_converters/legacy_anomaly_converter.py
 geti_sdk/deployment/resources/OVMS_README.md
 geti_sdk/deployment/resources/__init__.py
 geti_sdk/http_session/__init__.py
 geti_sdk/http_session/exception.py
 geti_sdk/http_session/geti_session.py
 geti_sdk/http_session/server_config.py
 geti_sdk/rest_clients/__init__.py
```

### Comparing `geti-sdk-1.8.0/geti_sdk.egg-info/requires.txt` & `geti-sdk-1.8.2/geti_sdk.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 datumaro==1.4.*
 requests==2.31.*
-numpy==1.22.*
+numpy==1.23.*
 omegaconf==2.3.*
-opencv-python==4.8.*
+opencv-python==4.9.*
 python-dotenv==1.0.*
 tqdm==4.65.*
-Pillow==9.5.*
+Pillow==10.2.*
 pathvalidate>=2.5.0
 simplejson==3.19.*
 ipython==8.12.*
-otx==1.4.*
+otx==1.4.4
 openvino==2023.0.*
 openvino-model-api==0.1.5
 certifi>=2022.12.7
 joblib>=1.1.1
 protobuf>=3.20.2
 ovmsclient>=2022.3
 orjson==3.9.2
 imageio-ffmpeg==0.4.8
 cryptography>=41.0.2
 semver>=3.0.1
+urllib3==1.26.*
 
 [dev]
-vcrpy==4.3.*
-pytest==7.3.*
+vcrpy==4.4.*
+pytest==7.4.*
 pytest-recording==0.12.*
 pytest-cov==4.1.*
-pytest-env==0.8.*
+pytest-env==1.0.*
 pytest-html==3.2.*
 flake8==6.0.*
 pydocstyle>=6.1
 black>=22.6
 isort>=5.12
-pre-commit>=2.20.0
-nbqa>=1.4.0
+pre-commit>=3.5
+nbqa>=1.7.0
 pytest-mock>=3.10.0
 
 [docs]
-sphinx>=4.5
-sphinx-rtd-theme>=1.0
-myst-parser>=0.18
+sphinx>=7.2
+sphinx-rtd-theme>=1.3
+myst-parser>=2.0
 
 [notebooks]
-jupyterlab>=3.5.3
+jupyterlab>=4.0
 jupyter-core>=4.11.2
-ipywidgets>=8.0.0
+ipywidgets>=8.1
 mistune>=2.0.3
```

### Comparing `geti-sdk-1.8.0/setup.py` & `geti-sdk-1.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/tests/__init__.py` & `geti-sdk-1.8.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/tests/conftest.py` & `geti-sdk-1.8.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/tests/helpers/__init__.py` & `geti-sdk-1.8.2/tests/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/tests/helpers/constants.py` & `geti-sdk-1.8.2/tests/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/tests/helpers/enums.py` & `geti-sdk-1.8.2/tests/helpers/enums.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/tests/helpers/finalizers.py` & `geti-sdk-1.8.2/tests/helpers/finalizers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/tests/helpers/fixtures.py` & `geti-sdk-1.8.2/tests/helpers/fixtures.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/tests/helpers/plotting.py` & `geti-sdk-1.8.2/tests/helpers/plotting.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/tests/helpers/project_helpers.py` & `geti-sdk-1.8.2/tests/helpers/project_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/tests/helpers/project_service.py` & `geti-sdk-1.8.2/tests/helpers/project_service.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/tests/helpers/training.py` & `geti-sdk-1.8.2/tests/helpers/training.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.8.0/tests/helpers/vcr_helpers.py` & `geti-sdk-1.8.2/tests/helpers/vcr_helpers.py`

 * *Files identical despite different names*

