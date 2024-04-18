# Comparing `tmp/ourskyai_platform_api-1.3.3197.tar.gz` & `tmp/ourskyai_platform_api-1.3.3368.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourskyai_platform_api-1.3.3197.tar", max compression
+gzip compressed data, was "ourskyai_platform_api-1.3.3368.tar", max compression
```

## Comparing `ourskyai_platform_api-1.3.3197.tar` & `ourskyai_platform_api-1.3.3368.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     8889 2024-03-30 00:36:07.610064 ourskyai_platform_api-1.3.3197/README.md
--rw-r--r--   0        0        0     5613 2024-03-30 00:36:11.010130 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/__init__.py
--rw-r--r--   0        0        0      109 2024-03-30 00:36:11.038130 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/api/__init__.py
--rw-r--r--   0        0        0   185893 2024-03-30 00:36:11.134132 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/api/default_api.py
--rw-r--r--   0        0        0    30373 2024-03-30 00:36:11.174133 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/api_client.py
--rw-r--r--   0        0        0      852 2024-03-30 00:36:11.226134 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/api_response.py
--rw-r--r--   0        0        0    14693 2024-03-30 00:36:11.290135 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/configuration.py
--rw-r--r--   0        0        0     5436 2024-03-30 00:36:11.342136 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/exceptions.py
--rw-r--r--   0        0        0     4942 2024-03-30 00:36:11.414137 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/__init__.py
--rw-r--r--   0        0        0      745 2024-03-30 00:36:11.482139 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/camera_mode.py
--rw-r--r--   0        0        0     1907 2024-03-30 00:36:11.586141 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/empty_success.py
--rw-r--r--   0        0        0     1189 2024-03-30 00:36:11.682143 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/filter_type.py
--rw-r--r--   0        0        0     2158 2024-03-30 00:36:11.774145 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/location.py
--rw-r--r--   0        0        0      777 2024-03-30 00:36:11.826146 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/metric_type.py
--rw-r--r--   0        0        0      750 2024-03-30 00:36:11.890147 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/mount_type.py
--rw-r--r--   0        0        0      890 2024-03-30 00:36:11.930148 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/node_state.py
--rw-r--r--   0        0        0      830 2024-03-30 00:36:11.974148 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/optical_tube_type.py
--rw-r--r--   0        0        0     2407 2024-03-30 00:36:12.010149 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/plate_solve_parameters.py
--rw-r--r--   0        0        0      754 2024-03-30 00:36:12.050150 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/shutter_type.py
--rw-r--r--   0        0        0     1895 2024-03-30 00:36:12.098151 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/successful_create.py
--rw-r--r--   0        0        0      771 2024-03-30 00:36:12.154152 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/tracking_type.py
--rw-r--r--   0        0        0     4920 2024-03-30 00:36:12.206153 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_camera.py
--rw-r--r--   0        0        0     2115 2024-03-30 00:36:12.254154 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_client_token.py
--rw-r--r--   0        0        0     2047 2024-03-30 00:36:12.310155 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_complete_observation_request.py
--rw-r--r--   0        0        0     2047 2024-03-30 00:36:12.350156 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_create_image_set_image_request.py
--rw-r--r--   0        0        0     2118 2024-03-30 00:36:12.406157 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_create_image_set_image_response.py
--rw-r--r--   0        0        0     2692 2024-03-30 00:36:12.494158 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_create_image_set_request.py
--rw-r--r--   0        0        0     2302 2024-03-30 00:36:12.590160 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_create_mount_request.py
--rw-r--r--   0        0        0     2710 2024-03-30 00:36:12.650161 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_create_node_diagnostic.py
--rw-r--r--   0        0        0     2715 2024-03-30 00:36:12.698162 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py
--rw-r--r--   0        0        0     3152 2024-03-30 00:36:12.750163 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_create_node_request.py
--rw-r--r--   0        0        0     2453 2024-03-30 00:36:12.806164 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_create_optical_tube_request.py
--rw-r--r--   0        0        0     2124 2024-03-30 00:36:12.862166 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_diagnostic_instruction.py
--rw-r--r--   0        0        0     2444 2024-03-30 00:36:12.906166 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_elevation_mask_point.py
--rw-r--r--   0        0        0     3298 2024-03-30 00:36:12.966168 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_gain_curve.py
--rw-r--r--   0        0        0     2054 2024-03-30 00:36:13.014168 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_gain_curve_point.py
--rw-r--r--   0        0        0     2570 2024-03-30 00:36:13.062169 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_get_instruction_request.py
--rw-r--r--   0        0        0     2370 2024-03-30 00:36:13.126171 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_get_nodes.py
--rw-r--r--   0        0        0     7081 2024-03-30 00:36:13.182172 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_get_or_create_camera_request.py
--rw-r--r--   0        0        0     2330 2024-03-30 00:36:13.226173 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_get_or_create_mount_request.py
--rw-r--r--   0        0        0     2519 2024-03-30 00:36:13.294174 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py
--rw-r--r--   0        0        0     3985 2024-03-30 00:36:13.342175 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_ground_station_participant.py
--rw-r--r--   0        0        0     3445 2024-03-30 00:36:13.390176 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_image_set.py
--rw-r--r--   0        0        0     5170 2024-03-30 00:36:13.454177 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_image_set_image.py
--rw-r--r--   0        0        0     3305 2024-03-30 00:36:13.498178 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_instruction.py
--rw-r--r--   0        0        0     2400 2024-03-30 00:36:13.550179 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_metric.py
--rw-r--r--   0        0        0     1917 2024-03-30 00:36:13.658181 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_mount.py
--rw-r--r--   0        0        0     4470 2024-03-30 00:36:13.714182 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_node.py
--rw-r--r--   0        0        0      850 2024-03-30 00:36:13.786183 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_node_component_type.py
--rw-r--r--   0        0        0     1595 2024-03-30 00:36:13.830184 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_node_diagnostic_type.py
--rw-r--r--   0        0        0     2573 2024-03-30 00:36:13.870185 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_node_with_location.py
--rw-r--r--   0        0        0     5537 2024-03-30 00:36:13.934186 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_observation_instruction.py
--rw-r--r--   0        0        0     2242 2024-03-30 00:36:14.022188 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_optical_tube.py
--rw-r--r--   0        0        0     2054 2024-03-30 00:36:14.074189 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_read_noise_point.py
--rw-r--r--   0        0        0     2053 2024-03-30 00:36:14.138190 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_setup_action.py
--rw-r--r--   0        0        0     2946 2024-03-30 00:36:14.202191 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_slew_timing.py
--rw-r--r--   0        0        0     2243 2024-03-30 00:36:14.246192 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_slew_timing_interval.py
--rw-r--r--   0        0        0     3601 2024-03-30 00:36:14.314194 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_update_node_components_request.py
--rw-r--r--   0        0        0     6269 2024-03-30 00:36:14.370195 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_update_node_components_request_camera.py
--rw-r--r--   0        0        0     2402 2024-03-30 00:36:14.430196 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_update_node_components_request_mount.py
--rw-r--r--   0        0        0     2591 2024-03-30 00:36:14.486197 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py
--rw-r--r--   0        0        0     4620 2024-03-30 00:36:14.538198 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_update_node_request.py
--rw-r--r--   0        0        0     2525 2024-03-30 00:36:14.578199 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_video_mode_framerate_property.py
--rw-r--r--   0        0        0     2224 2024-03-30 00:36:14.622200 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v2_complete_observation_request.py
--rw-r--r--   0        0        0        0 2024-03-30 00:36:14.654200 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/py.typed
--rw-r--r--   0        0        0    12941 2024-03-30 00:36:14.702201 ourskyai_platform_api-1.3.3197/ourskyai_platform_api/rest.py
--rw-r--r--   0        0        0      751 2024-03-30 00:36:14.774202 ourskyai_platform_api-1.3.3197/pyproject.toml
--rw-r--r--   0        0        0     9866 1970-01-01 00:00:00.000000 ourskyai_platform_api-1.3.3197/PKG-INFO
+-rw-r--r--   0        0        0     8889 2024-04-18 04:36:56.096271 ourskyai_platform_api-1.3.3368/README.md
+-rw-r--r--   0        0        0     5613 2024-04-18 04:36:59.540367 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/__init__.py
+-rw-r--r--   0        0        0      109 2024-04-18 04:36:59.576368 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/api/__init__.py
+-rw-r--r--   0        0        0   185893 2024-04-18 04:36:59.660370 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/api/default_api.py
+-rw-r--r--   0        0        0    30373 2024-04-18 04:36:59.732373 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/api_client.py
+-rw-r--r--   0        0        0      852 2024-04-18 04:36:59.784374 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/api_response.py
+-rw-r--r--   0        0        0    14693 2024-04-18 04:36:59.836376 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/configuration.py
+-rw-r--r--   0        0        0     5436 2024-04-18 04:36:59.892377 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/exceptions.py
+-rw-r--r--   0        0        0     4942 2024-04-18 04:36:59.960379 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/__init__.py
+-rw-r--r--   0        0        0      745 2024-04-18 04:37:00.020381 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/camera_mode.py
+-rw-r--r--   0        0        0     1907 2024-04-18 04:37:00.096383 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/empty_success.py
+-rw-r--r--   0        0        0     1189 2024-04-18 04:37:00.144384 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/filter_type.py
+-rw-r--r--   0        0        0     2158 2024-04-18 04:37:00.208386 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/location.py
+-rw-r--r--   0        0        0      777 2024-04-18 04:37:00.256387 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/metric_type.py
+-rw-r--r--   0        0        0      750 2024-04-18 04:37:00.308389 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/mount_type.py
+-rw-r--r--   0        0        0      890 2024-04-18 04:37:00.356390 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/node_state.py
+-rw-r--r--   0        0        0      830 2024-04-18 04:37:00.412392 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/optical_tube_type.py
+-rw-r--r--   0        0        0     2407 2024-04-18 04:37:00.460393 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/plate_solve_parameters.py
+-rw-r--r--   0        0        0      754 2024-04-18 04:37:00.500394 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/shutter_type.py
+-rw-r--r--   0        0        0     1895 2024-04-18 04:37:00.564396 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/successful_create.py
+-rw-r--r--   0        0        0      771 2024-04-18 04:37:00.624397 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/tracking_type.py
+-rw-r--r--   0        0        0     4920 2024-04-18 04:37:00.680399 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_camera.py
+-rw-r--r--   0        0        0     2115 2024-04-18 04:37:00.740401 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_client_token.py
+-rw-r--r--   0        0        0     2047 2024-04-18 04:37:00.788402 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_complete_observation_request.py
+-rw-r--r--   0        0        0     2047 2024-04-18 04:37:00.844404 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_image_set_image_request.py
+-rw-r--r--   0        0        0     2118 2024-04-18 04:37:00.912406 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_image_set_image_response.py
+-rw-r--r--   0        0        0     2692 2024-04-18 04:37:00.960407 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_image_set_request.py
+-rw-r--r--   0        0        0     2302 2024-04-18 04:37:00.996408 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_mount_request.py
+-rw-r--r--   0        0        0     2710 2024-04-18 04:37:01.052410 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_node_diagnostic.py
+-rw-r--r--   0        0        0     2715 2024-04-18 04:37:01.112411 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py
+-rw-r--r--   0        0        0     3152 2024-04-18 04:37:01.160412 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_node_request.py
+-rw-r--r--   0        0        0     2453 2024-04-18 04:37:01.196413 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2124 2024-04-18 04:37:01.272415 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_diagnostic_instruction.py
+-rw-r--r--   0        0        0     2444 2024-04-18 04:37:01.328417 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_elevation_mask_point.py
+-rw-r--r--   0        0        0     3298 2024-04-18 04:37:01.372418 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_gain_curve.py
+-rw-r--r--   0        0        0     2054 2024-04-18 04:37:01.432420 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_gain_curve_point.py
+-rw-r--r--   0        0        0     2570 2024-04-18 04:37:01.476421 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_get_instruction_request.py
+-rw-r--r--   0        0        0     2370 2024-04-18 04:37:01.528423 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_get_nodes.py
+-rw-r--r--   0        0        0     7081 2024-04-18 04:37:01.580424 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_get_or_create_camera_request.py
+-rw-r--r--   0        0        0     2330 2024-04-18 04:37:01.624426 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_get_or_create_mount_request.py
+-rw-r--r--   0        0        0     2519 2024-04-18 04:37:01.668427 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py
+-rw-r--r--   0        0        0     3985 2024-04-18 04:37:01.760429 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_ground_station_participant.py
+-rw-r--r--   0        0        0     3445 2024-04-18 04:37:01.820431 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_image_set.py
+-rw-r--r--   0        0        0     5170 2024-04-18 04:37:01.868432 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_image_set_image.py
+-rw-r--r--   0        0        0     3305 2024-04-18 04:37:01.936434 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_instruction.py
+-rw-r--r--   0        0        0     2400 2024-04-18 04:37:01.984435 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_metric.py
+-rw-r--r--   0        0        0     1917 2024-04-18 04:37:02.032437 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_mount.py
+-rw-r--r--   0        0        0     4470 2024-04-18 04:37:02.080438 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_node.py
+-rw-r--r--   0        0        0      850 2024-04-18 04:37:02.128440 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_node_component_type.py
+-rw-r--r--   0        0        0     1595 2024-04-18 04:37:02.172441 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_node_diagnostic_type.py
+-rw-r--r--   0        0        0     2573 2024-04-18 04:37:02.220442 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_node_with_location.py
+-rw-r--r--   0        0        0     5537 2024-04-18 04:37:02.260443 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_observation_instruction.py
+-rw-r--r--   0        0        0     2242 2024-04-18 04:37:02.296444 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_optical_tube.py
+-rw-r--r--   0        0        0     2054 2024-04-18 04:37:02.356446 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_read_noise_point.py
+-rw-r--r--   0        0        0     2053 2024-04-18 04:37:02.404447 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_setup_action.py
+-rw-r--r--   0        0        0     2946 2024-04-18 04:37:02.452449 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_slew_timing.py
+-rw-r--r--   0        0        0     2243 2024-04-18 04:37:02.500450 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_slew_timing_interval.py
+-rw-r--r--   0        0        0     3601 2024-04-18 04:37:02.560452 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_update_node_components_request.py
+-rw-r--r--   0        0        0     6269 2024-04-18 04:37:02.640454 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_update_node_components_request_camera.py
+-rw-r--r--   0        0        0     2402 2024-04-18 04:37:02.700456 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_update_node_components_request_mount.py
+-rw-r--r--   0        0        0     2591 2024-04-18 04:37:02.748457 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py
+-rw-r--r--   0        0        0     4620 2024-04-18 04:37:02.796458 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_update_node_request.py
+-rw-r--r--   0        0        0     2525 2024-04-18 04:37:02.876460 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_video_mode_framerate_property.py
+-rw-r--r--   0        0        0     2224 2024-04-18 04:37:02.924462 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v2_complete_observation_request.py
+-rw-r--r--   0        0        0        0 2024-04-18 04:37:02.960463 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/py.typed
+-rw-r--r--   0        0        0    12941 2024-04-18 04:37:03.012464 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/rest.py
+-rw-r--r--   0        0        0      751 2024-04-18 04:37:03.068466 ourskyai_platform_api-1.3.3368/pyproject.toml
+-rw-r--r--   0        0        0     9866 1970-01-01 00:00:00.000000 ourskyai_platform_api-1.3.3368/PKG-INFO
```

### Comparing `ourskyai_platform_api-1.3.3197/README.md` & `ourskyai_platform_api-1.3.3368/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ourskyai-platform-api
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

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/__init__.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.3197"
+__version__ = "1.3.3368"
 
 # import apis into sdk package
 from ourskyai_platform_api.api.default_api import DefaultApi
 
 # import ApiClient
 from ourskyai_platform_api.api_response import ApiResponse
 from ourskyai_platform_api.api_client import ApiClient
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/api/default_api.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import re  # noqa: F401
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/api_client.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
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

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/api_response.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/api_response.py`

 * *Files identical despite different names*

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/configuration.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
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

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/exceptions.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/__init__.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/camera_mode.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/camera_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/empty_success.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/empty_success.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/filter_type.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/filter_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/location.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/metric_type.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/metric_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/mount_type.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/shutter_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
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
+class ShutterType(str, Enum):
     """
-    MountType
+    ShutterType
     """
 
     """
     allowed enum values
     """
-    ALT_AZ = 'ALT_AZ'
-    EQUITORIAL = 'EQUITORIAL'
+    ROLLING = 'ROLLING'
+    GLOBAL = 'GLOBAL'
 
     @classmethod
-    def from_json(cls, json_str: str) -> MountType:
-        """Create an instance of MountType from a JSON string"""
-        return MountType(json.loads(json_str))
+    def from_json(cls, json_str: str) -> ShutterType:
+        """Create an instance of ShutterType from a JSON string"""
+        return ShutterType(json.loads(json_str))
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/node_state.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/node_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/optical_tube_type.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/optical_tube_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/plate_solve_parameters.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/plate_solve_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/shutter_type.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_node_component_type.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,24 +17,26 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class ShutterType(str, Enum):
+class V1NodeComponentType(str, Enum):
     """
-    ShutterType
+    V1NodeComponentType
     """
 
     """
     allowed enum values
     """
-    ROLLING = 'ROLLING'
-    GLOBAL = 'GLOBAL'
+    CAMERA = 'CAMERA'
+    MOUNT = 'MOUNT'
+    OPTICAL_TUBE = 'OPTICAL_TUBE'
+    COMPUTER = 'COMPUTER'
 
     @classmethod
-    def from_json(cls, json_str: str) -> ShutterType:
-        """Create an instance of ShutterType from a JSON string"""
-        return ShutterType(json.loads(json_str))
+    def from_json(cls, json_str: str) -> V1NodeComponentType:
+        """Create an instance of V1NodeComponentType from a JSON string"""
+        return V1NodeComponentType(json.loads(json_str))
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/successful_create.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/successful_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/tracking_type.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/tracking_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_camera.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_client_token.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_client_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_complete_observation_request.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_complete_observation_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_create_image_set_image_request.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_image_set_image_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_create_image_set_image_response.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_image_set_image_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_create_image_set_request.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_image_set_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_create_mount_request.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_mount_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_create_node_diagnostic.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_node_diagnostic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_create_node_request.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_node_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_create_optical_tube_request.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_optical_tube_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_diagnostic_instruction.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_diagnostic_instruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_elevation_mask_point.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_elevation_mask_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_gain_curve.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_gain_curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_gain_curve_point.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_gain_curve_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_get_instruction_request.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_get_instruction_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_get_nodes.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_get_nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_get_or_create_camera_request.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_get_or_create_camera_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_get_or_create_mount_request.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_get_or_create_mount_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_ground_station_participant.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_ground_station_participant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_image_set.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_image_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_image_set_image.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_image_set_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_instruction.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_instruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_metric.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_mount.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_mount.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_node.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_node_diagnostic_type.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_node_diagnostic_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_node_with_location.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_node_with_location.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_observation_instruction.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_observation_instruction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_optical_tube.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_optical_tube.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_read_noise_point.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_read_noise_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_setup_action.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_setup_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_slew_timing.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_slew_timing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_slew_timing_interval.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_slew_timing_interval.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_update_node_components_request.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_update_node_components_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_update_node_components_request_camera.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_update_node_components_request_camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_update_node_components_request_mount.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_update_node_components_request_mount.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_update_node_request.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_update_node_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v1_video_mode_framerate_property.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_video_mode_framerate_property.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/models/v2_complete_observation_request.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v2_complete_observation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3197/ourskyai_platform_api/rest.py` & `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `ourskyai_platform_api-1.3.3197/pyproject.toml` & `ourskyai_platform_api-1.3.3368/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ourskyai_platform_api"
-version = "1.3.3197"
+version = "1.3.3368"
 description = "OurSky Platform"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OurSky Platform"]
 include = ["ourskyai_platform_api/py.typed"]
```

### Comparing `ourskyai_platform_api-1.3.3197/PKG-INFO` & `ourskyai_platform_api-1.3.3368/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ourskyai_platform_api
-Version: 1.3.3197
+Version: 1.3.3368
 Summary: OurSky Platform
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,OurSky Platform
 Author: OpenAPI Generator Community
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
@@ -24,16 +24,16 @@
 Description-Content-Type: text/markdown
 
 # ourskyai-platform-api
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

