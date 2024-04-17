# Comparing `tmp/symbl-rest-1.0.8.tar.gz` & `tmp/symbl-rest-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\symbl-rest-1.0.8.tar", last modified: Thu Jul  8 09:54:00 2021, max compression
+gzip compressed data, was "dist\symbl-rest-1.0.9.tar", last modified: Mon Jul 26 06:22:14 2021, max compression
```

## Comparing `symbl-rest-1.0.8.tar` & `symbl-rest-1.0.9.tar`

### file list

```diff
@@ -1,194 +1,230 @@
-drwxrwxrwx   0        0        0        0 2021-07-08 09:54:00.212091 symbl-rest-1.0.8/
--rw-rw-rw-   0        0        0     1915 2021-07-08 09:54:00.204809 symbl-rest-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    13535 2021-07-08 09:50:49.000000 symbl-rest-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2021-07-08 09:54:00.216666 symbl-rest-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     3986 2021-07-08 09:52:57.000000 symbl-rest-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-07-08 09:53:51.412736 symbl-rest-1.0.8/symbl_rest/
--rw-rw-rw-   0        0        0     7245 2021-07-08 09:50:49.000000 symbl-rest-1.0.8/symbl_rest/__init__.py
-drwxrwxrwx   0        0        0        0 2021-07-08 09:53:52.890421 symbl-rest-1.0.8/symbl_rest/api/
--rw-rw-rw-   0        0        0     1056 2021-07-08 09:50:49.000000 symbl-rest-1.0.8/symbl_rest/api/__init__.py
--rw-rw-rw-   0        0        0     6337 2021-07-08 09:50:48.000000 symbl-rest-1.0.8/symbl_rest/api/action_items_api.py
--rw-rw-rw-   0        0        0    81174 2021-07-08 09:52:19.000000 symbl-rest-1.0.8/symbl_rest/api/async_api.py
--rw-rw-rw-   0        0        0    14672 2021-07-08 09:50:48.000000 symbl-rest-1.0.8/symbl_rest/api/authentication_api.py
--rw-rw-rw-   0        0        0     6444 2021-07-08 09:50:48.000000 symbl-rest-1.0.8/symbl_rest/api/connection_to_endpoint_api.py
--rw-rw-rw-   0        0        0     6397 2021-07-08 09:50:48.000000 symbl-rest-1.0.8/symbl_rest/api/conversation_data_api.py
--rw-rw-rw-   0        0        0    39798 2021-07-08 09:50:48.000000 symbl-rest-1.0.8/symbl_rest/api/conversations_api.py
--rw-rw-rw-   0        0        0     6604 2021-07-08 09:50:48.000000 symbl-rest-1.0.8/symbl_rest/api/external_event_web_hook_api.py
--rw-rw-rw-   0        0        0     6301 2021-07-08 09:50:49.000000 symbl-rest-1.0.8/symbl_rest/api/follow_ups_api.py
--rw-rw-rw-   0        0        0     6274 2021-07-08 09:50:49.000000 symbl-rest-1.0.8/symbl_rest/api/insights_api.py
--rw-rw-rw-   0        0        0     6222 2021-07-08 09:50:49.000000 symbl-rest-1.0.8/symbl_rest/api/intents_api.py
--rw-rw-rw-   0        0        0     5847 2021-07-08 09:50:49.000000 symbl-rest-1.0.8/symbl_rest/api/jobs_api.py
--rw-rw-rw-   0        0        0     6258 2021-07-08 09:50:49.000000 symbl-rest-1.0.8/symbl_rest/api/members_api.py
--rw-rw-rw-   0        0        0     6807 2021-07-08 09:50:49.000000 symbl-rest-1.0.8/symbl_rest/api/messages_api.py
--rw-rw-rw-   0        0        0     9979 2021-07-08 09:50:49.000000 symbl-rest-1.0.8/symbl_rest/api/metric_api.py
--rw-rw-rw-   0        0        0     6287 2021-07-08 09:50:49.000000 symbl-rest-1.0.8/symbl_rest/api/metric_entry_api.py
--rw-rw-rw-   0        0        0     6284 2021-07-08 09:50:49.000000 symbl-rest-1.0.8/symbl_rest/api/questions_api.py
--rw-rw-rw-   0        0        0     6770 2021-07-08 09:50:49.000000 symbl-rest-1.0.8/symbl_rest/api/topics_api.py
--rw-rw-rw-   0        0        0    26194 2021-07-08 09:50:49.000000 symbl-rest-1.0.8/symbl_rest/api_client.py
--rw-rw-rw-   0        0        0     9672 2021-07-08 09:50:49.000000 symbl-rest-1.0.8/symbl_rest/configuration.py
-drwxrwxrwx   0        0        0        0 2021-07-08 09:53:58.443621 symbl-rest-1.0.8/symbl_rest/models/
--rw-rw-rw-   0        0        0     6132 2021-07-08 09:50:49.000000 symbl-rest-1.0.8/symbl_rest/models/__init__.py
--rw-rw-rw-   0        0        0     6677 2021-07-08 09:50:45.000000 symbl-rest-1.0.8/symbl_rest/models/action.py
--rw-rw-rw-   0        0        0     4857 2021-07-08 09:50:46.000000 symbl-rest-1.0.8/symbl_rest/models/action_item_list_response.py
--rw-rw-rw-   0        0        0     7800 2021-07-08 09:50:46.000000 symbl-rest-1.0.8/symbl_rest/models/async_audio_url_parameters.py
--rw-rw-rw-   0        0        0     3925 2021-07-08 09:50:46.000000 symbl-rest-1.0.8/symbl_rest/models/async_confidence_threshold.py
--rw-rw-rw-   0        0        0     3901 2021-07-08 09:50:46.000000 symbl-rest-1.0.8/symbl_rest/models/async_detect_phrases.py
--rw-rw-rw-   0        0        0     3909 2021-07-08 09:50:46.000000 symbl-rest-1.0.8/symbl_rest/models/async_entities_payload.py
--rw-rw-rw-   0        0        0     3893 2021-07-08 09:50:46.000000 symbl-rest-1.0.8/symbl_rest/models/async_meeting_name.py
--rw-rw-rw-   0        0        0     3901 2021-07-08 09:50:46.000000 symbl-rest-1.0.8/symbl_rest/models/async_messages_field.py
--rw-rw-rw-   0        0        0     6111 2021-07-08 09:50:46.000000 symbl-rest-1.0.8/symbl_rest/models/async_messages_field_inner.py
--rw-rw-rw-   0        0        0     5613 2021-07-08 09:50:46.000000 symbl-rest-1.0.8/symbl_rest/models/async_response.py
--rw-rw-rw-   0        0        0     8595 2021-07-08 09:50:46.000000 symbl-rest-1.0.8/symbl_rest/models/async_text_parameters.py
--rw-rw-rw-   0        0        0     7800 2021-07-08 09:50:46.000000 symbl-rest-1.0.8/symbl_rest/models/async_video_url_parameters.py
--rw-rw-rw-   0        0        0     7130 2021-07-08 09:50:46.000000 symbl-rest-1.0.8/symbl_rest/models/audio_config.py
--rw-rw-rw-   0        0        0     4698 2021-07-08 09:50:46.000000 symbl-rest-1.0.8/symbl_rest/models/avatar.py
--rw-rw-rw-   0        0        0    11454 2021-07-08 09:50:46.000000 symbl-rest-1.0.8/symbl_rest/models/conversation_action_item.py
--rw-rw-rw-   0        0        0     8075 2021-07-08 09:50:46.000000 symbl-rest-1.0.8/symbl_rest/models/conversation_data_list_response.py
--rw-rw-rw-   0        0        0    11358 2021-07-08 09:50:46.000000 symbl-rest-1.0.8/symbl_rest/models/conversation_follow_up.py
--rw-rw-rw-   0        0        0     7886 2021-07-08 09:50:46.000000 symbl-rest-1.0.8/symbl_rest/models/conversation_insight_item.py
--rw-rw-rw-   0        0        0     9305 2021-07-08 09:50:46.000000 symbl-rest-1.0.8/symbl_rest/models/conversation_intent.py
--rw-rw-rw-   0        0        0    10038 2021-07-08 09:50:46.000000 symbl-rest-1.0.8/symbl_rest/models/conversation_message.py
--rw-rw-rw-   0        0        0     8560 2021-07-08 09:50:46.000000 symbl-rest-1.0.8/symbl_rest/models/conversation_question.py
--rw-rw-rw-   0        0        0     9311 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/conversation_topic.py
--rw-rw-rw-   0        0        0     7210 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/custom_entities.py
--rw-rw-rw-   0        0        0     5820 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/custom_entities_message_refs.py
--rw-rw-rw-   0        0        0     5893 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/duration_payload.py
--rw-rw-rw-   0        0        0    13099 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/endpoint.py
--rw-rw-rw-   0        0        0    13417 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/endpoint_connect_request.py
--rw-rw-rw-   0        0        0     8933 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/endpoint_connect_response.py
--rw-rw-rw-   0        0        0     4595 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/endpoint_request_data.py
--rw-rw-rw-   0        0        0     5534 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/error.py
--rw-rw-rw-   0        0        0     7300 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/external_event.py
--rw-rw-rw-   0        0        0     4793 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/follow_up_list_response.py
--rw-rw-rw-   0        0        0     6083 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/from_payload.py
--rw-rw-rw-   0        0        0     4512 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/generic_error.py
--rw-rw-rw-   0        0        0     8162 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/grant.py
--rw-rw-rw-   0        0        0     4761 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/insights_list_response.py
--rw-rw-rw-   0        0        0     5929 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/intent.py
--rw-rw-rw-   0        0        0     4709 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/intent_list_response.py
--rw-rw-rw-   0        0        0     5233 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/job_response.py
--rw-rw-rw-   0        0        0     4526 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/language.py
--rw-rw-rw-   0        0        0     4574 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/location_trunc.py
--rw-rw-rw-   0        0        0     4682 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/member_list_response.py
--rw-rw-rw-   0        0        0     5570 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/members_info.py
--rw-rw-rw-   0        0        0     4741 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/message_list_response.py
--rw-rw-rw-   0        0        0     8756 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/metric.py
--rw-rw-rw-   0        0        0     8450 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/metric_entry.py
--rw-rw-rw-   0        0        0     3897 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/metric_entry_create.py
--rw-rw-rw-   0        0        0     5451 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/metric_entry_response.py
--rw-rw-rw-   0        0        0     5017 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/metric_label.py
--rw-rw-rw-   0        0        0     5251 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/metric_response.py
--rw-rw-rw-   0        0        0     5938 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/model_from.py
--rw-rw-rw-   0        0        0     4993 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/parent_ref.py
--rw-rw-rw-   0        0        0     4957 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/phrase.py
--rw-rw-rw-   0        0        0     4773 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/question_list_response.py
--rw-rw-rw-   0        0        0     6445 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/refresh_token_request.py
--rw-rw-rw-   0        0        0     5539 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/revoke_token_request.py
--rw-rw-rw-   0        0        0     5215 2021-07-08 09:50:47.000000 symbl-rest-1.0.8/symbl_rest/models/sentiment.py
--rw-rw-rw-   0        0        0     4518 2021-07-08 09:50:48.000000 symbl-rest-1.0.8/symbl_rest/models/sentiment_polarity.py
--rw-rw-rw-   0        0        0     6892 2021-07-08 09:50:48.000000 symbl-rest-1.0.8/symbl_rest/models/session_trunc.py
--rw-rw-rw-   0        0        0     6344 2021-07-08 09:50:48.000000 symbl-rest-1.0.8/symbl_rest/models/session_user.py
--rw-rw-rw-   0        0        0     5249 2021-07-08 09:50:48.000000 symbl-rest-1.0.8/symbl_rest/models/summary_info.py
--rw-rw-rw-   0        0        0     6072 2021-07-08 09:50:48.000000 symbl-rest-1.0.8/symbl_rest/models/tag.py
--rw-rw-rw-   0        0        0     5478 2021-07-08 09:50:48.000000 symbl-rest-1.0.8/symbl_rest/models/text_payload.py
--rw-rw-rw-   0        0        0     5586 2021-07-08 09:50:48.000000 symbl-rest-1.0.8/symbl_rest/models/time_zone.py
--rw-rw-rw-   0        0        0     5957 2021-07-08 09:50:48.000000 symbl-rest-1.0.8/symbl_rest/models/token.py
--rw-rw-rw-   0        0        0     4677 2021-07-08 09:50:48.000000 symbl-rest-1.0.8/symbl_rest/models/topic_list_response.py
--rw-rw-rw-   0        0        0     4552 2021-07-08 09:50:48.000000 symbl-rest-1.0.8/symbl_rest/models/unauthorized_error.py
--rw-rw-rw-   0        0        0     9986 2021-07-08 09:50:48.000000 symbl-rest-1.0.8/symbl_rest/models/user_trunc.py
--rw-rw-rw-   0        0        0     6396 2021-07-08 09:50:48.000000 symbl-rest-1.0.8/symbl_rest/models/word.py
--rw-rw-rw-   0        0        0    14993 2021-07-08 09:52:46.000000 symbl-rest-1.0.8/symbl_rest/rest.py
-drwxrwxrwx   0        0        0        0 2021-07-08 09:53:51.758170 symbl-rest-1.0.8/symbl_rest.egg-info/
--rw-rw-rw-   0        0        0     1915 2021-07-08 09:53:44.000000 symbl-rest-1.0.8/symbl_rest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6123 2021-07-08 09:53:45.000000 symbl-rest-1.0.8/symbl_rest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-07-08 09:53:44.000000 symbl-rest-1.0.8/symbl_rest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2021-07-08 09:53:44.000000 symbl-rest-1.0.8/symbl_rest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2021-07-08 09:53:44.000000 symbl-rest-1.0.8/symbl_rest.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-07-08 09:54:00.189088 symbl-rest-1.0.8/test/
--rw-rw-rw-   0        0        0        0 2021-07-08 09:50:49.000000 symbl-rest-1.0.8/test/__init__.py
--rw-rw-rw-   0        0        0     2286 2021-07-08 04:57:41.000000 symbl-rest-1.0.8/test/test_action.py
--rw-rw-rw-   0        0        0     2420 2021-07-08 04:57:41.000000 symbl-rest-1.0.8/test/test_action_item_list_response.py
--rw-rw-rw-   0        0        0     2349 2021-07-08 04:57:44.000000 symbl-rest-1.0.8/test/test_action_items_api.py
--rw-rw-rw-   0        0        0     3676 2021-07-08 04:57:44.000000 symbl-rest-1.0.8/test/test_async_api.py
--rw-rw-rw-   0        0        0     2428 2021-07-08 04:57:41.000000 symbl-rest-1.0.8/test/test_async_audio_url_parameters.py
--rw-rw-rw-   0        0        0     2434 2021-07-08 04:57:41.000000 symbl-rest-1.0.8/test/test_async_confidence_threshold.py
--rw-rw-rw-   0        0        0     2386 2021-07-08 04:57:41.000000 symbl-rest-1.0.8/test/test_async_detect_phrases.py
--rw-rw-rw-   0        0        0     2402 2021-07-08 04:57:41.000000 symbl-rest-1.0.8/test/test_async_entities_payload.py
--rw-rw-rw-   0        0        0     2370 2021-07-08 04:57:41.000000 symbl-rest-1.0.8/test/test_async_meeting_name.py
--rw-rw-rw-   0        0        0     2386 2021-07-08 04:57:41.000000 symbl-rest-1.0.8/test/test_async_messages_field.py
--rw-rw-rw-   0        0        0     2428 2021-07-08 04:57:41.000000 symbl-rest-1.0.8/test/test_async_messages_field_inner.py
--rw-rw-rw-   0        0        0     2344 2021-07-08 04:57:41.000000 symbl-rest-1.0.8/test/test_async_response.py
--rw-rw-rw-   0        0        0     2394 2021-07-08 04:57:41.000000 symbl-rest-1.0.8/test/test_async_text_parameters.py
--rw-rw-rw-   0        0        0     2428 2021-07-08 04:57:41.000000 symbl-rest-1.0.8/test/test_async_video_url_parameters.py
--rw-rw-rw-   0        0        0     2328 2021-07-08 04:57:41.000000 symbl-rest-1.0.8/test/test_audio_config.py
--rw-rw-rw-   0        0        0     2641 2021-07-08 04:57:44.000000 symbl-rest-1.0.8/test/test_authentication_api.py
--rw-rw-rw-   0        0        0     2286 2021-07-08 04:57:41.000000 symbl-rest-1.0.8/test/test_avatar.py
--rw-rw-rw-   0        0        0     2387 2021-07-08 04:57:44.000000 symbl-rest-1.0.8/test/test_connection_to_endpoint_api.py
--rw-rw-rw-   0        0        0     2418 2021-07-08 04:57:42.000000 symbl-rest-1.0.8/test/test_conversation_action_item.py
--rw-rw-rw-   0        0        0     2399 2021-07-08 04:57:44.000000 symbl-rest-1.0.8/test/test_conversation_data_api.py
--rw-rw-rw-   0        0        0     2468 2021-07-08 04:57:42.000000 symbl-rest-1.0.8/test/test_conversation_data_list_response.py
--rw-rw-rw-   0        0        0     2402 2021-07-08 04:57:42.000000 symbl-rest-1.0.8/test/test_conversation_follow_up.py
--rw-rw-rw-   0        0        0     2426 2021-07-08 04:57:42.000000 symbl-rest-1.0.8/test/test_conversation_insight_item.py
--rw-rw-rw-   0        0        0     2384 2021-07-08 04:57:42.000000 symbl-rest-1.0.8/test/test_conversation_intent.py
--rw-rw-rw-   0        0        0     2392 2021-07-08 04:57:42.000000 symbl-rest-1.0.8/test/test_conversation_message.py
--rw-rw-rw-   0        0        0     2400 2021-07-08 04:57:42.000000 symbl-rest-1.0.8/test/test_conversation_question.py
--rw-rw-rw-   0        0        0     2376 2021-07-08 04:57:42.000000 symbl-rest-1.0.8/test/test_conversation_topic.py
--rw-rw-rw-   0        0        0     3949 2021-07-08 04:57:44.000000 symbl-rest-1.0.8/test/test_conversations_api.py
--rw-rw-rw-   0        0        0     2352 2021-07-08 04:57:42.000000 symbl-rest-1.0.8/test/test_custom_entities.py
--rw-rw-rw-   0        0        0     2444 2021-07-08 04:57:42.000000 symbl-rest-1.0.8/test/test_custom_entities_message_refs.py
--rw-rw-rw-   0        0        0     2360 2021-07-08 04:57:42.000000 symbl-rest-1.0.8/test/test_duration_payload.py
--rw-rw-rw-   0        0        0     2302 2021-07-08 04:57:42.000000 symbl-rest-1.0.8/test/test_endpoint.py
--rw-rw-rw-   0        0        0     2418 2021-07-08 04:57:42.000000 symbl-rest-1.0.8/test/test_endpoint_connect_request.py
--rw-rw-rw-   0        0        0     2426 2021-07-08 04:57:42.000000 symbl-rest-1.0.8/test/test_endpoint_connect_response.py
--rw-rw-rw-   0        0        0     2394 2021-07-08 04:57:42.000000 symbl-rest-1.0.8/test/test_endpoint_request_data.py
--rw-rw-rw-   0        0        0     2278 2021-07-08 04:57:43.000000 symbl-rest-1.0.8/test/test_error.py
--rw-rw-rw-   0        0        0     2344 2021-07-08 04:57:43.000000 symbl-rest-1.0.8/test/test_external_event.py
--rw-rw-rw-   0        0        0     2359 2021-07-08 04:57:44.000000 symbl-rest-1.0.8/test/test_external_event_web_hook_api.py
--rw-rw-rw-   0        0        0     2404 2021-07-08 04:57:43.000000 symbl-rest-1.0.8/test/test_follow_up_list_response.py
--rw-rw-rw-   0        0        0     2333 2021-07-08 04:57:44.000000 symbl-rest-1.0.8/test/test_follow_ups_api.py
--rw-rw-rw-   0        0        0     2328 2021-07-08 04:57:43.000000 symbl-rest-1.0.8/test/test_from_payload.py
--rw-rw-rw-   0        0        0     2336 2021-07-08 04:57:43.000000 symbl-rest-1.0.8/test/test_generic_error.py
--rw-rw-rw-   0        0        0     2278 2021-07-08 04:57:43.000000 symbl-rest-1.0.8/test/test_grant.py
--rw-rw-rw-   0        0        0     2321 2021-07-08 04:57:44.000000 symbl-rest-1.0.8/test/test_insights_api.py
--rw-rw-rw-   0        0        0     2402 2021-07-08 04:57:43.000000 symbl-rest-1.0.8/test/test_insights_list_response.py
--rw-rw-rw-   0        0        0     2286 2021-07-08 04:57:43.000000 symbl-rest-1.0.8/test/test_intent.py
--rw-rw-rw-   0        0        0     2386 2021-07-08 04:57:43.000000 symbl-rest-1.0.8/test/test_intent_list_response.py
--rw-rw-rw-   0        0        0     2312 2021-07-08 04:57:44.000000 symbl-rest-1.0.8/test/test_intents_api.py
--rw-rw-rw-   0        0        0     2328 2021-07-08 04:57:43.000000 symbl-rest-1.0.8/test/test_job_response.py
--rw-rw-rw-   0        0        0     2255 2021-07-08 04:57:45.000000 symbl-rest-1.0.8/test/test_jobs_api.py
--rw-rw-rw-   0        0        0     2302 2021-07-08 04:57:43.000000 symbl-rest-1.0.8/test/test_language.py
--rw-rw-rw-   0        0        0     2344 2021-07-08 04:57:43.000000 symbl-rest-1.0.8/test/test_location_trunc.py
--rw-rw-rw-   0        0        0     2386 2021-07-08 04:57:43.000000 symbl-rest-1.0.8/test/test_member_list_response.py
--rw-rw-rw-   0        0        0     2313 2021-07-08 04:57:45.000000 symbl-rest-1.0.8/test/test_members_api.py
--rw-rw-rw-   0        0        0     2328 2021-07-08 04:57:43.000000 symbl-rest-1.0.8/test/test_members_info.py
--rw-rw-rw-   0        0        0     2394 2021-07-08 04:57:43.000000 symbl-rest-1.0.8/test/test_message_list_response.py
--rw-rw-rw-   0        0        0     2321 2021-07-08 04:57:45.000000 symbl-rest-1.0.8/test/test_messages_api.py
--rw-rw-rw-   0        0        0     2286 2021-07-08 04:57:43.000000 symbl-rest-1.0.8/test/test_metric.py
--rw-rw-rw-   0        0        0     2409 2021-07-08 04:57:45.000000 symbl-rest-1.0.8/test/test_metric_api.py
--rw-rw-rw-   0        0        0     2328 2021-07-08 04:57:43.000000 symbl-rest-1.0.8/test/test_metric_entry.py
--rw-rw-rw-   0        0        0     2291 2021-07-08 04:57:45.000000 symbl-rest-1.0.8/test/test_metric_entry_api.py
--rw-rw-rw-   0        0        0     2378 2021-07-08 04:57:43.000000 symbl-rest-1.0.8/test/test_metric_entry_create.py
--rw-rw-rw-   0        0        0     2394 2021-07-08 04:57:43.000000 symbl-rest-1.0.8/test/test_metric_entry_response.py
--rw-rw-rw-   0        0        0     2328 2021-07-08 04:57:43.000000 symbl-rest-1.0.8/test/test_metric_label.py
--rw-rw-rw-   0        0        0     2352 2021-07-08 04:57:43.000000 symbl-rest-1.0.8/test/test_metric_response.py
--rw-rw-rw-   0        0        0     2312 2021-07-08 04:57:43.000000 symbl-rest-1.0.8/test/test_model_from.py
--rw-rw-rw-   0        0        0     2312 2021-07-08 04:57:43.000000 symbl-rest-1.0.8/test/test_parent_ref.py
--rw-rw-rw-   0        0        0     2286 2021-07-08 04:57:43.000000 symbl-rest-1.0.8/test/test_phrase.py
--rw-rw-rw-   0        0        0     2402 2021-07-08 04:57:44.000000 symbl-rest-1.0.8/test/test_question_list_response.py
--rw-rw-rw-   0        0        0     2328 2021-07-08 04:57:45.000000 symbl-rest-1.0.8/test/test_questions_api.py
--rw-rw-rw-   0        0        0     2394 2021-07-08 04:57:44.000000 symbl-rest-1.0.8/test/test_refresh_token_request.py
--rw-rw-rw-   0        0        0     2386 2021-07-08 04:57:44.000000 symbl-rest-1.0.8/test/test_revoke_token_request.py
--rw-rw-rw-   0        0        0     2310 2021-07-08 04:57:44.000000 symbl-rest-1.0.8/test/test_sentiment.py
--rw-rw-rw-   0        0        0     2376 2021-07-08 04:57:44.000000 symbl-rest-1.0.8/test/test_sentiment_polarity.py
--rw-rw-rw-   0        0        0     2336 2021-07-08 04:57:44.000000 symbl-rest-1.0.8/test/test_session_trunc.py
--rw-rw-rw-   0        0        0     2328 2021-07-08 04:57:44.000000 symbl-rest-1.0.8/test/test_session_user.py
--rw-rw-rw-   0        0        0     2328 2021-07-08 04:57:44.000000 symbl-rest-1.0.8/test/test_summary_info.py
--rw-rw-rw-   0        0        0     2262 2021-07-08 04:57:44.000000 symbl-rest-1.0.8/test/test_tag.py
--rw-rw-rw-   0        0        0     2328 2021-07-08 04:57:44.000000 symbl-rest-1.0.8/test/test_text_payload.py
--rw-rw-rw-   0        0        0     2304 2021-07-08 04:57:44.000000 symbl-rest-1.0.8/test/test_time_zone.py
--rw-rw-rw-   0        0        0     2278 2021-07-08 04:57:44.000000 symbl-rest-1.0.8/test/test_token.py
--rw-rw-rw-   0        0        0     2378 2021-07-08 04:57:44.000000 symbl-rest-1.0.8/test/test_topic_list_response.py
--rw-rw-rw-   0        0        0     2304 2021-07-08 04:57:45.000000 symbl-rest-1.0.8/test/test_topics_api.py
--rw-rw-rw-   0        0        0     2376 2021-07-08 04:57:44.000000 symbl-rest-1.0.8/test/test_unauthorized_error.py
--rw-rw-rw-   0        0        0     2312 2021-07-08 04:57:44.000000 symbl-rest-1.0.8/test/test_user_trunc.py
--rw-rw-rw-   0        0        0     2270 2021-07-08 04:57:44.000000 symbl-rest-1.0.8/test/test_word.py
+drwxrwxrwx   0        0        0        0 2021-07-26 06:22:14.396732 symbl-rest-1.0.9/
+-rw-rw-rw-   0        0        0     1915 2021-07-26 06:22:14.380703 symbl-rest-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    15677 2021-07-26 06:15:52.000000 symbl-rest-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2021-07-26 06:22:14.397658 symbl-rest-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     3986 2021-07-26 06:17:57.000000 symbl-rest-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-07-26 06:22:07.844011 symbl-rest-1.0.9/symbl_rest/
+-rw-rw-rw-   0        0        0     8563 2021-07-26 06:15:52.000000 symbl-rest-1.0.9/symbl_rest/__init__.py
+drwxrwxrwx   0        0        0        0 2021-07-26 06:22:08.420710 symbl-rest-1.0.9/symbl_rest/api/
+-rw-rw-rw-   0        0        0     1214 2021-07-26 06:15:52.000000 symbl-rest-1.0.9/symbl_rest/api/__init__.py
+-rw-rw-rw-   0        0        0     6337 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/api/action_items_api.py
+-rw-rw-rw-   0        0        0     6447 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/api/analytics_api.py
+-rw-rw-rw-   0        0        0    81757 2021-07-26 06:19:15.000000 symbl-rest-1.0.9/symbl_rest/api/async_api.py
+-rw-rw-rw-   0        0        0    14672 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/api/authentication_api.py
+-rw-rw-rw-   0        0        0     6444 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/api/connection_to_endpoint_api.py
+-rw-rw-rw-   0        0        0     6397 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/api/conversation_data_api.py
+-rw-rw-rw-   0        0        0    52193 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/api/conversations_api.py
+-rw-rw-rw-   0        0        0     6264 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/api/entities_api.py
+-rw-rw-rw-   0        0        0     6604 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/api/external_event_web_hook_api.py
+-rw-rw-rw-   0        0        0     6301 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/api/follow_ups_api.py
+-rw-rw-rw-   0        0        0     6274 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/api/insights_api.py
+-rw-rw-rw-   0        0        0     6222 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/api/intents_api.py
+-rw-rw-rw-   0        0        0     5847 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/api/jobs_api.py
+-rw-rw-rw-   0        0        0     6258 2021-07-26 06:15:52.000000 symbl-rest-1.0.9/symbl_rest/api/members_api.py
+-rw-rw-rw-   0        0        0     6807 2021-07-26 06:15:52.000000 symbl-rest-1.0.9/symbl_rest/api/messages_api.py
+-rw-rw-rw-   0        0        0     9979 2021-07-26 06:15:52.000000 symbl-rest-1.0.9/symbl_rest/api/metric_api.py
+-rw-rw-rw-   0        0        0     6287 2021-07-26 06:15:52.000000 symbl-rest-1.0.9/symbl_rest/api/metric_entry_api.py
+-rw-rw-rw-   0        0        0     6284 2021-07-26 06:15:52.000000 symbl-rest-1.0.9/symbl_rest/api/questions_api.py
+-rw-rw-rw-   0        0        0     6770 2021-07-26 06:15:52.000000 symbl-rest-1.0.9/symbl_rest/api/topics_api.py
+-rw-rw-rw-   0        0        0     6378 2021-07-26 06:15:52.000000 symbl-rest-1.0.9/symbl_rest/api/trackers_api.py
+-rw-rw-rw-   0        0        0    26194 2021-07-26 06:15:52.000000 symbl-rest-1.0.9/symbl_rest/api_client.py
+-rw-rw-rw-   0        0        0     9672 2021-07-26 06:15:52.000000 symbl-rest-1.0.9/symbl_rest/configuration.py
+drwxrwxrwx   0        0        0        0 2021-07-26 06:22:10.841861 symbl-rest-1.0.9/symbl_rest/models/
+-rw-rw-rw-   0        0        0     7292 2021-07-26 06:15:52.000000 symbl-rest-1.0.9/symbl_rest/models/__init__.py
+-rw-rw-rw-   0        0        0     6677 2021-07-26 06:15:48.000000 symbl-rest-1.0.9/symbl_rest/models/action.py
+-rw-rw-rw-   0        0        0     4857 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/symbl_rest/models/action_item_list_response.py
+-rw-rw-rw-   0        0        0     5395 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/symbl_rest/models/analytics_list_response.py
+-rw-rw-rw-   0        0        0     8772 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/symbl_rest/models/analytics_members_info.py
+-rw-rw-rw-   0        0        0     5897 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/symbl_rest/models/analytics_members_info_overlap.py
+-rw-rw-rw-   0        0        0     7703 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/symbl_rest/models/analytics_members_info_overlap_overlapping_members.py
+-rw-rw-rw-   0        0        0     4534 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/symbl_rest/models/analytics_members_info_pace.py
+-rw-rw-rw-   0        0        0     5413 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/symbl_rest/models/analytics_members_info_talk_time.py
+-rw-rw-rw-   0        0        0     5866 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/symbl_rest/models/analytics_metrics_info.py
+-rw-rw-rw-   0        0        0     9645 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/symbl_rest/models/async_audio_url_parameters.py
+-rw-rw-rw-   0        0        0     3925 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/symbl_rest/models/async_confidence_threshold.py
+-rw-rw-rw-   0        0        0     3901 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/symbl_rest/models/async_detect_phrases.py
+-rw-rw-rw-   0        0        0     3917 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/symbl_rest/models/async_enable_all_trackers.py
+-rw-rw-rw-   0        0        0     3909 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/symbl_rest/models/async_entities_payload.py
+-rw-rw-rw-   0        0        0     3893 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/symbl_rest/models/async_meeting_name.py
+-rw-rw-rw-   0        0        0     3901 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/symbl_rest/models/async_messages_field.py
+-rw-rw-rw-   0        0        0     6111 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/symbl_rest/models/async_messages_field_inner.py
+-rw-rw-rw-   0        0        0     5613 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/symbl_rest/models/async_response.py
+-rw-rw-rw-   0        0        0    10584 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/symbl_rest/models/async_text_parameters.py
+-rw-rw-rw-   0        0        0     3881 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/symbl_rest/models/async_trackers.py
+-rw-rw-rw-   0        0        0     5239 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/symbl_rest/models/async_trackers_inner.py
+-rw-rw-rw-   0        0        0     9645 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/symbl_rest/models/async_video_url_parameters.py
+-rw-rw-rw-   0        0        0     7130 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/symbl_rest/models/audio_config.py
+-rw-rw-rw-   0        0        0     4698 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/symbl_rest/models/avatar.py
+-rw-rw-rw-   0        0        0    11454 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/symbl_rest/models/conversation_action_item.py
+-rw-rw-rw-   0        0        0     8075 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/conversation_data_list_response.py
+-rw-rw-rw-   0        0        0    11358 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/conversation_follow_up.py
+-rw-rw-rw-   0        0        0     7886 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/conversation_insight_item.py
+-rw-rw-rw-   0        0        0     9305 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/conversation_intent.py
+-rw-rw-rw-   0        0        0    10038 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/conversation_message.py
+-rw-rw-rw-   0        0        0     7853 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/conversation_question.py
+-rw-rw-rw-   0        0        0     9311 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/conversation_topic.py
+-rw-rw-rw-   0        0        0     5192 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/custom_entities.py
+-rw-rw-rw-   0        0        0     5893 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/duration_payload.py
+-rw-rw-rw-   0        0        0    13099 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/endpoint.py
+-rw-rw-rw-   0        0        0    13417 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/endpoint_connect_request.py
+-rw-rw-rw-   0        0        0     8933 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/endpoint_connect_response.py
+-rw-rw-rw-   0        0        0     4595 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/endpoint_request_data.py
+-rw-rw-rw-   0        0        0     4725 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/entities_list_response.py
+-rw-rw-rw-   0        0        0     8514 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/entities_tag.py
+-rw-rw-rw-   0        0        0     5534 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/error.py
+-rw-rw-rw-   0        0        0     7300 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/external_event.py
+-rw-rw-rw-   0        0        0     4793 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/follow_up_list_response.py
+-rw-rw-rw-   0        0        0     6083 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/from_payload.py
+-rw-rw-rw-   0        0        0     4512 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/generic_error.py
+-rw-rw-rw-   0        0        0     8162 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/grant.py
+-rw-rw-rw-   0        0        0     4761 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/insights_list_response.py
+-rw-rw-rw-   0        0        0     5929 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/intent.py
+-rw-rw-rw-   0        0        0     4709 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/intent_list_response.py
+-rw-rw-rw-   0        0        0     5233 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/job_response.py
+-rw-rw-rw-   0        0        0     4526 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/language.py
+-rw-rw-rw-   0        0        0     4574 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/location_trunc.py
+-rw-rw-rw-   0        0        0     6677 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/matches_items.py
+-rw-rw-rw-   0        0        0     6403 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/matches_items_insight_refs.py
+-rw-rw-rw-   0        0        0     5782 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/matches_items_message_refs.py
+-rw-rw-rw-   0        0        0     4682 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/member_list_response.py
+-rw-rw-rw-   0        0        0     5570 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/members_info.py
+-rw-rw-rw-   0        0        0     4741 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/message_list_response.py
+-rw-rw-rw-   0        0        0     8756 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/metric.py
+-rw-rw-rw-   0        0        0     8450 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/metric_entry.py
+-rw-rw-rw-   0        0        0     3897 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/metric_entry_create.py
+-rw-rw-rw-   0        0        0     5451 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/metric_entry_response.py
+-rw-rw-rw-   0        0        0     5017 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/metric_label.py
+-rw-rw-rw-   0        0        0     5251 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/metric_response.py
+-rw-rw-rw-   0        0        0     5938 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/model_from.py
+-rw-rw-rw-   0        0        0     4993 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/parent_ref.py
+-rw-rw-rw-   0        0        0     4957 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/symbl_rest/models/phrase.py
+-rw-rw-rw-   0        0        0     4773 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/models/question_list_response.py
+-rw-rw-rw-   0        0        0     6445 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/models/refresh_token_request.py
+-rw-rw-rw-   0        0        0     5539 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/models/revoke_token_request.py
+-rw-rw-rw-   0        0        0     5215 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/models/sentiment.py
+-rw-rw-rw-   0        0        0     4518 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/models/sentiment_polarity.py
+-rw-rw-rw-   0        0        0     6892 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/models/session_trunc.py
+-rw-rw-rw-   0        0        0     6344 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/models/session_user.py
+-rw-rw-rw-   0        0        0     5249 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/models/summary_info.py
+-rw-rw-rw-   0        0        0     6072 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/models/tag.py
+-rw-rw-rw-   0        0        0     5478 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/models/text_payload.py
+-rw-rw-rw-   0        0        0     5586 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/models/time_zone.py
+-rw-rw-rw-   0        0        0     5957 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/models/token.py
+-rw-rw-rw-   0        0        0     4677 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/models/topic_list_response.py
+-rw-rw-rw-   0        0        0     5799 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/models/trackers_list_response.py
+-rw-rw-rw-   0        0        0     4552 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/models/unauthorized_error.py
+-rw-rw-rw-   0        0        0     9986 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/models/user_trunc.py
+-rw-rw-rw-   0        0        0     6396 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/symbl_rest/models/word.py
+-rw-rw-rw-   0        0        0    14991 2021-07-26 06:19:33.000000 symbl-rest-1.0.9/symbl_rest/rest.py
+drwxrwxrwx   0        0        0        0 2021-07-26 06:22:07.932557 symbl-rest-1.0.9/symbl_rest.egg-info/
+-rw-rw-rw-   0        0        0     1915 2021-07-26 06:21:53.000000 symbl-rest-1.0.9/symbl_rest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7552 2021-07-26 06:21:55.000000 symbl-rest-1.0.9/symbl_rest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-07-26 06:21:53.000000 symbl-rest-1.0.9/symbl_rest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2021-07-26 06:21:53.000000 symbl-rest-1.0.9/symbl_rest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2021-07-26 06:21:53.000000 symbl-rest-1.0.9/symbl_rest.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-07-26 06:22:14.346794 symbl-rest-1.0.9/test/
+-rw-rw-rw-   0        0        0        0 2021-07-26 06:15:52.000000 symbl-rest-1.0.9/test/__init__.py
+-rw-rw-rw-   0        0        0     2286 2021-07-26 06:15:48.000000 symbl-rest-1.0.9/test/test_action.py
+-rw-rw-rw-   0        0        0     2420 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/test/test_action_item_list_response.py
+-rw-rw-rw-   0        0        0     2349 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_action_items_api.py
+-rw-rw-rw-   0        0        0     2349 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_analytics_api.py
+-rw-rw-rw-   0        0        0     2410 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/test/test_analytics_list_response.py
+-rw-rw-rw-   0        0        0     2402 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/test/test_analytics_members_info.py
+-rw-rw-rw-   0        0        0     2460 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/test/test_analytics_members_info_overlap.py
+-rw-rw-rw-   0        0        0     2608 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/test/test_analytics_members_info_overlap_overlapping_members.py
+-rw-rw-rw-   0        0        0     2436 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/test/test_analytics_members_info_pace.py
+-rw-rw-rw-   0        0        0     2470 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/test/test_analytics_members_info_talk_time.py
+-rw-rw-rw-   0        0        0     2402 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/test/test_analytics_metrics_info.py
+-rw-rw-rw-   0        0        0     3676 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_async_api.py
+-rw-rw-rw-   0        0        0     2428 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/test/test_async_audio_url_parameters.py
+-rw-rw-rw-   0        0        0     2434 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/test/test_async_confidence_threshold.py
+-rw-rw-rw-   0        0        0     2386 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/test/test_async_detect_phrases.py
+-rw-rw-rw-   0        0        0     2420 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/test/test_async_enable_all_trackers.py
+-rw-rw-rw-   0        0        0     2402 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/test/test_async_entities_payload.py
+-rw-rw-rw-   0        0        0     2370 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/test/test_async_meeting_name.py
+-rw-rw-rw-   0        0        0     2386 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/test/test_async_messages_field.py
+-rw-rw-rw-   0        0        0     2428 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/test/test_async_messages_field_inner.py
+-rw-rw-rw-   0        0        0     2344 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/test/test_async_response.py
+-rw-rw-rw-   0        0        0     2394 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/test/test_async_text_parameters.py
+-rw-rw-rw-   0        0        0     2344 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/test/test_async_trackers.py
+-rw-rw-rw-   0        0        0     2386 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/test/test_async_trackers_inner.py
+-rw-rw-rw-   0        0        0     2428 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/test/test_async_video_url_parameters.py
+-rw-rw-rw-   0        0        0     2328 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/test/test_audio_config.py
+-rw-rw-rw-   0        0        0     2641 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_authentication_api.py
+-rw-rw-rw-   0        0        0     2286 2021-07-26 06:15:49.000000 symbl-rest-1.0.9/test/test_avatar.py
+-rw-rw-rw-   0        0        0     2387 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_connection_to_endpoint_api.py
+-rw-rw-rw-   0        0        0     2418 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_conversation_action_item.py
+-rw-rw-rw-   0        0        0     2389 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_conversation_data_api.py
+-rw-rw-rw-   0        0        0     2468 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_conversation_data_list_response.py
+-rw-rw-rw-   0        0        0     2402 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_conversation_follow_up.py
+-rw-rw-rw-   0        0        0     2426 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_conversation_insight_item.py
+-rw-rw-rw-   0        0        0     2384 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_conversation_intent.py
+-rw-rw-rw-   0        0        0     2392 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_conversation_message.py
+-rw-rw-rw-   0        0        0     2400 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_conversation_question.py
+-rw-rw-rw-   0        0        0     2376 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_conversation_topic.py
+-rw-rw-rw-   0        0        0     4536 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_conversations_api.py
+-rw-rw-rw-   0        0        0     2352 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_custom_entities.py
+-rw-rw-rw-   0        0        0     2360 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_duration_payload.py
+-rw-rw-rw-   0        0        0     2302 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_endpoint.py
+-rw-rw-rw-   0        0        0     2418 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_endpoint_connect_request.py
+-rw-rw-rw-   0        0        0     2426 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_endpoint_connect_response.py
+-rw-rw-rw-   0        0        0     2394 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_endpoint_request_data.py
+-rw-rw-rw-   0        0        0     2319 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_entities_api.py
+-rw-rw-rw-   0        0        0     2402 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_entities_list_response.py
+-rw-rw-rw-   0        0        0     2328 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_entities_tag.py
+-rw-rw-rw-   0        0        0     2278 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_error.py
+-rw-rw-rw-   0        0        0     2344 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_external_event.py
+-rw-rw-rw-   0        0        0     2359 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_external_event_web_hook_api.py
+-rw-rw-rw-   0        0        0     2404 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_follow_up_list_response.py
+-rw-rw-rw-   0        0        0     2333 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_follow_ups_api.py
+-rw-rw-rw-   0        0        0     2328 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_from_payload.py
+-rw-rw-rw-   0        0        0     2336 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_generic_error.py
+-rw-rw-rw-   0        0        0     2278 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_grant.py
+-rw-rw-rw-   0        0        0     2321 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_insights_api.py
+-rw-rw-rw-   0        0        0     2402 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_insights_list_response.py
+-rw-rw-rw-   0        0        0     2286 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_intent.py
+-rw-rw-rw-   0        0        0     2386 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_intent_list_response.py
+-rw-rw-rw-   0        0        0     2312 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_intents_api.py
+-rw-rw-rw-   0        0        0     2328 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_job_response.py
+-rw-rw-rw-   0        0        0     2255 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_jobs_api.py
+-rw-rw-rw-   0        0        0     2302 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_language.py
+-rw-rw-rw-   0        0        0     2344 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_location_trunc.py
+-rw-rw-rw-   0        0        0     2336 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_matches_items.py
+-rw-rw-rw-   0        0        0     2428 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_matches_items_insight_refs.py
+-rw-rw-rw-   0        0        0     2428 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_matches_items_message_refs.py
+-rw-rw-rw-   0        0        0     2386 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_member_list_response.py
+-rw-rw-rw-   0        0        0     2313 2021-07-26 06:15:52.000000 symbl-rest-1.0.9/test/test_members_api.py
+-rw-rw-rw-   0        0        0     2328 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_members_info.py
+-rw-rw-rw-   0        0        0     2394 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_message_list_response.py
+-rw-rw-rw-   0        0        0     2321 2021-07-26 06:15:52.000000 symbl-rest-1.0.9/test/test_messages_api.py
+-rw-rw-rw-   0        0        0     2286 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_metric.py
+-rw-rw-rw-   0        0        0     2409 2021-07-26 06:15:52.000000 symbl-rest-1.0.9/test/test_metric_api.py
+-rw-rw-rw-   0        0        0     2328 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_metric_entry.py
+-rw-rw-rw-   0        0        0     2291 2021-07-26 06:15:52.000000 symbl-rest-1.0.9/test/test_metric_entry_api.py
+-rw-rw-rw-   0        0        0     2378 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_metric_entry_create.py
+-rw-rw-rw-   0        0        0     2394 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_metric_entry_response.py
+-rw-rw-rw-   0        0        0     2328 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_metric_label.py
+-rw-rw-rw-   0        0        0     2352 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_metric_response.py
+-rw-rw-rw-   0        0        0     2312 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_model_from.py
+-rw-rw-rw-   0        0        0     2312 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_parent_ref.py
+-rw-rw-rw-   0        0        0     2286 2021-07-26 06:15:50.000000 symbl-rest-1.0.9/test/test_phrase.py
+-rw-rw-rw-   0        0        0     2402 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_question_list_response.py
+-rw-rw-rw-   0        0        0     2328 2021-07-26 06:15:52.000000 symbl-rest-1.0.9/test/test_questions_api.py
+-rw-rw-rw-   0        0        0     2394 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_refresh_token_request.py
+-rw-rw-rw-   0        0        0     2386 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_revoke_token_request.py
+-rw-rw-rw-   0        0        0     2310 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_sentiment.py
+-rw-rw-rw-   0        0        0     2376 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_sentiment_polarity.py
+-rw-rw-rw-   0        0        0     2336 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_session_trunc.py
+-rw-rw-rw-   0        0        0     2328 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_session_user.py
+-rw-rw-rw-   0        0        0     2328 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_summary_info.py
+-rw-rw-rw-   0        0        0     2262 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_tag.py
+-rw-rw-rw-   0        0        0     2328 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_text_payload.py
+-rw-rw-rw-   0        0        0     2304 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_time_zone.py
+-rw-rw-rw-   0        0        0     2278 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_token.py
+-rw-rw-rw-   0        0        0     2378 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_topic_list_response.py
+-rw-rw-rw-   0        0        0     2304 2021-07-26 06:15:52.000000 symbl-rest-1.0.9/test/test_topics_api.py
+-rw-rw-rw-   0        0        0     2312 2021-07-26 06:15:52.000000 symbl-rest-1.0.9/test/test_trackers_api.py
+-rw-rw-rw-   0        0        0     2402 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_trackers_list_response.py
+-rw-rw-rw-   0        0        0     2376 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_unauthorized_error.py
+-rw-rw-rw-   0        0        0     2312 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_user_trunc.py
+-rw-rw-rw-   0        0        0     2270 2021-07-26 06:15:51.000000 symbl-rest-1.0.9/test/test_word.py
```

### Comparing `symbl-rest-1.0.8/PKG-INFO` & `symbl-rest-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: symbl-rest
-Version: 1.0.8
+Version: 1.0.9
 Summary: symbl.ai APIs
 Home-page: UNKNOWN
 Author: UNKNOWN
 Author-email: info@symbl.ai
 License: UNKNOWN
 Description:     &lt;h1&gt;Symbl&#x27;s APIs for external consumers.&lt;/h1&gt; &lt;h2&gt;Language Insights API&lt;/h2&gt; Symbl&#x27;s Language Insights API provides an interface for applications to perform the analysis on the raw text and get insights from it. The API automatically detects sentence boundaries and punctuates the sentences, and also returns the updated messages in the response. Conversations are the most unstructured piece of information that we represent information in, and which most of the leads to lot of loss of information by not being able to capture them correctly.&lt;br/&gt; Language Insights API focuses on understanding such texts and generate the useful and important information from them. &lt;br/&gt; Currently the API supports detection of the Action Items in any type of unstructured text. In future the same API will also have support to detect \&quot;Information\&quot; and \&quot;Event\&quot;, where Information is any informational piece and Event is a reference to something that has happened in the past.&lt;br/&gt; &lt;h2&gt;Telephony Integration&lt;/h2&gt; Symbl can currently integrate with two types of telephony endpoints: 1. SIP trunks&lt;br/&gt; 2. PSTN endpoints&lt;br/&gt; Results are sent via HTTP WebHooks as and when they are available.&lt;br/&gt; &lt;h2&gt;Flow&lt;/h2&gt; 1. External Application invokes REST API to join a meeting/session, with the mode (SIP/PSTN) and joining details&lt;br/&gt; 2. Symbl joins the meeting via SIP or PSTN integration&lt;br/&gt; 3. Symbl continuously processes the audio stream received&lt;br/&gt; 4. Symbl calls WebHook whenever transcription results are available&lt;br/&gt;  # noqa: E501
```

### Comparing `symbl-rest-1.0.8/README.md` & `symbl-rest-1.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://api.symbl.ai*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *ActionItemsApi* | [**get_action_items_by_conversation_id**](docs/ActionItemsApi.md#get_action_items_by_conversation_id) | **GET** /v1/conversations/{conversationId}/action-items | Retrieve action items from conversations
+*AnalyticsApi* | [**get_analytics_by_conversation_id**](docs/AnalyticsApi.md#get_analytics_by_conversation_id) | **GET** /v1/conversations/{conversationId}/analytics | Retrieves speaker ratio, talk time etc from Conversations
 *AsyncApi* | [**add_audio**](docs/AsyncApi.md#add_audio) | **POST** /v1/process/audio | Audio - Submit New Audio File (wav/mp3)
 *AsyncApi* | [**add_audio_url**](docs/AsyncApi.md#add_audio_url) | **POST** /v1/process/audio/url | Audio(URL)  - Submit New Conversation
 *AsyncApi* | [**add_text**](docs/AsyncApi.md#add_text) | **POST** /v1/process/text | Add new Text Messages
 *AsyncApi* | [**add_video**](docs/AsyncApi.md#add_video) | **POST** /v1/process/video | Video - Submit New Video File (mp4)
 *AsyncApi* | [**add_video_url**](docs/AsyncApi.md#add_video_url) | **POST** /v1/process/video/url | Video (URL)  - Submit New Conversation
 *AsyncApi* | [**append_audio**](docs/AsyncApi.md#append_audio) | **PUT** /v1/process/audio/{conversationId} | Audio - Submit New Audio File (wav/mp3)
 *AsyncApi* | [**append_audio_url**](docs/AsyncApi.md#append_audio_url) | **PUT** /v1/process/audio/url/{conversationId} | Audio(URL)  - Submit New Conversation
@@ -88,78 +89,97 @@
 *AsyncApi* | [**append_video_url**](docs/AsyncApi.md#append_video_url) | **PUT** /v1/process/video/url/{conversationId} | Video (URL)  - Submit New Conversation
 *AuthenticationApi* | [**generate_token**](docs/AuthenticationApi.md#generate_token) | **POST** /oauth2/token:generate | Generates the token from the given credentials
 *AuthenticationApi* | [**refresh_token**](docs/AuthenticationApi.md#refresh_token) | **POST** /oauth2/token:refresh | Authenticate and refresh the current valid token
 *AuthenticationApi* | [**revoke_token**](docs/AuthenticationApi.md#revoke_token) | **DELETE** /oauth2/token:revoke | Revoke the given token
 *ConnectionToEndpointApi* | [**connect_to_endpoint**](docs/ConnectionToEndpointApi.md#connect_to_endpoint) | **POST** /v1/endpoint:connect | Connect to your SIP or PSTN endpoint, and control the connection
 *ConversationDataApi* | [**get_conversation_by_conversation_id**](docs/ConversationDataApi.md#get_conversation_by_conversation_id) | **GET** /v1/conversations/{conversationId} | Retrieve Conversation data/meta-data from Conversations
 *ConversationsApi* | [**get_action_items_by_conversation_id**](docs/ConversationsApi.md#get_action_items_by_conversation_id) | **GET** /v1/conversations/{conversationId}/action-items | Retrieve action items from conversations
+*ConversationsApi* | [**get_analytics_by_conversation_id**](docs/ConversationsApi.md#get_analytics_by_conversation_id) | **GET** /v1/conversations/{conversationId}/analytics | Retrieves speaker ratio, talk time etc from Conversations
 *ConversationsApi* | [**get_conversation_by_conversation_id**](docs/ConversationsApi.md#get_conversation_by_conversation_id) | **GET** /v1/conversations/{conversationId} | Retrieve Conversation data/meta-data from Conversations
+*ConversationsApi* | [**get_entities_by_conversation_id**](docs/ConversationsApi.md#get_entities_by_conversation_id) | **GET** /v1/conversations/{conversationId}/entities | Extract Entities from Conversation
 *ConversationsApi* | [**get_follow_ups_by_conversation_id**](docs/ConversationsApi.md#get_follow_ups_by_conversation_id) | **GET** /v1/conversations/{conversationId}/follow-ups | Retrieve follow ups from conversations
 *ConversationsApi* | [**get_insights_by_conversation_id**](docs/ConversationsApi.md#get_insights_by_conversation_id) | **GET** /v1/conversations/{conversationId}/insights | Retrieve insights from Conversations
 *ConversationsApi* | [**get_intents_by_conversation_id**](docs/ConversationsApi.md#get_intents_by_conversation_id) | **GET** /v1/conversations/{conversationId}/intents | Retrieve intents from conversation
 *ConversationsApi* | [**get_members_by_conversation_id**](docs/ConversationsApi.md#get_members_by_conversation_id) | **GET** /v1/conversations/{conversationId}/members | Retrieve members from Conversations
 *ConversationsApi* | [**get_messages_by_conversation_id**](docs/ConversationsApi.md#get_messages_by_conversation_id) | **GET** /v1/conversations/{conversationId}/messages | Retrieve messages from Conversations
 *ConversationsApi* | [**get_questions_by_conversation_id**](docs/ConversationsApi.md#get_questions_by_conversation_id) | **GET** /v1/conversations/{conversationId}/questions | Retrieve questions from conversation
 *ConversationsApi* | [**get_topics_by_conversation_id**](docs/ConversationsApi.md#get_topics_by_conversation_id) | **GET** /v1/conversations/{conversationId}/topics | Retrieve topics from conversation
+*ConversationsApi* | [**get_trackers_by_conversation_id**](docs/ConversationsApi.md#get_trackers_by_conversation_id) | **GET** /v1/conversations/{conversationId}/trackers | Track the Words and Phrases
+*EntitiesApi* | [**get_entities_by_conversation_id**](docs/EntitiesApi.md#get_entities_by_conversation_id) | **GET** /v1/conversations/{conversationId}/entities | Extract Entities from Conversation
 *ExternalEventWebHookApi* | [**external_event_web_hook**](docs/ExternalEventWebHookApi.md#external_event_web_hook) | **POST** /v1/event/{connectionId} | WebHook for external events
 *FollowUpsApi* | [**get_follow_ups_by_conversation_id**](docs/FollowUpsApi.md#get_follow_ups_by_conversation_id) | **GET** /v1/conversations/{conversationId}/follow-ups | Retrieve follow ups from conversations
 *InsightsApi* | [**get_insights_by_conversation_id**](docs/InsightsApi.md#get_insights_by_conversation_id) | **GET** /v1/conversations/{conversationId}/insights | Retrieve insights from Conversations
 *IntentsApi* | [**get_intents_by_conversation_id**](docs/IntentsApi.md#get_intents_by_conversation_id) | **GET** /v1/conversations/{conversationId}/intents | Retrieve intents from conversation
 *JobsApi* | [**get_job_status**](docs/JobsApi.md#get_job_status) | **GET** /v1/job/{jobId} | Retrieve status of a Job
 *MembersApi* | [**get_members_by_conversation_id**](docs/MembersApi.md#get_members_by_conversation_id) | **GET** /v1/conversations/{conversationId}/members | Retrieve members from Conversations
 *MessagesApi* | [**get_messages_by_conversation_id**](docs/MessagesApi.md#get_messages_by_conversation_id) | **GET** /v1/conversations/{conversationId}/messages | Retrieve messages from Conversations
 *MetricApi* | [**add_metric_entry**](docs/MetricApi.md#add_metric_entry) | **POST** /v1/metric/{metricId}/entry | Add new Metric Entry
 *MetricApi* | [**get_metric_by_id**](docs/MetricApi.md#get_metric_by_id) | **GET** /v1/metric/{metricId} | Retrieve Metric
 *MetricEntryApi* | [**add_metric_entry**](docs/MetricEntryApi.md#add_metric_entry) | **POST** /v1/metric/{metricId}/entry | Add new Metric Entry
 *QuestionsApi* | [**get_questions_by_conversation_id**](docs/QuestionsApi.md#get_questions_by_conversation_id) | **GET** /v1/conversations/{conversationId}/questions | Retrieve questions from conversation
 *TopicsApi* | [**get_topics_by_conversation_id**](docs/TopicsApi.md#get_topics_by_conversation_id) | **GET** /v1/conversations/{conversationId}/topics | Retrieve topics from conversation
+*TrackersApi* | [**get_trackers_by_conversation_id**](docs/TrackersApi.md#get_trackers_by_conversation_id) | **GET** /v1/conversations/{conversationId}/trackers | Track the Words and Phrases
 
 ## Documentation For Models
 
  - [Action](docs/Action.md)
  - [ActionItemListResponse](docs/ActionItemListResponse.md)
+ - [AnalyticsListResponse](docs/AnalyticsListResponse.md)
+ - [AnalyticsMembersInfo](docs/AnalyticsMembersInfo.md)
+ - [AnalyticsMembersInfoOverlap](docs/AnalyticsMembersInfoOverlap.md)
+ - [AnalyticsMembersInfoOverlapOverlappingMembers](docs/AnalyticsMembersInfoOverlapOverlappingMembers.md)
+ - [AnalyticsMembersInfoPace](docs/AnalyticsMembersInfoPace.md)
+ - [AnalyticsMembersInfoTalkTime](docs/AnalyticsMembersInfoTalkTime.md)
+ - [AnalyticsMetricsInfo](docs/AnalyticsMetricsInfo.md)
  - [AsyncAudioUrlParameters](docs/AsyncAudioUrlParameters.md)
  - [AsyncConfidenceThreshold](docs/AsyncConfidenceThreshold.md)
  - [AsyncDetectPhrases](docs/AsyncDetectPhrases.md)
+ - [AsyncEnableAllTrackers](docs/AsyncEnableAllTrackers.md)
  - [AsyncEntitiesPayload](docs/AsyncEntitiesPayload.md)
  - [AsyncMeetingName](docs/AsyncMeetingName.md)
  - [AsyncMessagesField](docs/AsyncMessagesField.md)
  - [AsyncMessagesFieldInner](docs/AsyncMessagesFieldInner.md)
  - [AsyncResponse](docs/AsyncResponse.md)
  - [AsyncTextParameters](docs/AsyncTextParameters.md)
+ - [AsyncTrackers](docs/AsyncTrackers.md)
+ - [AsyncTrackersInner](docs/AsyncTrackersInner.md)
  - [AsyncVideoUrlParameters](docs/AsyncVideoUrlParameters.md)
  - [AudioConfig](docs/AudioConfig.md)
  - [Avatar](docs/Avatar.md)
  - [ConversationActionItem](docs/ConversationActionItem.md)
  - [ConversationDataListResponse](docs/ConversationDataListResponse.md)
  - [ConversationFollowUp](docs/ConversationFollowUp.md)
  - [ConversationInsightItem](docs/ConversationInsightItem.md)
  - [ConversationIntent](docs/ConversationIntent.md)
  - [ConversationMessage](docs/ConversationMessage.md)
  - [ConversationQuestion](docs/ConversationQuestion.md)
  - [ConversationTopic](docs/ConversationTopic.md)
  - [CustomEntities](docs/CustomEntities.md)
- - [CustomEntitiesMessageRefs](docs/CustomEntitiesMessageRefs.md)
  - [DurationPayload](docs/DurationPayload.md)
  - [Endpoint](docs/Endpoint.md)
  - [EndpointConnectRequest](docs/EndpointConnectRequest.md)
  - [EndpointConnectResponse](docs/EndpointConnectResponse.md)
  - [EndpointRequestData](docs/EndpointRequestData.md)
+ - [EntitiesListResponse](docs/EntitiesListResponse.md)
+ - [EntitiesTag](docs/EntitiesTag.md)
  - [Error](docs/Error.md)
  - [ExternalEvent](docs/ExternalEvent.md)
  - [FollowUpListResponse](docs/FollowUpListResponse.md)
  - [FromPayload](docs/FromPayload.md)
  - [GenericError](docs/GenericError.md)
  - [Grant](docs/Grant.md)
  - [InsightsListResponse](docs/InsightsListResponse.md)
  - [Intent](docs/Intent.md)
  - [IntentListResponse](docs/IntentListResponse.md)
  - [JobResponse](docs/JobResponse.md)
  - [Language](docs/Language.md)
  - [LocationTrunc](docs/LocationTrunc.md)
+ - [MatchesItems](docs/MatchesItems.md)
+ - [MatchesItemsInsightRefs](docs/MatchesItemsInsightRefs.md)
+ - [MatchesItemsMessageRefs](docs/MatchesItemsMessageRefs.md)
  - [MemberListResponse](docs/MemberListResponse.md)
  - [MembersInfo](docs/MembersInfo.md)
  - [MessageListResponse](docs/MessageListResponse.md)
  - [Metric](docs/Metric.md)
  - [MetricEntry](docs/MetricEntry.md)
  - [MetricEntryCreate](docs/MetricEntryCreate.md)
  - [MetricEntryResponse](docs/MetricEntryResponse.md)
@@ -177,14 +197,15 @@
  - [SessionUser](docs/SessionUser.md)
  - [SummaryInfo](docs/SummaryInfo.md)
  - [Tag](docs/Tag.md)
  - [TextPayload](docs/TextPayload.md)
  - [TimeZone](docs/TimeZone.md)
  - [Token](docs/Token.md)
  - [TopicListResponse](docs/TopicListResponse.md)
+ - [TrackersListResponse](docs/TrackersListResponse.md)
  - [UnauthorizedError](docs/UnauthorizedError.md)
  - [UserTrunc](docs/UserTrunc.md)
  - [Word](docs/Word.md)
 
 ## Documentation For Authorization
```

### Comparing `symbl-rest-1.0.8/setup.py` & `symbl-rest-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Contact: info@symbl.ai
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "symbl-rest"
-VERSION = "1.0.8"
+VERSION = "1.0.9"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `symbl-rest-1.0.8/symbl_rest/__init__.py` & `symbl-rest-1.0.9/symbl_rest/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,75 +12,92 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 # import apis into sdk package
 from symbl_rest.api.action_items_api import ActionItemsApi
+from symbl_rest.api.analytics_api import AnalyticsApi
 from symbl_rest.api.async_api import AsyncApi
 from symbl_rest.api.authentication_api import AuthenticationApi
 from symbl_rest.api.connection_to_endpoint_api import ConnectionToEndpointApi
 from symbl_rest.api.conversation_data_api import ConversationDataApi
 from symbl_rest.api.conversations_api import ConversationsApi
+from symbl_rest.api.entities_api import EntitiesApi
 from symbl_rest.api.external_event_web_hook_api import ExternalEventWebHookApi
 from symbl_rest.api.follow_ups_api import FollowUpsApi
 from symbl_rest.api.insights_api import InsightsApi
 from symbl_rest.api.intents_api import IntentsApi
 from symbl_rest.api.jobs_api import JobsApi
 from symbl_rest.api.members_api import MembersApi
 from symbl_rest.api.messages_api import MessagesApi
 from symbl_rest.api.metric_api import MetricApi
 from symbl_rest.api.metric_entry_api import MetricEntryApi
 from symbl_rest.api.questions_api import QuestionsApi
 from symbl_rest.api.topics_api import TopicsApi
+from symbl_rest.api.trackers_api import TrackersApi
 # import ApiClient
 from symbl_rest.api_client import ApiClient
 from symbl_rest.configuration import Configuration
 # import models into sdk package
 from symbl_rest.models.action import Action
 from symbl_rest.models.action_item_list_response import ActionItemListResponse
+from symbl_rest.models.analytics_list_response import AnalyticsListResponse
+from symbl_rest.models.analytics_members_info import AnalyticsMembersInfo
+from symbl_rest.models.analytics_members_info_overlap import AnalyticsMembersInfoOverlap
+from symbl_rest.models.analytics_members_info_overlap_overlapping_members import AnalyticsMembersInfoOverlapOverlappingMembers
+from symbl_rest.models.analytics_members_info_pace import AnalyticsMembersInfoPace
+from symbl_rest.models.analytics_members_info_talk_time import AnalyticsMembersInfoTalkTime
+from symbl_rest.models.analytics_metrics_info import AnalyticsMetricsInfo
 from symbl_rest.models.async_audio_url_parameters import AsyncAudioUrlParameters
 from symbl_rest.models.async_confidence_threshold import AsyncConfidenceThreshold
 from symbl_rest.models.async_detect_phrases import AsyncDetectPhrases
+from symbl_rest.models.async_enable_all_trackers import AsyncEnableAllTrackers
 from symbl_rest.models.async_entities_payload import AsyncEntitiesPayload
 from symbl_rest.models.async_meeting_name import AsyncMeetingName
 from symbl_rest.models.async_messages_field import AsyncMessagesField
 from symbl_rest.models.async_messages_field_inner import AsyncMessagesFieldInner
 from symbl_rest.models.async_response import AsyncResponse
 from symbl_rest.models.async_text_parameters import AsyncTextParameters
+from symbl_rest.models.async_trackers import AsyncTrackers
+from symbl_rest.models.async_trackers_inner import AsyncTrackersInner
 from symbl_rest.models.async_video_url_parameters import AsyncVideoUrlParameters
 from symbl_rest.models.audio_config import AudioConfig
 from symbl_rest.models.avatar import Avatar
 from symbl_rest.models.conversation_action_item import ConversationActionItem
 from symbl_rest.models.conversation_data_list_response import ConversationDataListResponse
 from symbl_rest.models.conversation_follow_up import ConversationFollowUp
 from symbl_rest.models.conversation_insight_item import ConversationInsightItem
 from symbl_rest.models.conversation_intent import ConversationIntent
 from symbl_rest.models.conversation_message import ConversationMessage
 from symbl_rest.models.conversation_question import ConversationQuestion
 from symbl_rest.models.conversation_topic import ConversationTopic
 from symbl_rest.models.custom_entities import CustomEntities
-from symbl_rest.models.custom_entities_message_refs import CustomEntitiesMessageRefs
 from symbl_rest.models.duration_payload import DurationPayload
 from symbl_rest.models.endpoint import Endpoint
 from symbl_rest.models.endpoint_connect_request import EndpointConnectRequest
 from symbl_rest.models.endpoint_connect_response import EndpointConnectResponse
 from symbl_rest.models.endpoint_request_data import EndpointRequestData
+from symbl_rest.models.entities_list_response import EntitiesListResponse
+from symbl_rest.models.entities_tag import EntitiesTag
 from symbl_rest.models.error import Error
 from symbl_rest.models.external_event import ExternalEvent
 from symbl_rest.models.follow_up_list_response import FollowUpListResponse
 from symbl_rest.models.from_payload import FromPayload
 from symbl_rest.models.generic_error import GenericError
 from symbl_rest.models.grant import Grant
 from symbl_rest.models.insights_list_response import InsightsListResponse
 from symbl_rest.models.intent import Intent
 from symbl_rest.models.intent_list_response import IntentListResponse
 from symbl_rest.models.job_response import JobResponse
 from symbl_rest.models.language import Language
 from symbl_rest.models.location_trunc import LocationTrunc
+from symbl_rest.models.matches_items import MatchesItems
+from symbl_rest.models.matches_items_insight_refs import MatchesItemsInsightRefs
+from symbl_rest.models.matches_items_message_refs import MatchesItemsMessageRefs
 from symbl_rest.models.member_list_response import MemberListResponse
 from symbl_rest.models.members_info import MembersInfo
 from symbl_rest.models.message_list_response import MessageListResponse
 from symbl_rest.models.metric import Metric
 from symbl_rest.models.metric_entry import MetricEntry
 from symbl_rest.models.metric_entry_create import MetricEntryCreate
 from symbl_rest.models.metric_entry_response import MetricEntryResponse
@@ -98,10 +115,11 @@
 from symbl_rest.models.session_user import SessionUser
 from symbl_rest.models.summary_info import SummaryInfo
 from symbl_rest.models.tag import Tag
 from symbl_rest.models.text_payload import TextPayload
 from symbl_rest.models.time_zone import TimeZone
 from symbl_rest.models.token import Token
 from symbl_rest.models.topic_list_response import TopicListResponse
+from symbl_rest.models.trackers_list_response import TrackersListResponse
 from symbl_rest.models.unauthorized_error import UnauthorizedError
 from symbl_rest.models.user_trunc import UserTrunc
 from symbl_rest.models.word import Word
```

### Comparing `symbl-rest-1.0.8/symbl_rest/api/__init__.py` & `symbl-rest-1.0.9/symbl_rest/api/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from __future__ import absolute_import
 
 # flake8: noqa
 
 # import apis into api package
 from symbl_rest.api.action_items_api import ActionItemsApi
+from symbl_rest.api.analytics_api import AnalyticsApi
 from symbl_rest.api.async_api import AsyncApi
 from symbl_rest.api.authentication_api import AuthenticationApi
 from symbl_rest.api.connection_to_endpoint_api import ConnectionToEndpointApi
 from symbl_rest.api.conversation_data_api import ConversationDataApi
 from symbl_rest.api.conversations_api import ConversationsApi
+from symbl_rest.api.entities_api import EntitiesApi
 from symbl_rest.api.external_event_web_hook_api import ExternalEventWebHookApi
 from symbl_rest.api.follow_ups_api import FollowUpsApi
 from symbl_rest.api.insights_api import InsightsApi
 from symbl_rest.api.intents_api import IntentsApi
 from symbl_rest.api.jobs_api import JobsApi
 from symbl_rest.api.members_api import MembersApi
 from symbl_rest.api.messages_api import MessagesApi
 from symbl_rest.api.metric_api import MetricApi
 from symbl_rest.api.metric_entry_api import MetricEntryApi
 from symbl_rest.api.questions_api import QuestionsApi
 from symbl_rest.api.topics_api import TopicsApi
+from symbl_rest.api.trackers_api import TrackersApi
```

### Comparing `symbl-rest-1.0.8/symbl_rest/api/action_items_api.py` & `symbl-rest-1.0.9/symbl_rest/api/action_items_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/api/async_api.py` & `symbl-rest-1.0.9/symbl_rest/api/async_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,16 +44,17 @@
         :param async_req bool
         :param Object body: (required)
         :param str content_type: (required)
         :param str name:
         :param str webhook_url:
         :param list[str] custom_vocabulary:
         :param float confidence_threshold:
-        :param str custom_entities:
+        :param str entities:
         :param bool detect_entities:
+        :param bool enable_all_trackers:
         :param bool detect_phrases:
         :param bool enable_separate_recognition_per_channel:
         :param str channel_metadata:
         :param str language_code:
         :param str mode:
         :param str trackers:
         :param bool enable_speaker_diarization:
@@ -81,30 +82,31 @@
         :param async_req bool
         :param Object body: (required)
         :param str content_type: (required)
         :param str name:
         :param str webhook_url:
         :param list[str] custom_vocabulary:
         :param float confidence_threshold:
-        :param str custom_entities:
+        :param str entities:
         :param bool detect_entities:
+        :param bool enable_all_trackers:
         :param bool detect_phrases:
         :param bool enable_separate_recognition_per_channel:
         :param str channel_metadata:
         :param str language_code:
         :param str mode:
         :param str trackers:
         :param bool enable_speaker_diarization:
         :param float diarization_speaker_count:
         :return: AsyncResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['body', 'content_type', 'name', 'webhook_url', 'custom_vocabulary', 'confidence_threshold', 'custom_entities', 'detect_entities', 'detect_phrases', 'enable_separate_recognition_per_channel', 'channel_metadata', 'language_code', 'mode', 'trackers', 'enable_speaker_diarization', 'diarization_speaker_count']  # noqa: E501
+        all_params = ['body', 'content_type', 'name', 'webhook_url', 'custom_vocabulary', 'confidence_threshold', 'entities', 'detect_entities', 'enable_all_trackers', 'detect_phrases', 'enable_separate_recognition_per_channel', 'channel_metadata', 'language_code', 'mode', 'trackers', 'enable_speaker_diarization', 'diarization_speaker_count']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -134,18 +136,20 @@
         if 'webhook_url' in params:
             query_params.append(('webhookUrl', params['webhook_url']))  # noqa: E501
         if 'custom_vocabulary' in params:
             query_params.append(('customVocabulary', params['custom_vocabulary']))  # noqa: E501
             collection_formats['customVocabulary'] = 'multi'  # noqa: E501
         if 'confidence_threshold' in params:
             query_params.append(('confidenceThreshold', params['confidence_threshold']))  # noqa: E501
-        if 'custom_entities' in params:
-            query_params.append(('customEntities', params['custom_entities']))  # noqa: E501
+        if 'entities' in params:
+            query_params.append(('entities', params['entities']))  # noqa: E501
         if 'detect_entities' in params:
             query_params.append(('detectEntities', params['detect_entities']))  # noqa: E501
+        if 'enable_all_trackers' in params:
+            query_params.append(('enableAllTrackers', params['enable_all_trackers']))  # noqa: E501
         if 'detect_phrases' in params:
             query_params.append(('detectPhrases', params['detect_phrases']))  # noqa: E501
         if 'enable_separate_recognition_per_channel' in params:
             query_params.append(('enableSeparateRecognitionPerChannel', params['enable_separate_recognition_per_channel']))  # noqa: E501
         if 'channel_metadata' in params:
             query_params.append(('channelMetadata', params['channel_metadata']))  # noqa: E501
         if 'language_code' in params:
@@ -413,16 +417,17 @@
         :param async_req bool
         :param str body: (required)
         :param str content_type: (required)
         :param str name:
         :param str webhook_url:
         :param list[str] custom_vocabulary:
         :param float confidence_threshold:
-        :param str custom_entities:
+        :param str entities:
         :param bool detect_entities:
+        :param bool enable_all_trackers:
         :param bool detect_phrases:
         :param bool enable_separate_recognition_per_channel:
         :param str channel_metadata:
         :param str language_code:
         :param str mode:
         :param str trackers:
         :param bool enable_speaker_diarization:
@@ -450,30 +455,31 @@
         :param async_req bool
         :param str body: (required)
         :param str content_type: (required)
         :param str name:
         :param str webhook_url:
         :param list[str] custom_vocabulary:
         :param float confidence_threshold:
-        :param str custom_entities:
+        :param str entities:
         :param bool detect_entities:
+        :param bool enable_all_trackers:
         :param bool detect_phrases:
         :param bool enable_separate_recognition_per_channel:
         :param str channel_metadata:
         :param str language_code:
         :param str mode:
         :param str trackers:
         :param bool enable_speaker_diarization:
         :param float diarization_speaker_count:
         :return: AsyncResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['body', 'content_type', 'name', 'webhook_url', 'custom_vocabulary', 'confidence_threshold', 'custom_entities', 'detect_entities', 'detect_phrases', 'enable_separate_recognition_per_channel', 'channel_metadata', 'language_code', 'mode', 'trackers', 'enable_speaker_diarization', 'diarization_speaker_count']  # noqa: E501
+        all_params = ['body', 'content_type', 'name', 'webhook_url', 'custom_vocabulary', 'confidence_threshold', 'entities', 'detect_entities', 'enable_all_trackers', 'detect_phrases', 'enable_separate_recognition_per_channel', 'channel_metadata', 'language_code', 'mode', 'trackers', 'enable_speaker_diarization', 'diarization_speaker_count']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -503,18 +509,20 @@
         if 'webhook_url' in params:
             query_params.append(('webhookUrl', params['webhook_url']))  # noqa: E501
         if 'custom_vocabulary' in params:
             query_params.append(('customVocabulary', params['custom_vocabulary']))  # noqa: E501
             collection_formats['customVocabulary'] = 'multi'  # noqa: E501
         if 'confidence_threshold' in params:
             query_params.append(('confidenceThreshold', params['confidence_threshold']))  # noqa: E501
-        if 'custom_entities' in params:
-            query_params.append(('customEntities', params['custom_entities']))  # noqa: E501
+        if 'entities' in params:
+            query_params.append(('entities', params['entities']))  # noqa: E501
         if 'detect_entities' in params:
             query_params.append(('detectEntities', params['detect_entities']))  # noqa: E501
+        if 'enable_all_trackers' in params:
+            query_params.append(('enableAllTrackers', params['enable_all_trackers']))  # noqa: E501
         if 'detect_phrases' in params:
             query_params.append(('detectPhrases', params['detect_phrases']))  # noqa: E501
         if 'enable_separate_recognition_per_channel' in params:
             query_params.append(('enableSeparateRecognitionPerChannel', params['enable_separate_recognition_per_channel']))  # noqa: E501
         if 'channel_metadata' in params:
             query_params.append(('channelMetadata', params['channel_metadata']))  # noqa: E501
         if 'language_code' in params:
@@ -684,15 +692,16 @@
         :param Object body: (required)
         :param str content_type: (required)
         :param str conversation_id: ID of the conversation (required)
         :param str name:
         :param str webhook_url:
         :param list[str] custom_vocabulary:
         :param float confidence_threshold:
-        :param str custom_entities:
+        :param str entities:
+        :param bool enable_all_trackers:
         :param bool detect_entities:
         :param bool detect_phrases:
         :param bool enable_separate_recognition_per_channel:
         :param str channel_metadata:
         :param str language_code:
         :param str mode:
         :param str trackers:
@@ -722,30 +731,31 @@
         :param Object body: (required)
         :param str content_type: (required)
         :param str conversation_id: ID of the conversation (required)
         :param str name:
         :param str webhook_url:
         :param list[str] custom_vocabulary:
         :param float confidence_threshold:
-        :param str custom_entities:
+        :param str entities:
+        :param bool enable_all_trackers:
         :param bool detect_entities:
         :param bool detect_phrases:
         :param bool enable_separate_recognition_per_channel:
         :param str channel_metadata:
         :param str language_code:
         :param str mode:
         :param str trackers:
         :param bool enable_speaker_diarization:
         :param float diarization_speaker_count:
         :return: AsyncResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['body', 'content_type', 'conversation_id', 'name', 'webhook_url', 'custom_vocabulary', 'confidence_threshold', 'custom_entities', 'detect_entities', 'detect_phrases', 'enable_separate_recognition_per_channel', 'channel_metadata', 'language_code', 'mode', 'trackers', 'enable_speaker_diarization', 'diarization_speaker_count']  # noqa: E501
+        all_params = ['body', 'content_type', 'conversation_id', 'name', 'webhook_url', 'custom_vocabulary', 'confidence_threshold', 'entities', 'enable_all_trackers', 'detect_entities', 'detect_phrases', 'enable_separate_recognition_per_channel', 'channel_metadata', 'language_code', 'mode', 'trackers', 'enable_speaker_diarization', 'diarization_speaker_count']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -781,16 +791,18 @@
         if 'webhook_url' in params:
             query_params.append(('webhookUrl', params['webhook_url']))  # noqa: E501
         if 'custom_vocabulary' in params:
             query_params.append(('customVocabulary', params['custom_vocabulary']))  # noqa: E501
             collection_formats['customVocabulary'] = 'multi'  # noqa: E501
         if 'confidence_threshold' in params:
             query_params.append(('confidenceThreshold', params['confidence_threshold']))  # noqa: E501
-        if 'custom_entities' in params:
-            query_params.append(('customEntities', params['custom_entities']))  # noqa: E501
+        if 'entities' in params:
+            query_params.append(('entities', params['entities']))  # noqa: E501
+        if 'enable_all_trackers' in params:
+            query_params.append(('enableAllTrackers', params['enable_all_trackers']))  # noqa: E501
         if 'detect_entities' in params:
             query_params.append(('detectEntities', params['detect_entities']))  # noqa: E501
         if 'detect_phrases' in params:
             query_params.append(('detectPhrases', params['detect_phrases']))  # noqa: E501
         if 'enable_separate_recognition_per_channel' in params:
             query_params.append(('enableSeparateRecognitionPerChannel', params['enable_separate_recognition_per_channel']))  # noqa: E501
         if 'channel_metadata' in params:
@@ -1077,15 +1089,15 @@
         :param str body: (required)
         :param str content_type: (required)
         :param str conversation_id: ID of the conversation (required)
         :param str name:
         :param str webhook_url:
         :param list[str] custom_vocabulary:
         :param float confidence_threshold:
-        :param str custom_entities:
+        :param str entities:
         :param bool detect_entities:
         :param bool detect_phrases:
         :param bool enable_separate_recognition_per_channel:
         :param str channel_metadata:
         :param str language_code:
         :param str mode:
         :param str trackers:
@@ -1115,30 +1127,30 @@
         :param str body: (required)
         :param str content_type: (required)
         :param str conversation_id: ID of the conversation (required)
         :param str name:
         :param str webhook_url:
         :param list[str] custom_vocabulary:
         :param float confidence_threshold:
-        :param str custom_entities:
+        :param str entities:
         :param bool detect_entities:
         :param bool detect_phrases:
         :param bool enable_separate_recognition_per_channel:
         :param str channel_metadata:
         :param str language_code:
         :param str mode:
         :param str trackers:
         :param bool enable_speaker_diarization:
         :param float diarization_speaker_count:
         :return: AsyncResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['body', 'content_type', 'conversation_id', 'name', 'webhook_url', 'custom_vocabulary', 'confidence_threshold', 'custom_entities', 'detect_entities', 'detect_phrases', 'enable_separate_recognition_per_channel', 'channel_metadata', 'language_code', 'mode', 'trackers', 'enable_speaker_diarization', 'diarization_speaker_count']  # noqa: E501
+        all_params = ['body', 'content_type', 'conversation_id', 'name', 'webhook_url', 'custom_vocabulary', 'confidence_threshold', 'entities', 'detect_entities', 'detect_phrases', 'enable_separate_recognition_per_channel', 'channel_metadata', 'language_code', 'mode', 'trackers', 'enable_speaker_diarization', 'diarization_speaker_count']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -1174,16 +1186,16 @@
         if 'webhook_url' in params:
             query_params.append(('webhookUrl', params['webhook_url']))  # noqa: E501
         if 'custom_vocabulary' in params:
             query_params.append(('customVocabulary', params['custom_vocabulary']))  # noqa: E501
             collection_formats['customVocabulary'] = 'multi'  # noqa: E501
         if 'confidence_threshold' in params:
             query_params.append(('confidenceThreshold', params['confidence_threshold']))  # noqa: E501
-        if 'custom_entities' in params:
-            query_params.append(('customEntities', params['custom_entities']))  # noqa: E501
+        if 'entities' in params:
+            query_params.append(('entities', params['entities']))  # noqa: E501
         if 'detect_entities' in params:
             query_params.append(('detectEntities', params['detect_entities']))  # noqa: E501
         if 'detect_phrases' in params:
             query_params.append(('detectPhrases', params['detect_phrases']))  # noqa: E501
         if 'enable_separate_recognition_per_channel' in params:
             query_params.append(('enableSeparateRecognitionPerChannel', params['enable_separate_recognition_per_channel']))  # noqa: E501
         if 'channel_metadata' in params:
```

### Comparing `symbl-rest-1.0.8/symbl_rest/api/authentication_api.py` & `symbl-rest-1.0.9/symbl_rest/api/authentication_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/api/connection_to_endpoint_api.py` & `symbl-rest-1.0.9/symbl_rest/api/connection_to_endpoint_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/api/conversation_data_api.py` & `symbl-rest-1.0.9/symbl_rest/api/conversation_data_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/api/conversations_api.py` & `symbl-rest-1.0.9/symbl_rest/api/conversations_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -123,14 +123,109 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def get_analytics_by_conversation_id(self, conversation_id, **kwargs):  # noqa: E501
+        """Retrieves speaker ratio, talk time etc from Conversations  # noqa: E501
+
+        Get speaker ratio, talk time, silence, pace and overlap from conversation by Conversation Id. Returns an Analytic object.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_analytics_by_conversation_id(conversation_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str conversation_id: ID of the conversation (required)
+        :return: AnalyticsListResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.get_analytics_by_conversation_id_with_http_info(conversation_id, **kwargs)  # noqa: E501
+        else:
+            (data) = self.get_analytics_by_conversation_id_with_http_info(conversation_id, **kwargs)  # noqa: E501
+            return data
+
+    def get_analytics_by_conversation_id_with_http_info(self, conversation_id, **kwargs):  # noqa: E501
+        """Retrieves speaker ratio, talk time etc from Conversations  # noqa: E501
+
+        Get speaker ratio, talk time, silence, pace and overlap from conversation by Conversation Id. Returns an Analytic object.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_analytics_by_conversation_id_with_http_info(conversation_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str conversation_id: ID of the conversation (required)
+        :return: AnalyticsListResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['conversation_id']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_analytics_by_conversation_id" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'conversation_id' is set
+        if ('conversation_id' not in params or
+                params['conversation_id'] is None):
+            raise ValueError("Missing the required parameter `conversation_id` when calling `get_analytics_by_conversation_id`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'conversation_id' in params:
+            path_params['conversationId'] = params['conversation_id']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['bearerAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/v1/conversations/{conversationId}/analytics', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='AnalyticsListResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def get_conversation_by_conversation_id(self, conversation_id, **kwargs):  # noqa: E501
         """Retrieve Conversation data/meta-data from Conversations  # noqa: E501
 
         Get all conversation data by conversationId. Returns conversationData object.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_conversation_by_conversation_id(conversation_id, async_req=True)
@@ -218,14 +313,109 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def get_entities_by_conversation_id(self, conversation_id, **kwargs):  # noqa: E501
+        """Extract Entities from Conversation  # noqa: E501
+
+        Get all Entities  by conversationId. Returns Entity object.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_entities_by_conversation_id(conversation_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str conversation_id: ID of the conversation (required)
+        :return: EntitiesListResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.get_entities_by_conversation_id_with_http_info(conversation_id, **kwargs)  # noqa: E501
+        else:
+            (data) = self.get_entities_by_conversation_id_with_http_info(conversation_id, **kwargs)  # noqa: E501
+            return data
+
+    def get_entities_by_conversation_id_with_http_info(self, conversation_id, **kwargs):  # noqa: E501
+        """Extract Entities from Conversation  # noqa: E501
+
+        Get all Entities  by conversationId. Returns Entity object.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_entities_by_conversation_id_with_http_info(conversation_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str conversation_id: ID of the conversation (required)
+        :return: EntitiesListResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['conversation_id']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_entities_by_conversation_id" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'conversation_id' is set
+        if ('conversation_id' not in params or
+                params['conversation_id'] is None):
+            raise ValueError("Missing the required parameter `conversation_id` when calling `get_entities_by_conversation_id`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'conversation_id' in params:
+            path_params['conversationId'] = params['conversation_id']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['bearerAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/v1/conversations/{conversationId}/entities', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='EntitiesListResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def get_follow_ups_by_conversation_id(self, conversation_id, **kwargs):  # noqa: E501
         """Retrieve follow ups from conversations  # noqa: E501
 
         Get all follow-ups by conversationId. Returns follow-ups object.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_follow_ups_by_conversation_id(conversation_id, async_req=True)
@@ -898,7 +1088,102 @@
             response_type='TopicListResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
+
+    def get_trackers_by_conversation_id(self, conversation_id, **kwargs):  # noqa: E501
+        """Track the Words and Phrases  # noqa: E501
+
+        Track the occurrence of certain key words or phrases in a conversation by Conversation Id. Returns Tracker object.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_trackers_by_conversation_id(conversation_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str conversation_id: ID of the conversation (required)
+        :return: list[TrackersListResponse]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.get_trackers_by_conversation_id_with_http_info(conversation_id, **kwargs)  # noqa: E501
+        else:
+            (data) = self.get_trackers_by_conversation_id_with_http_info(conversation_id, **kwargs)  # noqa: E501
+            return data
+
+    def get_trackers_by_conversation_id_with_http_info(self, conversation_id, **kwargs):  # noqa: E501
+        """Track the Words and Phrases  # noqa: E501
+
+        Track the occurrence of certain key words or phrases in a conversation by Conversation Id. Returns Tracker object.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_trackers_by_conversation_id_with_http_info(conversation_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str conversation_id: ID of the conversation (required)
+        :return: list[TrackersListResponse]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['conversation_id']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_trackers_by_conversation_id" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'conversation_id' is set
+        if ('conversation_id' not in params or
+                params['conversation_id'] is None):
+            raise ValueError("Missing the required parameter `conversation_id` when calling `get_trackers_by_conversation_id`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'conversation_id' in params:
+            path_params['conversationId'] = params['conversation_id']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['bearerAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/v1/conversations/{conversationId}/trackers', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='list[TrackersListResponse]',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
```

### Comparing `symbl-rest-1.0.8/symbl_rest/api/external_event_web_hook_api.py` & `symbl-rest-1.0.9/symbl_rest/api/external_event_web_hook_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/api/follow_ups_api.py` & `symbl-rest-1.0.9/symbl_rest/api/follow_ups_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/api/insights_api.py` & `symbl-rest-1.0.9/symbl_rest/api/insights_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/api/intents_api.py` & `symbl-rest-1.0.9/symbl_rest/api/intents_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/api/jobs_api.py` & `symbl-rest-1.0.9/symbl_rest/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/api/members_api.py` & `symbl-rest-1.0.9/symbl_rest/api/members_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/api/messages_api.py` & `symbl-rest-1.0.9/symbl_rest/api/messages_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/api/metric_api.py` & `symbl-rest-1.0.9/symbl_rest/api/metric_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/api/metric_entry_api.py` & `symbl-rest-1.0.9/symbl_rest/api/metric_entry_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/api/questions_api.py` & `symbl-rest-1.0.9/symbl_rest/api/questions_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/api/topics_api.py` & `symbl-rest-1.0.9/symbl_rest/api/topics_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/api_client.py` & `symbl-rest-1.0.9/symbl_rest/api_client.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/configuration.py` & `symbl-rest-1.0.9/symbl_rest/configuration.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/action.py` & `symbl-rest-1.0.9/symbl_rest/models/action.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/action_item_list_response.py` & `symbl-rest-1.0.9/symbl_rest/models/action_item_list_response.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/async_audio_url_parameters.py` & `symbl-rest-1.0.9/symbl_rest/models/async_audio_url_parameters.py`

 * *Files 24% similar despite different names*

```diff
@@ -26,45 +26,55 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'url': 'str',
         'entities': 'AsyncEntitiesPayload',
+        'enable_all_trackers': 'AsyncEnableAllTrackers',
         'detect_phrases': 'AsyncDetectPhrases',
         'confidence_threshold': 'AsyncConfidenceThreshold',
-        'name': 'AsyncMeetingName'
+        'name': 'AsyncMeetingName',
+        'trackers': 'AsyncTrackers'
     }
 
     attribute_map = {
         'url': 'url',
         'entities': 'entities',
+        'enable_all_trackers': 'enableAllTrackers',
         'detect_phrases': 'detectPhrases',
         'confidence_threshold': 'confidenceThreshold',
-        'name': 'name'
+        'name': 'name',
+        'trackers': 'trackers'
     }
 
-    def __init__(self, url=None, entities=None, detect_phrases=None, confidence_threshold=None, name=None):  # noqa: E501
+    def __init__(self, url=None, entities=None, enable_all_trackers=None, detect_phrases=None, confidence_threshold=None, name=None, trackers=None):  # noqa: E501
         """AsyncAudioUrlParameters - a model defined in Swagger"""  # noqa: E501
         self._url = None
         self._entities = None
+        self._enable_all_trackers = None
         self._detect_phrases = None
         self._confidence_threshold = None
         self._name = None
+        self._trackers = None
         self.discriminator = None
         if url is not None:
             self.url = url
         if entities is not None:
             self.entities = entities
+        if enable_all_trackers is not None:
+            self.enable_all_trackers = enable_all_trackers
         if detect_phrases is not None:
             self.detect_phrases = detect_phrases
         if confidence_threshold is not None:
             self.confidence_threshold = confidence_threshold
         if name is not None:
             self.name = name
+        if trackers is not None:
+            self.trackers = trackers
 
     @property
     def url(self):
         """Gets the url of this AsyncAudioUrlParameters.  # noqa: E501
 
 
         :return: The url of this AsyncAudioUrlParameters.  # noqa: E501
@@ -101,14 +111,37 @@
         :param entities: The entities of this AsyncAudioUrlParameters.  # noqa: E501
         :type: AsyncEntitiesPayload
         """
 
         self._entities = entities
 
     @property
+    def enable_all_trackers(self):
+        """Gets the enable_all_trackers of this AsyncAudioUrlParameters.  # noqa: E501
+
+        Messages Body for a Async Submit Text request.  # noqa: E501
+
+        :return: The enable_all_trackers of this AsyncAudioUrlParameters.  # noqa: E501
+        :rtype: AsyncEnableAllTrackers
+        """
+        return self._enable_all_trackers
+
+    @enable_all_trackers.setter
+    def enable_all_trackers(self, enable_all_trackers):
+        """Sets the enable_all_trackers of this AsyncAudioUrlParameters.
+
+        Messages Body for a Async Submit Text request.  # noqa: E501
+
+        :param enable_all_trackers: The enable_all_trackers of this AsyncAudioUrlParameters.  # noqa: E501
+        :type: AsyncEnableAllTrackers
+        """
+
+        self._enable_all_trackers = enable_all_trackers
+
+    @property
     def detect_phrases(self):
         """Gets the detect_phrases of this AsyncAudioUrlParameters.  # noqa: E501
 
 
         :return: The detect_phrases of this AsyncAudioUrlParameters.  # noqa: E501
         :rtype: AsyncDetectPhrases
         """
@@ -163,14 +196,35 @@
 
         :param name: The name of this AsyncAudioUrlParameters.  # noqa: E501
         :type: AsyncMeetingName
         """
 
         self._name = name
 
+    @property
+    def trackers(self):
+        """Gets the trackers of this AsyncAudioUrlParameters.  # noqa: E501
+
+
+        :return: The trackers of this AsyncAudioUrlParameters.  # noqa: E501
+        :rtype: AsyncTrackers
+        """
+        return self._trackers
+
+    @trackers.setter
+    def trackers(self, trackers):
+        """Sets the trackers of this AsyncAudioUrlParameters.
+
+
+        :param trackers: The trackers of this AsyncAudioUrlParameters.  # noqa: E501
+        :type: AsyncTrackers
+        """
+
+        self._trackers = trackers
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `symbl-rest-1.0.8/symbl_rest/models/async_confidence_threshold.py` & `symbl-rest-1.0.9/symbl_rest/models/async_confidence_threshold.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/async_detect_phrases.py` & `symbl-rest-1.0.9/symbl_rest/models/async_detect_phrases.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/async_entities_payload.py` & `symbl-rest-1.0.9/symbl_rest/models/async_entities_payload.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/async_meeting_name.py` & `symbl-rest-1.0.9/symbl_rest/models/async_meeting_name.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/async_messages_field.py` & `symbl-rest-1.0.9/symbl_rest/models/async_messages_field.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/async_messages_field_inner.py` & `symbl-rest-1.0.9/symbl_rest/models/async_messages_field_inner.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/async_response.py` & `symbl-rest-1.0.9/symbl_rest/models/async_response.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/async_text_parameters.py` & `symbl-rest-1.0.9/symbl_rest/models/async_video_url_parameters.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,176 +11,220 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class AsyncTextParameters(object):
+class AsyncVideoUrlParameters(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'messages': 'AsyncMessagesField',
+        'url': 'str',
         'entities': 'AsyncEntitiesPayload',
+        'enable_all_trackers': 'AsyncEnableAllTrackers',
         'detect_phrases': 'AsyncDetectPhrases',
         'confidence_threshold': 'AsyncConfidenceThreshold',
-        'name': 'AsyncMeetingName'
+        'name': 'AsyncMeetingName',
+        'trackers': 'AsyncTrackers'
     }
 
     attribute_map = {
-        'messages': 'messages',
+        'url': 'url',
         'entities': 'entities',
+        'enable_all_trackers': 'enableAllTrackers',
         'detect_phrases': 'detectPhrases',
         'confidence_threshold': 'confidenceThreshold',
-        'name': 'name'
+        'name': 'name',
+        'trackers': 'trackers'
     }
 
-    def __init__(self, messages=None, entities=None, detect_phrases=None, confidence_threshold=None, name=None):  # noqa: E501
-        """AsyncTextParameters - a model defined in Swagger"""  # noqa: E501
-        self._messages = None
+    def __init__(self, url=None, entities=None, enable_all_trackers=None, detect_phrases=None, confidence_threshold=None, name=None, trackers=None):  # noqa: E501
+        """AsyncVideoUrlParameters - a model defined in Swagger"""  # noqa: E501
+        self._url = None
         self._entities = None
+        self._enable_all_trackers = None
         self._detect_phrases = None
         self._confidence_threshold = None
         self._name = None
+        self._trackers = None
         self.discriminator = None
-        if messages is not None:
-            self.messages = messages
+        if url is not None:
+            self.url = url
         if entities is not None:
             self.entities = entities
+        if enable_all_trackers is not None:
+            self.enable_all_trackers = enable_all_trackers
         if detect_phrases is not None:
             self.detect_phrases = detect_phrases
         if confidence_threshold is not None:
             self.confidence_threshold = confidence_threshold
         if name is not None:
             self.name = name
+        if trackers is not None:
+            self.trackers = trackers
 
     @property
-    def messages(self):
-        """Gets the messages of this AsyncTextParameters.  # noqa: E501
+    def url(self):
+        """Gets the url of this AsyncVideoUrlParameters.  # noqa: E501
 
-        Messages Body for a Async Submit Text request.  # noqa: E501
 
-        :return: The messages of this AsyncTextParameters.  # noqa: E501
-        :rtype: AsyncMessagesField
+        :return: The url of this AsyncVideoUrlParameters.  # noqa: E501
+        :rtype: str
         """
-        return self._messages
+        return self._url
 
-    @messages.setter
-    def messages(self, messages):
-        """Sets the messages of this AsyncTextParameters.
+    @url.setter
+    def url(self, url):
+        """Sets the url of this AsyncVideoUrlParameters.
 
-        Messages Body for a Async Submit Text request.  # noqa: E501
 
-        :param messages: The messages of this AsyncTextParameters.  # noqa: E501
-        :type: AsyncMessagesField
+        :param url: The url of this AsyncVideoUrlParameters.  # noqa: E501
+        :type: str
         """
 
-        self._messages = messages
+        self._url = url
 
     @property
     def entities(self):
-        """Gets the entities of this AsyncTextParameters.  # noqa: E501
+        """Gets the entities of this AsyncVideoUrlParameters.  # noqa: E501
 
-        Messages Body for a Async Submit Text request.  # noqa: E501
 
-        :return: The entities of this AsyncTextParameters.  # noqa: E501
+        :return: The entities of this AsyncVideoUrlParameters.  # noqa: E501
         :rtype: AsyncEntitiesPayload
         """
         return self._entities
 
     @entities.setter
     def entities(self, entities):
-        """Sets the entities of this AsyncTextParameters.
+        """Sets the entities of this AsyncVideoUrlParameters.
 
-        Messages Body for a Async Submit Text request.  # noqa: E501
 
-        :param entities: The entities of this AsyncTextParameters.  # noqa: E501
+        :param entities: The entities of this AsyncVideoUrlParameters.  # noqa: E501
         :type: AsyncEntitiesPayload
         """
 
         self._entities = entities
 
     @property
-    def detect_phrases(self):
-        """Gets the detect_phrases of this AsyncTextParameters.  # noqa: E501
+    def enable_all_trackers(self):
+        """Gets the enable_all_trackers of this AsyncVideoUrlParameters.  # noqa: E501
+
+        Messages Body for a Async Submit Text request.  # noqa: E501
+
+        :return: The enable_all_trackers of this AsyncVideoUrlParameters.  # noqa: E501
+        :rtype: AsyncEnableAllTrackers
+        """
+        return self._enable_all_trackers
+
+    @enable_all_trackers.setter
+    def enable_all_trackers(self, enable_all_trackers):
+        """Sets the enable_all_trackers of this AsyncVideoUrlParameters.
 
         Messages Body for a Async Submit Text request.  # noqa: E501
 
-        :return: The detect_phrases of this AsyncTextParameters.  # noqa: E501
+        :param enable_all_trackers: The enable_all_trackers of this AsyncVideoUrlParameters.  # noqa: E501
+        :type: AsyncEnableAllTrackers
+        """
+
+        self._enable_all_trackers = enable_all_trackers
+
+    @property
+    def detect_phrases(self):
+        """Gets the detect_phrases of this AsyncVideoUrlParameters.  # noqa: E501
+
+
+        :return: The detect_phrases of this AsyncVideoUrlParameters.  # noqa: E501
         :rtype: AsyncDetectPhrases
         """
         return self._detect_phrases
 
     @detect_phrases.setter
     def detect_phrases(self, detect_phrases):
-        """Sets the detect_phrases of this AsyncTextParameters.
+        """Sets the detect_phrases of this AsyncVideoUrlParameters.
 
-        Messages Body for a Async Submit Text request.  # noqa: E501
 
-        :param detect_phrases: The detect_phrases of this AsyncTextParameters.  # noqa: E501
+        :param detect_phrases: The detect_phrases of this AsyncVideoUrlParameters.  # noqa: E501
         :type: AsyncDetectPhrases
         """
 
         self._detect_phrases = detect_phrases
 
     @property
     def confidence_threshold(self):
-        """Gets the confidence_threshold of this AsyncTextParameters.  # noqa: E501
+        """Gets the confidence_threshold of this AsyncVideoUrlParameters.  # noqa: E501
 
-        Confidence threshold to be passed to Async API. Needs to be above 0.5.  # noqa: E501
 
-        :return: The confidence_threshold of this AsyncTextParameters.  # noqa: E501
+        :return: The confidence_threshold of this AsyncVideoUrlParameters.  # noqa: E501
         :rtype: AsyncConfidenceThreshold
         """
         return self._confidence_threshold
 
     @confidence_threshold.setter
     def confidence_threshold(self, confidence_threshold):
-        """Sets the confidence_threshold of this AsyncTextParameters.
+        """Sets the confidence_threshold of this AsyncVideoUrlParameters.
 
-        Confidence threshold to be passed to Async API. Needs to be above 0.5.  # noqa: E501
 
-        :param confidence_threshold: The confidence_threshold of this AsyncTextParameters.  # noqa: E501
+        :param confidence_threshold: The confidence_threshold of this AsyncVideoUrlParameters.  # noqa: E501
         :type: AsyncConfidenceThreshold
         """
 
         self._confidence_threshold = confidence_threshold
 
     @property
     def name(self):
-        """Gets the name of this AsyncTextParameters.  # noqa: E501
+        """Gets the name of this AsyncVideoUrlParameters.  # noqa: E501
 
-        Name of the conversation to be saved in Async API.  # noqa: E501
 
-        :return: The name of this AsyncTextParameters.  # noqa: E501
+        :return: The name of this AsyncVideoUrlParameters.  # noqa: E501
         :rtype: AsyncMeetingName
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this AsyncTextParameters.
+        """Sets the name of this AsyncVideoUrlParameters.
 
-        Name of the conversation to be saved in Async API.  # noqa: E501
 
-        :param name: The name of this AsyncTextParameters.  # noqa: E501
+        :param name: The name of this AsyncVideoUrlParameters.  # noqa: E501
         :type: AsyncMeetingName
         """
 
         self._name = name
 
+    @property
+    def trackers(self):
+        """Gets the trackers of this AsyncVideoUrlParameters.  # noqa: E501
+
+
+        :return: The trackers of this AsyncVideoUrlParameters.  # noqa: E501
+        :rtype: AsyncTrackers
+        """
+        return self._trackers
+
+    @trackers.setter
+    def trackers(self, trackers):
+        """Sets the trackers of this AsyncVideoUrlParameters.
+
+
+        :param trackers: The trackers of this AsyncVideoUrlParameters.  # noqa: E501
+        :type: AsyncTrackers
+        """
+
+        self._trackers = trackers
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -194,15 +238,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(AsyncTextParameters, dict):
+        if issubclass(AsyncVideoUrlParameters, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -210,15 +254,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, AsyncTextParameters):
+        if not isinstance(other, AsyncVideoUrlParameters):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `symbl-rest-1.0.8/symbl_rest/models/async_video_url_parameters.py` & `symbl-rest-1.0.9/symbl_rest/models/audio_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,165 +11,147 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class AsyncVideoUrlParameters(object):
+class AudioConfig(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'url': 'str',
-        'entities': 'AsyncEntitiesPayload',
-        'detect_phrases': 'AsyncDetectPhrases',
-        'confidence_threshold': 'AsyncConfidenceThreshold',
-        'name': 'AsyncMeetingName'
+        'encoding': 'str',
+        'sample_rate': 'float',
+        'sample_size': 'float',
+        'payload_type': 'float'
     }
 
     attribute_map = {
-        'url': 'url',
-        'entities': 'entities',
-        'detect_phrases': 'detectPhrases',
-        'confidence_threshold': 'confidenceThreshold',
-        'name': 'name'
+        'encoding': 'encoding',
+        'sample_rate': 'sampleRate',
+        'sample_size': 'sampleSize',
+        'payload_type': 'payloadType'
     }
 
-    def __init__(self, url=None, entities=None, detect_phrases=None, confidence_threshold=None, name=None):  # noqa: E501
-        """AsyncVideoUrlParameters - a model defined in Swagger"""  # noqa: E501
-        self._url = None
-        self._entities = None
-        self._detect_phrases = None
-        self._confidence_threshold = None
-        self._name = None
+    def __init__(self, encoding=None, sample_rate=None, sample_size=None, payload_type=None):  # noqa: E501
+        """AudioConfig - a model defined in Swagger"""  # noqa: E501
+        self._encoding = None
+        self._sample_rate = None
+        self._sample_size = None
+        self._payload_type = None
         self.discriminator = None
-        if url is not None:
-            self.url = url
-        if entities is not None:
-            self.entities = entities
-        if detect_phrases is not None:
-            self.detect_phrases = detect_phrases
-        if confidence_threshold is not None:
-            self.confidence_threshold = confidence_threshold
-        if name is not None:
-            self.name = name
+        if encoding is not None:
+            self.encoding = encoding
+        if sample_rate is not None:
+            self.sample_rate = sample_rate
+        if sample_size is not None:
+            self.sample_size = sample_size
+        if payload_type is not None:
+            self.payload_type = payload_type
 
     @property
-    def url(self):
-        """Gets the url of this AsyncVideoUrlParameters.  # noqa: E501
+    def encoding(self):
+        """Gets the encoding of this AudioConfig.  # noqa: E501
 
+        The encoding scheme to be used  # noqa: E501
 
-        :return: The url of this AsyncVideoUrlParameters.  # noqa: E501
+        :return: The encoding of this AudioConfig.  # noqa: E501
         :rtype: str
         """
-        return self._url
+        return self._encoding
 
-    @url.setter
-    def url(self, url):
-        """Sets the url of this AsyncVideoUrlParameters.
+    @encoding.setter
+    def encoding(self, encoding):
+        """Sets the encoding of this AudioConfig.
 
+        The encoding scheme to be used  # noqa: E501
 
-        :param url: The url of this AsyncVideoUrlParameters.  # noqa: E501
+        :param encoding: The encoding of this AudioConfig.  # noqa: E501
         :type: str
         """
 
-        self._url = url
+        self._encoding = encoding
 
     @property
-    def entities(self):
-        """Gets the entities of this AsyncVideoUrlParameters.  # noqa: E501
+    def sample_rate(self):
+        """Gets the sample_rate of this AudioConfig.  # noqa: E501
 
+        Sampling rate for audio stream  # noqa: E501
 
-        :return: The entities of this AsyncVideoUrlParameters.  # noqa: E501
-        :rtype: AsyncEntitiesPayload
+        :return: The sample_rate of this AudioConfig.  # noqa: E501
+        :rtype: float
         """
-        return self._entities
+        return self._sample_rate
 
-    @entities.setter
-    def entities(self, entities):
-        """Sets the entities of this AsyncVideoUrlParameters.
+    @sample_rate.setter
+    def sample_rate(self, sample_rate):
+        """Sets the sample_rate of this AudioConfig.
 
+        Sampling rate for audio stream  # noqa: E501
 
-        :param entities: The entities of this AsyncVideoUrlParameters.  # noqa: E501
-        :type: AsyncEntitiesPayload
+        :param sample_rate: The sample_rate of this AudioConfig.  # noqa: E501
+        :type: float
         """
 
-        self._entities = entities
+        self._sample_rate = sample_rate
 
     @property
-    def detect_phrases(self):
-        """Gets the detect_phrases of this AsyncVideoUrlParameters.  # noqa: E501
+    def sample_size(self):
+        """Gets the sample_size of this AudioConfig.  # noqa: E501
 
+        Sample Size for the audio stream  # noqa: E501
 
-        :return: The detect_phrases of this AsyncVideoUrlParameters.  # noqa: E501
-        :rtype: AsyncDetectPhrases
+        :return: The sample_size of this AudioConfig.  # noqa: E501
+        :rtype: float
         """
-        return self._detect_phrases
+        return self._sample_size
 
-    @detect_phrases.setter
-    def detect_phrases(self, detect_phrases):
-        """Sets the detect_phrases of this AsyncVideoUrlParameters.
+    @sample_size.setter
+    def sample_size(self, sample_size):
+        """Sets the sample_size of this AudioConfig.
 
+        Sample Size for the audio stream  # noqa: E501
 
-        :param detect_phrases: The detect_phrases of this AsyncVideoUrlParameters.  # noqa: E501
-        :type: AsyncDetectPhrases
+        :param sample_size: The sample_size of this AudioConfig.  # noqa: E501
+        :type: float
         """
 
-        self._detect_phrases = detect_phrases
+        self._sample_size = sample_size
 
     @property
-    def confidence_threshold(self):
-        """Gets the confidence_threshold of this AsyncVideoUrlParameters.  # noqa: E501
+    def payload_type(self):
+        """Gets the payload_type of this AudioConfig.  # noqa: E501
 
+        Payload Type for the given codec  # noqa: E501
 
-        :return: The confidence_threshold of this AsyncVideoUrlParameters.  # noqa: E501
-        :rtype: AsyncConfidenceThreshold
+        :return: The payload_type of this AudioConfig.  # noqa: E501
+        :rtype: float
         """
-        return self._confidence_threshold
+        return self._payload_type
 
-    @confidence_threshold.setter
-    def confidence_threshold(self, confidence_threshold):
-        """Sets the confidence_threshold of this AsyncVideoUrlParameters.
+    @payload_type.setter
+    def payload_type(self, payload_type):
+        """Sets the payload_type of this AudioConfig.
 
+        Payload Type for the given codec  # noqa: E501
 
-        :param confidence_threshold: The confidence_threshold of this AsyncVideoUrlParameters.  # noqa: E501
-        :type: AsyncConfidenceThreshold
+        :param payload_type: The payload_type of this AudioConfig.  # noqa: E501
+        :type: float
         """
 
-        self._confidence_threshold = confidence_threshold
-
-    @property
-    def name(self):
-        """Gets the name of this AsyncVideoUrlParameters.  # noqa: E501
-
-
-        :return: The name of this AsyncVideoUrlParameters.  # noqa: E501
-        :rtype: AsyncMeetingName
-        """
-        return self._name
-
-    @name.setter
-    def name(self, name):
-        """Sets the name of this AsyncVideoUrlParameters.
-
-
-        :param name: The name of this AsyncVideoUrlParameters.  # noqa: E501
-        :type: AsyncMeetingName
-        """
-
-        self._name = name
+        self._payload_type = payload_type
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -184,15 +166,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(AsyncVideoUrlParameters, dict):
+        if issubclass(AudioConfig, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -200,15 +182,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, AsyncVideoUrlParameters):
+        if not isinstance(other, AudioConfig):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `symbl-rest-1.0.8/symbl_rest/models/audio_config.py` & `symbl-rest-1.0.9/symbl_rest/models/session_user.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,147 +11,127 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class AudioConfig(object):
+class SessionUser(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'encoding': 'str',
-        'sample_rate': 'float',
-        'sample_size': 'float',
-        'payload_type': 'float'
+        'user': 'UserTrunc',
+        'status': 'str',
+        'mode': 'str'
     }
 
     attribute_map = {
-        'encoding': 'encoding',
-        'sample_rate': 'sampleRate',
-        'sample_size': 'sampleSize',
-        'payload_type': 'payloadType'
+        'user': 'user',
+        'status': 'status',
+        'mode': 'mode'
     }
 
-    def __init__(self, encoding=None, sample_rate=None, sample_size=None, payload_type=None):  # noqa: E501
-        """AudioConfig - a model defined in Swagger"""  # noqa: E501
-        self._encoding = None
-        self._sample_rate = None
-        self._sample_size = None
-        self._payload_type = None
+    def __init__(self, user=None, status=None, mode=None):  # noqa: E501
+        """SessionUser - a model defined in Swagger"""  # noqa: E501
+        self._user = None
+        self._status = None
+        self._mode = None
         self.discriminator = None
-        if encoding is not None:
-            self.encoding = encoding
-        if sample_rate is not None:
-            self.sample_rate = sample_rate
-        if sample_size is not None:
-            self.sample_size = sample_size
-        if payload_type is not None:
-            self.payload_type = payload_type
+        if user is not None:
+            self.user = user
+        if status is not None:
+            self.status = status
+        if mode is not None:
+            self.mode = mode
 
     @property
-    def encoding(self):
-        """Gets the encoding of this AudioConfig.  # noqa: E501
+    def user(self):
+        """Gets the user of this SessionUser.  # noqa: E501
 
-        The encoding scheme to be used  # noqa: E501
 
-        :return: The encoding of this AudioConfig.  # noqa: E501
-        :rtype: str
-        """
-        return self._encoding
-
-    @encoding.setter
-    def encoding(self, encoding):
-        """Sets the encoding of this AudioConfig.
-
-        The encoding scheme to be used  # noqa: E501
-
-        :param encoding: The encoding of this AudioConfig.  # noqa: E501
-        :type: str
-        """
-
-        self._encoding = encoding
-
-    @property
-    def sample_rate(self):
-        """Gets the sample_rate of this AudioConfig.  # noqa: E501
-
-        Sampling rate for audio stream  # noqa: E501
-
-        :return: The sample_rate of this AudioConfig.  # noqa: E501
-        :rtype: float
+        :return: The user of this SessionUser.  # noqa: E501
+        :rtype: UserTrunc
         """
-        return self._sample_rate
+        return self._user
 
-    @sample_rate.setter
-    def sample_rate(self, sample_rate):
-        """Sets the sample_rate of this AudioConfig.
+    @user.setter
+    def user(self, user):
+        """Sets the user of this SessionUser.
 
-        Sampling rate for audio stream  # noqa: E501
 
-        :param sample_rate: The sample_rate of this AudioConfig.  # noqa: E501
-        :type: float
+        :param user: The user of this SessionUser.  # noqa: E501
+        :type: UserTrunc
         """
 
-        self._sample_rate = sample_rate
+        self._user = user
 
     @property
-    def sample_size(self):
-        """Gets the sample_size of this AudioConfig.  # noqa: E501
+    def status(self):
+        """Gets the status of this SessionUser.  # noqa: E501
 
-        Sample Size for the audio stream  # noqa: E501
 
-        :return: The sample_size of this AudioConfig.  # noqa: E501
-        :rtype: float
+        :return: The status of this SessionUser.  # noqa: E501
+        :rtype: str
         """
-        return self._sample_size
+        return self._status
 
-    @sample_size.setter
-    def sample_size(self, sample_size):
-        """Sets the sample_size of this AudioConfig.
+    @status.setter
+    def status(self, status):
+        """Sets the status of this SessionUser.
 
-        Sample Size for the audio stream  # noqa: E501
 
-        :param sample_size: The sample_size of this AudioConfig.  # noqa: E501
-        :type: float
+        :param status: The status of this SessionUser.  # noqa: E501
+        :type: str
         """
+        allowed_values = ["joined", "not_joined", "left"]  # noqa: E501
+        if status not in allowed_values:
+            raise ValueError(
+                "Invalid value for `status` ({0}), must be one of {1}"  # noqa: E501
+                .format(status, allowed_values)
+            )
 
-        self._sample_size = sample_size
+        self._status = status
 
     @property
-    def payload_type(self):
-        """Gets the payload_type of this AudioConfig.  # noqa: E501
+    def mode(self):
+        """Gets the mode of this SessionUser.  # noqa: E501
 
-        Payload Type for the given codec  # noqa: E501
+        The mode of user's joining the session  # noqa: E501
 
-        :return: The payload_type of this AudioConfig.  # noqa: E501
-        :rtype: float
+        :return: The mode of this SessionUser.  # noqa: E501
+        :rtype: str
         """
-        return self._payload_type
+        return self._mode
 
-    @payload_type.setter
-    def payload_type(self, payload_type):
-        """Sets the payload_type of this AudioConfig.
+    @mode.setter
+    def mode(self, mode):
+        """Sets the mode of this SessionUser.
 
-        Payload Type for the given codec  # noqa: E501
+        The mode of user's joining the session  # noqa: E501
 
-        :param payload_type: The payload_type of this AudioConfig.  # noqa: E501
-        :type: float
+        :param mode: The mode of this SessionUser.  # noqa: E501
+        :type: str
         """
+        allowed_values = ["native", "external", "custom"]  # noqa: E501
+        if mode not in allowed_values:
+            raise ValueError(
+                "Invalid value for `mode` ({0}), must be one of {1}"  # noqa: E501
+                .format(mode, allowed_values)
+            )
 
-        self._payload_type = payload_type
+        self._mode = mode
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -166,15 +146,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(AudioConfig, dict):
+        if issubclass(SessionUser, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -182,15 +162,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, AudioConfig):
+        if not isinstance(other, SessionUser):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `symbl-rest-1.0.8/symbl_rest/models/avatar.py` & `symbl-rest-1.0.9/symbl_rest/models/avatar.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/conversation_action_item.py` & `symbl-rest-1.0.9/symbl_rest/models/conversation_action_item.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/conversation_data_list_response.py` & `symbl-rest-1.0.9/symbl_rest/models/conversation_data_list_response.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/conversation_follow_up.py` & `symbl-rest-1.0.9/symbl_rest/models/conversation_follow_up.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/conversation_insight_item.py` & `symbl-rest-1.0.9/symbl_rest/models/conversation_insight_item.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/conversation_intent.py` & `symbl-rest-1.0.9/symbl_rest/models/conversation_intent.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/conversation_message.py` & `symbl-rest-1.0.9/symbl_rest/models/conversation_message.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/conversation_question.py` & `symbl-rest-1.0.9/symbl_rest/models/conversation_question.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,50 +29,45 @@
     """
     swagger_types = {
         'id': 'str',
         'text': 'str',
         'type': 'str',
         'score': 'float',
         'message_ids': 'list[str]',
-        'entities': 'list[Tag]',
         '_from': 'FromPayload'
     }
 
     attribute_map = {
         'id': 'id',
         'text': 'text',
         'type': 'type',
         'score': 'score',
         'message_ids': 'messageIds',
-        'entities': 'entities',
         '_from': 'from'
     }
 
-    def __init__(self, id=None, text=None, type=None, score=None, message_ids=None, entities=None, _from=None):  # noqa: E501
+    def __init__(self, id=None, text=None, type=None, score=None, message_ids=None, _from=None):  # noqa: E501
         """ConversationQuestion - a model defined in Swagger"""  # noqa: E501
         self._id = None
         self._text = None
         self._type = None
         self._score = None
         self._message_ids = None
-        self._entities = None
         self.__from = None
         self.discriminator = None
         if id is not None:
             self.id = id
         if text is not None:
             self.text = text
         if type is not None:
             self.type = type
         if score is not None:
             self.score = score
         if message_ids is not None:
             self.message_ids = message_ids
-        if entities is not None:
-            self.entities = entities
         if _from is not None:
             self._from = _from
 
     @property
     def id(self):
         """Gets the id of this ConversationQuestion.  # noqa: E501
 
@@ -176,35 +171,14 @@
         :param message_ids: The message_ids of this ConversationQuestion.  # noqa: E501
         :type: list[str]
         """
 
         self._message_ids = message_ids
 
     @property
-    def entities(self):
-        """Gets the entities of this ConversationQuestion.  # noqa: E501
-
-
-        :return: The entities of this ConversationQuestion.  # noqa: E501
-        :rtype: list[Tag]
-        """
-        return self._entities
-
-    @entities.setter
-    def entities(self, entities):
-        """Sets the entities of this ConversationQuestion.
-
-
-        :param entities: The entities of this ConversationQuestion.  # noqa: E501
-        :type: list[Tag]
-        """
-
-        self._entities = entities
-
-    @property
     def _from(self):
         """Gets the _from of this ConversationQuestion.  # noqa: E501
 
 
         :return: The _from of this ConversationQuestion.  # noqa: E501
         :rtype: FromPayload
         """
```

### Comparing `symbl-rest-1.0.8/symbl_rest/models/conversation_topic.py` & `symbl-rest-1.0.9/symbl_rest/models/conversation_topic.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/custom_entities.py` & `symbl-rest-1.0.9/symbl_rest/models/session_trunc.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,165 +11,165 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class CustomEntities(object):
+class SessionTrunc(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'custom_type': 'str',
-        'text': 'str',
+        'id': 'str',
+        'name': 'str',
         'type': 'str',
-        'value': 'str',
-        'message_refs': 'list[CustomEntitiesMessageRefs]'
+        'users': 'list[SessionUser]',
+        'location': 'LocationTrunc'
     }
 
     attribute_map = {
-        'custom_type': 'customType',
-        'text': 'text',
+        'id': 'id',
+        'name': 'name',
         'type': 'type',
-        'value': 'value',
-        'message_refs': 'messageRefs'
+        'users': 'users',
+        'location': 'location'
     }
 
-    def __init__(self, custom_type=None, text=None, type=None, value=None, message_refs=None):  # noqa: E501
-        """CustomEntities - a model defined in Swagger"""  # noqa: E501
-        self._custom_type = None
-        self._text = None
+    def __init__(self, id=None, name=None, type=None, users=None, location=None):  # noqa: E501
+        """SessionTrunc - a model defined in Swagger"""  # noqa: E501
+        self._id = None
+        self._name = None
         self._type = None
-        self._value = None
-        self._message_refs = None
+        self._users = None
+        self._location = None
         self.discriminator = None
-        if custom_type is not None:
-            self.custom_type = custom_type
-        if text is not None:
-            self.text = text
+        if id is not None:
+            self.id = id
+        if name is not None:
+            self.name = name
         if type is not None:
             self.type = type
-        if value is not None:
-            self.value = value
-        if message_refs is not None:
-            self.message_refs = message_refs
+        if users is not None:
+            self.users = users
+        if location is not None:
+            self.location = location
 
     @property
-    def custom_type(self):
-        """Gets the custom_type of this CustomEntities.  # noqa: E501
+    def id(self):
+        """Gets the id of this SessionTrunc.  # noqa: E501
 
 
-        :return: The custom_type of this CustomEntities.  # noqa: E501
+        :return: The id of this SessionTrunc.  # noqa: E501
         :rtype: str
         """
-        return self._custom_type
+        return self._id
 
-    @custom_type.setter
-    def custom_type(self, custom_type):
-        """Sets the custom_type of this CustomEntities.
+    @id.setter
+    def id(self, id):
+        """Sets the id of this SessionTrunc.
 
 
-        :param custom_type: The custom_type of this CustomEntities.  # noqa: E501
+        :param id: The id of this SessionTrunc.  # noqa: E501
         :type: str
         """
 
-        self._custom_type = custom_type
+        self._id = id
 
     @property
-    def text(self):
-        """Gets the text of this CustomEntities.  # noqa: E501
+    def name(self):
+        """Gets the name of this SessionTrunc.  # noqa: E501
 
 
-        :return: The text of this CustomEntities.  # noqa: E501
+        :return: The name of this SessionTrunc.  # noqa: E501
         :rtype: str
         """
-        return self._text
+        return self._name
 
-    @text.setter
-    def text(self, text):
-        """Sets the text of this CustomEntities.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this SessionTrunc.
 
 
-        :param text: The text of this CustomEntities.  # noqa: E501
+        :param name: The name of this SessionTrunc.  # noqa: E501
         :type: str
         """
 
-        self._text = text
+        self._name = name
 
     @property
     def type(self):
-        """Gets the type of this CustomEntities.  # noqa: E501
+        """Gets the type of this SessionTrunc.  # noqa: E501
 
 
-        :return: The type of this CustomEntities.  # noqa: E501
+        :return: The type of this SessionTrunc.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
-        """Sets the type of this CustomEntities.
+        """Sets the type of this SessionTrunc.
 
 
-        :param type: The type of this CustomEntities.  # noqa: E501
+        :param type: The type of this SessionTrunc.  # noqa: E501
         :type: str
         """
 
         self._type = type
 
     @property
-    def value(self):
-        """Gets the value of this CustomEntities.  # noqa: E501
+    def users(self):
+        """Gets the users of this SessionTrunc.  # noqa: E501
 
 
-        :return: The value of this CustomEntities.  # noqa: E501
-        :rtype: str
+        :return: The users of this SessionTrunc.  # noqa: E501
+        :rtype: list[SessionUser]
         """
-        return self._value
+        return self._users
 
-    @value.setter
-    def value(self, value):
-        """Sets the value of this CustomEntities.
+    @users.setter
+    def users(self, users):
+        """Sets the users of this SessionTrunc.
 
 
-        :param value: The value of this CustomEntities.  # noqa: E501
-        :type: str
+        :param users: The users of this SessionTrunc.  # noqa: E501
+        :type: list[SessionUser]
         """
 
-        self._value = value
+        self._users = users
 
     @property
-    def message_refs(self):
-        """Gets the message_refs of this CustomEntities.  # noqa: E501
+    def location(self):
+        """Gets the location of this SessionTrunc.  # noqa: E501
 
 
-        :return: The message_refs of this CustomEntities.  # noqa: E501
-        :rtype: list[CustomEntitiesMessageRefs]
+        :return: The location of this SessionTrunc.  # noqa: E501
+        :rtype: LocationTrunc
         """
-        return self._message_refs
+        return self._location
 
-    @message_refs.setter
-    def message_refs(self, message_refs):
-        """Sets the message_refs of this CustomEntities.
+    @location.setter
+    def location(self, location):
+        """Sets the location of this SessionTrunc.
 
 
-        :param message_refs: The message_refs of this CustomEntities.  # noqa: E501
-        :type: list[CustomEntitiesMessageRefs]
+        :param location: The location of this SessionTrunc.  # noqa: E501
+        :type: LocationTrunc
         """
 
-        self._message_refs = message_refs
+        self._location = location
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -184,15 +184,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(CustomEntities, dict):
+        if issubclass(SessionTrunc, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -200,15 +200,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CustomEntities):
+        if not isinstance(other, SessionTrunc):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `symbl-rest-1.0.8/symbl_rest/models/custom_entities_message_refs.py` & `symbl-rest-1.0.9/symbl_rest/models/matches_items_message_refs.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,110 +11,110 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class CustomEntitiesMessageRefs(object):
+class MatchesItemsMessageRefs(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'id': 'str',
         'text': 'str',
-        'offset': 'float'
+        'offset': 'int'
     }
 
     attribute_map = {
         'id': 'id',
         'text': 'text',
         'offset': 'offset'
     }
 
     def __init__(self, id=None, text=None, offset=None):  # noqa: E501
-        """CustomEntitiesMessageRefs - a model defined in Swagger"""  # noqa: E501
+        """MatchesItemsMessageRefs - a model defined in Swagger"""  # noqa: E501
         self._id = None
         self._text = None
         self._offset = None
         self.discriminator = None
         if id is not None:
             self.id = id
         if text is not None:
             self.text = text
         if offset is not None:
             self.offset = offset
 
     @property
     def id(self):
-        """Gets the id of this CustomEntitiesMessageRefs.  # noqa: E501
+        """Gets the id of this MatchesItemsMessageRefs.  # noqa: E501
 
 
-        :return: The id of this CustomEntitiesMessageRefs.  # noqa: E501
+        :return: The id of this MatchesItemsMessageRefs.  # noqa: E501
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this CustomEntitiesMessageRefs.
+        """Sets the id of this MatchesItemsMessageRefs.
 
 
-        :param id: The id of this CustomEntitiesMessageRefs.  # noqa: E501
+        :param id: The id of this MatchesItemsMessageRefs.  # noqa: E501
         :type: str
         """
 
         self._id = id
 
     @property
     def text(self):
-        """Gets the text of this CustomEntitiesMessageRefs.  # noqa: E501
+        """Gets the text of this MatchesItemsMessageRefs.  # noqa: E501
 
 
-        :return: The text of this CustomEntitiesMessageRefs.  # noqa: E501
+        :return: The text of this MatchesItemsMessageRefs.  # noqa: E501
         :rtype: str
         """
         return self._text
 
     @text.setter
     def text(self, text):
-        """Sets the text of this CustomEntitiesMessageRefs.
+        """Sets the text of this MatchesItemsMessageRefs.
 
 
-        :param text: The text of this CustomEntitiesMessageRefs.  # noqa: E501
+        :param text: The text of this MatchesItemsMessageRefs.  # noqa: E501
         :type: str
         """
 
         self._text = text
 
     @property
     def offset(self):
-        """Gets the offset of this CustomEntitiesMessageRefs.  # noqa: E501
+        """Gets the offset of this MatchesItemsMessageRefs.  # noqa: E501
 
 
-        :return: The offset of this CustomEntitiesMessageRefs.  # noqa: E501
-        :rtype: float
+        :return: The offset of this MatchesItemsMessageRefs.  # noqa: E501
+        :rtype: int
         """
         return self._offset
 
     @offset.setter
     def offset(self, offset):
-        """Sets the offset of this CustomEntitiesMessageRefs.
+        """Sets the offset of this MatchesItemsMessageRefs.
 
 
-        :param offset: The offset of this CustomEntitiesMessageRefs.  # noqa: E501
-        :type: float
+        :param offset: The offset of this MatchesItemsMessageRefs.  # noqa: E501
+        :type: int
         """
 
         self._offset = offset
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
@@ -132,15 +132,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(CustomEntitiesMessageRefs, dict):
+        if issubclass(MatchesItemsMessageRefs, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -148,15 +148,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CustomEntitiesMessageRefs):
+        if not isinstance(other, MatchesItemsMessageRefs):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `symbl-rest-1.0.8/symbl_rest/models/duration_payload.py` & `symbl-rest-1.0.9/symbl_rest/models/duration_payload.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/endpoint.py` & `symbl-rest-1.0.9/symbl_rest/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/endpoint_connect_request.py` & `symbl-rest-1.0.9/symbl_rest/models/endpoint_connect_request.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/endpoint_connect_response.py` & `symbl-rest-1.0.9/symbl_rest/models/endpoint_connect_response.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/endpoint_request_data.py` & `symbl-rest-1.0.9/symbl_rest/models/endpoint_request_data.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/error.py` & `symbl-rest-1.0.9/symbl_rest/models/error.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/external_event.py` & `symbl-rest-1.0.9/symbl_rest/models/external_event.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/follow_up_list_response.py` & `symbl-rest-1.0.9/symbl_rest/models/follow_up_list_response.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/from_payload.py` & `symbl-rest-1.0.9/symbl_rest/models/from_payload.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/generic_error.py` & `symbl-rest-1.0.9/symbl_rest/models/generic_error.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/grant.py` & `symbl-rest-1.0.9/symbl_rest/models/grant.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/insights_list_response.py` & `symbl-rest-1.0.9/symbl_rest/models/insights_list_response.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/intent.py` & `symbl-rest-1.0.9/symbl_rest/models/intent.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/intent_list_response.py` & `symbl-rest-1.0.9/symbl_rest/models/intent_list_response.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/job_response.py` & `symbl-rest-1.0.9/symbl_rest/models/job_response.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/language.py` & `symbl-rest-1.0.9/symbl_rest/models/language.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/location_trunc.py` & `symbl-rest-1.0.9/symbl_rest/models/location_trunc.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/member_list_response.py` & `symbl-rest-1.0.9/symbl_rest/models/member_list_response.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/members_info.py` & `symbl-rest-1.0.9/symbl_rest/models/members_info.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/message_list_response.py` & `symbl-rest-1.0.9/symbl_rest/models/message_list_response.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/metric.py` & `symbl-rest-1.0.9/symbl_rest/models/metric.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/metric_entry.py` & `symbl-rest-1.0.9/symbl_rest/models/metric_entry.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/metric_entry_create.py` & `symbl-rest-1.0.9/symbl_rest/models/metric_entry_create.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/metric_entry_response.py` & `symbl-rest-1.0.9/symbl_rest/models/metric_entry_response.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/metric_label.py` & `symbl-rest-1.0.9/symbl_rest/models/metric_label.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/metric_response.py` & `symbl-rest-1.0.9/symbl_rest/models/metric_response.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/model_from.py` & `symbl-rest-1.0.9/symbl_rest/models/model_from.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/parent_ref.py` & `symbl-rest-1.0.9/symbl_rest/models/parent_ref.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/phrase.py` & `symbl-rest-1.0.9/symbl_rest/models/phrase.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/question_list_response.py` & `symbl-rest-1.0.9/symbl_rest/models/question_list_response.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/refresh_token_request.py` & `symbl-rest-1.0.9/symbl_rest/models/refresh_token_request.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/revoke_token_request.py` & `symbl-rest-1.0.9/symbl_rest/models/revoke_token_request.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/sentiment.py` & `symbl-rest-1.0.9/symbl_rest/models/sentiment.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/sentiment_polarity.py` & `symbl-rest-1.0.9/symbl_rest/models/sentiment_polarity.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/session_trunc.py` & `symbl-rest-1.0.9/symbl_rest/models/analytics_metrics_info.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,165 +11,113 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class SessionTrunc(object):
+class AnalyticsMetricsInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'id': 'str',
-        'name': 'str',
         'type': 'str',
-        'users': 'list[SessionUser]',
-        'location': 'LocationTrunc'
+        'percent': 'float',
+        'seconds': 'float'
     }
 
     attribute_map = {
-        'id': 'id',
-        'name': 'name',
         'type': 'type',
-        'users': 'users',
-        'location': 'location'
+        'percent': 'percent',
+        'seconds': 'seconds'
     }
 
-    def __init__(self, id=None, name=None, type=None, users=None, location=None):  # noqa: E501
-        """SessionTrunc - a model defined in Swagger"""  # noqa: E501
-        self._id = None
-        self._name = None
+    def __init__(self, type=None, percent=None, seconds=None):  # noqa: E501
+        """AnalyticsMetricsInfo - a model defined in Swagger"""  # noqa: E501
         self._type = None
-        self._users = None
-        self._location = None
+        self._percent = None
+        self._seconds = None
         self.discriminator = None
-        if id is not None:
-            self.id = id
-        if name is not None:
-            self.name = name
         if type is not None:
             self.type = type
-        if users is not None:
-            self.users = users
-        if location is not None:
-            self.location = location
-
-    @property
-    def id(self):
-        """Gets the id of this SessionTrunc.  # noqa: E501
-
-
-        :return: The id of this SessionTrunc.  # noqa: E501
-        :rtype: str
-        """
-        return self._id
-
-    @id.setter
-    def id(self, id):
-        """Sets the id of this SessionTrunc.
-
-
-        :param id: The id of this SessionTrunc.  # noqa: E501
-        :type: str
-        """
-
-        self._id = id
-
-    @property
-    def name(self):
-        """Gets the name of this SessionTrunc.  # noqa: E501
-
-
-        :return: The name of this SessionTrunc.  # noqa: E501
-        :rtype: str
-        """
-        return self._name
-
-    @name.setter
-    def name(self, name):
-        """Sets the name of this SessionTrunc.
-
-
-        :param name: The name of this SessionTrunc.  # noqa: E501
-        :type: str
-        """
-
-        self._name = name
+        if percent is not None:
+            self.percent = percent
+        if seconds is not None:
+            self.seconds = seconds
 
     @property
     def type(self):
-        """Gets the type of this SessionTrunc.  # noqa: E501
+        """Gets the type of this AnalyticsMetricsInfo.  # noqa: E501
 
 
-        :return: The type of this SessionTrunc.  # noqa: E501
+        :return: The type of this AnalyticsMetricsInfo.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
-        """Sets the type of this SessionTrunc.
+        """Sets the type of this AnalyticsMetricsInfo.
 
 
-        :param type: The type of this SessionTrunc.  # noqa: E501
+        :param type: The type of this AnalyticsMetricsInfo.  # noqa: E501
         :type: str
         """
 
         self._type = type
 
     @property
-    def users(self):
-        """Gets the users of this SessionTrunc.  # noqa: E501
+    def percent(self):
+        """Gets the percent of this AnalyticsMetricsInfo.  # noqa: E501
 
 
-        :return: The users of this SessionTrunc.  # noqa: E501
-        :rtype: list[SessionUser]
+        :return: The percent of this AnalyticsMetricsInfo.  # noqa: E501
+        :rtype: float
         """
-        return self._users
+        return self._percent
 
-    @users.setter
-    def users(self, users):
-        """Sets the users of this SessionTrunc.
+    @percent.setter
+    def percent(self, percent):
+        """Sets the percent of this AnalyticsMetricsInfo.
 
 
-        :param users: The users of this SessionTrunc.  # noqa: E501
-        :type: list[SessionUser]
+        :param percent: The percent of this AnalyticsMetricsInfo.  # noqa: E501
+        :type: float
         """
 
-        self._users = users
+        self._percent = percent
 
     @property
-    def location(self):
-        """Gets the location of this SessionTrunc.  # noqa: E501
+    def seconds(self):
+        """Gets the seconds of this AnalyticsMetricsInfo.  # noqa: E501
 
 
-        :return: The location of this SessionTrunc.  # noqa: E501
-        :rtype: LocationTrunc
+        :return: The seconds of this AnalyticsMetricsInfo.  # noqa: E501
+        :rtype: float
         """
-        return self._location
+        return self._seconds
 
-    @location.setter
-    def location(self, location):
-        """Sets the location of this SessionTrunc.
+    @seconds.setter
+    def seconds(self, seconds):
+        """Sets the seconds of this AnalyticsMetricsInfo.
 
 
-        :param location: The location of this SessionTrunc.  # noqa: E501
-        :type: LocationTrunc
+        :param seconds: The seconds of this AnalyticsMetricsInfo.  # noqa: E501
+        :type: float
         """
 
-        self._location = location
+        self._seconds = seconds
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -184,15 +132,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(SessionTrunc, dict):
+        if issubclass(AnalyticsMetricsInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -200,15 +148,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SessionTrunc):
+        if not isinstance(other, AnalyticsMetricsInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `symbl-rest-1.0.8/symbl_rest/models/session_user.py` & `symbl-rest-1.0.9/symbl_rest/models/custom_entities.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,127 +11,87 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class SessionUser(object):
+class CustomEntities(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'user': 'UserTrunc',
-        'status': 'str',
-        'mode': 'str'
+        'custom_type': 'str',
+        'text': 'str'
     }
 
     attribute_map = {
-        'user': 'user',
-        'status': 'status',
-        'mode': 'mode'
+        'custom_type': 'customType',
+        'text': 'text'
     }
 
-    def __init__(self, user=None, status=None, mode=None):  # noqa: E501
-        """SessionUser - a model defined in Swagger"""  # noqa: E501
-        self._user = None
-        self._status = None
-        self._mode = None
+    def __init__(self, custom_type=None, text=None):  # noqa: E501
+        """CustomEntities - a model defined in Swagger"""  # noqa: E501
+        self._custom_type = None
+        self._text = None
         self.discriminator = None
-        if user is not None:
-            self.user = user
-        if status is not None:
-            self.status = status
-        if mode is not None:
-            self.mode = mode
+        if custom_type is not None:
+            self.custom_type = custom_type
+        if text is not None:
+            self.text = text
 
     @property
-    def user(self):
-        """Gets the user of this SessionUser.  # noqa: E501
+    def custom_type(self):
+        """Gets the custom_type of this CustomEntities.  # noqa: E501
 
 
-        :return: The user of this SessionUser.  # noqa: E501
-        :rtype: UserTrunc
-        """
-        return self._user
-
-    @user.setter
-    def user(self, user):
-        """Sets the user of this SessionUser.
-
-
-        :param user: The user of this SessionUser.  # noqa: E501
-        :type: UserTrunc
-        """
-
-        self._user = user
-
-    @property
-    def status(self):
-        """Gets the status of this SessionUser.  # noqa: E501
-
-
-        :return: The status of this SessionUser.  # noqa: E501
+        :return: The custom_type of this CustomEntities.  # noqa: E501
         :rtype: str
         """
-        return self._status
+        return self._custom_type
 
-    @status.setter
-    def status(self, status):
-        """Sets the status of this SessionUser.
+    @custom_type.setter
+    def custom_type(self, custom_type):
+        """Sets the custom_type of this CustomEntities.
 
 
-        :param status: The status of this SessionUser.  # noqa: E501
+        :param custom_type: The custom_type of this CustomEntities.  # noqa: E501
         :type: str
         """
-        allowed_values = ["joined", "not_joined", "left"]  # noqa: E501
-        if status not in allowed_values:
-            raise ValueError(
-                "Invalid value for `status` ({0}), must be one of {1}"  # noqa: E501
-                .format(status, allowed_values)
-            )
 
-        self._status = status
+        self._custom_type = custom_type
 
     @property
-    def mode(self):
-        """Gets the mode of this SessionUser.  # noqa: E501
+    def text(self):
+        """Gets the text of this CustomEntities.  # noqa: E501
 
-        The mode of user's joining the session  # noqa: E501
 
-        :return: The mode of this SessionUser.  # noqa: E501
+        :return: The text of this CustomEntities.  # noqa: E501
         :rtype: str
         """
-        return self._mode
+        return self._text
 
-    @mode.setter
-    def mode(self, mode):
-        """Sets the mode of this SessionUser.
+    @text.setter
+    def text(self, text):
+        """Sets the text of this CustomEntities.
 
-        The mode of user's joining the session  # noqa: E501
 
-        :param mode: The mode of this SessionUser.  # noqa: E501
+        :param text: The text of this CustomEntities.  # noqa: E501
         :type: str
         """
-        allowed_values = ["native", "external", "custom"]  # noqa: E501
-        if mode not in allowed_values:
-            raise ValueError(
-                "Invalid value for `mode` ({0}), must be one of {1}"  # noqa: E501
-                .format(mode, allowed_values)
-            )
 
-        self._mode = mode
+        self._text = text
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -146,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(SessionUser, dict):
+        if issubclass(CustomEntities, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -162,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SessionUser):
+        if not isinstance(other, CustomEntities):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `symbl-rest-1.0.8/symbl_rest/models/summary_info.py` & `symbl-rest-1.0.9/symbl_rest/models/summary_info.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/tag.py` & `symbl-rest-1.0.9/symbl_rest/models/tag.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/text_payload.py` & `symbl-rest-1.0.9/symbl_rest/models/text_payload.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/time_zone.py` & `symbl-rest-1.0.9/symbl_rest/models/time_zone.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/token.py` & `symbl-rest-1.0.9/symbl_rest/models/token.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/topic_list_response.py` & `symbl-rest-1.0.9/symbl_rest/models/topic_list_response.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/unauthorized_error.py` & `symbl-rest-1.0.9/symbl_rest/models/unauthorized_error.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/user_trunc.py` & `symbl-rest-1.0.9/symbl_rest/models/user_trunc.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/models/word.py` & `symbl-rest-1.0.9/symbl_rest/models/word.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/symbl_rest/rest.py` & `symbl-rest-1.0.9/symbl_rest/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,24 +191,22 @@
                     request_body = body
                     r = self.pool_manager.request(
                         method, url,
                         body=request_body,
                         preload_content=_preload_content,
                         timeout=timeout,
                         headers=headers)
-
                 elif isinstance(body, bytes):
                     request_body = body
                     r = self.pool_manager.request(
                         method, url,
                         body=request_body,
                         preload_content=_preload_content,
                         timeout=timeout,
                         headers=headers)
-
                 else:
                     # Cannot generate the request from given parameters
                     msg = """Cannot prepare a request message for provided
                              arguments. Please check that your arguments match
                              declared content type."""
                     raise ApiException(status=0, reason=msg)
             # For `GET`, `HEAD`
```

### Comparing `symbl-rest-1.0.8/symbl_rest.egg-info/PKG-INFO` & `symbl-rest-1.0.9/symbl_rest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: symbl-rest
-Version: 1.0.8
+Version: 1.0.9
 Summary: symbl.ai APIs
 Home-page: UNKNOWN
 Author: UNKNOWN
 Author-email: info@symbl.ai
 License: UNKNOWN
 Description:     &lt;h1&gt;Symbl&#x27;s APIs for external consumers.&lt;/h1&gt; &lt;h2&gt;Language Insights API&lt;/h2&gt; Symbl&#x27;s Language Insights API provides an interface for applications to perform the analysis on the raw text and get insights from it. The API automatically detects sentence boundaries and punctuates the sentences, and also returns the updated messages in the response. Conversations are the most unstructured piece of information that we represent information in, and which most of the leads to lot of loss of information by not being able to capture them correctly.&lt;br/&gt; Language Insights API focuses on understanding such texts and generate the useful and important information from them. &lt;br/&gt; Currently the API supports detection of the Action Items in any type of unstructured text. In future the same API will also have support to detect \&quot;Information\&quot; and \&quot;Event\&quot;, where Information is any informational piece and Event is a reference to something that has happened in the past.&lt;br/&gt; &lt;h2&gt;Telephony Integration&lt;/h2&gt; Symbl can currently integrate with two types of telephony endpoints: 1. SIP trunks&lt;br/&gt; 2. PSTN endpoints&lt;br/&gt; Results are sent via HTTP WebHooks as and when they are available.&lt;br/&gt; &lt;h2&gt;Flow&lt;/h2&gt; 1. External Application invokes REST API to join a meeting/session, with the mode (SIP/PSTN) and joining details&lt;br/&gt; 2. Symbl joins the meeting via SIP or PSTN integration&lt;br/&gt; 3. Symbl continuously processes the audio stream received&lt;br/&gt; 4. Symbl calls WebHook whenever transcription results are available&lt;br/&gt;  # noqa: E501
```

### Comparing `symbl-rest-1.0.8/symbl_rest.egg-info/SOURCES.txt` & `symbl-rest-1.0.9/symbl_rest.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -7,72 +7,89 @@
 symbl_rest.egg-info/PKG-INFO
 symbl_rest.egg-info/SOURCES.txt
 symbl_rest.egg-info/dependency_links.txt
 symbl_rest.egg-info/requires.txt
 symbl_rest.egg-info/top_level.txt
 symbl_rest/api/__init__.py
 symbl_rest/api/action_items_api.py
+symbl_rest/api/analytics_api.py
 symbl_rest/api/async_api.py
 symbl_rest/api/authentication_api.py
 symbl_rest/api/connection_to_endpoint_api.py
 symbl_rest/api/conversation_data_api.py
 symbl_rest/api/conversations_api.py
+symbl_rest/api/entities_api.py
 symbl_rest/api/external_event_web_hook_api.py
 symbl_rest/api/follow_ups_api.py
 symbl_rest/api/insights_api.py
 symbl_rest/api/intents_api.py
 symbl_rest/api/jobs_api.py
 symbl_rest/api/members_api.py
 symbl_rest/api/messages_api.py
 symbl_rest/api/metric_api.py
 symbl_rest/api/metric_entry_api.py
 symbl_rest/api/questions_api.py
 symbl_rest/api/topics_api.py
+symbl_rest/api/trackers_api.py
 symbl_rest/models/__init__.py
 symbl_rest/models/action.py
 symbl_rest/models/action_item_list_response.py
+symbl_rest/models/analytics_list_response.py
+symbl_rest/models/analytics_members_info.py
+symbl_rest/models/analytics_members_info_overlap.py
+symbl_rest/models/analytics_members_info_overlap_overlapping_members.py
+symbl_rest/models/analytics_members_info_pace.py
+symbl_rest/models/analytics_members_info_talk_time.py
+symbl_rest/models/analytics_metrics_info.py
 symbl_rest/models/async_audio_url_parameters.py
 symbl_rest/models/async_confidence_threshold.py
 symbl_rest/models/async_detect_phrases.py
+symbl_rest/models/async_enable_all_trackers.py
 symbl_rest/models/async_entities_payload.py
 symbl_rest/models/async_meeting_name.py
 symbl_rest/models/async_messages_field.py
 symbl_rest/models/async_messages_field_inner.py
 symbl_rest/models/async_response.py
 symbl_rest/models/async_text_parameters.py
+symbl_rest/models/async_trackers.py
+symbl_rest/models/async_trackers_inner.py
 symbl_rest/models/async_video_url_parameters.py
 symbl_rest/models/audio_config.py
 symbl_rest/models/avatar.py
 symbl_rest/models/conversation_action_item.py
 symbl_rest/models/conversation_data_list_response.py
 symbl_rest/models/conversation_follow_up.py
 symbl_rest/models/conversation_insight_item.py
 symbl_rest/models/conversation_intent.py
 symbl_rest/models/conversation_message.py
 symbl_rest/models/conversation_question.py
 symbl_rest/models/conversation_topic.py
 symbl_rest/models/custom_entities.py
-symbl_rest/models/custom_entities_message_refs.py
 symbl_rest/models/duration_payload.py
 symbl_rest/models/endpoint.py
 symbl_rest/models/endpoint_connect_request.py
 symbl_rest/models/endpoint_connect_response.py
 symbl_rest/models/endpoint_request_data.py
+symbl_rest/models/entities_list_response.py
+symbl_rest/models/entities_tag.py
 symbl_rest/models/error.py
 symbl_rest/models/external_event.py
 symbl_rest/models/follow_up_list_response.py
 symbl_rest/models/from_payload.py
 symbl_rest/models/generic_error.py
 symbl_rest/models/grant.py
 symbl_rest/models/insights_list_response.py
 symbl_rest/models/intent.py
 symbl_rest/models/intent_list_response.py
 symbl_rest/models/job_response.py
 symbl_rest/models/language.py
 symbl_rest/models/location_trunc.py
+symbl_rest/models/matches_items.py
+symbl_rest/models/matches_items_insight_refs.py
+symbl_rest/models/matches_items_message_refs.py
 symbl_rest/models/member_list_response.py
 symbl_rest/models/members_info.py
 symbl_rest/models/message_list_response.py
 symbl_rest/models/metric.py
 symbl_rest/models/metric_entry.py
 symbl_rest/models/metric_entry_create.py
 symbl_rest/models/metric_entry_response.py
@@ -90,31 +107,43 @@
 symbl_rest/models/session_user.py
 symbl_rest/models/summary_info.py
 symbl_rest/models/tag.py
 symbl_rest/models/text_payload.py
 symbl_rest/models/time_zone.py
 symbl_rest/models/token.py
 symbl_rest/models/topic_list_response.py
+symbl_rest/models/trackers_list_response.py
 symbl_rest/models/unauthorized_error.py
 symbl_rest/models/user_trunc.py
 symbl_rest/models/word.py
 test/__init__.py
 test/test_action.py
 test/test_action_item_list_response.py
 test/test_action_items_api.py
+test/test_analytics_api.py
+test/test_analytics_list_response.py
+test/test_analytics_members_info.py
+test/test_analytics_members_info_overlap.py
+test/test_analytics_members_info_overlap_overlapping_members.py
+test/test_analytics_members_info_pace.py
+test/test_analytics_members_info_talk_time.py
+test/test_analytics_metrics_info.py
 test/test_async_api.py
 test/test_async_audio_url_parameters.py
 test/test_async_confidence_threshold.py
 test/test_async_detect_phrases.py
+test/test_async_enable_all_trackers.py
 test/test_async_entities_payload.py
 test/test_async_meeting_name.py
 test/test_async_messages_field.py
 test/test_async_messages_field_inner.py
 test/test_async_response.py
 test/test_async_text_parameters.py
+test/test_async_trackers.py
+test/test_async_trackers_inner.py
 test/test_async_video_url_parameters.py
 test/test_audio_config.py
 test/test_authentication_api.py
 test/test_avatar.py
 test/test_connection_to_endpoint_api.py
 test/test_conversation_action_item.py
 test/test_conversation_data_api.py
@@ -123,20 +152,22 @@
 test/test_conversation_insight_item.py
 test/test_conversation_intent.py
 test/test_conversation_message.py
 test/test_conversation_question.py
 test/test_conversation_topic.py
 test/test_conversations_api.py
 test/test_custom_entities.py
-test/test_custom_entities_message_refs.py
 test/test_duration_payload.py
 test/test_endpoint.py
 test/test_endpoint_connect_request.py
 test/test_endpoint_connect_response.py
 test/test_endpoint_request_data.py
+test/test_entities_api.py
+test/test_entities_list_response.py
+test/test_entities_tag.py
 test/test_error.py
 test/test_external_event.py
 test/test_external_event_web_hook_api.py
 test/test_follow_up_list_response.py
 test/test_follow_ups_api.py
 test/test_from_payload.py
 test/test_generic_error.py
@@ -146,14 +177,17 @@
 test/test_intent.py
 test/test_intent_list_response.py
 test/test_intents_api.py
 test/test_job_response.py
 test/test_jobs_api.py
 test/test_language.py
 test/test_location_trunc.py
+test/test_matches_items.py
+test/test_matches_items_insight_refs.py
+test/test_matches_items_message_refs.py
 test/test_member_list_response.py
 test/test_members_api.py
 test/test_members_info.py
 test/test_message_list_response.py
 test/test_messages_api.py
 test/test_metric.py
 test/test_metric_api.py
@@ -177,10 +211,12 @@
 test/test_summary_info.py
 test/test_tag.py
 test/test_text_payload.py
 test/test_time_zone.py
 test/test_token.py
 test/test_topic_list_response.py
 test/test_topics_api.py
+test/test_trackers_api.py
+test/test_trackers_list_response.py
 test/test_unauthorized_error.py
 test/test_user_trunc.py
 test/test_word.py
```

### Comparing `symbl-rest-1.0.8/test/test_action.py` & `symbl-rest-1.0.9/test/test_action.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_action_item_list_response.py` & `symbl-rest-1.0.9/test/test_action_item_list_response.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_action_items_api.py` & `symbl-rest-1.0.9/test/test_action_items_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_async_api.py` & `symbl-rest-1.0.9/test/test_async_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_async_audio_url_parameters.py` & `symbl-rest-1.0.9/test/test_async_audio_url_parameters.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_async_confidence_threshold.py` & `symbl-rest-1.0.9/test/test_async_confidence_threshold.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_async_detect_phrases.py` & `symbl-rest-1.0.9/test/test_async_detect_phrases.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_async_entities_payload.py` & `symbl-rest-1.0.9/test/test_async_entities_payload.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_async_meeting_name.py` & `symbl-rest-1.0.9/test/test_async_meeting_name.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_async_messages_field.py` & `symbl-rest-1.0.9/test/test_async_messages_field.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_async_messages_field_inner.py` & `symbl-rest-1.0.9/test/test_async_messages_field_inner.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_async_response.py` & `symbl-rest-1.0.9/test/test_async_response.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_async_text_parameters.py` & `symbl-rest-1.0.9/test/test_async_text_parameters.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_async_video_url_parameters.py` & `symbl-rest-1.0.9/test/test_async_video_url_parameters.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_audio_config.py` & `symbl-rest-1.0.9/test/test_audio_config.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_authentication_api.py` & `symbl-rest-1.0.9/test/test_authentication_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_avatar.py` & `symbl-rest-1.0.9/test/test_avatar.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_connection_to_endpoint_api.py` & `symbl-rest-1.0.9/test/test_connection_to_endpoint_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_conversation_action_item.py` & `symbl-rest-1.0.9/test/test_conversation_action_item.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_conversation_data_api.py` & `symbl-rest-1.0.9/test/test_conversation_data_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 
     def setUp(self):
         self.api = ConversationDataApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_get_conversation_data_by_conversation_id(self):
-        """Test case for get_conversation_data_by_conversation_id
+    def test_get_conversation_by_conversation_id(self):
+        """Test case for get_conversation_by_conversation_id
 
         Retrieve Conversation data/meta-data from Conversations  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
```

### Comparing `symbl-rest-1.0.8/test/test_conversation_data_list_response.py` & `symbl-rest-1.0.9/test/test_conversation_data_list_response.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_conversation_follow_up.py` & `symbl-rest-1.0.9/test/test_conversation_follow_up.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_conversation_insight_item.py` & `symbl-rest-1.0.9/test/test_conversation_insight_item.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_conversation_intent.py` & `symbl-rest-1.0.9/test/test_conversation_intent.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_conversation_message.py` & `symbl-rest-1.0.9/test/test_conversation_message.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_conversation_question.py` & `symbl-rest-1.0.9/test/test_conversation_question.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_conversation_topic.py` & `symbl-rest-1.0.9/test/test_conversation_topic.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_conversations_api.py` & `symbl-rest-1.0.9/test/test_conversations_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,21 +31,35 @@
     def test_get_action_items_by_conversation_id(self):
         """Test case for get_action_items_by_conversation_id
 
         Retrieve action items from conversations  # noqa: E501
         """
         pass
 
-    def test_get_conversation_data_by_conversation_id(self):
-        """Test case for get_conversation_data_by_conversation_id
+    def test_get_analytics_by_conversation_id(self):
+        """Test case for get_analytics_by_conversation_id
+
+        Retrieves speaker ratio, talk time etc from Conversations  # noqa: E501
+        """
+        pass
+
+    def test_get_conversation_by_conversation_id(self):
+        """Test case for get_conversation_by_conversation_id
 
         Retrieve Conversation data/meta-data from Conversations  # noqa: E501
         """
         pass
 
+    def test_get_entities_by_conversation_id(self):
+        """Test case for get_entities_by_conversation_id
+
+        Extract Entities from Conversation  # noqa: E501
+        """
+        pass
+
     def test_get_follow_ups_by_conversation_id(self):
         """Test case for get_follow_ups_by_conversation_id
 
         Retrieve follow ups from conversations  # noqa: E501
         """
         pass
 
@@ -87,10 +101,17 @@
     def test_get_topics_by_conversation_id(self):
         """Test case for get_topics_by_conversation_id
 
         Retrieve topics from conversation  # noqa: E501
         """
         pass
 
+    def test_get_trackers_by_conversation_id(self):
+        """Test case for get_trackers_by_conversation_id
+
+        Track the Words and Phrases  # noqa: E501
+        """
+        pass
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `symbl-rest-1.0.8/test/test_custom_entities.py` & `symbl-rest-1.0.9/test/test_custom_entities.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_custom_entities_message_refs.py` & `symbl-rest-1.0.9/test/test_message_list_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import symbl_rest
-from symbl_rest.models.custom_entities_message_refs import CustomEntitiesMessageRefs  # noqa: E501
+from symbl_rest.models.message_list_response import MessageListResponse  # noqa: E501
 from symbl_rest.rest import ApiException
 
 
-class TestCustomEntitiesMessageRefs(unittest.TestCase):
-    """CustomEntitiesMessageRefs unit test stubs"""
+class TestMessageListResponse(unittest.TestCase):
+    """MessageListResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCustomEntitiesMessageRefs(self):
-        """Test CustomEntitiesMessageRefs"""
+    def testMessageListResponse(self):
+        """Test MessageListResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = symbl_rest.models.custom_entities_message_refs.CustomEntitiesMessageRefs()  # noqa: E501
+        # model = symbl_rest.models.message_list_response.MessageListResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `symbl-rest-1.0.8/test/test_duration_payload.py` & `symbl-rest-1.0.9/test/test_duration_payload.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_endpoint.py` & `symbl-rest-1.0.9/test/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_endpoint_connect_request.py` & `symbl-rest-1.0.9/test/test_endpoint_connect_request.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_endpoint_connect_response.py` & `symbl-rest-1.0.9/test/test_endpoint_connect_response.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_endpoint_request_data.py` & `symbl-rest-1.0.9/test/test_endpoint_request_data.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_error.py` & `symbl-rest-1.0.9/test/test_error.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_external_event.py` & `symbl-rest-1.0.9/test/test_external_event.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_external_event_web_hook_api.py` & `symbl-rest-1.0.9/test/test_external_event_web_hook_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_follow_up_list_response.py` & `symbl-rest-1.0.9/test/test_follow_up_list_response.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_follow_ups_api.py` & `symbl-rest-1.0.9/test/test_follow_ups_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_from_payload.py` & `symbl-rest-1.0.9/test/test_from_payload.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_generic_error.py` & `symbl-rest-1.0.9/test/test_generic_error.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_grant.py` & `symbl-rest-1.0.9/test/test_grant.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_insights_api.py` & `symbl-rest-1.0.9/test/test_insights_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_insights_list_response.py` & `symbl-rest-1.0.9/test/test_insights_list_response.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_intent.py` & `symbl-rest-1.0.9/test/test_intent.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_intent_list_response.py` & `symbl-rest-1.0.9/test/test_intent_list_response.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_intents_api.py` & `symbl-rest-1.0.9/test/test_intents_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_job_response.py` & `symbl-rest-1.0.9/test/test_job_response.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_jobs_api.py` & `symbl-rest-1.0.9/test/test_jobs_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_language.py` & `symbl-rest-1.0.9/test/test_language.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_location_trunc.py` & `symbl-rest-1.0.9/test/test_location_trunc.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_member_list_response.py` & `symbl-rest-1.0.9/test/test_member_list_response.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_members_api.py` & `symbl-rest-1.0.9/test/test_members_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_members_info.py` & `symbl-rest-1.0.9/test/test_members_info.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_message_list_response.py` & `symbl-rest-1.0.9/test/test_metric_entry.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import symbl_rest
-from symbl_rest.models.message_list_response import MessageListResponse  # noqa: E501
+from symbl_rest.models.metric_entry import MetricEntry  # noqa: E501
 from symbl_rest.rest import ApiException
 
 
-class TestMessageListResponse(unittest.TestCase):
-    """MessageListResponse unit test stubs"""
+class TestMetricEntry(unittest.TestCase):
+    """MetricEntry unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMessageListResponse(self):
-        """Test MessageListResponse"""
+    def testMetricEntry(self):
+        """Test MetricEntry"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = symbl_rest.models.message_list_response.MessageListResponse()  # noqa: E501
+        # model = symbl_rest.models.metric_entry.MetricEntry()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `symbl-rest-1.0.8/test/test_messages_api.py` & `symbl-rest-1.0.9/test/test_messages_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_metric.py` & `symbl-rest-1.0.9/test/test_metric.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_metric_api.py` & `symbl-rest-1.0.9/test/test_metric_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_metric_entry.py` & `symbl-rest-1.0.9/test/test_metric_label.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import symbl_rest
-from symbl_rest.models.metric_entry import MetricEntry  # noqa: E501
+from symbl_rest.models.metric_label import MetricLabel  # noqa: E501
 from symbl_rest.rest import ApiException
 
 
-class TestMetricEntry(unittest.TestCase):
-    """MetricEntry unit test stubs"""
+class TestMetricLabel(unittest.TestCase):
+    """MetricLabel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMetricEntry(self):
-        """Test MetricEntry"""
+    def testMetricLabel(self):
+        """Test MetricLabel"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = symbl_rest.models.metric_entry.MetricEntry()  # noqa: E501
+        # model = symbl_rest.models.metric_label.MetricLabel()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `symbl-rest-1.0.8/test/test_metric_entry_api.py` & `symbl-rest-1.0.9/test/test_metric_entry_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_metric_entry_create.py` & `symbl-rest-1.0.9/test/test_metric_entry_create.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_metric_entry_response.py` & `symbl-rest-1.0.9/test/test_metric_entry_response.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_metric_label.py` & `symbl-rest-1.0.9/test/test_metric_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import symbl_rest
-from symbl_rest.models.metric_label import MetricLabel  # noqa: E501
+from symbl_rest.models.metric_response import MetricResponse  # noqa: E501
 from symbl_rest.rest import ApiException
 
 
-class TestMetricLabel(unittest.TestCase):
-    """MetricLabel unit test stubs"""
+class TestMetricResponse(unittest.TestCase):
+    """MetricResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMetricLabel(self):
-        """Test MetricLabel"""
+    def testMetricResponse(self):
+        """Test MetricResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = symbl_rest.models.metric_label.MetricLabel()  # noqa: E501
+        # model = symbl_rest.models.metric_response.MetricResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `symbl-rest-1.0.8/test/test_metric_response.py` & `symbl-rest-1.0.9/test/test_user_trunc.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import symbl_rest
-from symbl_rest.models.metric_response import MetricResponse  # noqa: E501
+from symbl_rest.models.user_trunc import UserTrunc  # noqa: E501
 from symbl_rest.rest import ApiException
 
 
-class TestMetricResponse(unittest.TestCase):
-    """MetricResponse unit test stubs"""
+class TestUserTrunc(unittest.TestCase):
+    """UserTrunc unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMetricResponse(self):
-        """Test MetricResponse"""
+    def testUserTrunc(self):
+        """Test UserTrunc"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = symbl_rest.models.metric_response.MetricResponse()  # noqa: E501
+        # model = symbl_rest.models.user_trunc.UserTrunc()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `symbl-rest-1.0.8/test/test_model_from.py` & `symbl-rest-1.0.9/test/test_model_from.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_parent_ref.py` & `symbl-rest-1.0.9/test/test_parent_ref.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_phrase.py` & `symbl-rest-1.0.9/test/test_phrase.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_question_list_response.py` & `symbl-rest-1.0.9/test/test_question_list_response.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_questions_api.py` & `symbl-rest-1.0.9/test/test_questions_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_refresh_token_request.py` & `symbl-rest-1.0.9/test/test_refresh_token_request.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_revoke_token_request.py` & `symbl-rest-1.0.9/test/test_revoke_token_request.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_sentiment.py` & `symbl-rest-1.0.9/test/test_sentiment.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_sentiment_polarity.py` & `symbl-rest-1.0.9/test/test_sentiment_polarity.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_session_trunc.py` & `symbl-rest-1.0.9/test/test_session_trunc.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_session_user.py` & `symbl-rest-1.0.9/test/test_session_user.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_summary_info.py` & `symbl-rest-1.0.9/test/test_summary_info.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_tag.py` & `symbl-rest-1.0.9/test/test_tag.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_text_payload.py` & `symbl-rest-1.0.9/test/test_text_payload.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_time_zone.py` & `symbl-rest-1.0.9/test/test_time_zone.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_token.py` & `symbl-rest-1.0.9/test/test_token.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_topic_list_response.py` & `symbl-rest-1.0.9/test/test_topic_list_response.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_topics_api.py` & `symbl-rest-1.0.9/test/test_topics_api.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_unauthorized_error.py` & `symbl-rest-1.0.9/test/test_unauthorized_error.py`

 * *Files identical despite different names*

### Comparing `symbl-rest-1.0.8/test/test_user_trunc.py` & `symbl-rest-1.0.9/test/test_analytics_members_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import symbl_rest
-from symbl_rest.models.user_trunc import UserTrunc  # noqa: E501
+from symbl_rest.models.analytics_members_info import AnalyticsMembersInfo  # noqa: E501
 from symbl_rest.rest import ApiException
 
 
-class TestUserTrunc(unittest.TestCase):
-    """UserTrunc unit test stubs"""
+class TestAnalyticsMembersInfo(unittest.TestCase):
+    """AnalyticsMembersInfo unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUserTrunc(self):
-        """Test UserTrunc"""
+    def testAnalyticsMembersInfo(self):
+        """Test AnalyticsMembersInfo"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = symbl_rest.models.user_trunc.UserTrunc()  # noqa: E501
+        # model = symbl_rest.models.analytics_members_info.AnalyticsMembersInfo()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `symbl-rest-1.0.8/test/test_word.py` & `symbl-rest-1.0.9/test/test_word.py`

 * *Files identical despite different names*

