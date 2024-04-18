# Comparing `tmp/ourskyai_sda_api-1.3.3197.tar.gz` & `tmp/ourskyai_sda_api-1.3.3368.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourskyai_sda_api-1.3.3197.tar", max compression
+gzip compressed data, was "ourskyai_sda_api-1.3.3368.tar", max compression
```

## Comparing `ourskyai_sda_api-1.3.3197.tar` & `ourskyai_sda_api-1.3.3368.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     9896 2024-03-30 00:36:07.466061 ourskyai_sda_api-1.3.3197/README.md
--rw-r--r--   0        0        0     5092 2024-03-30 00:36:10.246115 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/__init__.py
--rw-r--r--   0        0        0      104 2024-03-30 00:36:10.270115 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/api/__init__.py
--rw-r--r--   0        0        0   212616 2024-03-30 00:36:10.358117 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/api/default_api.py
--rw-r--r--   0        0        0    30830 2024-03-30 00:36:10.414118 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/api_client.py
--rw-r--r--   0        0        0      852 2024-03-30 00:36:10.466119 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/api_response.py
--rw-r--r--   0        0        0    15175 2024-03-30 00:36:10.510120 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/configuration.py
--rw-r--r--   0        0        0     5923 2024-03-30 00:36:10.570121 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/exceptions.py
--rw-r--r--   0        0        0     4471 2024-03-30 00:36:10.618122 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/__init__.py
--rw-r--r--   0        0        0     3578 2024-03-30 00:36:10.662123 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/astrometric_offsets.py
--rw-r--r--   0        0        0     2394 2024-03-30 00:36:10.714124 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/empty_success.py
--rw-r--r--   0        0        0     1676 2024-03-30 00:36:10.766125 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/filter_type.py
--rw-r--r--   0        0        0     2645 2024-03-30 00:36:10.822126 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/location.py
--rw-r--r--   0        0        0     1237 2024-03-30 00:36:10.866127 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/mount_type.py
--rw-r--r--   0        0        0     2756 2024-03-30 00:36:10.926128 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/observation_bounding_box.py
--rw-r--r--   0        0        0     3713 2024-03-30 00:36:10.974129 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/observation_quality.py
--rw-r--r--   0        0        0     5767 2024-03-30 00:36:11.014130 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/observation_result.py
--rw-r--r--   0        0        0     1320 2024-03-30 00:36:11.066131 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/observation_state.py
--rw-r--r--   0        0        0     1369 2024-03-30 00:36:11.106132 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/orbit_type.py
--rw-r--r--   0        0        0     1361 2024-03-30 00:36:11.198133 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/satellite_target_tracking_status.py
--rw-r--r--   0        0        0     1241 2024-03-30 00:36:11.246134 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/shutter_type.py
--rw-r--r--   0        0        0     2382 2024-03-30 00:36:11.286135 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/successful_create.py
--rw-r--r--   0        0        0     1258 2024-03-30 00:36:11.326136 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/tracking_type.py
--rw-r--r--   0        0        0     2534 2024-03-30 00:36:11.382137 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_create_image_set_image_request.py
--rw-r--r--   0        0        0     2605 2024-03-30 00:36:11.446138 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_create_image_set_image_response.py
--rw-r--r--   0        0        0     3169 2024-03-30 00:36:11.490139 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_create_image_set_request.py
--rw-r--r--   0        0        0     2609 2024-03-30 00:36:11.574141 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_create_organization_target_request.py
--rw-r--r--   0        0        0     2761 2024-03-30 00:36:11.642142 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_create_satellite_target_request.py
--rw-r--r--   0        0        0     3373 2024-03-30 00:36:11.682143 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_create_search_instruction_request.py
--rw-r--r--   0        0        0     3173 2024-03-30 00:36:11.742144 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_create_survey_instruction_request.py
--rw-r--r--   0        0        0     3017 2024-03-30 00:36:11.818145 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_get_satellite_targets_response.py
--rw-r--r--   0        0        0     4457 2024-03-30 00:36:11.862146 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_ground_station_participant.py
--rw-r--r--   0        0        0     3922 2024-03-30 00:36:11.902147 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_image_set.py
--rw-r--r--   0        0        0     5657 2024-03-30 00:36:11.958148 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_image_set_image.py
--rw-r--r--   0        0        0     4459 2024-03-30 00:36:12.106151 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_observation_feature.py
--rw-r--r--   0        0        0     3748 2024-03-30 00:36:12.146152 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_observation_sequence_result.py
--rw-r--r--   0        0        0     4306 2024-03-30 00:36:12.218153 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_observation_sequence_result_image_sets_inner.py
--rw-r--r--   0        0        0     4637 2024-03-30 00:36:12.298155 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_observation_status.py
--rw-r--r--   0        0        0     3192 2024-03-30 00:36:12.390156 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_organization_target.py
--rw-r--r--   0        0        0     3226 2024-03-30 00:36:12.446158 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_satellite_potential.py
--rw-r--r--   0        0        0     3528 2024-03-30 00:36:12.530159 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_satellite_target.py
--rw-r--r--   0        0        0     3733 2024-03-30 00:36:12.602161 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_search_instruction.py
--rw-r--r--   0        0        0     3466 2024-03-30 00:36:12.706163 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_search_instruction_step.py
--rw-r--r--   0        0        0     3464 2024-03-30 00:36:12.766164 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_survey_instruction.py
--rw-r--r--   0        0        0     2858 2024-03-30 00:36:12.830165 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_survey_instruction_step.py
--rw-r--r--   0        0        0     2695 2024-03-30 00:36:12.886166 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_target_correlation.py
--rw-r--r--   0        0        0     3185 2024-03-30 00:36:12.934167 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_tdm.py
--rw-r--r--   0        0        0     2575 2024-03-30 00:36:13.002168 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_update_email_configuration_request.py
--rw-r--r--   0        0        0     2913 2024-03-30 00:36:13.086170 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_update_satellite_target_request.py
--rw-r--r--   0        0        0     3146 2024-03-30 00:36:13.154171 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_update_webhook_configuration_request.py
--rw-r--r--   0        0        0     2963 2024-03-30 00:36:13.182172 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_webhook_configuration.py
--rw-r--r--   0        0        0     1350 2024-03-30 00:36:13.222173 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/webhook_auth_type.py
--rw-r--r--   0        0        0     1734 2024-03-30 00:36:13.266173 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/webhook_event.py
--rw-r--r--   0        0        0        0 2024-03-30 00:36:13.298174 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/py.typed
--rw-r--r--   0        0        0    13423 2024-03-30 00:36:13.350175 ourskyai_sda_api-1.3.3197/ourskyai_sda_api/rest.py
--rw-r--r--   0        0        0      731 2024-03-30 00:36:13.406176 ourskyai_sda_api-1.3.3197/pyproject.toml
--rw-r--r--   0        0        0    10858 1970-01-01 00:00:00.000000 ourskyai_sda_api-1.3.3197/PKG-INFO
+-rw-r--r--   0        0        0     9896 2024-04-18 04:36:56.088271 ourskyai_sda_api-1.3.3368/README.md
+-rw-r--r--   0        0        0     5092 2024-04-18 04:36:58.664343 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/__init__.py
+-rw-r--r--   0        0        0      104 2024-04-18 04:36:58.704344 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/api/__init__.py
+-rw-r--r--   0        0        0   213326 2024-04-18 04:36:58.808347 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/api/default_api.py
+-rw-r--r--   0        0        0    30830 2024-04-18 04:36:58.856348 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/api_client.py
+-rw-r--r--   0        0        0      852 2024-04-18 04:36:58.908350 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/api_response.py
+-rw-r--r--   0        0        0    15175 2024-04-18 04:36:58.980352 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/configuration.py
+-rw-r--r--   0        0        0     5923 2024-04-18 04:36:59.032353 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/exceptions.py
+-rw-r--r--   0        0        0     4471 2024-04-18 04:36:59.104355 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/__init__.py
+-rw-r--r--   0        0        0     3578 2024-04-18 04:36:59.144356 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/astrometric_offsets.py
+-rw-r--r--   0        0        0     2394 2024-04-18 04:36:59.204358 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/empty_success.py
+-rw-r--r--   0        0        0     1676 2024-04-18 04:36:59.260359 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/filter_type.py
+-rw-r--r--   0        0        0     2645 2024-04-18 04:36:59.308361 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/location.py
+-rw-r--r--   0        0        0     1237 2024-04-18 04:36:59.348362 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/mount_type.py
+-rw-r--r--   0        0        0     2756 2024-04-18 04:36:59.408363 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/observation_bounding_box.py
+-rw-r--r--   0        0        0     3713 2024-04-18 04:36:59.456365 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/observation_quality.py
+-rw-r--r--   0        0        0     5767 2024-04-18 04:36:59.516367 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/observation_result.py
+-rw-r--r--   0        0        0     1320 2024-04-18 04:36:59.568368 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/observation_state.py
+-rw-r--r--   0        0        0     1529 2024-04-18 04:36:59.620370 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/orbit_type.py
+-rw-r--r--   0        0        0     1361 2024-04-18 04:36:59.676371 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/satellite_target_tracking_status.py
+-rw-r--r--   0        0        0     1241 2024-04-18 04:36:59.728372 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/shutter_type.py
+-rw-r--r--   0        0        0     2382 2024-04-18 04:36:59.792374 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/successful_create.py
+-rw-r--r--   0        0        0     1258 2024-04-18 04:36:59.844376 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/tracking_type.py
+-rw-r--r--   0        0        0     2534 2024-04-18 04:36:59.908378 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_create_image_set_image_request.py
+-rw-r--r--   0        0        0     2605 2024-04-18 04:36:59.964379 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_create_image_set_image_response.py
+-rw-r--r--   0        0        0     3169 2024-04-18 04:37:00.032381 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_create_image_set_request.py
+-rw-r--r--   0        0        0     2609 2024-04-18 04:37:00.140384 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_create_organization_target_request.py
+-rw-r--r--   0        0        0     2761 2024-04-18 04:37:00.188385 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_create_satellite_target_request.py
+-rw-r--r--   0        0        0     3373 2024-04-18 04:37:00.240387 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_create_search_instruction_request.py
+-rw-r--r--   0        0        0     3353 2024-04-18 04:37:00.296388 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_create_survey_instruction_request.py
+-rw-r--r--   0        0        0     3017 2024-04-18 04:37:00.344390 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_get_satellite_targets_response.py
+-rw-r--r--   0        0        0     4457 2024-04-18 04:37:00.440392 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_ground_station_participant.py
+-rw-r--r--   0        0        0     3922 2024-04-18 04:37:00.508394 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_image_set.py
+-rw-r--r--   0        0        0     5657 2024-04-18 04:37:00.540395 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_image_set_image.py
+-rw-r--r--   0        0        0     4459 2024-04-18 04:37:00.588396 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_observation_feature.py
+-rw-r--r--   0        0        0     3748 2024-04-18 04:37:00.648398 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_observation_sequence_result.py
+-rw-r--r--   0        0        0     4306 2024-04-18 04:37:00.728400 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_observation_sequence_result_image_sets_inner.py
+-rw-r--r--   0        0        0     4637 2024-04-18 04:37:00.784402 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_observation_status.py
+-rw-r--r--   0        0        0     3192 2024-04-18 04:37:00.848404 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_organization_target.py
+-rw-r--r--   0        0        0     3226 2024-04-18 04:37:00.908405 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_satellite_potential.py
+-rw-r--r--   0        0        0     3528 2024-04-18 04:37:00.956407 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_satellite_target.py
+-rw-r--r--   0        0        0     3733 2024-04-18 04:37:01.012408 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_search_instruction.py
+-rw-r--r--   0        0        0     3407 2024-04-18 04:37:01.068410 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_search_instruction_step.py
+-rw-r--r--   0        0        0     3634 2024-04-18 04:37:01.144412 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_survey_instruction.py
+-rw-r--r--   0        0        0     2799 2024-04-18 04:37:01.188413 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_survey_instruction_step.py
+-rw-r--r--   0        0        0     2695 2024-04-18 04:37:01.260415 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_target_correlation.py
+-rw-r--r--   0        0        0     3185 2024-04-18 04:37:01.312417 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_tdm.py
+-rw-r--r--   0        0        0     2575 2024-04-18 04:37:01.376418 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_update_email_configuration_request.py
+-rw-r--r--   0        0        0     2913 2024-04-18 04:37:01.432420 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_update_satellite_target_request.py
+-rw-r--r--   0        0        0     3146 2024-04-18 04:37:01.492422 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_update_webhook_configuration_request.py
+-rw-r--r--   0        0        0     2963 2024-04-18 04:37:01.528423 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_webhook_configuration.py
+-rw-r--r--   0        0        0     1350 2024-04-18 04:37:01.576424 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/webhook_auth_type.py
+-rw-r--r--   0        0        0     1734 2024-04-18 04:37:01.624426 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/webhook_event.py
+-rw-r--r--   0        0        0        0 2024-04-18 04:37:01.660426 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/py.typed
+-rw-r--r--   0        0        0    13423 2024-04-18 04:37:01.716428 ourskyai_sda_api-1.3.3368/ourskyai_sda_api/rest.py
+-rw-r--r--   0        0        0      731 2024-04-18 04:37:01.768429 ourskyai_sda_api-1.3.3368/pyproject.toml
+-rw-r--r--   0        0        0    10858 1970-01-01 00:00:00.000000 ourskyai_sda_api-1.3.3368/PKG-INFO
```

### Comparing `ourskyai_sda_api-1.3.3197/README.md` & `ourskyai_sda_api-1.3.3368/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 The basic flow for a new organization is as follows:
 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe.
 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above.
 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
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

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/__init__.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.3197"
+__version__ = "1.3.3368"
 
 # import apis into sdk package
 from ourskyai_sda_api.api.default_api import DefaultApi
 
 # import ApiClient
 from ourskyai_sda_api.api_response import ApiResponse
 from ourskyai_sda_api.api_client import ApiClient
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/api/default_api.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/api/default_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import re  # noqa: F401
@@ -661,15 +661,15 @@
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
     def v1_create_search_instruction(self, v1_create_search_instruction_request : V1CreateSearchInstructionRequest, **kwargs) -> SuccessfulCreate:  # noqa: E501
         """v1_create_search_instruction  # noqa: E501
 
-        Create a search instruction. Search instructions are the highest priority request in the system. The system will execute the search and the results will be available in the observation status endpoint.  # noqa: E501
+        Create a search instruction. Search instructions are the highest priority request in the system. The maximum duration for all steps is 5 minutes. Search patterns can be defined through both step offsets and timing. The system will execute the search and the resulting observations will be available in the observation status endpoint.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.v1_create_search_instruction(v1_create_search_instruction_request, async_req=True)
         >>> result = thread.get()
 
         :param v1_create_search_instruction_request: (required)
@@ -691,15 +691,15 @@
             raise ValueError(message)
         return self.v1_create_search_instruction_with_http_info(v1_create_search_instruction_request, **kwargs)  # noqa: E501
 
     @validate_arguments
     def v1_create_search_instruction_with_http_info(self, v1_create_search_instruction_request : V1CreateSearchInstructionRequest, **kwargs) -> ApiResponse:  # noqa: E501
         """v1_create_search_instruction  # noqa: E501
 
-        Create a search instruction. Search instructions are the highest priority request in the system. The system will execute the search and the results will be available in the observation status endpoint.  # noqa: E501
+        Create a search instruction. Search instructions are the highest priority request in the system. The maximum duration for all steps is 5 minutes. Search patterns can be defined through both step offsets and timing. The system will execute the search and the resulting observations will be available in the observation status endpoint.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.v1_create_search_instruction_with_http_info(v1_create_search_instruction_request, async_req=True)
         >>> result = thread.get()
 
         :param v1_create_search_instruction_request: (required)
@@ -808,15 +808,15 @@
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
     def v1_create_survey_instruction(self, v1_create_survey_instruction_request : V1CreateSurveyInstructionRequest, **kwargs) -> SuccessfulCreate:  # noqa: E501
         """v1_create_survey_instruction  # noqa: E501
 
-        Create a survey instruction. Survey instructions are the highest priority request in the system. The system will execute the survey and the results will be available in the observation status endpoint.  # noqa: E501
+        Create a survey instruction. Survey instructions are the highest priority request in the system. The system will execute the survey and the results will be available in the observation status endpoint.  If `firstStepAt` is not specified, then the first node that is able to view an RA/Dec of any step will execute the instruction. If `firstStepAt` is specified, then the instruction will only execute starting at that time.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.v1_create_survey_instruction(v1_create_survey_instruction_request, async_req=True)
         >>> result = thread.get()
 
         :param v1_create_survey_instruction_request: (required)
@@ -838,15 +838,15 @@
             raise ValueError(message)
         return self.v1_create_survey_instruction_with_http_info(v1_create_survey_instruction_request, **kwargs)  # noqa: E501
 
     @validate_arguments
     def v1_create_survey_instruction_with_http_info(self, v1_create_survey_instruction_request : V1CreateSurveyInstructionRequest, **kwargs) -> ApiResponse:  # noqa: E501
         """v1_create_survey_instruction  # noqa: E501
 
-        Create a survey instruction. Survey instructions are the highest priority request in the system. The system will execute the survey and the results will be available in the observation status endpoint.  # noqa: E501
+        Create a survey instruction. Survey instructions are the highest priority request in the system. The system will execute the survey and the results will be available in the observation status endpoint.  If `firstStepAt` is not specified, then the first node that is able to view an RA/Dec of any step will execute the instruction. If `firstStepAt` is specified, then the instruction will only execute starting at that time.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.v1_create_survey_instruction_with_http_info(v1_create_survey_instruction_request, async_req=True)
         >>> result = thread.get()
 
         :param v1_create_survey_instruction_request: (required)
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/api_client.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
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

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/api_response.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/api_response.py`

 * *Files identical despite different names*

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/configuration.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
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

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/exceptions.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/__init__.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/astrometric_offsets.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/astrometric_offsets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/empty_success.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/empty_success.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/filter_type.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/filter_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/location.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/location.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/mount_type.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/mount_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/observation_bounding_box.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/observation_bounding_box.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/observation_quality.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/observation_quality.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/observation_result.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/observation_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/observation_state.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/observation_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/orbit_type.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/webhook_auth_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,30 +17,25 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class OrbitType(str, Enum):
+class WebhookAuthType(str, Enum):
     """
-    OrbitType
+    Authorization mechanism required for webhook endpoint, if any. Use `NONE` if not required.
     """
 
     """
     allowed enum values
     """
-    GEOSTATIONARY = 'GEOSTATIONARY'
-    GEOSYNCHRONOUS = 'GEOSYNCHRONOUS'
-    MEO = 'MEO'
-    LEO = 'LEO'
-    GTO = 'GTO'
-    SSO = 'SSO'
-    TUNDRA = 'TUNDRA'
-    MOLNIYA = 'MOLNIYA'
+    NONE = 'NONE'
+    BASIC = 'BASIC'
+    BEARER = 'BEARER'
 
     @classmethod
-    def from_json(cls, json_str: str) -> OrbitType:
-        """Create an instance of OrbitType from a JSON string"""
-        return OrbitType(json.loads(json_str))
+    def from_json(cls, json_str: str) -> WebhookAuthType:
+        """Create an instance of WebhookAuthType from a JSON string"""
+        return WebhookAuthType(json.loads(json_str))
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/satellite_target_tracking_status.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/satellite_target_tracking_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/shutter_type.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/shutter_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/successful_create.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/successful_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/tracking_type.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/tracking_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_create_image_set_image_request.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_create_image_set_image_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_create_image_set_image_response.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_create_image_set_image_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_create_image_set_request.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_create_image_set_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_create_organization_target_request.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_create_organization_target_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_create_satellite_target_request.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_create_satellite_target_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_create_search_instruction_request.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_create_search_instruction_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_create_survey_instruction_request.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_create_survey_instruction_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
-from typing import List
+from datetime import datetime
+from typing import List, Optional
 from pydantic import BaseModel, Field, StrictStr, conlist
 from ourskyai_sda_api.models.v1_survey_instruction_step import V1SurveyInstructionStep
 
 class V1CreateSurveyInstructionRequest(BaseModel):
     """
     V1CreateSurveyInstructionRequest
     """
     target_id: StrictStr = Field(..., alias="targetId")
     steps: conlist(V1SurveyInstructionStep) = Field(...)
-    __properties = ["targetId", "steps"]
+    first_step_at: Optional[datetime] = Field(None, alias="firstStepAt")
+    __properties = ["targetId", "steps", "firstStepAt"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -70,12 +71,13 @@
             return None
 
         if not isinstance(obj, dict):
             return V1CreateSurveyInstructionRequest.parse_obj(obj)
 
         _obj = V1CreateSurveyInstructionRequest.parse_obj({
             "target_id": obj.get("targetId"),
-            "steps": [V1SurveyInstructionStep.from_dict(_item) for _item in obj.get("steps")] if obj.get("steps") is not None else None
+            "steps": [V1SurveyInstructionStep.from_dict(_item) for _item in obj.get("steps")] if obj.get("steps") is not None else None,
+            "first_step_at": obj.get("firstStepAt")
         })
         return _obj
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_get_satellite_targets_response.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_get_satellite_targets_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_ground_station_participant.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_ground_station_participant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_image_set.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_image_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_image_set_image.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_image_set_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_observation_feature.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_observation_feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_observation_sequence_result.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_observation_sequence_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_observation_sequence_result_image_sets_inner.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_observation_sequence_result_image_sets_inner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_observation_status.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_observation_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_organization_target.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_organization_target.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_satellite_potential.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_satellite_potential.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_satellite_target.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_satellite_target.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_search_instruction.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_search_instruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_search_instruction_step.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_search_instruction_step.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
+
 from typing import Union
 from pydantic import BaseModel, Field, StrictFloat, StrictInt
 
 class V1SearchInstructionStep(BaseModel):
     """
-    Search Instruction Step  # noqa: E501
+    Search Instruction Step. Each step is associated with one observation.  # noqa: E501
     """
     along_track_offset_meters: Union[StrictFloat, StrictInt] = Field(..., alias="alongTrackOffsetMeters", description="Along-track offset in the local spacecraft frame.")
     cross_track_offset_meters: Union[StrictFloat, StrictInt] = Field(..., alias="crossTrackOffsetMeters", description="Cross-track offset in the local spacecraft frame.")
     radial_offset_meters: Union[StrictFloat, StrictInt] = Field(..., alias="radialOffsetMeters", description="Radial offset in the local spacecraft frame.")
-    start_time: datetime = Field(..., alias="startTime")
-    end_time: datetime = Field(..., alias="endTime")
-    __properties = ["alongTrackOffsetMeters", "crossTrackOffsetMeters", "radialOffsetMeters", "startTime", "endTime"]
+    duration_seconds: StrictInt = Field(..., alias="durationSeconds")
+    __properties = ["alongTrackOffsetMeters", "crossTrackOffsetMeters", "radialOffsetMeters", "durationSeconds"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -67,13 +66,12 @@
         if not isinstance(obj, dict):
             return V1SearchInstructionStep.parse_obj(obj)
 
         _obj = V1SearchInstructionStep.parse_obj({
             "along_track_offset_meters": obj.get("alongTrackOffsetMeters"),
             "cross_track_offset_meters": obj.get("crossTrackOffsetMeters"),
             "radial_offset_meters": obj.get("radialOffsetMeters"),
-            "start_time": obj.get("startTime"),
-            "end_time": obj.get("endTime")
+            "duration_seconds": obj.get("durationSeconds")
         })
         return _obj
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_survey_instruction.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_survey_instruction.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
+from datetime import datetime
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictStr, conlist
 from ourskyai_sda_api.models.v1_survey_instruction_step import V1SurveyInstructionStep
 
 class V1SurveyInstruction(BaseModel):
     """
     V1SurveyInstruction
     """
     id: StrictStr = Field(...)
     node_id: Optional[StrictStr] = Field(None, alias="nodeId")
     target_id: StrictStr = Field(..., alias="targetId")
+    first_step_at: Optional[datetime] = Field(None, alias="firstStepAt")
     steps: conlist(V1SurveyInstructionStep) = Field(..., description="Each step indicates a sidereal observation attempt at a given (Ra, Dec). When supplying coordinates, they should be given in J2000 reference frames using an SGP4 model for propagation.")
-    __properties = ["id", "nodeId", "targetId", "steps"]
+    __properties = ["id", "nodeId", "targetId", "firstStepAt", "steps"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -74,12 +75,13 @@
         if not isinstance(obj, dict):
             return V1SurveyInstruction.parse_obj(obj)
 
         _obj = V1SurveyInstruction.parse_obj({
             "id": obj.get("id"),
             "node_id": obj.get("nodeId"),
             "target_id": obj.get("targetId"),
+            "first_step_at": obj.get("firstStepAt"),
             "steps": [V1SurveyInstructionStep.from_dict(_item) for _item in obj.get("steps")] if obj.get("steps") is not None else None
         })
         return _obj
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_survey_instruction_step.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_survey_instruction_step.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
+
 from typing import Union
 from pydantic import BaseModel, Field, StrictFloat, StrictInt
 
 class V1SurveyInstructionStep(BaseModel):
     """
-    Survey Instruction Step  # noqa: E501
+    Survey Instruction Step. Each step is associated with one observation.  # noqa: E501
     """
     ra: Union[StrictFloat, StrictInt] = Field(...)
     dec: Union[StrictFloat, StrictInt] = Field(...)
-    start_time: datetime = Field(..., alias="startTime")
-    end_time: datetime = Field(..., alias="endTime")
-    __properties = ["ra", "dec", "startTime", "endTime"]
+    duration_seconds: StrictInt = Field(..., alias="durationSeconds")
+    __properties = ["ra", "dec", "durationSeconds"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -65,13 +64,12 @@
 
         if not isinstance(obj, dict):
             return V1SurveyInstructionStep.parse_obj(obj)
 
         _obj = V1SurveyInstructionStep.parse_obj({
             "ra": obj.get("ra"),
             "dec": obj.get("dec"),
-            "start_time": obj.get("startTime"),
-            "end_time": obj.get("endTime")
+            "duration_seconds": obj.get("durationSeconds")
         })
         return _obj
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_target_correlation.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_target_correlation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_tdm.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_tdm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_update_email_configuration_request.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_update_email_configuration_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_update_satellite_target_request.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_update_satellite_target_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_update_webhook_configuration_request.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_update_webhook_configuration_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/v1_webhook_configuration.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/v1_webhook_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/models/webhook_auth_type.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/models/webhook_event.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,25 +17,29 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class WebhookAuthType(str, Enum):
+class WebhookEvent(str, Enum):
     """
-    Authorization mechanism required for webhook endpoint, if any. Use `NONE` if not required.
+    Webhook events that can be subscribed to. For `EO_OBSERVATION` events, please refer to the Unified Data Library for the full schema.
     """
 
     """
     allowed enum values
     """
-    NONE = 'NONE'
-    BASIC = 'BASIC'
-    BEARER = 'BEARER'
+    V1_TDM_CREATED = 'V1_TDM_CREATED'
+    V1_OBSERVATION_SEQUENCE_RESULT_CREATED = 'V1_OBSERVATION_SEQUENCE_RESULT_CREATED'
+    V1_OBSERVATION_CREATED = 'V1_OBSERVATION_CREATED'
+    V1_IMAGE_CREATED = 'V1_IMAGE_CREATED'
+    V1_STREAK_CREATED = 'V1_STREAK_CREATED'
+    V1_SATELLITE_TARGET_TRACKING_DEACTIVATED = 'V1_SATELLITE_TARGET_TRACKING_DEACTIVATED'
+    V1_EO_OBSERVATION_CREATED = 'V1_EO_OBSERVATION_CREATED'
 
     @classmethod
-    def from_json(cls, json_str: str) -> WebhookAuthType:
-        """Create an instance of WebhookAuthType from a JSON string"""
-        return WebhookAuthType(json.loads(json_str))
+    def from_json(cls, json_str: str) -> WebhookEvent:
+        """Create an instance of WebhookEvent from a JSON string"""
+        return WebhookEvent(json.loads(json_str))
```

### Comparing `ourskyai_sda_api-1.3.3197/ourskyai_sda_api/rest.py` & `ourskyai_sda_api-1.3.3368/ourskyai_sda_api/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3197
+    The version of the OpenAPI document: 1.3.3368
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `ourskyai_sda_api-1.3.3197/pyproject.toml` & `ourskyai_sda_api-1.3.3368/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ourskyai_sda_api"
-version = "1.3.3197"
+version = "1.3.3368"
 description = "OurSky SDA"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OurSky SDA"]
 include = ["ourskyai_sda_api/py.typed"]
```

### Comparing `ourskyai_sda_api-1.3.3197/PKG-INFO` & `ourskyai_sda_api-1.3.3368/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ourskyai_sda_api
-Version: 1.3.3197
+Version: 1.3.3368
 Summary: OurSky SDA
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,OurSky SDA
 Author: OpenAPI Generator Community
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
@@ -27,16 +27,16 @@
 The basic flow for a new organization is as follows:
 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe.
 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above.
 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
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

