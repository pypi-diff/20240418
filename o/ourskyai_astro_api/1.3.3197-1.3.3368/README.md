# Comparing `tmp/ourskyai_astro_api-1.3.3197.tar.gz` & `tmp/ourskyai_astro_api-1.3.3368.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourskyai_astro_api-1.3.3197.tar", max compression
+gzip compressed data, was "ourskyai_astro_api-1.3.3368.tar", max compression
```

## Comparing `ourskyai_astro_api-1.3.3197.tar` & `ourskyai_astro_api-1.3.3368.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0    11057 2024-03-30 00:36:07.502062 ourskyai_astro_api-1.3.3197/README.md
--rw-r--r--   0        0        0     5741 2024-03-30 00:36:11.086131 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/__init__.py
--rw-r--r--   0        0        0      106 2024-03-30 00:36:11.114132 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/api/__init__.py
--rw-r--r--   0        0        0   253842 2024-03-30 00:36:11.214134 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/api/default_api.py
--rw-r--r--   0        0        0    30352 2024-03-30 00:36:11.246134 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/api_client.py
--rw-r--r--   0        0        0      852 2024-03-30 00:36:11.290135 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/api_response.py
--rw-r--r--   0        0        0    14687 2024-03-30 00:36:11.354136 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/configuration.py
--rw-r--r--   0        0        0     5433 2024-03-30 00:36:11.442138 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/exceptions.py
--rw-r--r--   0        0        0     5100 2024-03-30 00:36:11.490139 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/__init__.py
--rw-r--r--   0        0        0      819 2024-03-30 00:36:11.530140 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/asset_file_type.py
--rw-r--r--   0        0        0      931 2024-03-30 00:36:11.594141 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/asset_type.py
--rw-r--r--   0        0        0      809 2024-03-30 00:36:11.654142 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/calibration_master_type.py
--rw-r--r--   0        0        0     1904 2024-03-30 00:36:11.706143 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/empty_success.py
--rw-r--r--   0        0        0     1186 2024-03-30 00:36:11.754144 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/filter_type.py
--rw-r--r--   0        0        0     2155 2024-03-30 00:36:11.810145 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/location.py
--rw-r--r--   0        0        0      747 2024-03-30 00:36:11.858146 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/mount_type.py
--rw-r--r--   0        0        0      887 2024-03-30 00:36:12.042150 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/node_state.py
--rw-r--r--   0        0        0      827 2024-03-30 00:36:12.102151 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/optical_tube_type.py
--rw-r--r--   0        0        0      751 2024-03-30 00:36:12.138152 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/shutter_type.py
--rw-r--r--   0        0        0     1892 2024-03-30 00:36:12.206153 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/successful_create.py
--rw-r--r--   0        0        0      768 2024-03-30 00:36:12.274154 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/tracking_type.py
--rw-r--r--   0        0        0     2985 2024-03-30 00:36:12.318155 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_astro_project.py
--rw-r--r--   0        0        0     3969 2024-03-30 00:36:12.370156 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_astro_project_asset.py
--rw-r--r--   0        0        0     2569 2024-03-30 00:36:12.418157 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py
--rw-r--r--   0        0        0     2399 2024-03-30 00:36:12.482158 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py
--rw-r--r--   0        0        0     2381 2024-03-30 00:36:12.530159 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_astro_target.py
--rw-r--r--   0        0        0     3640 2024-03-30 00:36:12.562160 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_calibration_master.py
--rw-r--r--   0        0        0     4908 2024-03-30 00:36:12.602161 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_camera.py
--rw-r--r--   0        0        0     2421 2024-03-30 00:36:12.646161 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py
--rw-r--r--   0        0        0     2668 2024-03-30 00:36:12.694162 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_create_astro_project_request.py
--rw-r--r--   0        0        0     2121 2024-03-30 00:36:12.762163 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_create_astro_project_response.py
--rw-r--r--   0        0        0     3777 2024-03-30 00:36:12.846165 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_create_calibration_master_request.py
--rw-r--r--   0        0        0     2147 2024-03-30 00:36:12.922167 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_create_calibration_master_response.py
--rw-r--r--   0        0        0     7059 2024-03-30 00:36:12.990168 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_create_camera_request.py
--rw-r--r--   0        0        0     2044 2024-03-30 00:36:13.122171 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_create_image_set_image_request.py
--rw-r--r--   0        0        0     2115 2024-03-30 00:36:13.162171 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_create_image_set_image_response.py
--rw-r--r--   0        0        0     2683 2024-03-30 00:36:13.214172 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_create_image_set_request.py
--rw-r--r--   0        0        0     2296 2024-03-30 00:36:13.262173 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_create_mount_request.py
--rw-r--r--   0        0        0     3146 2024-03-30 00:36:13.314174 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_create_node_request.py
--rw-r--r--   0        0        0     2447 2024-03-30 00:36:13.362175 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_create_optical_tube_request.py
--rw-r--r--   0        0        0     2441 2024-03-30 00:36:13.406176 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_elevation_mask_point.py
--rw-r--r--   0        0        0     3289 2024-03-30 00:36:13.450177 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_gain_curve.py
--rw-r--r--   0        0        0     2051 2024-03-30 00:36:13.494178 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_gain_curve_point.py
--rw-r--r--   0        0        0     2096 2024-03-30 00:36:13.586180 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py
--rw-r--r--   0        0        0     2364 2024-03-30 00:36:13.654181 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_get_nodes.py
--rw-r--r--   0        0        0     7066 2024-03-30 00:36:13.702182 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_get_or_create_camera_request.py
--rw-r--r--   0        0        0     2324 2024-03-30 00:36:13.766183 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_get_or_create_mount_request.py
--rw-r--r--   0        0        0     2513 2024-03-30 00:36:13.818184 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py
--rw-r--r--   0        0        0     3436 2024-03-30 00:36:13.878185 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_image_set.py
--rw-r--r--   0        0        0     5167 2024-03-30 00:36:13.982187 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_image_set_image.py
--rw-r--r--   0        0        0      795 2024-03-30 00:36:14.034188 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_job_kind.py
--rw-r--r--   0        0        0     2632 2024-03-30 00:36:14.122190 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_job_log.py
--rw-r--r--   0        0        0      803 2024-03-30 00:36:14.178191 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_job_status.py
--rw-r--r--   0        0        0     1914 2024-03-30 00:36:14.230192 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_mount.py
--rw-r--r--   0        0        0     4458 2024-03-30 00:36:14.274193 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_node.py
--rw-r--r--   0        0        0     2564 2024-03-30 00:36:14.322194 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_node_with_location.py
--rw-r--r--   0        0        0     2239 2024-03-30 00:36:14.366195 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_optical_tube.py
--rw-r--r--   0        0        0     3057 2024-03-30 00:36:14.414196 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_platform_credit.py
--rw-r--r--   0        0        0      870 2024-03-30 00:36:14.466197 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_platform_credit_source.py
--rw-r--r--   0        0        0      800 2024-03-30 00:36:14.542198 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_platform_credit_type.py
--rw-r--r--   0        0        0      776 2024-03-30 00:36:14.586199 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_platform_credit_unit.py
--rw-r--r--   0        0        0     2045 2024-03-30 00:36:14.646200 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py
--rw-r--r--   0        0        0     2051 2024-03-30 00:36:14.694201 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_read_noise_point.py
--rw-r--r--   0        0        0     2050 2024-03-30 00:36:14.742202 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_setup_action.py
--rw-r--r--   0        0        0     2940 2024-03-30 00:36:14.794203 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_slew_timing.py
--rw-r--r--   0        0        0     2240 2024-03-30 00:36:14.862204 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_slew_timing_interval.py
--rw-r--r--   0        0        0     4605 2024-03-30 00:36:14.922205 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_update_node_request.py
--rw-r--r--   0        0        0     2522 2024-03-30 00:36:15.030207 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_video_mode_framerate_property.py
--rw-r--r--   0        0        0        0 2024-03-30 00:36:15.062208 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/py.typed
--rw-r--r--   0        0        0    12935 2024-03-30 00:36:15.114209 ourskyai_astro_api-1.3.3197/ourskyai_astro_api/rest.py
--rw-r--r--   0        0        0      739 2024-03-30 00:36:15.186210 ourskyai_astro_api-1.3.3197/pyproject.toml
--rw-r--r--   0        0        0    12025 1970-01-01 00:00:00.000000 ourskyai_astro_api-1.3.3197/PKG-INFO
+-rw-r--r--   0        0        0    11057 2024-04-18 04:36:56.128272 ourskyai_astro_api-1.3.3368/README.md
+-rw-r--r--   0        0        0     5741 2024-04-18 04:36:59.984380 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/__init__.py
+-rw-r--r--   0        0        0      106 2024-04-18 04:37:00.024381 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/api/__init__.py
+-rw-r--r--   0        0        0   253842 2024-04-18 04:37:00.136384 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/api/default_api.py
+-rw-r--r--   0        0        0    30352 2024-04-18 04:37:00.176385 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/api_client.py
+-rw-r--r--   0        0        0      852 2024-04-18 04:37:00.240387 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/api_response.py
+-rw-r--r--   0        0        0    14687 2024-04-18 04:37:00.276388 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/configuration.py
+-rw-r--r--   0        0        0     5433 2024-04-18 04:37:00.352390 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/exceptions.py
+-rw-r--r--   0        0        0     5100 2024-04-18 04:37:00.408391 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/__init__.py
+-rw-r--r--   0        0        0      819 2024-04-18 04:37:00.456393 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/asset_file_type.py
+-rw-r--r--   0        0        0      931 2024-04-18 04:37:00.536395 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/asset_type.py
+-rw-r--r--   0        0        0      809 2024-04-18 04:37:00.596397 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/calibration_master_type.py
+-rw-r--r--   0        0        0     1904 2024-04-18 04:37:00.644398 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/empty_success.py
+-rw-r--r--   0        0        0     1186 2024-04-18 04:37:00.728400 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/filter_type.py
+-rw-r--r--   0        0        0     2155 2024-04-18 04:37:00.776402 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/location.py
+-rw-r--r--   0        0        0      747 2024-04-18 04:37:00.836403 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/mount_type.py
+-rw-r--r--   0        0        0      887 2024-04-18 04:37:00.900405 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/node_state.py
+-rw-r--r--   0        0        0      827 2024-04-18 04:37:00.952407 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/optical_tube_type.py
+-rw-r--r--   0        0        0      751 2024-04-18 04:37:01.012408 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/shutter_type.py
+-rw-r--r--   0        0        0     1892 2024-04-18 04:37:01.076410 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/successful_create.py
+-rw-r--r--   0        0        0      768 2024-04-18 04:37:01.128412 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/tracking_type.py
+-rw-r--r--   0        0        0     3258 2024-04-18 04:37:01.180413 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_astro_project.py
+-rw-r--r--   0        0        0     3969 2024-04-18 04:37:01.224414 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_astro_project_asset.py
+-rw-r--r--   0        0        0     2569 2024-04-18 04:37:01.280416 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py
+-rw-r--r--   0        0        0     2399 2024-04-18 04:37:01.344418 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py
+-rw-r--r--   0        0        0     2381 2024-04-18 04:37:01.392419 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_astro_target.py
+-rw-r--r--   0        0        0     3640 2024-04-18 04:37:01.484422 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_calibration_master.py
+-rw-r--r--   0        0        0     4908 2024-04-18 04:37:01.528423 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_camera.py
+-rw-r--r--   0        0        0     2421 2024-04-18 04:37:01.568424 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py
+-rw-r--r--   0        0        0     2668 2024-04-18 04:37:01.628425 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_astro_project_request.py
+-rw-r--r--   0        0        0     2121 2024-04-18 04:37:01.712428 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_astro_project_response.py
+-rw-r--r--   0        0        0     3777 2024-04-18 04:37:01.772430 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_calibration_master_request.py
+-rw-r--r--   0        0        0     2147 2024-04-18 04:37:01.808431 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_calibration_master_response.py
+-rw-r--r--   0        0        0     7059 2024-04-18 04:37:01.840432 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_camera_request.py
+-rw-r--r--   0        0        0     2044 2024-04-18 04:37:01.884433 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_image_set_image_request.py
+-rw-r--r--   0        0        0     2115 2024-04-18 04:37:01.940434 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_image_set_image_response.py
+-rw-r--r--   0        0        0     2683 2024-04-18 04:37:02.004436 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_image_set_request.py
+-rw-r--r--   0        0        0     2296 2024-04-18 04:37:02.060438 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_mount_request.py
+-rw-r--r--   0        0        0     3146 2024-04-18 04:37:02.116439 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_node_request.py
+-rw-r--r--   0        0        0     2447 2024-04-18 04:37:02.160441 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2441 2024-04-18 04:37:02.208442 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_elevation_mask_point.py
+-rw-r--r--   0        0        0     3289 2024-04-18 04:37:02.256443 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_gain_curve.py
+-rw-r--r--   0        0        0     2051 2024-04-18 04:37:02.296444 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_gain_curve_point.py
+-rw-r--r--   0        0        0     2096 2024-04-18 04:37:02.332445 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py
+-rw-r--r--   0        0        0     2364 2024-04-18 04:37:02.388447 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_get_nodes.py
+-rw-r--r--   0        0        0     7066 2024-04-18 04:37:02.432448 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_get_or_create_camera_request.py
+-rw-r--r--   0        0        0     2324 2024-04-18 04:37:02.464449 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_get_or_create_mount_request.py
+-rw-r--r--   0        0        0     2513 2024-04-18 04:37:02.512450 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py
+-rw-r--r--   0        0        0     3436 2024-04-18 04:37:02.568452 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_image_set.py
+-rw-r--r--   0        0        0     5167 2024-04-18 04:37:02.628454 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_image_set_image.py
+-rw-r--r--   0        0        0      795 2024-04-18 04:37:02.672455 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_job_kind.py
+-rw-r--r--   0        0        0     2632 2024-04-18 04:37:02.716456 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_job_log.py
+-rw-r--r--   0        0        0      803 2024-04-18 04:37:02.808459 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_job_status.py
+-rw-r--r--   0        0        0     1914 2024-04-18 04:37:02.852460 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_mount.py
+-rw-r--r--   0        0        0     4458 2024-04-18 04:37:02.928462 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_node.py
+-rw-r--r--   0        0        0     2564 2024-04-18 04:37:03.004464 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_node_with_location.py
+-rw-r--r--   0        0        0     2239 2024-04-18 04:37:03.044465 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_optical_tube.py
+-rw-r--r--   0        0        0     3057 2024-04-18 04:37:03.080466 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_platform_credit.py
+-rw-r--r--   0        0        0      870 2024-04-18 04:37:03.128467 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_platform_credit_source.py
+-rw-r--r--   0        0        0      800 2024-04-18 04:37:03.188469 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_platform_credit_type.py
+-rw-r--r--   0        0        0      776 2024-04-18 04:37:03.236471 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_platform_credit_unit.py
+-rw-r--r--   0        0        0     2045 2024-04-18 04:37:03.300472 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py
+-rw-r--r--   0        0        0     2051 2024-04-18 04:37:03.352474 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_read_noise_point.py
+-rw-r--r--   0        0        0     2050 2024-04-18 04:37:03.400475 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_setup_action.py
+-rw-r--r--   0        0        0     2940 2024-04-18 04:37:03.448476 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_slew_timing.py
+-rw-r--r--   0        0        0     2240 2024-04-18 04:37:03.532479 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_slew_timing_interval.py
+-rw-r--r--   0        0        0     4605 2024-04-18 04:37:03.596481 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_update_node_request.py
+-rw-r--r--   0        0        0     2522 2024-04-18 04:37:03.648482 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_video_mode_framerate_property.py
+-rw-r--r--   0        0        0        0 2024-04-18 04:37:03.684483 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/py.typed
+-rw-r--r--   0        0        0    12935 2024-04-18 04:37:03.776486 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/rest.py
+-rw-r--r--   0        0        0      739 2024-04-18 04:37:03.836487 ourskyai_astro_api-1.3.3368/pyproject.toml
+-rw-r--r--   0        0        0    12025 1970-01-01 00:00:00.000000 ourskyai_astro_api-1.3.3368/PKG-INFO
```

### Comparing `ourskyai_astro_api-1.3.3197/README.md` & `ourskyai_astro_api-1.3.3368/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ourskyai-astro-api
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3197
-- Package version: 1.3.3197
+- API version: 1.3.3368
+- Package version: 1.3.3368
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/__init__.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.3197"
+__version__ = "1.3.3368"
 
 # import apis into sdk package
 from ourskyai_astro_api.api.default_api import DefaultApi
 
 # import ApiClient
 from ourskyai_astro_api.api_response import ApiResponse
 from ourskyai_astro_api.api_client import ApiClient
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/api/default_api.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import re  # noqa: F401
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/api_client.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import atexit
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.3.3197/python'
+        self.user_agent = 'OpenAPI-Generator/1.3.3368/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/api_response.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/api_response.py`

 * *Files identical despite different names*

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/configuration.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import copy
@@ -371,16 +371,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.3.3197\n"\
-               "SDK Package Version: 1.3.3197".\
+               "Version of the API: 1.3.3368\n"\
+               "SDK Package Version: 1.3.3368".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/exceptions.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/__init__.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/asset_file_type.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/asset_file_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/asset_type.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/asset_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/calibration_master_type.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/calibration_master_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/empty_success.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/empty_success.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/filter_type.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/filter_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/location.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/mount_type.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/tracking_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,24 +17,24 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class MountType(str, Enum):
+class TrackingType(str, Enum):
     """
-    MountType
+    TrackingType
     """
 
     """
     allowed enum values
     """
-    ALT_AZ = 'ALT_AZ'
-    EQUITORIAL = 'EQUITORIAL'
+    SIDEREAL = 'SIDEREAL'
+    TARGET_RATE = 'TARGET_RATE'
 
     @classmethod
-    def from_json(cls, json_str: str) -> MountType:
-        """Create an instance of MountType from a JSON string"""
-        return MountType(json.loads(json_str))
+    def from_json(cls, json_str: str) -> TrackingType:
+        """Create an instance of TrackingType from a JSON string"""
+        return TrackingType(json.loads(json_str))
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/node_state.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/node_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/optical_tube_type.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/optical_tube_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/shutter_type.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_job_kind.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,24 +17,25 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class ShutterType(str, Enum):
+class V1JobKind(str, Enum):
     """
-    ShutterType
+    V1JobKind
     """
 
     """
     allowed enum values
     """
-    ROLLING = 'ROLLING'
-    GLOBAL = 'GLOBAL'
+    STACK = 'STACK'
+    REPROCESS = 'REPROCESS'
+    OBSERVATION_POTENTIAL = 'OBSERVATION_POTENTIAL'
 
     @classmethod
-    def from_json(cls, json_str: str) -> ShutterType:
-        """Create an instance of ShutterType from a JSON string"""
-        return ShutterType(json.loads(json_str))
+    def from_json(cls, json_str: str) -> V1JobKind:
+        """Create an instance of V1JobKind from a JSON string"""
+        return V1JobKind(json.loads(json_str))
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/successful_create.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/successful_create.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/tracking_type.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_platform_credit_unit.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,24 +17,23 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class TrackingType(str, Enum):
+class V1PlatformCreditUnit(str, Enum):
     """
-    TrackingType
+    V1PlatformCreditUnit
     """
 
     """
     allowed enum values
     """
-    SIDEREAL = 'SIDEREAL'
-    TARGET_RATE = 'TARGET_RATE'
+    MEGABYTE = 'MEGABYTE'
 
     @classmethod
-    def from_json(cls, json_str: str) -> TrackingType:
-        """Create an instance of TrackingType from a JSON string"""
-        return TrackingType(json.loads(json_str))
+    def from_json(cls, json_str: str) -> V1PlatformCreditUnit:
+        """Create an instance of V1PlatformCreditUnit from a JSON string"""
+        return V1PlatformCreditUnit(json.loads(json_str))
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_astro_project.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_astro_project.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -31,15 +31,17 @@
     ra: Optional[Union[StrictFloat, StrictInt]] = None
     dec: Optional[Union[StrictFloat, StrictInt]] = None
     camera_id: StrictStr = Field(..., alias="cameraId")
     ota_id: StrictStr = Field(..., alias="otaId")
     image_sets: Optional[conlist(StrictStr)] = Field(None, alias="imageSets")
     created_at: datetime = Field(..., alias="createdAt")
     updated_at: Optional[datetime] = Field(None, alias="updatedAt")
-    __properties = ["id", "name", "targetId", "ra", "dec", "cameraId", "otaId", "imageSets", "createdAt", "updatedAt"]
+    total_images: StrictInt = Field(..., alias="totalImages")
+    uploaded_images: StrictInt = Field(..., alias="uploadedImages")
+    __properties = ["id", "name", "targetId", "ra", "dec", "cameraId", "otaId", "imageSets", "createdAt", "updatedAt", "totalImages", "uploadedImages"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -78,12 +80,14 @@
             "target_id": obj.get("targetId"),
             "ra": obj.get("ra"),
             "dec": obj.get("dec"),
             "camera_id": obj.get("cameraId"),
             "ota_id": obj.get("otaId"),
             "image_sets": obj.get("imageSets"),
             "created_at": obj.get("createdAt"),
-            "updated_at": obj.get("updatedAt")
+            "updated_at": obj.get("updatedAt"),
+            "total_images": obj.get("totalImages"),
+            "uploaded_images": obj.get("uploadedImages")
         })
         return _obj
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_astro_project_asset.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_astro_project_asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_astro_target.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_astro_target.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_calibration_master.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_calibration_master.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_camera.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_camera.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_create_astro_project_request.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_astro_project_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_create_astro_project_response.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_astro_project_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_create_calibration_master_request.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_calibration_master_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_create_calibration_master_response.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_calibration_master_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_create_camera_request.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_camera_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_create_image_set_image_request.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_image_set_image_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_create_image_set_image_response.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_image_set_image_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_create_image_set_request.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_image_set_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_create_mount_request.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_mount_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_create_node_request.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_node_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_create_optical_tube_request.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_optical_tube_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_elevation_mask_point.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_elevation_mask_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_gain_curve.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_gain_curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_gain_curve_point.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_gain_curve_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_get_nodes.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_get_nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_get_or_create_camera_request.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_get_or_create_camera_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_get_or_create_mount_request.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_get_or_create_mount_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_image_set.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_image_set.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_image_set_image.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_image_set_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_job_kind.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/shutter_type.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,25 +17,24 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class V1JobKind(str, Enum):
+class ShutterType(str, Enum):
     """
-    V1JobKind
+    ShutterType
     """
 
     """
     allowed enum values
     """
-    STACK = 'STACK'
-    REPROCESS = 'REPROCESS'
-    OBSERVATION_POTENTIAL = 'OBSERVATION_POTENTIAL'
+    ROLLING = 'ROLLING'
+    GLOBAL = 'GLOBAL'
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1JobKind:
-        """Create an instance of V1JobKind from a JSON string"""
-        return V1JobKind(json.loads(json_str))
+    def from_json(cls, json_str: str) -> ShutterType:
+        """Create an instance of ShutterType from a JSON string"""
+        return ShutterType(json.loads(json_str))
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_job_log.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_job_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_job_status.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_job_status.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_mount.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_mount.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_node.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_node_with_location.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_node_with_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_optical_tube.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_optical_tube.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_platform_credit.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_platform_credit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_platform_credit_source.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_platform_credit_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_platform_credit_unit.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/mount_type.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,23 +17,24 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class V1PlatformCreditUnit(str, Enum):
+class MountType(str, Enum):
     """
-    V1PlatformCreditUnit
+    MountType
     """
 
     """
     allowed enum values
     """
-    MEGABYTE = 'MEGABYTE'
+    ALT_AZ = 'ALT_AZ'
+    EQUITORIAL = 'EQUITORIAL'
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1PlatformCreditUnit:
-        """Create an instance of V1PlatformCreditUnit from a JSON string"""
-        return V1PlatformCreditUnit(json.loads(json_str))
+    def from_json(cls, json_str: str) -> MountType:
+        """Create an instance of MountType from a JSON string"""
+        return MountType(json.loads(json_str))
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_read_noise_point.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_read_noise_point.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_setup_action.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_setup_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_slew_timing.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_slew_timing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_slew_timing_interval.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_slew_timing_interval.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_update_node_request.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_update_node_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/models/v1_video_mode_framerate_property.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_video_mode_framerate_property.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3197/ourskyai_astro_api/rest.py` & `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `ourskyai_astro_api-1.3.3197/pyproject.toml` & `ourskyai_astro_api-1.3.3368/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ourskyai_astro_api"
-version = "1.3.3197"
+version = "1.3.3368"
 description = "OurSky Astro"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OurSky Astro"]
 include = ["ourskyai_astro_api/py.typed"]
```

### Comparing `ourskyai_astro_api-1.3.3197/PKG-INFO` & `ourskyai_astro_api-1.3.3368/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ourskyai_astro_api
-Version: 1.3.3197
+Version: 1.3.3368
 Summary: OurSky Astro
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,OurSky Astro
 Author: OpenAPI Generator Community
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
@@ -24,16 +24,16 @@
 Description-Content-Type: text/markdown
 
 # ourskyai-astro-api
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3197
-- Package version: 1.3.3197
+- API version: 1.3.3368
+- Package version: 1.3.3368
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
```

