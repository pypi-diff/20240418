# Comparing `tmp/elevenlabs-1.0.5.tar.gz` & `tmp/elevenlabs-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabs-1.0.5.tar", max compression
+gzip compressed data, was "elevenlabs-1.1.0.tar", max compression
```

## Comparing `elevenlabs-1.0.5.tar` & `elevenlabs-1.1.0.tar`

### file list

```diff
@@ -1,122 +1,130 @@
--rw-r--r--   0        0        0     1067 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/LICENSE
--rw-r--r--   0        0        0     9366 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/README.md
--rw-r--r--   0        0        0      659 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     4749 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/__init__.py
--rw-r--r--   0        0        0       65 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/audio_native/__init__.py
--rw-r--r--   0        0        0    13565 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/audio_native/client.py
--rw-r--r--   0        0        0     7523 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/base_client.py
--rw-r--r--   0        0        0       65 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/chapters/__init__.py
--rw-r--r--   0        0        0    34318 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/chapters/client.py
--rw-r--r--   0        0        0    20882 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/client.py
--rw-r--r--   0        0        0      790 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/core/api_error.py
--rw-r--r--   0        0        0     1683 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/core/file.py
--rw-r--r--   0        0        0     5059 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/core/http_client.py
--rw-r--r--   0        0        0     3799 2024-04-08 11:45:42.467552 elevenlabs-1.0.5/src/elevenlabs/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/core/request_options.py
--rw-r--r--   0        0        0       65 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/dubbing/__init__.py
--rw-r--r--   0        0        0    27974 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/dubbing/client.py
--rw-r--r--   0        0        0      164 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/environment.py
--rw-r--r--   0        0        0      170 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0       65 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/history/__init__.py
--rw-r--r--   0        0        0    28349 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/history/client.py
--rw-r--r--   0        0        0       65 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/models/__init__.py
--rw-r--r--   0        0        0     5069 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/models/client.py
--rw-r--r--   0        0        0     2715 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/play.py
--rw-r--r--   0        0        0       65 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/projects/__init__.py
--rw-r--r--   0        0        0    54697 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/projects/client.py
--rw-r--r--   0        0        0       65 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/pronunciation_dictionary/__init__.py
--rw-r--r--   0        0        0    18330 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/pronunciation_dictionary/client.py
--rw-r--r--   0        0        0        0 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/py.typed
--rw-r--r--   0        0        0     5093 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/realtime_tts.py
--rw-r--r--   0        0        0       65 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/samples/__init__.py
--rw-r--r--   0        0        0    11145 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/samples/client.py
--rw-r--r--   0        0        0       65 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/speech_to_speech/__init__.py
--rw-r--r--   0        0        0    27928 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/speech_to_speech/client.py
--rw-r--r--   0        0        0       65 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/text_to_speech/__init__.py
--rw-r--r--   0        0        0    23081 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/text_to_speech/client.py
--rw-r--r--   0        0        0     6208 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/__init__.py
--rw-r--r--   0        0        0      191 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/accent.py
--rw-r--r--   0        0        0      978 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/add_project_response_model.py
--rw-r--r--   0        0        0     1058 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/add_pronunciation_dictionary_response_model.py
--rw-r--r--   0        0        0      919 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/add_voice_response_model.py
--rw-r--r--   0        0        0      161 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/age.py
--rw-r--r--   0        0        0      980 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/audio_native_create_project_response_model.py
--rw-r--r--   0        0        0      130 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/audio_native_get_embed_code_response_model.py
--rw-r--r--   0        0        0     1560 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/audio_output.py
--rw-r--r--   0        0        0     1196 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/chapter_response.py
--rw-r--r--   0        0        0     1011 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/chapter_snapshot_response.py
--rw-r--r--   0        0        0     1019 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/chapter_snapshots_response.py
--rw-r--r--   0        0        0      164 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/chapter_state.py
--rw-r--r--   0        0        0     1029 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/chapter_statistics_response.py
--rw-r--r--   0        0        0      149 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/currency.py
--rw-r--r--   0        0        0      950 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/do_dubbing_response.py
--rw-r--r--   0        0        0     1007 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/dubbing_metadata_response.py
--rw-r--r--   0        0        0      214 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/extended_subscription_response_model_billing_period.py
--rw-r--r--   0        0        0     1082 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/feedback_item.py
--rw-r--r--   0        0        0     1837 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/fine_tuning_response.py
--rw-r--r--   0        0        0      223 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/finetuning_state.py
--rw-r--r--   0        0        0      151 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/gender.py
--rw-r--r--   0        0        0     2288 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/generation_config.py
--rw-r--r--   0        0        0      988 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/get_chapters_response.py
--rw-r--r--   0        0        0     1048 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/get_library_voices_response.py
--rw-r--r--   0        0        0      988 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/get_projects_response.py
--rw-r--r--   0        0        0     1068 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/get_pronunciation_dictionary_metadata_response.py
--rw-r--r--   0        0        0     1073 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/get_speech_history_response.py
--rw-r--r--   0        0        0      953 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/get_voices_response.py
--rw-r--r--   0        0        0      101 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/history.py
--rw-r--r--   0        0        0      992 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/history_item.py
--rw-r--r--   0        0        0     1010 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/http_validation_error.py
--rw-r--r--   0        0        0      948 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/invoice.py
--rw-r--r--   0        0        0      931 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/language_response.py
--rw-r--r--   0        0        0     1639 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/library_voice_response.py
--rw-r--r--   0        0        0     1011 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/manual_verification_file_response.py
--rw-r--r--   0        0        0     1086 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/manual_verification_response.py
--rw-r--r--   0        0        0     1671 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/model.py
--rw-r--r--   0        0        0     2207 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/normalized_alignment.py
--rw-r--r--   0        0        0      176 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/optimize_streaming_latency.py
--rw-r--r--   0        0        0      408 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/output_format.py
--rw-r--r--   0        0        0     1278 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/project_extended_response_model.py
--rw-r--r--   0        0        0     1259 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/project_response.py
--rw-r--r--   0        0        0      991 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/project_snapshot_response.py
--rw-r--r--   0        0        0     1019 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/project_snapshots_response.py
--rw-r--r--   0        0        0      164 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/project_state.py
--rw-r--r--   0        0        0      974 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/pronunciation_dictionary_version_locator.py
--rw-r--r--   0        0        0     1477 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/realtime_voice_settings.py
--rw-r--r--   0        0        0     1007 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/recording_response.py
--rw-r--r--   0        0        0      220 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/review_status.py
--rw-r--r--   0        0        0     2353 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/send_text.py
--rw-r--r--   0        0        0      147 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/source.py
--rw-r--r--   0        0        0     1865 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/speech_history_item_response.py
--rw-r--r--   0        0        0      226 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/speech_history_item_response_model_voice_category.py
--rw-r--r--   0        0        0     1079 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/sso_provider_db_model.py
--rw-r--r--   0        0        0      173 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/sso_provider_db_model_provider_type.py
--rw-r--r--   0        0        0     1879 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/subscription.py
--rw-r--r--   0        0        0     1611 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/subscription_response.py
--rw-r--r--   0        0        0      200 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/subscription_response_model_billing_period.py
--rw-r--r--   0        0        0      256 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/subscription_status.py
--rw-r--r--   0        0        0     1141 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/user.py
--rw-r--r--   0        0        0     1029 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     1120 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/verification_attempt_response.py
--rw-r--r--   0        0        0     2089 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/voice.py
--rw-r--r--   0        0        0      946 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/voice_generation_parameter_option_response.py
--rw-r--r--   0        0        0     1325 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/voice_generation_parameter_response.py
--rw-r--r--   0        0        0      216 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/voice_response_model_safety_control.py
--rw-r--r--   0        0        0     1102 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/voice_sample.py
--rw-r--r--   0        0        0     1083 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/voice_settings.py
--rw-r--r--   0        0        0     2354 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/voice_sharing_response.py
--rw-r--r--   0        0        0      196 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/voice_sharing_state.py
--rw-r--r--   0        0        0     1245 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/types/voice_verification_response.py
--rw-r--r--   0        0        0       65 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/user/__init__.py
--rw-r--r--   0        0        0     9207 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/user/client.py
--rw-r--r--   0        0        0       78 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/version.py
--rw-r--r--   0        0        0       65 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/voice_generation/__init__.py
--rw-r--r--   0        0        0    20232 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/voice_generation/client.py
--rw-r--r--   0        0        0       65 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/voices/__init__.py
--rw-r--r--   0        0        0    59193 2024-04-08 11:45:42.471552 elevenlabs-1.0.5/src/elevenlabs/voices/client.py
--rw-r--r--   0        0        0     9958 1970-01-01 00:00:00.000000 elevenlabs-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-17 16:33:51.958117 elevenlabs-1.1.0/LICENSE
+-rw-r--r--   0        0        0     9366 2024-04-17 16:33:51.958117 elevenlabs-1.1.0/README.md
+-rw-r--r--   0        0        0      659 2024-04-17 16:33:51.958117 elevenlabs-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5957 2024-04-17 16:33:51.958117 elevenlabs-1.1.0/src/elevenlabs/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-17 16:33:51.958117 elevenlabs-1.1.0/src/elevenlabs/audio_native/__init__.py
+-rw-r--r--   0        0        0    13767 2024-04-17 16:33:51.958117 elevenlabs-1.1.0/src/elevenlabs/audio_native/client.py
+-rw-r--r--   0        0        0     8308 2024-04-17 16:33:51.958117 elevenlabs-1.1.0/src/elevenlabs/base_client.py
+-rw-r--r--   0        0        0       65 2024-04-17 16:33:51.958117 elevenlabs-1.1.0/src/elevenlabs/chapters/__init__.py
+-rw-r--r--   0        0        0    35488 2024-04-17 16:33:51.958117 elevenlabs-1.1.0/src/elevenlabs/chapters/client.py
+-rw-r--r--   0        0        0    20882 2024-04-17 16:33:51.958117 elevenlabs-1.1.0/src/elevenlabs/client.py
+-rw-r--r--   0        0        0     1006 2024-04-17 16:33:51.958117 elevenlabs-1.1.0/src/elevenlabs/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-17 16:33:51.958117 elevenlabs-1.1.0/src/elevenlabs/core/api_error.py
+-rw-r--r--   0        0        0     1683 2024-04-17 16:33:51.958117 elevenlabs-1.1.0/src/elevenlabs/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-17 16:33:51.958117 elevenlabs-1.1.0/src/elevenlabs/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-17 16:33:51.958117 elevenlabs-1.1.0/src/elevenlabs/core/file.py
+-rw-r--r--   0        0        0     5059 2024-04-17 16:33:51.958117 elevenlabs-1.1.0/src/elevenlabs/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-04-17 16:33:51.958117 elevenlabs-1.1.0/src/elevenlabs/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-04-17 16:33:51.958117 elevenlabs-1.1.0/src/elevenlabs/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-04-17 16:33:51.958117 elevenlabs-1.1.0/src/elevenlabs/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-17 16:33:51.958117 elevenlabs-1.1.0/src/elevenlabs/core/request_options.py
+-rw-r--r--   0        0        0     7123 2024-04-17 16:33:51.958117 elevenlabs-1.1.0/src/elevenlabs/core/unchecked_base_model.py
+-rw-r--r--   0        0        0       65 2024-04-17 16:33:51.958117 elevenlabs-1.1.0/src/elevenlabs/dubbing/__init__.py
+-rw-r--r--   0        0        0    28716 2024-04-17 16:33:51.958117 elevenlabs-1.1.0/src/elevenlabs/dubbing/client.py
+-rw-r--r--   0        0        0      164 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/environment.py
+-rw-r--r--   0        0        0      170 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0       65 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/history/__init__.py
+-rw-r--r--   0        0        0    29109 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/history/client.py
+-rw-r--r--   0        0        0       65 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/models/__init__.py
+-rw-r--r--   0        0        0     5233 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/models/client.py
+-rw-r--r--   0        0        0     2715 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/play.py
+-rw-r--r--   0        0        0       65 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/projects/__init__.py
+-rw-r--r--   0        0        0    56331 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/projects/client.py
+-rw-r--r--   0        0        0      851 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/pronunciation_dictionary/__init__.py
+-rw-r--r--   0        0        0    34040 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/pronunciation_dictionary/client.py
+-rw-r--r--   0        0        0      977 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/pronunciation_dictionary/types/__init__.py
+-rw-r--r--   0        0        0     1657 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/pronunciation_dictionary/types/body_add_rules_to_the_pronunciation_dictionary_v_1_pronunciation_dictionaries_pronunciation_dictionary_id_add_rules_post_rules_item.py
+-rw-r--r--   0        0        0        0 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/py.typed
+-rw-r--r--   0        0        0     5093 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/realtime_tts.py
+-rw-r--r--   0        0        0       65 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/samples/__init__.py
+-rw-r--r--   0        0        0    11435 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/samples/client.py
+-rw-r--r--   0        0        0       65 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/speech_to_speech/__init__.py
+-rw-r--r--   0        0        0    27928 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/speech_to_speech/client.py
+-rw-r--r--   0        0        0       65 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/text_to_speech/__init__.py
+-rw-r--r--   0        0        0    23081 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/text_to_speech/client.py
+-rw-r--r--   0        0        0     6863 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/__init__.py
+-rw-r--r--   0        0        0      188 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/accent.py
+-rw-r--r--   0        0        0      977 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/add_project_response_model.py
+-rw-r--r--   0        0        0     1057 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/add_pronunciation_dictionary_response_model.py
+-rw-r--r--   0        0        0      955 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/add_pronunciation_dictionary_rules_response_model.py
+-rw-r--r--   0        0        0      918 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/add_voice_response_model.py
+-rw-r--r--   0        0        0      158 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/age.py
+-rw-r--r--   0        0        0      979 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/audio_native_create_project_response_model.py
+-rw-r--r--   0        0        0      130 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/audio_native_get_embed_code_response_model.py
+-rw-r--r--   0        0        0     1568 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/audio_output.py
+-rw-r--r--   0        0        0     1195 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/chapter_response.py
+-rw-r--r--   0        0        0     1010 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/chapter_snapshot_response.py
+-rw-r--r--   0        0        0     1018 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/chapter_snapshots_response.py
+-rw-r--r--   0        0        0      161 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/chapter_state.py
+-rw-r--r--   0        0        0     1028 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/chapter_statistics_response.py
+-rw-r--r--   0        0        0      146 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/currency.py
+-rw-r--r--   0        0        0      949 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/do_dubbing_response.py
+-rw-r--r--   0        0        0     1006 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/dubbing_metadata_response.py
+-rw-r--r--   0        0        0      211 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/extended_subscription_response_model_billing_period.py
+-rw-r--r--   0        0        0     1081 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/feedback_item.py
+-rw-r--r--   0        0        0     1836 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/fine_tuning_response.py
+-rw-r--r--   0        0        0      220 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/finetuning_state.py
+-rw-r--r--   0        0        0      148 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/gender.py
+-rw-r--r--   0        0        0     2290 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/generation_config.py
+-rw-r--r--   0        0        0      987 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/get_chapters_response.py
+-rw-r--r--   0        0        0     1047 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/get_library_voices_response.py
+-rw-r--r--   0        0        0      987 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/get_projects_response.py
+-rw-r--r--   0        0        0     1067 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/get_pronunciation_dictionary_metadata_response.py
+-rw-r--r--   0        0        0     1072 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/get_speech_history_response.py
+-rw-r--r--   0        0        0      952 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/get_voices_response.py
+-rw-r--r--   0        0        0      101 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/history.py
+-rw-r--r--   0        0        0      991 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/history_item.py
+-rw-r--r--   0        0        0     1009 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/http_validation_error.py
+-rw-r--r--   0        0        0      947 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/invoice.py
+-rw-r--r--   0        0        0      930 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/language_response.py
+-rw-r--r--   0        0        0     1740 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/library_voice_response.py
+-rw-r--r--   0        0        0     1010 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/manual_verification_file_response.py
+-rw-r--r--   0        0        0     1085 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/manual_verification_response.py
+-rw-r--r--   0        0        0     1670 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/model.py
+-rw-r--r--   0        0        0     2215 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/normalized_alignment.py
+-rw-r--r--   0        0        0      173 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/optimize_streaming_latency.py
+-rw-r--r--   0        0        0      405 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/output_format.py
+-rw-r--r--   0        0        0     1277 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/project_extended_response_model.py
+-rw-r--r--   0        0        0     1258 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/project_response.py
+-rw-r--r--   0        0        0      990 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/project_snapshot_response.py
+-rw-r--r--   0        0        0     1018 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/project_snapshots_response.py
+-rw-r--r--   0        0        0      161 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/project_state.py
+-rw-r--r--   0        0        0      965 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/pronunciation_dictionary_alias_rule_request_model.py
+-rw-r--r--   0        0        0      987 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/pronunciation_dictionary_phoneme_rule_request_model.py
+-rw-r--r--   0        0        0      973 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/pronunciation_dictionary_version_locator.py
+-rw-r--r--   0        0        0     1488 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/realtime_voice_settings.py
+-rw-r--r--   0        0        0     1006 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/recording_response.py
+-rw-r--r--   0        0        0      958 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/remove_pronunciation_dictionary_rules_response_model.py
+-rw-r--r--   0        0        0      217 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/review_status.py
+-rw-r--r--   0        0        0     2361 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/send_text.py
+-rw-r--r--   0        0        0      144 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/source.py
+-rw-r--r--   0        0        0     1864 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/speech_history_item_response.py
+-rw-r--r--   0        0        0      223 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/speech_history_item_response_model_voice_category.py
+-rw-r--r--   0        0        0     1078 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/sso_provider_db_model.py
+-rw-r--r--   0        0        0      170 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/sso_provider_db_model_provider_type.py
+-rw-r--r--   0        0        0     1878 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/subscription.py
+-rw-r--r--   0        0        0     1610 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/subscription_response.py
+-rw-r--r--   0        0        0      197 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/subscription_response_model_billing_period.py
+-rw-r--r--   0        0        0      253 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/subscription_status.py
+-rw-r--r--   0        0        0     1140 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/user.py
+-rw-r--r--   0        0        0     1028 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     1119 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/verification_attempt_response.py
+-rw-r--r--   0        0        0     2088 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/voice.py
+-rw-r--r--   0        0        0      945 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/voice_generation_parameter_option_response.py
+-rw-r--r--   0        0        0     1324 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/voice_generation_parameter_response.py
+-rw-r--r--   0        0        0      213 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/voice_response_model_safety_control.py
+-rw-r--r--   0        0        0     1101 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/voice_sample.py
+-rw-r--r--   0        0        0     1082 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/voice_settings.py
+-rw-r--r--   0        0        0     2353 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/voice_sharing_response.py
+-rw-r--r--   0        0        0      193 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/voice_sharing_state.py
+-rw-r--r--   0        0        0     1244 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/types/voice_verification_response.py
+-rw-r--r--   0        0        0       65 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/user/__init__.py
+-rw-r--r--   0        0        0     9553 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/user/client.py
+-rw-r--r--   0        0        0       78 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/version.py
+-rw-r--r--   0        0        0       65 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/voice_generation/__init__.py
+-rw-r--r--   0        0        0    20478 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/voice_generation/client.py
+-rw-r--r--   0        0        0       65 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/voices/__init__.py
+-rw-r--r--   0        0        0    61141 2024-04-17 16:33:51.962117 elevenlabs-1.1.0/src/elevenlabs/voices/client.py
+-rw-r--r--   0        0        0     9958 1970-01-01 00:00:00.000000 elevenlabs-1.1.0/PKG-INFO
```

### Comparing `elevenlabs-1.0.5/LICENSE` & `elevenlabs-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.5/README.md` & `elevenlabs-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.5/pyproject.toml` & `elevenlabs-1.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "elevenlabs"
-version = "v1.0.5"
+version = "v1.1.0"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "elevenlabs", from = "src"}
 ]
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/__init__.py` & `elevenlabs-1.1.0/src/elevenlabs/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .types import (
     Accent,
     AddProjectResponseModel,
     AddPronunciationDictionaryResponseModel,
+    AddPronunciationDictionaryRulesResponseModel,
     AddVoiceResponseModel,
     Age,
     AudioNativeCreateProjectResponseModel,
     AudioNativeGetEmbedCodeResponseModel,
     AudioOutput,
     ChapterResponse,
     ChapterSnapshotResponse,
@@ -42,17 +43,20 @@
     OptimizeStreamingLatency,
     OutputFormat,
     ProjectExtendedResponseModel,
     ProjectResponse,
     ProjectSnapshotResponse,
     ProjectSnapshotsResponse,
     ProjectState,
+    PronunciationDictionaryAliasRuleRequestModel,
+    PronunciationDictionaryPhonemeRuleRequestModel,
     PronunciationDictionaryVersionLocator,
     RealtimeVoiceSettings,
     RecordingResponse,
+    RemovePronunciationDictionaryRulesResponseModel,
     ReviewStatus,
     SendText,
     Source,
     SpeechHistoryItemResponse,
     SpeechHistoryItemResponseModelVoiceCategory,
     SsoProviderDbModel,
     SsoProviderDbModelProviderType,
@@ -88,25 +92,34 @@
     text_to_speech,
     user,
     voice_generation,
     voices,
 )
 from .environment import ElevenLabsEnvironment
 from .play import play, save, stream
+from .pronunciation_dictionary import (
+    BodyAddRulesToThePronunciationDictionaryV1PronunciationDictionariesPronunciationDictionaryIdAddRulesPostRulesItem,
+    BodyAddRulesToThePronunciationDictionaryV1PronunciationDictionariesPronunciationDictionaryIdAddRulesPostRulesItem_Alias,
+    BodyAddRulesToThePronunciationDictionaryV1PronunciationDictionariesPronunciationDictionaryIdAddRulesPostRulesItem_Phoneme,
+)
 from .version import __version__
 
 __all__ = [
     "Accent",
     "AddProjectResponseModel",
     "AddPronunciationDictionaryResponseModel",
+    "AddPronunciationDictionaryRulesResponseModel",
     "AddVoiceResponseModel",
     "Age",
     "AudioNativeCreateProjectResponseModel",
     "AudioNativeGetEmbedCodeResponseModel",
     "AudioOutput",
+    "BodyAddRulesToThePronunciationDictionaryV1PronunciationDictionariesPronunciationDictionaryIdAddRulesPostRulesItem",
+    "BodyAddRulesToThePronunciationDictionaryV1PronunciationDictionariesPronunciationDictionaryIdAddRulesPostRulesItem_Alias",
+    "BodyAddRulesToThePronunciationDictionaryV1PronunciationDictionariesPronunciationDictionaryIdAddRulesPostRulesItem_Phoneme",
     "ChapterResponse",
     "ChapterSnapshotResponse",
     "ChapterSnapshotsResponse",
     "ChapterState",
     "ChapterStatisticsResponse",
     "Currency",
     "DoDubbingResponse",
@@ -137,17 +150,20 @@
     "OptimizeStreamingLatency",
     "OutputFormat",
     "ProjectExtendedResponseModel",
     "ProjectResponse",
     "ProjectSnapshotResponse",
     "ProjectSnapshotsResponse",
     "ProjectState",
+    "PronunciationDictionaryAliasRuleRequestModel",
+    "PronunciationDictionaryPhonemeRuleRequestModel",
     "PronunciationDictionaryVersionLocator",
     "RealtimeVoiceSettings",
     "RecordingResponse",
+    "RemovePronunciationDictionaryRulesResponseModel",
     "ReviewStatus",
     "SendText",
     "Source",
     "SpeechHistoryItemResponse",
     "SpeechHistoryItemResponseModelVoiceCategory",
     "SsoProviderDbModel",
     "SsoProviderDbModelProviderType",
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/audio_native/client.py` & `elevenlabs-1.1.0/src/elevenlabs/audio_native/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,19 @@
 
 from .. import core
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.audio_native_create_project_response_model import AudioNativeCreateProjectResponseModel
 from ..types.http_validation_error import HttpValidationError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class AudioNativeClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
@@ -137,17 +133,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AudioNativeCreateProjectResponseModel, _response.json())  # type: ignore
+            return typing.cast(AudioNativeCreateProjectResponseModel, construct_type(type_=AudioNativeCreateProjectResponseModel, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -265,15 +263,17 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AudioNativeCreateProjectResponseModel, _response.json())  # type: ignore
+            return typing.cast(AudioNativeCreateProjectResponseModel, construct_type(type_=AudioNativeCreateProjectResponseModel, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/base_client.py` & `elevenlabs-1.1.0/src/elevenlabs/base_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 
                                               Defaults to ElevenLabsEnvironment.PRODUCTION
 
         - api_key: typing.Optional[str].
 
         - timeout: typing.Optional[float]. The timeout to be used, in seconds, for requests by default the timeout is 60 seconds, unless a custom httpx client is used, in which case a default is not set.
 
+        - follow_redirects: typing.Optional[bool]. Whether the default httpx client follows redirects or not, this is irrelevant if a custom httpx client is passed in.
+
         - httpx_client: typing.Optional[httpx.Client]. The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
     ---
     from elevenlabs.client import ElevenLabs
 
     client = ElevenLabs(
         api_key="YOUR_API_KEY",
     )
@@ -49,21 +51,26 @@
     def __init__(
         self,
         *,
         base_url: typing.Optional[str] = None,
         environment: ElevenLabsEnvironment = ElevenLabsEnvironment.PRODUCTION,
         api_key: typing.Optional[str] = os.getenv("ELEVEN_API_KEY"),
         timeout: typing.Optional[float] = None,
+        follow_redirects: typing.Optional[bool] = None,
         httpx_client: typing.Optional[httpx.Client] = None
     ):
         _defaulted_timeout = timeout if timeout is not None else 60 if httpx_client is None else None
         self._client_wrapper = SyncClientWrapper(
             base_url=_get_base_url(base_url=base_url, environment=environment),
             api_key=api_key,
-            httpx_client=httpx.Client(timeout=_defaulted_timeout) if httpx_client is None else httpx_client,
+            httpx_client=httpx_client
+            if httpx_client is not None
+            else httpx.Client(timeout=_defaulted_timeout, follow_redirects=follow_redirects)
+            if follow_redirects is not None
+            else httpx.Client(timeout=_defaulted_timeout),
             timeout=_defaulted_timeout,
         )
         self.history = HistoryClient(client_wrapper=self._client_wrapper)
         self.samples = SamplesClient(client_wrapper=self._client_wrapper)
         self.text_to_speech = TextToSpeechClient(client_wrapper=self._client_wrapper)
         self.speech_to_speech = SpeechToSpeechClient(client_wrapper=self._client_wrapper)
         self.voice_generation = VoiceGenerationClient(client_wrapper=self._client_wrapper)
@@ -88,14 +95,16 @@
 
                                               Defaults to ElevenLabsEnvironment.PRODUCTION
 
         - api_key: typing.Optional[str].
 
         - timeout: typing.Optional[float]. The timeout to be used, in seconds, for requests by default the timeout is 60 seconds, unless a custom httpx client is used, in which case a default is not set.
 
+        - follow_redirects: typing.Optional[bool]. Whether the default httpx client follows redirects or not, this is irrelevant if a custom httpx client is passed in.
+
         - httpx_client: typing.Optional[httpx.AsyncClient]. The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
     ---
     from elevenlabs.client import AsyncElevenLabs
 
     client = AsyncElevenLabs(
         api_key="YOUR_API_KEY",
     )
@@ -104,21 +113,26 @@
     def __init__(
         self,
         *,
         base_url: typing.Optional[str] = None,
         environment: ElevenLabsEnvironment = ElevenLabsEnvironment.PRODUCTION,
         api_key: typing.Optional[str] = os.getenv("ELEVEN_API_KEY"),
         timeout: typing.Optional[float] = None,
+        follow_redirects: typing.Optional[bool] = None,
         httpx_client: typing.Optional[httpx.AsyncClient] = None
     ):
         _defaulted_timeout = timeout if timeout is not None else 60 if httpx_client is None else None
         self._client_wrapper = AsyncClientWrapper(
             base_url=_get_base_url(base_url=base_url, environment=environment),
             api_key=api_key,
-            httpx_client=httpx.AsyncClient(timeout=_defaulted_timeout) if httpx_client is None else httpx_client,
+            httpx_client=httpx_client
+            if httpx_client is not None
+            else httpx.AsyncClient(timeout=_defaulted_timeout, follow_redirects=follow_redirects)
+            if follow_redirects is not None
+            else httpx.AsyncClient(timeout=_defaulted_timeout),
             timeout=_defaulted_timeout,
         )
         self.history = AsyncHistoryClient(client_wrapper=self._client_wrapper)
         self.samples = AsyncSamplesClient(client_wrapper=self._client_wrapper)
         self.text_to_speech = AsyncTextToSpeechClient(client_wrapper=self._client_wrapper)
         self.speech_to_speech = AsyncSpeechToSpeechClient(client_wrapper=self._client_wrapper)
         self.voice_generation = AsyncVoiceGenerationClient(client_wrapper=self._client_wrapper)
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/chapters/client.py` & `elevenlabs-1.1.0/src/elevenlabs/chapters/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,25 +5,21 @@
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.chapter_response import ChapterResponse
 from ..types.chapter_snapshots_response import ChapterSnapshotsResponse
 from ..types.get_chapters_response import GetChaptersResponse
 from ..types.http_validation_error import HttpValidationError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 
 class ChaptersClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def get_all(
         self, project_id: str, *, request_options: typing.Optional[RequestOptions] = None
@@ -64,17 +60,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetChaptersResponse, _response.json())  # type: ignore
+            return typing.cast(GetChaptersResponse, construct_type(type_=GetChaptersResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(
@@ -120,17 +118,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ChapterResponse, _response.json())  # type: ignore
+            return typing.cast(ChapterResponse, construct_type(type_=ChapterResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(
@@ -176,17 +176,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def convert(
@@ -235,17 +237,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_all_snapshots(
@@ -291,17 +295,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ChapterSnapshotsResponse, _response.json())  # type: ignore
+            return typing.cast(ChapterSnapshotsResponse, construct_type(type_=ChapterSnapshotsResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def stream_snapshot(
@@ -360,15 +366,17 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -415,17 +423,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetChaptersResponse, _response.json())  # type: ignore
+            return typing.cast(GetChaptersResponse, construct_type(type_=GetChaptersResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(
@@ -471,17 +481,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ChapterResponse, _response.json())  # type: ignore
+            return typing.cast(ChapterResponse, construct_type(type_=ChapterResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(
@@ -527,17 +539,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def convert(
@@ -586,17 +600,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_all_snapshots(
@@ -642,17 +658,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ChapterSnapshotsResponse, _response.json())  # type: ignore
+            return typing.cast(ChapterSnapshotsResponse, construct_type(type_=ChapterSnapshotsResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def stream_snapshot(
@@ -711,13 +729,15 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/client.py` & `elevenlabs-1.1.0/src/elevenlabs/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.5/src/elevenlabs/core/client_wrapper.py` & `elevenlabs-1.1.0/src/elevenlabs/core/client_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "elevenlabs",
-            "X-Fern-SDK-Version": "v1.0.5",
+            "X-Fern-SDK-Version": "v1.1.0",
         }
         if self._api_key is not None:
             headers["xi-api-key"] = self._api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/core/datetime_utils.py` & `elevenlabs-1.1.0/src/elevenlabs/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.5/src/elevenlabs/core/file.py` & `elevenlabs-1.1.0/src/elevenlabs/core/file.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.5/src/elevenlabs/core/http_client.py` & `elevenlabs-1.1.0/src/elevenlabs/core/http_client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.5/src/elevenlabs/core/jsonable_encoder.py` & `elevenlabs-1.1.0/src/elevenlabs/core/jsonable_encoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,47 +12,43 @@
 import datetime as dt
 from collections import defaultdict
 from enum import Enum
 from pathlib import PurePath
 from types import GeneratorType
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 from .datetime_utils import serialize_datetime
+from .pydantic_utilities import pydantic_v1
 
 SetIntStr = Set[Union[int, str]]
 DictIntStrAny = Dict[Union[int, str], Any]
 
 
 def generate_encoders_by_class_tuples(
     type_encoder_map: Dict[Any, Callable[[Any], Any]]
 ) -> Dict[Callable[[Any], Any], Tuple[Any, ...]]:
     encoders_by_class_tuples: Dict[Callable[[Any], Any], Tuple[Any, ...]] = defaultdict(tuple)
     for type_, encoder in type_encoder_map.items():
         encoders_by_class_tuples[encoder] += (type_,)
     return encoders_by_class_tuples
 
 
-encoders_by_class_tuples = generate_encoders_by_class_tuples(pydantic.json.ENCODERS_BY_TYPE)
+encoders_by_class_tuples = generate_encoders_by_class_tuples(pydantic_v1.json.ENCODERS_BY_TYPE)
 
 
 def jsonable_encoder(obj: Any, custom_encoder: Optional[Dict[Any, Callable[[Any], Any]]] = None) -> Any:
     custom_encoder = custom_encoder or {}
     if custom_encoder:
         if type(obj) in custom_encoder:
             return custom_encoder[type(obj)](obj)
         else:
             for encoder_type, encoder_instance in custom_encoder.items():
                 if isinstance(obj, encoder_type):
                     return encoder_instance(obj)
-    if isinstance(obj, pydantic.BaseModel):
+    if isinstance(obj, pydantic_v1.BaseModel):
         encoder = getattr(obj.__config__, "json_encoders", {})
         if custom_encoder:
             encoder.update(custom_encoder)
         obj_dict = obj.dict(by_alias=True)
         if "__root__" in obj_dict:
             obj_dict = obj_dict["__root__"]
         return jsonable_encoder(obj_dict, custom_encoder=encoder)
@@ -80,16 +76,16 @@
         return encoded_dict
     if isinstance(obj, (list, set, frozenset, GeneratorType, tuple)):
         encoded_list = []
         for item in obj:
             encoded_list.append(jsonable_encoder(item, custom_encoder=custom_encoder))
         return encoded_list
 
-    if type(obj) in pydantic.json.ENCODERS_BY_TYPE:
-        return pydantic.json.ENCODERS_BY_TYPE[type(obj)](obj)
+    if type(obj) in pydantic_v1.json.ENCODERS_BY_TYPE:
+        return pydantic_v1.json.ENCODERS_BY_TYPE[type(obj)](obj)
     for encoder, classes_tuple in encoders_by_class_tuples.items():
         if isinstance(obj, classes_tuple):
             return encoder(obj)
 
     try:
         data = dict(obj)
     except Exception as e:
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/core/request_options.py` & `elevenlabs-1.1.0/src/elevenlabs/core/request_options.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.5/src/elevenlabs/dubbing/client.py` & `elevenlabs-1.1.0/src/elevenlabs/dubbing/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,20 @@
 
 from .. import core
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.do_dubbing_response import DoDubbingResponse
 from ..types.dubbing_metadata_response import DubbingMetadataResponse
 from ..types.http_validation_error import HttpValidationError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class DubbingClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
@@ -156,17 +152,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DoDubbingResponse, _response.json())  # type: ignore
+            return typing.cast(DoDubbingResponse, construct_type(type_=DoDubbingResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_dubbing_project_metadata(
@@ -208,17 +206,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DubbingMetadataResponse, _response.json())  # type: ignore
+            return typing.cast(DubbingMetadataResponse, construct_type(type_=DubbingMetadataResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete_dubbing_project(
@@ -260,17 +260,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_dubbed_file(
@@ -318,15 +320,17 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -462,17 +466,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DoDubbingResponse, _response.json())  # type: ignore
+            return typing.cast(DoDubbingResponse, construct_type(type_=DoDubbingResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_dubbing_project_metadata(
@@ -514,17 +520,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DubbingMetadataResponse, _response.json())  # type: ignore
+            return typing.cast(DubbingMetadataResponse, construct_type(type_=DubbingMetadataResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete_dubbing_project(
@@ -566,17 +574,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_dubbed_file(
@@ -624,13 +634,15 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/history/client.py` & `elevenlabs-1.1.0/src/elevenlabs/history/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,20 @@
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.get_speech_history_response import GetSpeechHistoryResponse
 from ..types.http_validation_error import HttpValidationError
 from ..types.speech_history_item_response import SpeechHistoryItemResponse
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class HistoryClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
@@ -82,17 +78,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetSpeechHistoryResponse, _response.json())  # type: ignore
+            return typing.cast(GetSpeechHistoryResponse, construct_type(type_=GetSpeechHistoryResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(
@@ -134,17 +132,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(SpeechHistoryItemResponse, _response.json())  # type: ignore
+            return typing.cast(SpeechHistoryItemResponse, construct_type(type_=SpeechHistoryItemResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, history_item_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
@@ -184,17 +184,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_audio(
@@ -304,15 +306,17 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -375,17 +379,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetSpeechHistoryResponse, _response.json())  # type: ignore
+            return typing.cast(GetSpeechHistoryResponse, construct_type(type_=GetSpeechHistoryResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(
@@ -427,17 +433,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(SpeechHistoryItemResponse, _response.json())  # type: ignore
+            return typing.cast(SpeechHistoryItemResponse, construct_type(type_=SpeechHistoryItemResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(
@@ -479,17 +487,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_audio(
@@ -599,13 +609,15 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/models/client.py` & `elevenlabs-1.1.0/src/elevenlabs/models/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,23 +5,19 @@
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.http_validation_error import HttpValidationError
 from ..types.model import Model
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 
 class ModelsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def get_all(self, *, request_options: typing.Optional[RequestOptions] = None) -> typing.List[Model]:
         """
@@ -54,17 +50,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[Model], _response.json())  # type: ignore
+            return typing.cast(typing.List[Model], construct_type(type_=typing.List[Model], object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -103,15 +101,17 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[Model], _response.json())  # type: ignore
+            return typing.cast(typing.List[Model], construct_type(type_=typing.List[Model], object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/play.py` & `elevenlabs-1.1.0/src/elevenlabs/play.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.5/src/elevenlabs/projects/client.py` & `elevenlabs-1.1.0/src/elevenlabs/projects/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,23 @@
 
 from .. import core
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.add_project_response_model import AddProjectResponseModel
 from ..types.get_projects_response import GetProjectsResponse
 from ..types.http_validation_error import HttpValidationError
 from ..types.project_extended_response_model import ProjectExtendedResponseModel
 from ..types.project_snapshots_response import ProjectSnapshotsResponse
 from ..types.pronunciation_dictionary_version_locator import PronunciationDictionaryVersionLocator
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class ProjectsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
@@ -62,17 +58,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetProjectsResponse, _response.json())  # type: ignore
+            return typing.cast(GetProjectsResponse, construct_type(type_=GetProjectsResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def add(
@@ -198,17 +196,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AddProjectResponseModel, _response.json())  # type: ignore
+            return typing.cast(AddProjectResponseModel, construct_type(type_=AddProjectResponseModel, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(
@@ -250,17 +250,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ProjectExtendedResponseModel, _response.json())  # type: ignore
+            return typing.cast(ProjectExtendedResponseModel, construct_type(type_=ProjectExtendedResponseModel, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, project_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
@@ -300,17 +302,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def convert(self, project_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
@@ -353,17 +357,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_snapshots(
@@ -405,17 +411,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ProjectSnapshotsResponse, _response.json())  # type: ignore
+            return typing.cast(ProjectSnapshotsResponse, construct_type(type_=ProjectSnapshotsResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def stream_audio(
@@ -466,15 +474,17 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update_pronunciation_dictionaries(
@@ -536,17 +546,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -585,17 +597,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetProjectsResponse, _response.json())  # type: ignore
+            return typing.cast(GetProjectsResponse, construct_type(type_=GetProjectsResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def add(
@@ -721,17 +735,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AddProjectResponseModel, _response.json())  # type: ignore
+            return typing.cast(AddProjectResponseModel, construct_type(type_=AddProjectResponseModel, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(
@@ -773,17 +789,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ProjectExtendedResponseModel, _response.json())  # type: ignore
+            return typing.cast(ProjectExtendedResponseModel, construct_type(type_=ProjectExtendedResponseModel, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, project_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
@@ -823,17 +841,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def convert(self, project_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
@@ -876,17 +896,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_snapshots(
@@ -928,17 +950,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ProjectSnapshotsResponse, _response.json())  # type: ignore
+            return typing.cast(ProjectSnapshotsResponse, construct_type(type_=ProjectSnapshotsResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def stream_audio(
@@ -989,15 +1013,17 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update_pronunciation_dictionaries(
@@ -1059,15 +1085,17 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/realtime_tts.py` & `elevenlabs-1.1.0/src/elevenlabs/realtime_tts.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.5/src/elevenlabs/samples/client.py` & `elevenlabs-1.1.0/src/elevenlabs/samples/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,22 +5,18 @@
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.http_validation_error import HttpValidationError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 
 class SamplesClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def delete(
         self, voice_id: str, sample_id: str, *, request_options: typing.Optional[RequestOptions] = None
@@ -65,17 +61,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_audio(
@@ -123,15 +121,17 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -182,17 +182,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_audio(
@@ -240,13 +242,15 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/speech_to_speech/client.py` & `elevenlabs-1.1.0/src/elevenlabs/speech_to_speech/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.5/src/elevenlabs/text_to_speech/client.py` & `elevenlabs-1.1.0/src/elevenlabs/text_to_speech/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/__init__.py` & `elevenlabs-1.1.0/src/elevenlabs/types/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .accent import Accent
 from .add_project_response_model import AddProjectResponseModel
 from .add_pronunciation_dictionary_response_model import AddPronunciationDictionaryResponseModel
+from .add_pronunciation_dictionary_rules_response_model import AddPronunciationDictionaryRulesResponseModel
 from .add_voice_response_model import AddVoiceResponseModel
 from .age import Age
 from .audio_native_create_project_response_model import AudioNativeCreateProjectResponseModel
 from .audio_native_get_embed_code_response_model import AudioNativeGetEmbedCodeResponseModel
 from .audio_output import AudioOutput
 from .chapter_response import ChapterResponse
 from .chapter_snapshot_response import ChapterSnapshotResponse
@@ -41,17 +42,20 @@
 from .optimize_streaming_latency import OptimizeStreamingLatency
 from .output_format import OutputFormat
 from .project_extended_response_model import ProjectExtendedResponseModel
 from .project_response import ProjectResponse
 from .project_snapshot_response import ProjectSnapshotResponse
 from .project_snapshots_response import ProjectSnapshotsResponse
 from .project_state import ProjectState
+from .pronunciation_dictionary_alias_rule_request_model import PronunciationDictionaryAliasRuleRequestModel
+from .pronunciation_dictionary_phoneme_rule_request_model import PronunciationDictionaryPhonemeRuleRequestModel
 from .pronunciation_dictionary_version_locator import PronunciationDictionaryVersionLocator
 from .realtime_voice_settings import RealtimeVoiceSettings
 from .recording_response import RecordingResponse
+from .remove_pronunciation_dictionary_rules_response_model import RemovePronunciationDictionaryRulesResponseModel
 from .review_status import ReviewStatus
 from .send_text import SendText
 from .source import Source
 from .speech_history_item_response import SpeechHistoryItemResponse
 from .speech_history_item_response_model_voice_category import SpeechHistoryItemResponseModelVoiceCategory
 from .sso_provider_db_model import SsoProviderDbModel
 from .sso_provider_db_model_provider_type import SsoProviderDbModelProviderType
@@ -73,14 +77,15 @@
 from .voice_sharing_state import VoiceSharingState
 from .voice_verification_response import VoiceVerificationResponse
 
 __all__ = [
     "Accent",
     "AddProjectResponseModel",
     "AddPronunciationDictionaryResponseModel",
+    "AddPronunciationDictionaryRulesResponseModel",
     "AddVoiceResponseModel",
     "Age",
     "AudioNativeCreateProjectResponseModel",
     "AudioNativeGetEmbedCodeResponseModel",
     "AudioOutput",
     "ChapterResponse",
     "ChapterSnapshotResponse",
@@ -115,17 +120,20 @@
     "OptimizeStreamingLatency",
     "OutputFormat",
     "ProjectExtendedResponseModel",
     "ProjectResponse",
     "ProjectSnapshotResponse",
     "ProjectSnapshotsResponse",
     "ProjectState",
+    "PronunciationDictionaryAliasRuleRequestModel",
+    "PronunciationDictionaryPhonemeRuleRequestModel",
     "PronunciationDictionaryVersionLocator",
     "RealtimeVoiceSettings",
     "RecordingResponse",
+    "RemovePronunciationDictionaryRulesResponseModel",
     "ReviewStatus",
     "SendText",
     "Source",
     "SpeechHistoryItemResponse",
     "SpeechHistoryItemResponseModelVoiceCategory",
     "SsoProviderDbModel",
     "SsoProviderDbModelProviderType",
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/add_project_response_model.py` & `elevenlabs-1.1.0/src/elevenlabs/types/project_snapshot_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .project_response import ProjectResponse
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AddProjectResponseModel(pydantic.BaseModel):
-    project: ProjectResponse
+class ProjectSnapshotResponse(UncheckedBaseModel):
+    project_snapshot_id: str
+    project_id: str
+    created_at_unix: int
+    name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/add_pronunciation_dictionary_response_model.py` & `elevenlabs-1.1.0/src/elevenlabs/types/user.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .subscription_response import SubscriptionResponse
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AddPronunciationDictionaryResponseModel(pydantic.BaseModel):
-    id: str
-    name: str
-    created_by: str
-    creation_time_unix: int
-    version_id: str
-    description: typing.Optional[str] = None
+class User(UncheckedBaseModel):
+    subscription: SubscriptionResponse
+    is_new_user: bool
+    xi_api_key: str
+    can_use_delayed_payment_methods: bool
+    is_onboarding_completed: bool
+    first_name: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/add_voice_response_model.py` & `elevenlabs-1.1.0/src/elevenlabs/types/audio_native_create_project_response_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AddVoiceResponseModel(pydantic.BaseModel):
-    voice_id: str
+class AudioNativeCreateProjectResponseModel(UncheckedBaseModel):
+    project_id: str
+    converting: bool
+    html_snippet: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/audio_native_create_project_response_model.py` & `elevenlabs-1.1.0/src/elevenlabs/types/get_projects_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .project_response import ProjectResponse
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AudioNativeCreateProjectResponseModel(pydantic.BaseModel):
-    project_id: str
-    converting: bool
-    html_snippet: str
+class GetProjectsResponse(UncheckedBaseModel):
+    projects: typing.List[ProjectResponse]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/audio_output.py` & `elevenlabs-1.1.0/src/elevenlabs/types/audio_output.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .normalized_alignment import NormalizedAlignment
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AudioOutput(pydantic.BaseModel):
-    audio: typing.Optional[str] = pydantic.Field(default=None)
+class AudioOutput(UncheckedBaseModel):
+    audio: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     A generated partial audio chunk, encoded using the selected output_format, by default this
     is MP3 encoded as a base64 string.
     """
 
-    is_final: typing.Optional[bool] = pydantic.Field(alias="isFinal", default=None)
+    is_final: typing.Optional[bool] = pydantic_v1.Field(alias="isFinal", default=None)
     """
     Indicates if the generation is complete. If set to `True`, `audio` will be null.
     """
 
-    normalized_alignment: typing.Optional[NormalizedAlignment] = pydantic.Field(
+    normalized_alignment: typing.Optional[NormalizedAlignment] = pydantic_v1.Field(
         alias="normalizedAlignment", default=None
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
@@ -37,9 +34,9 @@
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/chapter_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/chapter_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .chapter_state import ChapterState
 from .chapter_statistics_response import ChapterStatisticsResponse
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ChapterResponse(pydantic.BaseModel):
+class ChapterResponse(UncheckedBaseModel):
     chapter_id: str
     name: str
     last_conversion_date_unix: int
     conversion_progress: float
     can_be_downloaded: bool
     state: ChapterState
     statistics: ChapterStatisticsResponse
@@ -29,9 +26,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/chapter_snapshot_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/manual_verification_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .manual_verification_file_response import ManualVerificationFileResponse
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ChapterSnapshotResponse(pydantic.BaseModel):
-    chapter_snapshot_id: str
-    project_id: str
-    chapter_id: str
-    created_at_unix: int
-    name: str
+class ManualVerificationResponse(UncheckedBaseModel):
+    extra_text: str
+    request_time_unix: int
+    files: typing.List[ManualVerificationFileResponse]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/chapter_snapshots_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/project_extended_response_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .chapter_snapshot_response import ChapterSnapshotResponse
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class ChapterSnapshotsResponse(pydantic.BaseModel):
-    snapshots: typing.List[ChapterSnapshotResponse]
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .chapter_response import ChapterResponse
+from .project_state import ProjectState
+
+
+class ProjectExtendedResponseModel(UncheckedBaseModel):
+    project_id: str
+    name: str
+    create_date_unix: int
+    default_title_voice_id: str
+    default_paragraph_voice_id: str
+    default_model_id: str
+    last_conversion_date_unix: int
+    can_be_downloaded: bool
+    state: ProjectState
+    chapters: typing.List[ChapterResponse]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/chapter_statistics_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/chapter_statistics_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ChapterStatisticsResponse(pydantic.BaseModel):
+class ChapterStatisticsResponse(UncheckedBaseModel):
     characters_unconverted: int
     characters_converted: int
     paragraphs_converted: int
     paragraphs_unconverted: int
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
@@ -24,9 +21,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/do_dubbing_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/remove_pronunciation_dictionary_rules_response_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class DoDubbingResponse(pydantic.BaseModel):
-    dubbing_id: str
-    expected_duration_sec: float
+class RemovePronunciationDictionaryRulesResponseModel(UncheckedBaseModel):
+    id: str
+    version_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/dubbing_metadata_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/recording_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class DubbingMetadataResponse(pydantic.BaseModel):
-    dubbing_id: str
-    name: str
-    status: str
-    error: str
-    target_languages: typing.List[str]
+class RecordingResponse(UncheckedBaseModel):
+    recording_id: str
+    mime_type: str
+    size_bytes: int
+    upload_date_unix: int
+    transcription: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/feedback_item.py` & `elevenlabs-1.1.0/src/elevenlabs/types/add_pronunciation_dictionary_response_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class FeedbackItem(pydantic.BaseModel):
-    thumbs_up: bool
-    feedback: str
-    emotions: bool
-    inaccurate_clone: bool
-    glitches: bool
-    audio_quality: bool
-    other: bool
-    review_status: typing.Optional[str] = None
+class AddPronunciationDictionaryResponseModel(UncheckedBaseModel):
+    id: str
+    name: str
+    created_by: str
+    creation_time_unix: int
+    version_id: str
+    description: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/fine_tuning_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/fine_tuning_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .finetuning_state import FinetuningState
 from .manual_verification_response import ManualVerificationResponse
 from .verification_attempt_response import VerificationAttemptResponse
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class FineTuningResponse(pydantic.BaseModel):
+class FineTuningResponse(UncheckedBaseModel):
     is_allowed_to_fine_tune: typing.Optional[bool] = None
     finetuning_state: typing.Optional[FinetuningState] = None
     verification_failures: typing.Optional[typing.List[str]] = None
     verification_attempts_count: typing.Optional[int] = None
     manual_verification_requested: typing.Optional[bool] = None
     language: typing.Optional[str] = None
     finetuning_progress: typing.Optional[typing.Dict[str, float]] = None
@@ -35,9 +32,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/generation_config.py` & `elevenlabs-1.1.0/src/elevenlabs/types/generation_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class GenerationConfig(pydantic.BaseModel):
-    chunk_length_schedule: typing.Optional[typing.List[float]] = pydantic.Field(default=None)
+class GenerationConfig(UncheckedBaseModel):
+    chunk_length_schedule: typing.Optional[typing.List[float]] = pydantic_v1.Field(default=None)
     """
     This is an advanced setting that most users shouldn't need to use. It relates to our
     generation schedule explained [here](https://elevenlabs.io/docs/api-reference/websockets#understanding-how-our-websockets-buffer-text).
     
     Determines the minimum amount of text that needs to be sent and present in our
     buffer before audio starts being generated. This is to maximise the amount of context available to
     the model to improve audio quality, whilst balancing latency of the returned audio chunks.
@@ -42,9 +39,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/get_chapters_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/pronunciation_dictionary_version_locator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .chapter_response import ChapterResponse
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class GetChaptersResponse(pydantic.BaseModel):
-    chapters: typing.List[ChapterResponse]
+class PronunciationDictionaryVersionLocator(UncheckedBaseModel):
+    pronunciation_dictionary_id: str
+    version_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/get_library_voices_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/get_voices_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .library_voice_response import LibraryVoiceResponse
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .voice import Voice
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class GetLibraryVoicesResponse(pydantic.BaseModel):
-    voices: typing.List[LibraryVoiceResponse]
-    last_sort_id: str
-    has_more: bool
+class GetVoicesResponse(UncheckedBaseModel):
+    voices: typing.List[Voice]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/get_projects_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/voice_sample.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .project_response import ProjectResponse
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class GetProjectsResponse(pydantic.BaseModel):
-    projects: typing.List[ProjectResponse]
+class VoiceSample(UncheckedBaseModel):
+    sample_id: typing.Optional[str] = None
+    file_name: typing.Optional[str] = None
+    mime_type: typing.Optional[str] = None
+    size_bytes: typing.Optional[int] = None
+    hash: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/get_pronunciation_dictionary_metadata_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/get_pronunciation_dictionary_metadata_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class GetPronunciationDictionaryMetadataResponse(pydantic.BaseModel):
+class GetPronunciationDictionaryMetadataResponse(UncheckedBaseModel):
     id: str
     latest_version_id: str
     name: str
     created_by: str
     creation_time_unix: int
     description: typing.Optional[str] = None
 
@@ -26,9 +23,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/get_speech_history_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/pronunciation_dictionary_alias_rule_request_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .speech_history_item_response import SpeechHistoryItemResponse
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class GetSpeechHistoryResponse(pydantic.BaseModel):
-    history: typing.List[SpeechHistoryItemResponse]
-    last_history_item_id: str
-    has_more: bool
+class PronunciationDictionaryAliasRuleRequestModel(UncheckedBaseModel):
+    string_to_replace: str
+    alias: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/get_voices_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/add_voice_response_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .voice import Voice
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class GetVoicesResponse(pydantic.BaseModel):
-    voices: typing.List[Voice]
+class AddVoiceResponseModel(UncheckedBaseModel):
+    voice_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/history_item.py` & `elevenlabs-1.1.0/src/elevenlabs/types/voice_generation_parameter_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .voice_generation_parameter_option_response import VoiceGenerationParameterOptionResponse
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class HistoryItem(pydantic.BaseModel):
-    state: typing.Optional[typing.Any] = None
-    voice_category: typing.Optional[typing.Any] = None
+class VoiceGenerationParameterResponse(UncheckedBaseModel):
+    genders: typing.List[VoiceGenerationParameterOptionResponse]
+    accents: typing.List[VoiceGenerationParameterOptionResponse]
+    ages: typing.List[VoiceGenerationParameterOptionResponse]
+    minimum_characters: int
+    maximum_characters: int
+    minimum_accent_strength: float
+    maximum_accent_strength: float
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/http_validation_error.py` & `elevenlabs-1.1.0/src/elevenlabs/types/voice_settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .validation_error import ValidationError
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class HttpValidationError(pydantic.BaseModel):
-    detail: typing.Optional[typing.List[ValidationError]] = None
+class VoiceSettings(UncheckedBaseModel):
+    stability: typing.Optional[float] = None
+    similarity_boost: typing.Optional[float] = None
+    style: typing.Optional[float] = None
+    use_speaker_boost: typing.Optional[bool] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/invoice.py` & `elevenlabs-1.1.0/src/elevenlabs/types/invoice.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Invoice(pydantic.BaseModel):
+class Invoice(UncheckedBaseModel):
     amount_due_cents: int
     next_payment_attempt_unix: int
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/language_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/get_chapters_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .chapter_response import ChapterResponse
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class LanguageResponse(pydantic.BaseModel):
-    language_id: str
-    name: str
+class GetChaptersResponse(UncheckedBaseModel):
+    chapters: typing.List[ChapterResponse]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/library_voice_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/library_voice_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,52 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class LibraryVoiceResponse(pydantic.BaseModel):
+class LibraryVoiceResponse(UncheckedBaseModel):
     public_owner_id: str
     voice_id: str
     date_unix: int
     name: str
     accent: str
     gender: str
     age: str
     descriptive: str
     use_case: str
     category: str
     language: str
     description: str
     preview_url: str
-    usage_character_count_1_y: int = pydantic.Field(alias="usage_character_count_1y")
-    usage_character_count_7_d: int = pydantic.Field(alias="usage_character_count_7d")
+    usage_character_count_1_y: int = pydantic_v1.Field(alias="usage_character_count_1y")
+    usage_character_count_7_d: int = pydantic_v1.Field(alias="usage_character_count_7d")
     cloned_by_count: int
     rate: float
     free_users_allowed: bool
     live_moderation_enabled: bool
     notice_period: int
-    instagram_username: str
-    twitter_username: str
-    youtube_username: str
-    tiktok_username: str
     featured: bool
+    instagram_username: typing.Optional[str] = None
+    twitter_username: typing.Optional[str] = None
+    youtube_username: typing.Optional[str] = None
+    tiktok_username: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/manual_verification_file_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/manual_verification_file_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ManualVerificationFileResponse(pydantic.BaseModel):
+class ManualVerificationFileResponse(UncheckedBaseModel):
     file_id: str
     file_name: str
     mime_type: str
     size_bytes: int
     upload_date_unix: int
 
     def json(self, **kwargs: typing.Any) -> str:
@@ -25,9 +22,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/manual_verification_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/http_validation_error.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .manual_verification_file_response import ManualVerificationFileResponse
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .validation_error import ValidationError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ManualVerificationResponse(pydantic.BaseModel):
-    extra_text: str
-    request_time_unix: int
-    files: typing.List[ManualVerificationFileResponse]
+class HttpValidationError(UncheckedBaseModel):
+    detail: typing.Optional[typing.List[ValidationError]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/model.py` & `elevenlabs-1.1.0/src/elevenlabs/types/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .language_response import LanguageResponse
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Model(pydantic.BaseModel):
+class Model(UncheckedBaseModel):
     model_id: str
     name: typing.Optional[str] = None
     can_be_finetuned: typing.Optional[bool] = None
     can_do_text_to_speech: typing.Optional[bool] = None
     can_do_voice_conversion: typing.Optional[bool] = None
     can_use_style: typing.Optional[bool] = None
     can_use_speaker_boost: typing.Optional[bool] = None
@@ -35,9 +32,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/normalized_alignment.py` & `elevenlabs-1.1.0/src/elevenlabs/types/normalized_alignment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class NormalizedAlignment(pydantic.BaseModel):
+class NormalizedAlignment(UncheckedBaseModel):
     """
     Alignment information for the generated audio given the input normalized text sequence.
     """
 
-    char_start_times_ms: typing.Optional[typing.List[int]] = pydantic.Field(default=None)
+    char_start_times_ms: typing.Optional[typing.List[int]] = pydantic_v1.Field(default=None)
     """
     A list of starting times (in milliseconds) for each character in the normalized text as it
     corresponds to the audio. For instance, the character 'H' starts at time 0 ms in the audio.  
     Note these times are relative to the returned chunk from the model, and not the
     full audio response.
     """
 
-    chars_durations_ms: typing.Optional[typing.List[int]] = pydantic.Field(default=None)
+    chars_durations_ms: typing.Optional[typing.List[int]] = pydantic_v1.Field(default=None)
     """
     A list of durations (in milliseconds) for each character in the normalized text as it
     corresponds to the audio. For instance, the character 'H' lasts for 3 ms in the audio.  
     Note these times are relative to the returned chunk from the model, and not the
     full audio response.
     """
 
-    chars: typing.Optional[typing.List[str]] = pydantic.Field(default=None)
+    chars: typing.Optional[typing.List[str]] = pydantic_v1.Field(default=None)
     """
     A list of characters in the normalized text sequence. For instance, the first character is 'H'.
     Note that this list may contain spaces, punctuation, and other special characters.
     The length of this list should be the same as the lengths of `char_start_times_ms` and `chars_durations_ms`.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
@@ -46,9 +43,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/project_extended_response_model.py` & `elevenlabs-1.1.0/src/elevenlabs/types/project_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .chapter_response import ChapterResponse
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .project_state import ProjectState
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ProjectExtendedResponseModel(pydantic.BaseModel):
+class ProjectResponse(UncheckedBaseModel):
     project_id: str
     name: str
     create_date_unix: int
     default_title_voice_id: str
     default_paragraph_voice_id: str
     default_model_id: str
     last_conversion_date_unix: int
     can_be_downloaded: bool
+    title: str
+    author: str
+    isbn_number: str
+    volume_normalization: bool
     state: ProjectState
-    chapters: typing.List[ChapterResponse]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/project_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/feedback_item.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .project_state import ProjectState
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class ProjectResponse(pydantic.BaseModel):
-    project_id: str
-    name: str
-    create_date_unix: int
-    default_title_voice_id: str
-    default_paragraph_voice_id: str
-    default_model_id: str
-    last_conversion_date_unix: int
-    can_be_downloaded: bool
-    title: str
-    author: str
-    isbn_number: str
-    volume_normalization: bool
-    state: ProjectState
+
+class FeedbackItem(UncheckedBaseModel):
+    thumbs_up: bool
+    feedback: str
+    emotions: bool
+    inaccurate_clone: bool
+    glitches: bool
+    audio_quality: bool
+    other: bool
+    review_status: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/project_snapshot_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/chapter_snapshot_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ProjectSnapshotResponse(pydantic.BaseModel):
-    project_snapshot_id: str
+class ChapterSnapshotResponse(UncheckedBaseModel):
+    chapter_snapshot_id: str
     project_id: str
+    chapter_id: str
     created_at_unix: int
     name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/project_snapshots_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/project_snapshots_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .project_snapshot_response import ProjectSnapshotResponse
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ProjectSnapshotsResponse(pydantic.BaseModel):
+class ProjectSnapshotsResponse(UncheckedBaseModel):
     snapshots: typing.List[ProjectSnapshotResponse]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/pronunciation_dictionary_version_locator.py` & `elevenlabs-1.1.0/src/elevenlabs/types/pronunciation_dictionary_phoneme_rule_request_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class PronunciationDictionaryVersionLocator(pydantic.BaseModel):
-    pronunciation_dictionary_id: str
-    version_id: str
+class PronunciationDictionaryPhonemeRuleRequestModel(UncheckedBaseModel):
+    string_to_replace: str
+    phoneme: str
+    alphabet: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/realtime_voice_settings.py` & `elevenlabs-1.1.0/src/elevenlabs/types/realtime_voice_settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class RealtimeVoiceSettings(pydantic.BaseModel):
-    stability: float = pydantic.Field()
+class RealtimeVoiceSettings(UncheckedBaseModel):
+    stability: float = pydantic_v1.Field()
     """
     Defines the stability for voice settings.
     """
 
-    similarity_boost: float = pydantic.Field()
+    similarity_boost: float = pydantic_v1.Field()
     """
     Defines the similarity boost for voice settings.
     """
 
-    style: typing.Optional[float] = pydantic.Field(default=None)
+    style: typing.Optional[float] = pydantic_v1.Field(default=None)
     """
     Defines the style for voice settings. This parameter is available on V2+ models.
     """
 
-    use_speaker_boost: typing.Optional[bool] = pydantic.Field(default=None)
+    use_speaker_boost: typing.Optional[bool] = pydantic_v1.Field(default=None)
     """
     Defines the use speaker boost for voice settings. This parameter is available on V2+ models.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -39,9 +36,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/recording_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/validation_error.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .validation_error_loc_item import ValidationErrorLocItem
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class RecordingResponse(pydantic.BaseModel):
-    recording_id: str
-    mime_type: str
-    size_bytes: int
-    upload_date_unix: int
-    transcription: str
+class ValidationError(UncheckedBaseModel):
+    loc: typing.List[ValidationErrorLocItem]
+    msg: str
+    type: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/send_text.py` & `elevenlabs-1.1.0/src/elevenlabs/types/send_text.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .generation_config import GenerationConfig
 from .realtime_voice_settings import RealtimeVoiceSettings
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SendText(pydantic.BaseModel):
-    text: str = pydantic.Field()
+class SendText(UncheckedBaseModel):
+    text: str = pydantic_v1.Field()
     """
     Should always end with a single space string `" "`. In the first message, the text should be a space `" "`.
     """
 
-    try_trigger_generation: typing.Optional[bool] = pydantic.Field(default=None)
+    try_trigger_generation: typing.Optional[bool] = pydantic_v1.Field(default=None)
     """
     This is an advanced setting that most users shouldn't need to use. It relates to our generation schedule
     explained [here](#understanding-how-our-websockets-buffer-text).
     
     Use this to attempt to immediately trigger the generation of audio, overriding the `chunk_length_schedule`.
     Unlike flush, `try_trigger_generation` will only generate audio if our
     buffer contains more than a minimum
@@ -32,15 +29,15 @@
     Note that overriding the chunk schedule to generate small amounts of
     text may result in lower quality audio, therefore, only use this parameter if you
     really need text to be processed immediately. We generally recommend keeping the default value of
     `false` and adjusting the `chunk_length_schedule` in the `generation_config` instead.
     """
 
     voice_settings: typing.Optional[RealtimeVoiceSettings] = None
-    generation_config: typing.Optional[GenerationConfig] = pydantic.Field(default=None)
+    generation_config: typing.Optional[GenerationConfig] = pydantic_v1.Field(default=None)
     """
     This property should only be provided in the first message you send.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -48,9 +45,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/speech_history_item_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/speech_history_item_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .feedback_item import FeedbackItem
 from .source import Source
 from .speech_history_item_response_model_voice_category import SpeechHistoryItemResponseModelVoiceCategory
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SpeechHistoryItemResponse(pydantic.BaseModel):
+class SpeechHistoryItemResponse(UncheckedBaseModel):
     history_item_id: str
     request_id: typing.Optional[str] = None
     voice_id: typing.Optional[str] = None
     model_id: typing.Optional[str] = None
     voice_name: typing.Optional[str] = None
     voice_category: typing.Optional[SpeechHistoryItemResponseModelVoiceCategory] = None
     text: typing.Optional[str] = None
@@ -39,9 +36,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/sso_provider_db_model.py` & `elevenlabs-1.1.0/src/elevenlabs/types/history_item.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .sso_provider_db_model_provider_type import SsoProviderDbModelProviderType
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SsoProviderDbModel(pydantic.BaseModel):
-    provider_type: SsoProviderDbModelProviderType
-    provider_id: str
-    domains: typing.List[str]
+class HistoryItem(UncheckedBaseModel):
+    state: typing.Optional[typing.Any] = None
+    voice_category: typing.Optional[typing.Any] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/subscription.py` & `elevenlabs-1.1.0/src/elevenlabs/types/subscription.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .currency import Currency
 from .extended_subscription_response_model_billing_period import ExtendedSubscriptionResponseModelBillingPeriod
 from .invoice import Invoice
 from .subscription_status import SubscriptionStatus
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Subscription(pydantic.BaseModel):
+class Subscription(UncheckedBaseModel):
     tier: str
     character_count: int
     character_limit: int
     can_extend_character_limit: bool
     allowed_to_extend_character_limit: bool
     next_character_count_reset_unix: int
     voice_limit: int
@@ -42,9 +39,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/subscription_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/subscription_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .currency import Currency
 from .subscription_response_model_billing_period import SubscriptionResponseModelBillingPeriod
 from .subscription_status import SubscriptionStatus
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SubscriptionResponse(pydantic.BaseModel):
+class SubscriptionResponse(UncheckedBaseModel):
     tier: str
     character_count: int
     character_limit: int
     can_extend_character_limit: bool
     allowed_to_extend_character_limit: bool
     next_character_count_reset_unix: int
     voice_limit: int
@@ -39,9 +36,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/user.py` & `elevenlabs-1.1.0/src/elevenlabs/types/do_dubbing_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .subscription_response import SubscriptionResponse
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class User(pydantic.BaseModel):
-    subscription: SubscriptionResponse
-    is_new_user: bool
-    xi_api_key: str
-    can_use_delayed_payment_methods: bool
-    is_onboarding_completed: bool
-    first_name: typing.Optional[str] = None
+class DoDubbingResponse(UncheckedBaseModel):
+    dubbing_id: str
+    expected_duration_sec: float
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/validation_error.py` & `elevenlabs-1.1.0/src/elevenlabs/types/add_pronunciation_dictionary_rules_response_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .validation_error_loc_item import ValidationErrorLocItem
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ValidationError(pydantic.BaseModel):
-    loc: typing.List[ValidationErrorLocItem]
-    msg: str
-    type: str
+class AddPronunciationDictionaryRulesResponseModel(UncheckedBaseModel):
+    id: str
+    version_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/voice.py` & `elevenlabs-1.1.0/src/elevenlabs/types/voice.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .fine_tuning_response import FineTuningResponse
 from .voice_response_model_safety_control import VoiceResponseModelSafetyControl
 from .voice_sample import VoiceSample
 from .voice_settings import VoiceSettings
 from .voice_sharing_response import VoiceSharingResponse
 from .voice_verification_response import VoiceVerificationResponse
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Voice(pydantic.BaseModel):
+class Voice(UncheckedBaseModel):
     voice_id: str
     name: typing.Optional[str] = None
     samples: typing.Optional[typing.List[VoiceSample]] = None
     category: typing.Optional[str] = None
     fine_tuning: typing.Optional[FineTuningResponse] = None
     labels: typing.Optional[typing.Dict[str, str]] = None
     description: typing.Optional[str] = None
@@ -42,9 +39,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/voice_generation_parameter_option_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/voice_generation_parameter_option_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class VoiceGenerationParameterOptionResponse(pydantic.BaseModel):
+class VoiceGenerationParameterOptionResponse(UncheckedBaseModel):
     name: str
     code: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/voice_generation_parameter_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/sso_provider_db_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .voice_generation_parameter_option_response import VoiceGenerationParameterOptionResponse
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .sso_provider_db_model_provider_type import SsoProviderDbModelProviderType
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class VoiceGenerationParameterResponse(pydantic.BaseModel):
-    genders: typing.List[VoiceGenerationParameterOptionResponse]
-    accents: typing.List[VoiceGenerationParameterOptionResponse]
-    ages: typing.List[VoiceGenerationParameterOptionResponse]
-    minimum_characters: int
-    maximum_characters: int
-    minimum_accent_strength: float
-    maximum_accent_strength: float
+
+class SsoProviderDbModel(UncheckedBaseModel):
+    provider_type: SsoProviderDbModelProviderType
+    provider_id: str
+    domains: typing.List[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/voice_sample.py` & `elevenlabs-1.1.0/src/elevenlabs/types/get_speech_history_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .speech_history_item_response import SpeechHistoryItemResponse
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class VoiceSample(pydantic.BaseModel):
-    sample_id: typing.Optional[str] = None
-    file_name: typing.Optional[str] = None
-    mime_type: typing.Optional[str] = None
-    size_bytes: typing.Optional[int] = None
-    hash: typing.Optional[str] = None
+class GetSpeechHistoryResponse(UncheckedBaseModel):
+    history: typing.List[SpeechHistoryItemResponse]
+    last_history_item_id: str
+    has_more: bool
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/voice_sharing_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/voice_sharing_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .review_status import ReviewStatus
 from .voice_sharing_state import VoiceSharingState
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class VoiceSharingResponse(pydantic.BaseModel):
+class VoiceSharingResponse(UncheckedBaseModel):
     status: typing.Optional[VoiceSharingState] = None
     history_item_sample_id: typing.Optional[str] = None
     date_unix: typing.Optional[int] = None
     whitelisted_emails: typing.Optional[typing.List[str]] = None
     public_owner_id: typing.Optional[str] = None
     original_voice_id: typing.Optional[str] = None
     financial_rewards_enabled: typing.Optional[bool] = None
@@ -49,9 +46,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/types/voice_verification_response.py` & `elevenlabs-1.1.0/src/elevenlabs/types/voice_verification_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .verification_attempt_response import VerificationAttemptResponse
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class VoiceVerificationResponse(pydantic.BaseModel):
+class VoiceVerificationResponse(UncheckedBaseModel):
     requires_verification: bool
     is_verified: bool
     verification_failures: typing.List[str]
     verification_attempts_count: int
     language: typing.Optional[str] = None
     verification_attempts: typing.Optional[typing.List[VerificationAttemptResponse]] = None
 
@@ -27,9 +24,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        extra = pydantic.Extra.allow
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/user/client.py` & `elevenlabs-1.1.0/src/elevenlabs/user/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,24 +5,20 @@
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.http_validation_error import HttpValidationError
 from ..types.subscription import Subscription
 from ..types.user import User
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 
 class UserClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def get_subscription(self, *, request_options: typing.Optional[RequestOptions] = None) -> Subscription:
         """
@@ -55,17 +51,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Subscription, _response.json())  # type: ignore
+            return typing.cast(Subscription, construct_type(type_=Subscription, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, *, request_options: typing.Optional[RequestOptions] = None) -> User:
@@ -99,17 +97,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(User, _response.json())  # type: ignore
+            return typing.cast(User, construct_type(type_=User, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -148,17 +148,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Subscription, _response.json())  # type: ignore
+            return typing.cast(Subscription, construct_type(type_=Subscription, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(self, *, request_options: typing.Optional[RequestOptions] = None) -> User:
@@ -192,15 +194,17 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(User, _response.json())  # type: ignore
+            return typing.cast(User, construct_type(type_=User, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/voice_generation/client.py` & `elevenlabs-1.1.0/src/elevenlabs/voice_generation/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,22 @@
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.age import Age
 from ..types.gender import Gender
 from ..types.http_validation_error import HttpValidationError
 from ..types.voice import Voice
 from ..types.voice_generation_parameter_response import VoiceGenerationParameterResponse
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class VoiceGenerationClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
@@ -64,15 +60,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(VoiceGenerationParameterResponse, _response.json())  # type: ignore
+            return typing.cast(VoiceGenerationParameterResponse, construct_type(type_=VoiceGenerationParameterResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def generate(
@@ -219,17 +215,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Voice, _response.json())  # type: ignore
+            return typing.cast(Voice, construct_type(type_=Voice, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -272,15 +270,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(VoiceGenerationParameterResponse, _response.json())  # type: ignore
+            return typing.cast(VoiceGenerationParameterResponse, construct_type(type_=VoiceGenerationParameterResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def generate(
@@ -427,15 +425,17 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Voice, _response.json())  # type: ignore
+            return typing.cast(Voice, construct_type(type_=Voice, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `elevenlabs-1.0.5/src/elevenlabs/voices/client.py` & `elevenlabs-1.1.0/src/elevenlabs/voices/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,27 +6,23 @@
 
 from .. import core
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.add_voice_response_model import AddVoiceResponseModel
 from ..types.get_library_voices_response import GetLibraryVoicesResponse
 from ..types.get_voices_response import GetVoicesResponse
 from ..types.http_validation_error import HttpValidationError
 from ..types.voice import Voice
 from ..types.voice_settings import VoiceSettings
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class VoicesClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
@@ -62,17 +58,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetVoicesResponse, _response.json())  # type: ignore
+            return typing.cast(GetVoicesResponse, construct_type(type_=GetVoicesResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_default_settings(self, *, request_options: typing.Optional[RequestOptions] = None) -> VoiceSettings:
@@ -106,15 +104,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(VoiceSettings, _response.json())  # type: ignore
+            return typing.cast(VoiceSettings, construct_type(type_=VoiceSettings, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_settings(self, voice_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> VoiceSettings:
@@ -154,17 +152,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(VoiceSettings, _response.json())  # type: ignore
+            return typing.cast(VoiceSettings, construct_type(type_=VoiceSettings, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(
@@ -219,17 +219,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Voice, _response.json())  # type: ignore
+            return typing.cast(Voice, construct_type(type_=Voice, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, voice_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
@@ -267,17 +269,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def edit_settings(
@@ -329,17 +333,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def add(
@@ -396,17 +402,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AddVoiceResponseModel, _response.json())  # type: ignore
+            return typing.cast(AddVoiceResponseModel, construct_type(type_=AddVoiceResponseModel, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def edit(
@@ -470,17 +478,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def add_sharing_voice(
@@ -540,17 +550,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AddVoiceResponseModel, _response.json())  # type: ignore
+            return typing.cast(AddVoiceResponseModel, construct_type(type_=AddVoiceResponseModel, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_shared(
@@ -644,17 +656,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetLibraryVoicesResponse, _response.json())  # type: ignore
+            return typing.cast(GetLibraryVoicesResponse, construct_type(type_=GetLibraryVoicesResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -693,17 +707,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetVoicesResponse, _response.json())  # type: ignore
+            return typing.cast(GetVoicesResponse, construct_type(type_=GetVoicesResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_default_settings(self, *, request_options: typing.Optional[RequestOptions] = None) -> VoiceSettings:
@@ -737,15 +753,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(VoiceSettings, _response.json())  # type: ignore
+            return typing.cast(VoiceSettings, construct_type(type_=VoiceSettings, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_settings(
@@ -787,17 +803,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(VoiceSettings, _response.json())  # type: ignore
+            return typing.cast(VoiceSettings, construct_type(type_=VoiceSettings, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(
@@ -852,17 +870,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Voice, _response.json())  # type: ignore
+            return typing.cast(Voice, construct_type(type_=Voice, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, voice_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
@@ -900,17 +920,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def edit_settings(
@@ -962,17 +984,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def add(
@@ -1029,17 +1053,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AddVoiceResponseModel, _response.json())  # type: ignore
+            return typing.cast(AddVoiceResponseModel, construct_type(type_=AddVoiceResponseModel, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def edit(
@@ -1103,17 +1129,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def add_sharing_voice(
@@ -1173,17 +1201,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AddVoiceResponseModel, _response.json())  # type: ignore
+            return typing.cast(AddVoiceResponseModel, construct_type(type_=AddVoiceResponseModel, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_shared(
@@ -1277,15 +1307,17 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetLibraryVoicesResponse, _response.json())  # type: ignore
+            return typing.cast(GetLibraryVoicesResponse, construct_type(type_=GetLibraryVoicesResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `elevenlabs-1.0.5/PKG-INFO` & `elevenlabs-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabs
-Version: 1.0.5
+Version: 1.1.0
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

