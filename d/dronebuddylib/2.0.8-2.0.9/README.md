# Comparing `tmp/dronebuddylib-2.0.8.tar.gz` & `tmp/dronebuddylib-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dronebuddylib-2.0.8.tar", last modified: Mon Jan  8 02:23:13 2024, max compression
+gzip compressed data, was "dronebuddylib-2.0.9.tar", last modified: Mon Jan  8 02:52:03 2024, max compression
```

## Comparing `dronebuddylib-2.0.8.tar` & `dronebuddylib-2.0.9.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxrwx   0        0        0        0 2024-01-08 02:23:13.165570 dronebuddylib-2.0.8/
--rw-rw-rw-   0        0        0     1349 2023-11-17 03:03:13.000000 dronebuddylib-2.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      740 2024-01-08 02:23:13.165570 dronebuddylib-2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      855 2023-10-09 06:33:51.000000 dronebuddylib-2.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-01-08 02:23:12.663847 dronebuddylib-2.0.8/dronebuddylib/
--rw-rw-rw-   0        0        0      157 2024-01-08 02:22:34.000000 dronebuddylib-2.0.8/dronebuddylib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-08 02:23:12.679472 dronebuddylib-2.0.8/dronebuddylib/atoms/
--rw-rw-rw-   0        0        0      823 2024-01-08 02:22:34.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-08 02:23:12.713310 dronebuddylib-2.0.8/dronebuddylib/atoms/bodyfeatureextraction/
--rw-rw-rw-   0        0        0      286 2024-01-08 02:22:34.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/bodyfeatureextraction/__init__.py
--rw-rw-rw-   0        0        0     6549 2024-01-04 13:23:37.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/bodyfeatureextraction/body_feature_extraction_impl.py
--rw-rw-rw-   0        0        0     9496 2024-01-04 13:56:21.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/bodyfeatureextraction/hand_feature_extraction_impl.py
--rw-rw-rw-   0        0        0     3904 2023-11-02 09:58:20.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/bodyfeatureextraction/head_feature_extraction_impl.py
--rw-rw-rw-   0        0        0      605 2023-11-02 09:56:42.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/bodyfeatureextraction/i_feature_extraction.py
-drwxrwxrwx   0        0        0        0 2024-01-08 02:23:12.726816 dronebuddylib-2.0.8/dronebuddylib/atoms/facerecognition/
--rw-rw-rw-   0        0        0      131 2024-01-08 02:22:34.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/facerecognition/__init__.py
--rw-rw-rw-   0        0        0     1809 2024-01-05 11:02:41.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/facerecognition/face_recognition_engine.py
--rw-rw-rw-   0        0        0     7098 2024-01-03 08:40:23.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/facerecognition/face_recognition_impl.py
--rw-rw-rw-   0        0        0     1462 2023-11-02 09:51:24.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/facerecognition/i_face_recognition.py
--rw-rw-rw-   0        0        0      590 2023-10-25 04:01:33.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/gpt_integration.py
-drwxrwxrwx   0        0        0        0 2024-01-08 02:23:12.742473 dronebuddylib-2.0.8/dronebuddylib/atoms/intentrecognition/
--rw-rw-rw-   0        0        0      223 2024-01-08 02:22:34.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/intentrecognition/__init__.py
--rw-rw-rw-   0        0        0     7344 2024-01-05 06:18:46.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/intentrecognition/gpt_intent_recognition_impl.py
--rw-rw-rw-   0        0        0     1889 2024-01-05 06:18:46.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/intentrecognition/i_intent_recognition.py
--rw-rw-rw-   0        0        0     4650 2024-01-05 11:02:41.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/intentrecognition/intent_recognition_engine.py
--rw-rw-rw-   0        0        0      517 2024-01-02 03:33:07.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/intentrecognition/recognized_intent.py
--rw-rw-rw-   0        0        0     6452 2024-01-05 06:18:46.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/intentrecognition/snips_intent_recognition_impl.py
-drwxrwxrwx   0        0        0        0 2024-01-08 02:23:12.773777 dronebuddylib-2.0.8/dronebuddylib/atoms/objectdetection/
--rw-rw-rw-   0        0        0      201 2024-01-08 02:22:34.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/objectdetection/__init__.py
--rw-rw-rw-   0        0        0      976 2024-01-05 06:18:46.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/objectdetection/detected_object.py
--rw-rw-rw-   0        0        0     1457 2024-01-05 06:18:46.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/objectdetection/i_object_detection.py
--rw-rw-rw-   0        0        0     4925 2024-01-05 06:18:46.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/objectdetection/mp_object_detection_impl.py
--rw-rw-rw-   0        0        0     2071 2024-01-05 11:02:41.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/objectdetection/object_detection_engine.py
--rw-rw-rw-   0        0        0     4091 2024-01-05 06:18:46.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/objectdetection/yolo_object_detection_impl.py
-drwxrwxrwx   0        0        0        0 2024-01-08 02:23:12.821046 dronebuddylib-2.0.8/dronebuddylib/atoms/speechgeneration/
--rw-rw-rw-   0        0        0      210 2024-01-08 02:22:34.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/speechgeneration/__init__.py
--rw-rw-rw-   0        0        0     2194 2023-11-02 09:38:49.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/speechgeneration/i_speech_generation.py
--rw-rw-rw-   0        0        0     1318 2024-01-05 11:02:41.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/speechgeneration/speech_generation_engine.py
--rw-rw-rw-   0        0        0     4865 2024-01-04 11:53:55.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/speechgeneration/tts_speech_generation_impl.py
-drwxrwxrwx   0        0        0        0 2024-01-08 02:23:12.898335 dronebuddylib-2.0.8/dronebuddylib/atoms/speechrecognition/
--rw-rw-rw-   0        0        0      561 2024-01-08 02:22:34.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/speechrecognition/__init__.py
--rw-rw-rw-   0        0        0     6786 2024-01-05 06:18:46.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/speechrecognition/google_speech_recognition_impl.py
--rw-rw-rw-   0        0        0     1282 2024-01-05 06:18:46.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/speechrecognition/i_speech_recognition.py
--rw-rw-rw-   0        0        0     3591 2024-01-03 04:05:34.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/speechrecognition/microphone_stream.py
--rw-rw-rw-   0        0        0     8549 2024-01-05 06:18:46.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/speechrecognition/multi_algo_speech_recognition_impl.py
--rw-rw-rw-   0        0        0      170 2024-01-02 07:52:24.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/speechrecognition/recognized_speech.py
--rw-rw-rw-   0        0        0     5544 2024-01-03 06:03:35.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/speechrecognition/resumable_microphone_stream.py
--rw-rw-rw-   0        0        0     2493 2024-01-05 11:02:41.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/speechrecognition/speech_recognition_engine.py
--rw-rw-rw-   0        0        0     3965 2024-01-05 06:18:46.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/speechrecognition/vosk_speech_recognition_impl.py
-drwxrwxrwx   0        0        0        0 2024-01-08 02:23:12.945695 dronebuddylib-2.0.8/dronebuddylib/atoms/textrecognition/
--rw-rw-rw-   0        0        0      204 2024-01-08 02:22:34.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/textrecognition/__init__.py
--rw-rw-rw-   0        0        0     2585 2024-01-04 11:53:55.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/textrecognition/google_text_recognition_impl.py
--rw-rw-rw-   0        0        0      975 2023-12-12 05:56:15.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/textrecognition/i_text_recognition.py
--rw-rw-rw-   0        0        0     1518 2024-01-04 11:53:55.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/textrecognition/text_recognition_engine.py
--rw-rw-rw-   0        0        0      193 2023-12-12 06:04:42.000000 dronebuddylib-2.0.8/dronebuddylib/atoms/textrecognition/text_recognition_result.py
-drwxrwxrwx   0        0        0        0 2024-01-08 02:23:12.961395 dronebuddylib-2.0.8/dronebuddylib/configurations/
--rw-rw-rw-   0        0        0       25 2024-01-08 02:22:34.000000 dronebuddylib-2.0.8/dronebuddylib/configurations/__init__.py
--rw-rw-rw-   0        0        0      109 2023-08-15 12:04:39.000000 dronebuddylib-2.0.8/dronebuddylib/configurations/config.py
-drwxrwxrwx   0        0        0        0 2024-01-08 02:23:12.992672 dronebuddylib-2.0.8/dronebuddylib/exceptions/
--rw-rw-rw-   0        0        0       95 2024-01-05 10:48:22.000000 dronebuddylib-2.0.8/dronebuddylib/exceptions/__init__.py
--rw-rw-rw-   0        0        0      404 2023-12-28 07:54:55.000000 dronebuddylib-2.0.8/dronebuddylib/exceptions/intent_resolution_exception.py
-drwxrwxrwx   0        0        0        0 2024-01-08 02:23:13.071206 dronebuddylib-2.0.8/dronebuddylib/models/
--rw-rw-rw-   0        0        0      169 2024-01-08 02:22:34.000000 dronebuddylib-2.0.8/dronebuddylib/models/__init__.py
--rw-rw-rw-   0        0        0     2893 2023-12-28 09:19:41.000000 dronebuddylib-2.0.8/dronebuddylib/models/chat_session.py
--rw-rw-rw-   0        0        0      465 2023-10-25 04:13:37.000000 dronebuddylib-2.0.8/dronebuddylib/models/conversation.py
--rw-rw-rw-   0        0        0      960 2023-11-02 05:56:23.000000 dronebuddylib-2.0.8/dronebuddylib/models/engine_configurations.py
--rw-rw-rw-   0        0        0     4382 2024-01-03 08:29:30.000000 dronebuddylib-2.0.8/dronebuddylib/models/enums.py
--rw-rw-rw-   0        0        0      418 2023-10-18 05:26:06.000000 dronebuddylib-2.0.8/dronebuddylib/models/gpt_configs.py
--rw-rw-rw-   0        0        0      441 2023-10-27 07:52:14.000000 dronebuddylib-2.0.8/dronebuddylib/models/i_dbl_function.py
--rw-rw-rw-   0        0        0      689 2023-10-25 04:13:44.000000 dronebuddylib-2.0.8/dronebuddylib/models/session_logger.py
--rw-rw-rw-   0        0        0     1878 2023-10-18 05:26:10.000000 dronebuddylib-2.0.8/dronebuddylib/models/token_counter.py
-drwxrwxrwx   0        0        0        0 2024-01-08 02:23:13.113569 dronebuddylib-2.0.8/dronebuddylib/utils/
--rw-rw-rw-   0        0        0       71 2024-01-08 02:22:34.000000 dronebuddylib-2.0.8/dronebuddylib/utils/__init__.py
--rw-rw-rw-   0        0        0     2292 2024-01-02 05:28:44.000000 dronebuddylib-2.0.8/dronebuddylib/utils/chat_prompts.py
--rw-rw-rw-   0        0        0     1739 2024-01-03 07:03:51.000000 dronebuddylib-2.0.8/dronebuddylib/utils/enums.py
--rw-rw-rw-   0        0        0      440 2023-10-18 05:25:47.000000 dronebuddylib-2.0.8/dronebuddylib/utils/exceptions.py
--rw-rw-rw-   0        0        0     1506 2024-01-03 08:56:13.000000 dronebuddylib-2.0.8/dronebuddylib/utils/logging_config.py
--rw-rw-rw-   0        0        0     2201 2024-01-05 03:39:50.000000 dronebuddylib-2.0.8/dronebuddylib/utils/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-08 02:23:13.165570 dronebuddylib-2.0.8/dronebuddylib.egg-info/
--rw-rw-rw-   0        0        0      740 2024-01-08 02:23:12.000000 dronebuddylib-2.0.8/dronebuddylib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3730 2024-01-08 02:23:12.000000 dronebuddylib-2.0.8/dronebuddylib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-08 02:23:12.000000 dronebuddylib-2.0.8/dronebuddylib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-11-02 09:21:08.000000 dronebuddylib-2.0.8/dronebuddylib.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      213 2024-01-08 02:23:12.000000 dronebuddylib-2.0.8/dronebuddylib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-01-08 02:23:12.000000 dronebuddylib-2.0.8/dronebuddylib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      134 2024-01-05 11:17:31.000000 dronebuddylib-2.0.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-01-08 02:23:13.165570 dronebuddylib-2.0.8/setup.cfg
--rw-rw-rw-   0        0        0      862 2024-01-08 02:22:34.000000 dronebuddylib-2.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-08 02:23:13.165570 dronebuddylib-2.0.8/test/
--rw-rw-rw-   0        0        0      373 2024-01-05 06:28:49.000000 dronebuddylib-2.0.8/test/__init__.py
--rw-rw-rw-   0        0        0     2198 2024-01-05 03:49:40.000000 dronebuddylib-2.0.8/test/test_face_recognition.py
--rw-rw-rw-   0        0        0     5514 2024-01-04 14:00:19.000000 dronebuddylib-2.0.8/test/test_feature_extraction.py
--rw-rw-rw-   0        0        0     2436 2024-01-04 12:02:42.000000 dronebuddylib-2.0.8/test/test_intent_recognition.py
--rw-rw-rw-   0        0        0     6134 2024-01-04 13:13:18.000000 dronebuddylib-2.0.8/test/test_object_detection.py
--rw-rw-rw-   0        0        0    12692 2024-01-05 03:53:33.000000 dronebuddylib-2.0.8/test/test_speech_recognition.py
--rw-rw-rw-   0        0        0     3496 2024-01-05 03:53:33.000000 dronebuddylib-2.0.8/test/test_text_recognition.py
--rw-rw-rw-   0        0        0     2272 2024-01-08 02:22:34.000000 dronebuddylib-2.0.8/test/test_update_version.py
+drwxrwxrwx   0        0        0        0 2024-01-08 02:52:03.717541 dronebuddylib-2.0.9/
+-rw-rw-rw-   0        0        0     1349 2023-11-17 03:03:13.000000 dronebuddylib-2.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      740 2024-01-08 02:52:03.717541 dronebuddylib-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      855 2023-10-09 06:33:51.000000 dronebuddylib-2.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-01-08 02:52:03.657367 dronebuddylib-2.0.9/dronebuddylib/
+-rw-rw-rw-   0        0        0      157 2024-01-08 02:49:39.000000 dronebuddylib-2.0.9/dronebuddylib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-08 02:52:03.671092 dronebuddylib-2.0.9/dronebuddylib/atoms/
+-rw-rw-rw-   0        0        0      823 2024-01-08 02:49:39.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-08 02:52:03.671092 dronebuddylib-2.0.9/dronebuddylib/atoms/bodyfeatureextraction/
+-rw-rw-rw-   0        0        0      286 2024-01-08 02:49:39.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/bodyfeatureextraction/__init__.py
+-rw-rw-rw-   0        0        0     6549 2024-01-04 13:23:37.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/bodyfeatureextraction/body_feature_extraction_impl.py
+-rw-rw-rw-   0        0        0     9496 2024-01-04 13:56:21.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/bodyfeatureextraction/hand_feature_extraction_impl.py
+-rw-rw-rw-   0        0        0     3904 2023-11-02 09:58:20.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/bodyfeatureextraction/head_feature_extraction_impl.py
+-rw-rw-rw-   0        0        0      605 2023-11-02 09:56:42.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/bodyfeatureextraction/i_feature_extraction.py
+drwxrwxrwx   0        0        0        0 2024-01-08 02:52:03.677631 dronebuddylib-2.0.9/dronebuddylib/atoms/facerecognition/
+-rw-rw-rw-   0        0        0      133 2024-01-08 02:50:40.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/facerecognition/__init__.py
+-rw-rw-rw-   0        0        0     1809 2024-01-05 11:02:41.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/facerecognition/face_recognition_engine.py
+-rw-rw-rw-   0        0        0     7098 2024-01-03 08:40:23.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/facerecognition/face_recognition_impl.py
+-rw-rw-rw-   0        0        0     1462 2023-11-02 09:51:24.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/facerecognition/i_face_recognition.py
+-rw-rw-rw-   0        0        0      590 2023-10-25 04:01:33.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/gpt_integration.py
+drwxrwxrwx   0        0        0        0 2024-01-08 02:52:03.677631 dronebuddylib-2.0.9/dronebuddylib/atoms/intentrecognition/
+-rw-rw-rw-   0        0        0      223 2024-01-08 02:49:39.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/intentrecognition/__init__.py
+-rw-rw-rw-   0        0        0     7344 2024-01-05 06:18:46.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/intentrecognition/gpt_intent_recognition_impl.py
+-rw-rw-rw-   0        0        0     1889 2024-01-05 06:18:46.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/intentrecognition/i_intent_recognition.py
+-rw-rw-rw-   0        0        0     4650 2024-01-05 11:02:41.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/intentrecognition/intent_recognition_engine.py
+-rw-rw-rw-   0        0        0      517 2024-01-02 03:33:07.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/intentrecognition/recognized_intent.py
+-rw-rw-rw-   0        0        0     6452 2024-01-05 06:18:46.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/intentrecognition/snips_intent_recognition_impl.py
+drwxrwxrwx   0        0        0        0 2024-01-08 02:52:03.683366 dronebuddylib-2.0.9/dronebuddylib/atoms/objectdetection/
+-rw-rw-rw-   0        0        0      205 2024-01-08 02:49:39.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/objectdetection/__init__.py
+-rw-rw-rw-   0        0        0      976 2024-01-05 06:18:46.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/objectdetection/detected_object.py
+-rw-rw-rw-   0        0        0     1457 2024-01-05 06:18:46.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/objectdetection/i_object_detection.py
+-rw-rw-rw-   0        0        0     4925 2024-01-05 06:18:46.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/objectdetection/mp_object_detection_impl.py
+-rw-rw-rw-   0        0        0     2071 2024-01-05 11:02:41.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/objectdetection/object_detection_engine.py
+-rw-rw-rw-   0        0        0     4091 2024-01-05 06:18:46.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/objectdetection/yolo_object_detection_impl.py
+drwxrwxrwx   0        0        0        0 2024-01-08 02:52:03.687370 dronebuddylib-2.0.9/dronebuddylib/atoms/speechgeneration/
+-rw-rw-rw-   0        0        0      150 2024-01-08 02:50:40.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/speechgeneration/__init__.py
+-rw-rw-rw-   0        0        0     2194 2023-11-02 09:38:49.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/speechgeneration/i_speech_generation.py
+-rw-rw-rw-   0        0        0     1318 2024-01-05 11:02:41.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/speechgeneration/speech_generation_engine.py
+-rw-rw-rw-   0        0        0     4865 2024-01-04 11:53:55.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/speechgeneration/tts_speech_generation_impl.py
+drwxrwxrwx   0        0        0        0 2024-01-08 02:52:03.687370 dronebuddylib-2.0.9/dronebuddylib/atoms/speechrecognition/
+-rw-rw-rw-   0        0        0      573 2024-01-08 02:49:39.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/speechrecognition/__init__.py
+-rw-rw-rw-   0        0        0     6786 2024-01-05 06:18:46.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/speechrecognition/google_speech_recognition_impl.py
+-rw-rw-rw-   0        0        0     1282 2024-01-05 06:18:46.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/speechrecognition/i_speech_recognition.py
+-rw-rw-rw-   0        0        0     3591 2024-01-03 04:05:34.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/speechrecognition/microphone_stream.py
+-rw-rw-rw-   0        0        0     8549 2024-01-05 06:18:46.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/speechrecognition/multi_algo_speech_recognition_impl.py
+-rw-rw-rw-   0        0        0      170 2024-01-02 07:52:24.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/speechrecognition/recognized_speech.py
+-rw-rw-rw-   0        0        0     5544 2024-01-03 06:03:35.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/speechrecognition/resumable_microphone_stream.py
+-rw-rw-rw-   0        0        0     2493 2024-01-05 11:02:41.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/speechrecognition/speech_recognition_engine.py
+-rw-rw-rw-   0        0        0     3965 2024-01-05 06:18:46.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/speechrecognition/vosk_speech_recognition_impl.py
+drwxrwxrwx   0        0        0        0 2024-01-08 02:52:03.697389 dronebuddylib-2.0.9/dronebuddylib/atoms/textrecognition/
+-rw-rw-rw-   0        0        0      206 2024-01-08 02:49:39.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/textrecognition/__init__.py
+-rw-rw-rw-   0        0        0     2585 2024-01-04 11:53:55.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/textrecognition/google_text_recognition_impl.py
+-rw-rw-rw-   0        0        0      975 2023-12-12 05:56:15.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/textrecognition/i_text_recognition.py
+-rw-rw-rw-   0        0        0     1518 2024-01-04 11:53:55.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/textrecognition/text_recognition_engine.py
+-rw-rw-rw-   0        0        0      193 2023-12-12 06:04:42.000000 dronebuddylib-2.0.9/dronebuddylib/atoms/textrecognition/text_recognition_result.py
+drwxrwxrwx   0        0        0        0 2024-01-08 02:52:03.699427 dronebuddylib-2.0.9/dronebuddylib/configurations/
+-rw-rw-rw-   0        0        0       25 2024-01-08 02:49:39.000000 dronebuddylib-2.0.9/dronebuddylib/configurations/__init__.py
+-rw-rw-rw-   0        0        0      109 2023-08-15 12:04:39.000000 dronebuddylib-2.0.9/dronebuddylib/configurations/config.py
+drwxrwxrwx   0        0        0        0 2024-01-08 02:52:03.699427 dronebuddylib-2.0.9/dronebuddylib/exceptions/
+-rw-rw-rw-   0        0        0       95 2024-01-05 10:48:22.000000 dronebuddylib-2.0.9/dronebuddylib/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      404 2023-12-28 07:54:55.000000 dronebuddylib-2.0.9/dronebuddylib/exceptions/intent_resolution_exception.py
+drwxrwxrwx   0        0        0        0 2024-01-08 02:52:03.707431 dronebuddylib-2.0.9/dronebuddylib/models/
+-rw-rw-rw-   0        0        0      169 2024-01-08 02:49:39.000000 dronebuddylib-2.0.9/dronebuddylib/models/__init__.py
+-rw-rw-rw-   0        0        0     2893 2023-12-28 09:19:41.000000 dronebuddylib-2.0.9/dronebuddylib/models/chat_session.py
+-rw-rw-rw-   0        0        0      465 2023-10-25 04:13:37.000000 dronebuddylib-2.0.9/dronebuddylib/models/conversation.py
+-rw-rw-rw-   0        0        0      960 2023-11-02 05:56:23.000000 dronebuddylib-2.0.9/dronebuddylib/models/engine_configurations.py
+-rw-rw-rw-   0        0        0     4382 2024-01-03 08:29:30.000000 dronebuddylib-2.0.9/dronebuddylib/models/enums.py
+-rw-rw-rw-   0        0        0      418 2023-10-18 05:26:06.000000 dronebuddylib-2.0.9/dronebuddylib/models/gpt_configs.py
+-rw-rw-rw-   0        0        0      441 2023-10-27 07:52:14.000000 dronebuddylib-2.0.9/dronebuddylib/models/i_dbl_function.py
+-rw-rw-rw-   0        0        0      689 2023-10-25 04:13:44.000000 dronebuddylib-2.0.9/dronebuddylib/models/session_logger.py
+-rw-rw-rw-   0        0        0     1878 2023-10-18 05:26:10.000000 dronebuddylib-2.0.9/dronebuddylib/models/token_counter.py
+drwxrwxrwx   0        0        0        0 2024-01-08 02:52:03.707431 dronebuddylib-2.0.9/dronebuddylib/utils/
+-rw-rw-rw-   0        0        0       71 2024-01-08 02:49:39.000000 dronebuddylib-2.0.9/dronebuddylib/utils/__init__.py
+-rw-rw-rw-   0        0        0     2292 2024-01-02 05:28:44.000000 dronebuddylib-2.0.9/dronebuddylib/utils/chat_prompts.py
+-rw-rw-rw-   0        0        0     1739 2024-01-03 07:03:51.000000 dronebuddylib-2.0.9/dronebuddylib/utils/enums.py
+-rw-rw-rw-   0        0        0      440 2023-10-18 05:25:47.000000 dronebuddylib-2.0.9/dronebuddylib/utils/exceptions.py
+-rw-rw-rw-   0        0        0     1506 2024-01-03 08:56:13.000000 dronebuddylib-2.0.9/dronebuddylib/utils/logging_config.py
+-rw-rw-rw-   0        0        0     2201 2024-01-05 03:39:50.000000 dronebuddylib-2.0.9/dronebuddylib/utils/utils.py
+drwxrwxrwx   0        0        0        0 2024-01-08 02:52:03.717541 dronebuddylib-2.0.9/dronebuddylib.egg-info/
+-rw-rw-rw-   0        0        0      740 2024-01-08 02:52:03.000000 dronebuddylib-2.0.9/dronebuddylib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3730 2024-01-08 02:52:03.000000 dronebuddylib-2.0.9/dronebuddylib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-08 02:52:03.000000 dronebuddylib-2.0.9/dronebuddylib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-11-02 09:21:08.000000 dronebuddylib-2.0.9/dronebuddylib.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      213 2024-01-08 02:52:03.000000 dronebuddylib-2.0.9/dronebuddylib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-01-08 02:52:03.000000 dronebuddylib-2.0.9/dronebuddylib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      134 2024-01-05 11:17:31.000000 dronebuddylib-2.0.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-01-08 02:52:03.717541 dronebuddylib-2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      862 2024-01-08 02:49:39.000000 dronebuddylib-2.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-01-08 02:52:03.717541 dronebuddylib-2.0.9/test/
+-rw-rw-rw-   0        0        0      373 2024-01-05 06:28:49.000000 dronebuddylib-2.0.9/test/__init__.py
+-rw-rw-rw-   0        0        0     2198 2024-01-05 03:49:40.000000 dronebuddylib-2.0.9/test/test_face_recognition.py
+-rw-rw-rw-   0        0        0     5514 2024-01-04 14:00:19.000000 dronebuddylib-2.0.9/test/test_feature_extraction.py
+-rw-rw-rw-   0        0        0     2436 2024-01-04 12:02:42.000000 dronebuddylib-2.0.9/test/test_intent_recognition.py
+-rw-rw-rw-   0        0        0     6134 2024-01-04 13:13:18.000000 dronebuddylib-2.0.9/test/test_object_detection.py
+-rw-rw-rw-   0        0        0    12692 2024-01-05 03:53:33.000000 dronebuddylib-2.0.9/test/test_speech_recognition.py
+-rw-rw-rw-   0        0        0     3496 2024-01-05 03:53:33.000000 dronebuddylib-2.0.9/test/test_text_recognition.py
+-rw-rw-rw-   0        0        0     2272 2024-01-08 02:49:38.000000 dronebuddylib-2.0.9/test/test_update_version.py
```

### Comparing `dronebuddylib-2.0.8/MANIFEST.in` & `dronebuddylib-2.0.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/PKG-INFO` & `dronebuddylib-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dronebuddylib
-Version: 2.0.8
+Version: 2.0.9
 Summary: Everything to control and customize Tello
 Author: Malsha de Zoysa
 Author-email: malsha@ahlab.org
 License: MIT
 Requires-Python: >=3.9
 Requires-Dist: requests~=2.28.0
 Requires-Dist: numpy~=1.23.0
```

### Comparing `dronebuddylib-2.0.8/README.md` & `dronebuddylib-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/__init__.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 from .facerecognition.face_recognition_engine import FaceRecognitionEngine
 
 from .intentrecognition.intent_recognition_engine import IntentRecognitionEngine
 
 from .objectdetection.object_detection_engine import ObjectDetectionEngine
```

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/bodyfeatureextraction/body_feature_extraction_impl.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/bodyfeatureextraction/body_feature_extraction_impl.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/bodyfeatureextraction/hand_feature_extraction_impl.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/bodyfeatureextraction/hand_feature_extraction_impl.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/bodyfeatureextraction/head_feature_extraction_impl.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/bodyfeatureextraction/head_feature_extraction_impl.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/bodyfeatureextraction/i_feature_extraction.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/bodyfeatureextraction/i_feature_extraction.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/facerecognition/face_recognition_engine.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/facerecognition/face_recognition_engine.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/facerecognition/face_recognition_impl.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/facerecognition/face_recognition_impl.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/facerecognition/i_face_recognition.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/facerecognition/i_face_recognition.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/gpt_integration.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/gpt_integration.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/intentrecognition/gpt_intent_recognition_impl.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/intentrecognition/gpt_intent_recognition_impl.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/intentrecognition/i_intent_recognition.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/intentrecognition/i_intent_recognition.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/intentrecognition/intent_recognition_engine.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/intentrecognition/intent_recognition_engine.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/intentrecognition/recognized_intent.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/intentrecognition/recognized_intent.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/intentrecognition/snips_intent_recognition_impl.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/intentrecognition/snips_intent_recognition_impl.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/objectdetection/detected_object.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/objectdetection/detected_object.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/objectdetection/i_object_detection.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/objectdetection/i_object_detection.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/objectdetection/mp_object_detection_impl.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/objectdetection/mp_object_detection_impl.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/objectdetection/object_detection_engine.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/objectdetection/object_detection_engine.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/objectdetection/yolo_object_detection_impl.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/objectdetection/yolo_object_detection_impl.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/speechgeneration/i_speech_generation.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/speechgeneration/i_speech_generation.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/speechgeneration/speech_generation_engine.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/speechgeneration/speech_generation_engine.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/speechgeneration/tts_speech_generation_impl.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/speechgeneration/tts_speech_generation_impl.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/speechrecognition/__init__.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/speechrecognition/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
-from .microphone_stream import MicrophoneStream
-from .resumable_microphone_stream import ResumableMicrophoneStream
-from .speech_recognition_engine import SpeechRecognitionEngine
-from .multi_algo_speech_recognition_impl import MultiAlgoSpeechToTextConversionImplementation
-from .google_speech_recognition_impl import GoogleSpeechRecognitionImpl
-from .vosk_speech_recognition_impl import VoskSpeechRecognitionImpl
+# from .microphone_stream import MicrophoneStream
+# from .resumable_microphone_stream import ResumableMicrophoneStream
+# from .speech_recognition_engine import SpeechRecognitionEngine
+# from .multi_algo_speech_recognition_impl import MultiAlgoSpeechToTextConversionImplementation
+# from .google_speech_recognition_impl import GoogleSpeechRecognitionImpl
+# from .vosk_speech_recognition_impl import VoskSpeechRecognitionImpl
 from .i_speech_recognition import ISpeechRecognition
 from .speech_recognition_engine import SpeechRecognitionEngine
```

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/speechrecognition/google_speech_recognition_impl.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/speechrecognition/google_speech_recognition_impl.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/speechrecognition/i_speech_recognition.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/speechrecognition/i_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/speechrecognition/microphone_stream.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/speechrecognition/microphone_stream.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/speechrecognition/multi_algo_speech_recognition_impl.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/speechrecognition/multi_algo_speech_recognition_impl.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/speechrecognition/resumable_microphone_stream.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/speechrecognition/resumable_microphone_stream.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/speechrecognition/speech_recognition_engine.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/speechrecognition/speech_recognition_engine.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/speechrecognition/vosk_speech_recognition_impl.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/speechrecognition/vosk_speech_recognition_impl.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/textrecognition/google_text_recognition_impl.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/textrecognition/google_text_recognition_impl.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/textrecognition/i_text_recognition.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/textrecognition/i_text_recognition.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/atoms/textrecognition/text_recognition_engine.py` & `dronebuddylib-2.0.9/dronebuddylib/atoms/textrecognition/text_recognition_engine.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/models/chat_session.py` & `dronebuddylib-2.0.9/dronebuddylib/models/chat_session.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/models/engine_configurations.py` & `dronebuddylib-2.0.9/dronebuddylib/models/engine_configurations.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/models/enums.py` & `dronebuddylib-2.0.9/dronebuddylib/models/enums.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/models/session_logger.py` & `dronebuddylib-2.0.9/dronebuddylib/models/session_logger.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/models/token_counter.py` & `dronebuddylib-2.0.9/dronebuddylib/models/token_counter.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/utils/chat_prompts.py` & `dronebuddylib-2.0.9/dronebuddylib/utils/chat_prompts.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/utils/enums.py` & `dronebuddylib-2.0.9/dronebuddylib/utils/enums.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/utils/logging_config.py` & `dronebuddylib-2.0.9/dronebuddylib/utils/logging_config.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib/utils/utils.py` & `dronebuddylib-2.0.9/dronebuddylib/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/dronebuddylib.egg-info/PKG-INFO` & `dronebuddylib-2.0.9/dronebuddylib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dronebuddylib
-Version: 2.0.8
+Version: 2.0.9
 Summary: Everything to control and customize Tello
 Author: Malsha de Zoysa
 Author-email: malsha@ahlab.org
 License: MIT
 Requires-Python: >=3.9
 Requires-Dist: requests~=2.28.0
 Requires-Dist: numpy~=1.23.0
```

### Comparing `dronebuddylib-2.0.8/dronebuddylib.egg-info/SOURCES.txt` & `dronebuddylib-2.0.9/dronebuddylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/setup.py` & `dronebuddylib-2.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fh:
     requirements = fh.read().splitlines()
 
 setup(
     name='dronebuddylib',
-    version='2.0.8',
+    version='2.0.9',
     packages=find_packages(),
     include_package_data=True,
     package_data={
         'dronebuddylib': ['resources/*'],
     },
     zip_safe=False,
     setup_requires=[
```

### Comparing `dronebuddylib-2.0.8/test/test_face_recognition.py` & `dronebuddylib-2.0.9/test/test_face_recognition.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/test/test_feature_extraction.py` & `dronebuddylib-2.0.9/test/test_feature_extraction.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/test/test_intent_recognition.py` & `dronebuddylib-2.0.9/test/test_intent_recognition.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/test/test_object_detection.py` & `dronebuddylib-2.0.9/test/test_object_detection.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/test/test_speech_recognition.py` & `dronebuddylib-2.0.9/test/test_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/test/test_text_recognition.py` & `dronebuddylib-2.0.9/test/test_text_recognition.py`

 * *Files identical despite different names*

### Comparing `dronebuddylib-2.0.8/test/test_update_version.py` & `dronebuddylib-2.0.9/test/test_update_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,10 +31,10 @@
         content = file.read()
     modified_content = re.sub(r"version=['\"]\d+\.\d+\.\d+['\"]", 'version=\'' + new_version + '\'', content)
     with open(setup_file_path, 'w') as file:
         file.write(modified_content)
 
 
 if __name__ == '__main__':
-    new_version = '2.0.8'
+    new_version = '2.0.9'
     change_init_version(new_version)
     change_setup_version(new_version)
```

