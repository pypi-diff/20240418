# Comparing `tmp/google-apps-chat-0.1.3.tar.gz` & `tmp/google-apps-chat-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-apps-chat-0.1.3.tar", last modified: Tue Apr 16 14:29:21 2024, max compression
+gzip compressed data, was "google-apps-chat-0.1.4.tar", last modified: Thu Apr 18 14:31:31 2024, max compression
```

## Comparing `google-apps-chat-0.1.3.tar` & `google-apps-chat-0.1.4.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 14:29:21.472355 google-apps-chat-0.1.3/
--rw-rw-r--   0 root         (0)     1003    11358 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4941 2024-04-16 14:29:21.472355 google-apps-chat-0.1.3/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3540 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 14:29:21.456357 google-apps-chat-0.1.3/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 14:29:21.456357 google-apps-chat-0.1.3/google/apps/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 14:29:21.456357 google-apps-chat-0.1.3/google/apps/chat/
--rw-rw-r--   0 root         (0)     1003     4509 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       77 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 14:29:21.460357 google-apps-chat-0.1.3/google/apps/chat_v1/
--rw-rw-r--   0 root         (0)     1003     4107 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     8704 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       77 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 14:29:21.460357 google-apps-chat-0.1.3/google/apps/chat_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 14:29:21.460357 google-apps-chat-0.1.3/google/apps/chat_v1/services/chat_service/
--rw-rw-r--   0 root         (0)     1003      757 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/services/chat_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   128729 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/services/chat_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   143945 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/services/chat_service/client.py
--rw-rw-r--   0 root         (0)     1003    20313 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/services/chat_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 14:29:21.464356 google-apps-chat-0.1.3/google/apps/chat_v1/services/chat_service/transports/
--rw-rw-r--   0 root         (0)     1003     1358 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/services/chat_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    23907 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/services/chat_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    49004 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/services/chat_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    49817 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/services/chat_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   113110 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/services/chat_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 14:29:21.468356 google-apps-chat-0.1.3/google/apps/chat_v1/types/
--rw-rw-r--   0 root         (0)     1003     3769 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     1612 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/types/action_status.py
--rw-rw-r--   0 root         (0)     1003     8722 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/types/annotation.py
--rw-rw-r--   0 root         (0)     1003     6485 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/types/attachment.py
--rw-rw-r--   0 root         (0)     1003      757 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/types/chat_service.py
--rw-rw-r--   0 root         (0)     1003     6693 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/types/contextual_addon.py
--rw-rw-r--   0 root         (0)     1003     2297 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/types/deletion_metadata.py
--rw-rw-r--   0 root         (0)     1003     1295 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/types/group.py
--rw-rw-r--   0 root         (0)     1003     1591 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/types/history_state.py
--rw-rw-r--   0 root         (0)     1003     1266 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/types/matched_url.py
--rw-rw-r--   0 root         (0)     1003    15211 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/types/membership.py
--rw-rw-r--   0 root         (0)     1003    37994 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/types/message.py
--rw-rw-r--   0 root         (0)     1003     8900 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/types/reaction.py
--rw-rw-r--   0 root         (0)     1003     1206 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/types/slash_command.py
--rw-rw-r--   0 root         (0)     1003    19623 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/types/space.py
--rw-rw-r--   0 root         (0)     1003     4710 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/types/space_setup.py
--rw-rw-r--   0 root         (0)     1003     3682 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/types/user.py
--rw-rw-r--   0 root         (0)     1003    18296 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/google/apps/chat_v1/types/widgets.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 14:29:21.468356 google-apps-chat-0.1.3/google_apps_chat.egg-info/
--rw-r--r--   0 root         (0)     1003     4941 2024-04-16 14:29:21.000000 google-apps-chat-0.1.3/google_apps_chat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1951 2024-04-16 14:29:21.000000 google-apps-chat-0.1.3/google_apps_chat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-16 14:29:21.000000 google-apps-chat-0.1.3/google_apps_chat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-16 14:29:21.000000 google-apps-chat-0.1.3/google_apps_chat.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      339 2024-04-16 14:29:21.000000 google-apps-chat-0.1.3/google_apps_chat.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-04-16 14:29:21.000000 google-apps-chat-0.1.3/google_apps_chat.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-04-16 14:29:21.472355 google-apps-chat-0.1.3/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3191 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 14:29:21.468356 google-apps-chat-0.1.3/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 14:29:21.468356 google-apps-chat-0.1.3/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 14:29:21.468356 google-apps-chat-0.1.3/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 14:29:21.468356 google-apps-chat-0.1.3/tests/unit/gapic/chat_v1/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/tests/unit/gapic/chat_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   596811 2024-04-16 14:26:06.000000 google-apps-chat-0.1.3/tests/unit/gapic/chat_v1/test_chat_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:31.732341 google-apps-chat-0.1.4/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4941 2024-04-18 14:31:31.732341 google-apps-chat-0.1.4/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3540 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:31.716340 google-apps-chat-0.1.4/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:31.716340 google-apps-chat-0.1.4/google/apps/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:31.720340 google-apps-chat-0.1.4/google/apps/chat/
+-rw-rw-r--   0 root         (0)     1003     4569 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       77 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:31.720340 google-apps-chat-0.1.4/google/apps/chat_v1/
+-rw-rw-r--   0 root         (0)     1003     4167 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9088 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       77 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:31.720340 google-apps-chat-0.1.4/google/apps/chat_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:31.720340 google-apps-chat-0.1.4/google/apps/chat_v1/services/chat_service/
+-rw-rw-r--   0 root         (0)     1003      757 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/services/chat_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   134045 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/services/chat_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   149106 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/services/chat_service/client.py
+-rw-rw-r--   0 root         (0)     1003    20313 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/services/chat_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:31.724341 google-apps-chat-0.1.4/google/apps/chat_v1/services/chat_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1358 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/services/chat_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24693 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/services/chat_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    50203 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/services/chat_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    51052 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/services/chat_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   118482 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/services/chat_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:31.728341 google-apps-chat-0.1.4/google/apps/chat_v1/types/
+-rw-rw-r--   0 root         (0)     1003     3829 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1612 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/types/action_status.py
+-rw-rw-r--   0 root         (0)     1003     8722 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/types/annotation.py
+-rw-rw-r--   0 root         (0)     1003     6485 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/types/attachment.py
+-rw-rw-r--   0 root         (0)     1003      757 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/types/chat_service.py
+-rw-rw-r--   0 root         (0)     1003     6693 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/types/contextual_addon.py
+-rw-rw-r--   0 root         (0)     1003     2297 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/types/deletion_metadata.py
+-rw-rw-r--   0 root         (0)     1003     1295 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/types/group.py
+-rw-rw-r--   0 root         (0)     1003     1591 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/types/history_state.py
+-rw-rw-r--   0 root         (0)     1003     1266 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/types/matched_url.py
+-rw-rw-r--   0 root         (0)     1003    16046 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/types/membership.py
+-rw-rw-r--   0 root         (0)     1003    37994 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/types/message.py
+-rw-rw-r--   0 root         (0)     1003     8900 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/types/reaction.py
+-rw-rw-r--   0 root         (0)     1003     1206 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/types/slash_command.py
+-rw-rw-r--   0 root         (0)     1003    19623 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/types/space.py
+-rw-rw-r--   0 root         (0)     1003     4710 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/types/space_setup.py
+-rw-rw-r--   0 root         (0)     1003     3682 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/types/user.py
+-rw-rw-r--   0 root         (0)     1003    18296 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/google/apps/chat_v1/types/widgets.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:31.728341 google-apps-chat-0.1.4/google_apps_chat.egg-info/
+-rw-r--r--   0 root         (0)     1003     4941 2024-04-18 14:31:31.000000 google-apps-chat-0.1.4/google_apps_chat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1951 2024-04-18 14:31:31.000000 google-apps-chat-0.1.4/google_apps_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-18 14:31:31.000000 google-apps-chat-0.1.4/google_apps_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-18 14:31:31.000000 google-apps-chat-0.1.4/google_apps_chat.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      339 2024-04-18 14:31:31.000000 google-apps-chat-0.1.4/google_apps_chat.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-04-18 14:31:31.000000 google-apps-chat-0.1.4/google_apps_chat.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-04-18 14:31:31.732341 google-apps-chat-0.1.4/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3191 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:31.728341 google-apps-chat-0.1.4/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:31.728341 google-apps-chat-0.1.4/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:31.728341 google-apps-chat-0.1.4/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:31.732341 google-apps-chat-0.1.4/tests/unit/gapic/chat_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/tests/unit/gapic/chat_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   622617 2024-04-18 14:28:16.000000 google-apps-chat-0.1.4/tests/unit/gapic/chat_v1/test_chat_service.py
```

### Comparing `google-apps-chat-0.1.3/LICENSE` & `google-apps-chat-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/MANIFEST.in` & `google-apps-chat-0.1.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/PKG-INFO` & `google-apps-chat-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-apps-chat
-Version: 0.1.3
+Version: 0.1.4
 Summary: Google Apps Chat API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-apps-chat
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-apps-chat-0.1.3/README.rst` & `google-apps-chat-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/google/apps/chat/__init__.py` & `google-apps-chat-0.1.4/google/apps/chat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 from google.apps.chat_v1.types.membership import (
     CreateMembershipRequest,
     DeleteMembershipRequest,
     GetMembershipRequest,
     ListMembershipsRequest,
     ListMembershipsResponse,
     Membership,
+    UpdateMembershipRequest,
 )
 from google.apps.chat_v1.types.message import (
     AccessoryWidget,
     ActionResponse,
     AttachedGif,
     CardWithId,
     CreateMessageRequest,
@@ -119,14 +120,15 @@
     "MatchedUrl",
     "CreateMembershipRequest",
     "DeleteMembershipRequest",
     "GetMembershipRequest",
     "ListMembershipsRequest",
     "ListMembershipsResponse",
     "Membership",
+    "UpdateMembershipRequest",
     "AccessoryWidget",
     "ActionResponse",
     "AttachedGif",
     "CardWithId",
     "CreateMessageRequest",
     "DeleteMessageRequest",
     "Dialog",
```

### Comparing `google-apps-chat-0.1.3/google/apps/chat/gapic_version.py` & `google-apps-chat-0.1.4/google/apps/chat/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.3"  # {x-release-please-version}
+__version__ = "0.1.4"  # {x-release-please-version}
```

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/__init__.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 from .types.membership import (
     CreateMembershipRequest,
     DeleteMembershipRequest,
     GetMembershipRequest,
     ListMembershipsRequest,
     ListMembershipsResponse,
     Membership,
+    UpdateMembershipRequest,
 )
 from .types.message import (
     AccessoryWidget,
     ActionResponse,
     AttachedGif,
     CardWithId,
     CreateMessageRequest,
@@ -146,14 +147,15 @@
     "Reaction",
     "RichLinkMetadata",
     "SetUpSpaceRequest",
     "SlashCommand",
     "SlashCommandMetadata",
     "Space",
     "Thread",
+    "UpdateMembershipRequest",
     "UpdateMessageRequest",
     "UpdateSpaceRequest",
     "UploadAttachmentRequest",
     "UploadAttachmentResponse",
     "User",
     "UserMentionMetadata",
     "WidgetMarkup",
```

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/gapic_metadata.json` & `google-apps-chat-0.1.4/google/apps/chat_v1/gapic_metadata.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998867753623188%*

 * *Differences: {"'services'": "{'ChatService': {'clients': {'grpc': {'rpcs': {'UpdateMembership': "*

 * *               "OrderedDict([('methods', ['update_membership'])])}}, 'grpc-async': {'rpcs': "*

 * *               "{'UpdateMembership': OrderedDict([('methods', ['update_membership'])])}}, 'rest': "*

 * *               "{'rpcs': {'UpdateMembership': OrderedDict([('methods', "*

 * *               "['update_membership'])])}}}}}"}*

```diff
@@ -101,14 +101,19 @@
                             ]
                         },
                         "SetUpSpace": {
                             "methods": [
                                 "set_up_space"
                             ]
                         },
+                        "UpdateMembership": {
+                            "methods": [
+                                "update_membership"
+                            ]
+                        },
                         "UpdateMessage": {
                             "methods": [
                                 "update_message"
                             ]
                         },
                         "UpdateSpace": {
                             "methods": [
@@ -216,14 +221,19 @@
                             ]
                         },
                         "SetUpSpace": {
                             "methods": [
                                 "set_up_space"
                             ]
                         },
+                        "UpdateMembership": {
+                            "methods": [
+                                "update_membership"
+                            ]
+                        },
                         "UpdateMessage": {
                             "methods": [
                                 "update_message"
                             ]
                         },
                         "UpdateSpace": {
                             "methods": [
@@ -331,14 +341,19 @@
                             ]
                         },
                         "SetUpSpace": {
                             "methods": [
                                 "set_up_space"
                             ]
                         },
+                        "UpdateMembership": {
+                            "methods": [
+                                "update_membership"
+                            ]
+                        },
                         "UpdateMessage": {
                             "methods": [
                                 "update_message"
                             ]
                         },
                         "UpdateSpace": {
                             "methods": [
```

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/gapic_version.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.3"  # {x-release-please-version}
+__version__ = "0.1.4"  # {x-release-please-version}
```

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/services/__init__.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/services/chat_service/__init__.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/services/chat_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/services/chat_service/async_client.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/services/chat_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -6776,1271 +6776,1603 @@
 0001a770: 2020 2020 2020 2020 2020 6d65 7461 6461            metada
 0001a780: 7461 3d6d 6574 6164 6174 612c 0a20 2020  ta=metadata,.   
 0001a790: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
 0001a7a0: 2320 446f 6e65 3b20 7265 7475 726e 2074  # Done; return t
 0001a7b0: 6865 2072 6573 706f 6e73 652e 0a20 2020  he response..   
 0001a7c0: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
 0001a7d0: 6f6e 7365 0a0a 2020 2020 6173 796e 6320  onse..    async 
-0001a7e0: 6465 6620 6465 6c65 7465 5f6d 656d 6265  def delete_membe
+0001a7e0: 6465 6620 7570 6461 7465 5f6d 656d 6265  def update_membe
 0001a7f0: 7273 6869 7028 0a20 2020 2020 2020 2073  rship(.        s
 0001a800: 656c 662c 0a20 2020 2020 2020 2072 6571  elf,.        req
 0001a810: 7565 7374 3a20 4f70 7469 6f6e 616c 5b55  uest: Optional[U
-0001a820: 6e69 6f6e 5b6d 656d 6265 7273 6869 702e  nion[membership.
-0001a830: 4465 6c65 7465 4d65 6d62 6572 7368 6970  DeleteMembership
-0001a840: 5265 7175 6573 742c 2064 6963 745d 5d20  Request, dict]] 
-0001a850: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0001a860: 2a2c 0a20 2020 2020 2020 206e 616d 653a  *,.        name:
-0001a870: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-0001a880: 204e 6f6e 652c 0a20 2020 2020 2020 2072   None,.        r
-0001a890: 6574 7279 3a20 4f70 7469 6f6e 616c 5265  etry: OptionalRe
-0001a8a0: 7472 7920 3d20 6761 7069 635f 7631 2e6d  try = gapic_v1.m
-0001a8b0: 6574 686f 642e 4445 4641 554c 542c 0a20  ethod.DEFAULT,. 
-0001a8c0: 2020 2020 2020 2074 696d 656f 7574 3a20         timeout: 
-0001a8d0: 556e 696f 6e5b 666c 6f61 742c 206f 626a  Union[float, obj
-0001a8e0: 6563 745d 203d 2067 6170 6963 5f76 312e  ect] = gapic_v1.
-0001a8f0: 6d65 7468 6f64 2e44 4546 4155 4c54 2c0a  method.DEFAULT,.
-0001a900: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
-0001a910: 3a20 5365 7175 656e 6365 5b54 7570 6c65  : Sequence[Tuple
-0001a920: 5b73 7472 2c20 7374 725d 5d20 3d20 2829  [str, str]] = ()
-0001a930: 2c0a 2020 2020 2920 2d3e 206d 656d 6265  ,.    ) -> membe
-0001a940: 7273 6869 702e 4d65 6d62 6572 7368 6970  rship.Membership
-0001a950: 3a0a 2020 2020 2020 2020 7222 2222 4465  :.        r"""De
-0001a960: 6c65 7465 7320 6120 6d65 6d62 6572 7368  letes a membersh
-0001a970: 6970 2e20 466f 7220 616e 2065 7861 6d70  ip. For an examp
-0001a980: 6c65 2c20 7365 6520 6052 656d 6f76 6520  le, see `Remove 
-0001a990: 6120 7573 6572 206f 7220 610a 2020 2020  a user or a.    
-0001a9a0: 2020 2020 476f 6f67 6c65 2043 6861 7420      Google Chat 
-0001a9b0: 6170 7020 6672 6f6d 2061 0a20 2020 2020  app from a.     
-0001a9c0: 2020 2073 7061 6365 203c 6874 7470 733a     space <https:
-0001a9d0: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
-0001a9e0: 676c 652e 636f 6d2f 776f 726b 7370 6163  gle.com/workspac
-0001a9f0: 652f 6368 6174 2f64 656c 6574 652d 6d65  e/chat/delete-me
-0001aa00: 6d62 6572 733e 605f 5f2e 0a0a 2020 2020  mbers>`__...    
-0001aa10: 2020 2020 5265 7175 6972 6573 2060 7573      Requires `us
-0001aa20: 6572 0a20 2020 2020 2020 2061 7574 6865  er.        authe
-0001aa30: 6e74 6963 6174 696f 6e20 3c68 7474 7073  ntication <https
-0001aa40: 3a2f 2f64 6576 656c 6f70 6572 732e 676f  ://developers.go
-0001aa50: 6f67 6c65 2e63 6f6d 2f77 6f72 6b73 7061  ogle.com/workspa
-0001aa60: 6365 2f63 6861 742f 6175 7468 656e 7469  ce/chat/authenti
-0001aa70: 6361 7465 2d61 7574 686f 7269 7a65 2d63  cate-authorize-c
-0001aa80: 6861 742d 7573 6572 3e60 5f5f 2e0a 0a20  hat-user>`__... 
-0001aa90: 2020 2020 2020 202e 2e20 636f 6465 2d62         .. code-b
-0001aaa0: 6c6f 636b 3a3a 2070 7974 686f 6e0a 0a20  lock:: python.. 
-0001aab0: 2020 2020 2020 2020 2020 2023 2054 6869             # Thi
-0001aac0: 7320 736e 6970 7065 7420 6861 7320 6265  s snippet has be
-0001aad0: 656e 2061 7574 6f6d 6174 6963 616c 6c79  en automatically
-0001aae0: 2067 656e 6572 6174 6564 2061 6e64 2073   generated and s
-0001aaf0: 686f 756c 6420 6265 2072 6567 6172 6465  hould be regarde
-0001ab00: 6420 6173 2061 0a20 2020 2020 2020 2020  d as a.         
-0001ab10: 2020 2023 2063 6f64 6520 7465 6d70 6c61     # code templa
-0001ab20: 7465 206f 6e6c 792e 0a20 2020 2020 2020  te only..       
-0001ab30: 2020 2020 2023 2049 7420 7769 6c6c 2072       # It will r
-0001ab40: 6571 7569 7265 206d 6f64 6966 6963 6174  equire modificat
-0001ab50: 696f 6e73 2074 6f20 776f 726b 3a0a 2020  ions to work:.  
-0001ab60: 2020 2020 2020 2020 2020 2320 2d20 4974            # - It
-0001ab70: 206d 6179 2072 6571 7569 7265 2063 6f72   may require cor
-0001ab80: 7265 6374 2f69 6e2d 7261 6e67 6520 7661  rect/in-range va
-0001ab90: 6c75 6573 2066 6f72 2072 6571 7565 7374  lues for request
-0001aba0: 2069 6e69 7469 616c 697a 6174 696f 6e2e   initialization.
-0001abb0: 0a20 2020 2020 2020 2020 2020 2023 202d  .            # -
-0001abc0: 2049 7420 6d61 7920 7265 7175 6972 6520   It may require 
-0001abd0: 7370 6563 6966 7969 6e67 2072 6567 696f  specifying regio
-0001abe0: 6e61 6c20 656e 6470 6f69 6e74 7320 7768  nal endpoints wh
-0001abf0: 656e 2063 7265 6174 696e 6720 7468 6520  en creating the 
-0001ac00: 7365 7276 6963 650a 2020 2020 2020 2020  service.        
-0001ac10: 2020 2020 2320 2020 636c 6965 6e74 2061      #   client a
-0001ac20: 7320 7368 6f77 6e20 696e 3a0a 2020 2020  s shown in:.    
-0001ac30: 2020 2020 2020 2020 2320 2020 6874 7470          #   http
-0001ac40: 733a 2f2f 676f 6f67 6c65 6170 6973 2e64  s://googleapis.d
-0001ac50: 6576 2f70 7974 686f 6e2f 676f 6f67 6c65  ev/python/google
-0001ac60: 2d61 7069 2d63 6f72 652f 6c61 7465 7374  -api-core/latest
-0001ac70: 2f63 6c69 656e 745f 6f70 7469 6f6e 732e  /client_options.
-0001ac80: 6874 6d6c 0a20 2020 2020 2020 2020 2020  html.           
-0001ac90: 2066 726f 6d20 676f 6f67 6c65 2e61 7070   from google.app
-0001aca0: 7320 696d 706f 7274 2063 6861 745f 7631  s import chat_v1
-0001acb0: 0a0a 2020 2020 2020 2020 2020 2020 6173  ..            as
-0001acc0: 796e 6320 6465 6620 7361 6d70 6c65 5f64  ync def sample_d
-0001acd0: 656c 6574 655f 6d65 6d62 6572 7368 6970  elete_membership
-0001ace0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0001acf0: 2020 2020 2320 4372 6561 7465 2061 2063      # Create a c
-0001ad00: 6c69 656e 740a 2020 2020 2020 2020 2020  lient.          
-0001ad10: 2020 2020 2020 636c 6965 6e74 203d 2063        client = c
-0001ad20: 6861 745f 7631 2e43 6861 7453 6572 7669  hat_v1.ChatServi
-0001ad30: 6365 4173 796e 6343 6c69 656e 7428 290a  ceAsyncClient().
-0001ad40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ad50: 2023 2049 6e69 7469 616c 697a 6520 7265   # Initialize re
-0001ad60: 7175 6573 7420 6172 6775 6d65 6e74 2873  quest argument(s
-0001ad70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001ad80: 2020 7265 7175 6573 7420 3d20 6368 6174    request = chat
-0001ad90: 5f76 312e 4465 6c65 7465 4d65 6d62 6572  _v1.DeleteMember
-0001ada0: 7368 6970 5265 7175 6573 7428 0a20 2020  shipRequest(.   
-0001adb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001adc0: 206e 616d 653d 226e 616d 655f 7661 6c75   name="name_valu
-0001add0: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-0001ade0: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
-0001adf0: 2020 2020 2020 2023 204d 616b 6520 7468         # Make th
-0001ae00: 6520 7265 7175 6573 740a 2020 2020 2020  e request.      
-0001ae10: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
-0001ae20: 7365 203d 2061 7761 6974 2063 6c69 656e  se = await clien
-0001ae30: 742e 6465 6c65 7465 5f6d 656d 6265 7273  t.delete_members
-0001ae40: 6869 7028 7265 7175 6573 743d 7265 7175  hip(request=requ
-0001ae50: 6573 7429 0a0a 2020 2020 2020 2020 2020  est)..          
-0001ae60: 2020 2020 2020 2320 4861 6e64 6c65 2074        # Handle t
-0001ae70: 6865 2072 6573 706f 6e73 650a 2020 2020  he response.    
-0001ae80: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0001ae90: 7428 7265 7370 6f6e 7365 290a 0a20 2020  t(response)..   
-0001aea0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-0001aeb0: 2020 2020 2020 2072 6571 7565 7374 2028         request (
-0001aec0: 4f70 7469 6f6e 616c 5b55 6e69 6f6e 5b67  Optional[Union[g
-0001aed0: 6f6f 676c 652e 6170 7073 2e63 6861 745f  oogle.apps.chat_
-0001aee0: 7631 2e74 7970 6573 2e44 656c 6574 654d  v1.types.DeleteM
-0001aef0: 656d 6265 7273 6869 7052 6571 7565 7374  embershipRequest
-0001af00: 2c20 6469 6374 5d5d 293a 0a20 2020 2020  , dict]]):.     
-0001af10: 2020 2020 2020 2020 2020 2054 6865 2072             The r
-0001af20: 6571 7565 7374 206f 626a 6563 742e 2052  equest object. R
-0001af30: 6571 7565 7374 2074 6f20 6465 6c65 7465  equest to delete
-0001af40: 2061 206d 656d 6265 7273 6869 7020 696e   a membership in
-0001af50: 2061 0a20 2020 2020 2020 2020 2020 2020   a.             
-0001af60: 2020 2073 7061 6365 2e0a 2020 2020 2020     space..      
-0001af70: 2020 2020 2020 6e61 6d65 2028 3a63 6c61        name (:cla
-0001af80: 7373 3a60 7374 7260 293a 0a20 2020 2020  ss:`str`):.     
-0001af90: 2020 2020 2020 2020 2020 2052 6571 7569             Requi
-0001afa0: 7265 642e 2052 6573 6f75 7263 6520 6e61  red. Resource na
-0001afb0: 6d65 206f 6620 7468 6520 6d65 6d62 6572  me of the member
-0001afc0: 7368 6970 2074 6f20 6465 6c65 7465 2e0a  ship to delete..
-0001afd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001afe0: 4368 6174 2061 7070 7320 6361 6e20 6465  Chat apps can de
-0001aff0: 6c65 7465 2068 756d 616e 2075 7365 7273  lete human users
-0001b000: 2720 6f72 2074 6865 6972 206f 776e 0a20  ' or their own. 
-0001b010: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0001b020: 656d 6265 7273 6869 7073 2e20 4368 6174  emberships. Chat
-0001b030: 2061 7070 7320 6361 6e27 7420 6465 6c65   apps can't dele
-0001b040: 7465 206f 7468 6572 2061 7070 7327 0a20  te other apps'. 
-0001b050: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0001b060: 656d 6265 7273 6869 7073 2e0a 0a20 2020  emberships...   
-0001b070: 2020 2020 2020 2020 2020 2020 2057 6865               Whe
-0001b080: 6e20 6465 6c65 7469 6e67 2061 2068 756d  n deleting a hum
-0001b090: 616e 206d 656d 6265 7273 6869 702c 2072  an membership, r
-0001b0a0: 6571 7569 7265 7320 7468 650a 2020 2020  equires the.    
-0001b0b0: 2020 2020 2020 2020 2020 2020 6060 6368              ``ch
-0001b0c0: 6174 2e6d 656d 6265 7273 6869 7073 6060  at.memberships``
-0001b0d0: 2073 636f 7065 2061 6e64 0a20 2020 2020   scope and.     
-0001b0e0: 2020 2020 2020 2020 2020 2060 6073 7061             ``spa
-0001b0f0: 6365 732f 7b73 7061 6365 7d2f 6d65 6d62  ces/{space}/memb
-0001b100: 6572 732f 7b6d 656d 6265 727d 6060 2066  ers/{member}`` f
-0001b110: 6f72 6d61 742e 2059 6f75 2063 616e 2075  ormat. You can u
-0001b120: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
-0001b130: 2020 2074 6865 2065 6d61 696c 2061 7320     the email as 
-0001b140: 616e 2061 6c69 6173 2066 6f72 2060 607b  an alias for ``{
-0001b150: 6d65 6d62 6572 7d60 602e 2046 6f72 2065  member}``. For e
-0001b160: 7861 6d70 6c65 2c0a 2020 2020 2020 2020  xample,.        
-0001b170: 2020 2020 2020 2020 6060 7370 6163 6573          ``spaces
-0001b180: 2f7b 7370 6163 657d 2f6d 656d 6265 7273  /{space}/members
-0001b190: 2f65 7861 6d70 6c65 4067 6d61 696c 2e63  /example@gmail.c
-0001b1a0: 6f6d 6060 2077 6865 7265 0a20 2020 2020  om`` where.     
-0001b1b0: 2020 2020 2020 2020 2020 2060 6065 7861             ``exa
-0001b1c0: 6d70 6c65 4067 6d61 696c 2e63 6f6d 6060  mple@gmail.com``
-0001b1d0: 2069 7320 7468 6520 656d 6169 6c20 6f66   is the email of
-0001b1e0: 2074 6865 2047 6f6f 676c 6520 4368 6174   the Google Chat
-0001b1f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b200: 2075 7365 722e 0a0a 2020 2020 2020 2020   user...        
-0001b210: 2020 2020 2020 2020 5768 656e 2064 656c          When del
-0001b220: 6574 696e 6720 616e 2061 7070 206d 656d  eting an app mem
-0001b230: 6265 7273 6869 702c 2072 6571 7569 7265  bership, require
-0001b240: 7320 7468 650a 2020 2020 2020 2020 2020  s the.          
-0001b250: 2020 2020 2020 6060 6368 6174 2e6d 656d        ``chat.mem
-0001b260: 6265 7273 6869 7073 2e61 7070 6060 2073  berships.app`` s
-0001b270: 636f 7065 2061 6e64 0a20 2020 2020 2020  cope and.       
-0001b280: 2020 2020 2020 2020 2060 6073 7061 6365           ``space
-0001b290: 732f 7b73 7061 6365 7d2f 6d65 6d62 6572  s/{space}/member
-0001b2a0: 732f 6170 7060 6020 666f 726d 6174 2e0a  s/app`` format..
-0001b2b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b2c0: 2046 6f72 6d61 743a 2060 6073 7061 6365   Format: ``space
-0001b2d0: 732f 7b73 7061 6365 7d2f 6d65 6d62 6572  s/{space}/member
-0001b2e0: 732f 7b6d 656d 6265 727d 6060 206f 720a  s/{member}`` or.
-0001b2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b300: 6060 7370 6163 6573 2f7b 7370 6163 657d  ``spaces/{space}
-0001b310: 2f6d 656d 6265 7273 2f61 7070 6060 2e0a  /members/app``..
-0001b320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b330: 2054 6869 7320 636f 7272 6573 706f 6e64   This correspond
-0001b340: 7320 746f 2074 6865 2060 606e 616d 6560  s to the ``name`
-0001b350: 6020 6669 656c 640a 2020 2020 2020 2020  ` field.        
-0001b360: 2020 2020 2020 2020 6f6e 2074 6865 2060          on the `
-0001b370: 6072 6571 7565 7374 6060 2069 6e73 7461  `request`` insta
-0001b380: 6e63 653b 2069 6620 6060 7265 7175 6573  nce; if ``reques
-0001b390: 7460 6020 6973 2070 726f 7669 6465 642c  t`` is provided,
-0001b3a0: 2074 6869 730a 2020 2020 2020 2020 2020   this.          
-0001b3b0: 2020 2020 2020 7368 6f75 6c64 206e 6f74        should not
-0001b3c0: 2062 6520 7365 742e 0a20 2020 2020 2020   be set..       
-0001b3d0: 2020 2020 2072 6574 7279 2028 676f 6f67       retry (goog
-0001b3e0: 6c65 2e61 7069 5f63 6f72 652e 7265 7472  le.api_core.retr
-0001b3f0: 795f 6173 796e 632e 4173 796e 6352 6574  y_async.AsyncRet
-0001b400: 7279 293a 2044 6573 6967 6e61 7469 6f6e  ry): Designation
-0001b410: 206f 6620 7768 6174 2065 7272 6f72 732c   of what errors,
-0001b420: 2069 6620 616e 792c 0a20 2020 2020 2020   if any,.       
-0001b430: 2020 2020 2020 2020 2073 686f 756c 6420           should 
-0001b440: 6265 2072 6574 7269 6564 2e0a 2020 2020  be retried..    
-0001b450: 2020 2020 2020 2020 7469 6d65 6f75 7420          timeout 
-0001b460: 2866 6c6f 6174 293a 2054 6865 2074 696d  (float): The tim
-0001b470: 656f 7574 2066 6f72 2074 6869 7320 7265  eout for this re
-0001b480: 7175 6573 742e 0a20 2020 2020 2020 2020  quest..         
-0001b490: 2020 206d 6574 6164 6174 6120 2853 6571     metadata (Seq
-0001b4a0: 7565 6e63 655b 5475 706c 655b 7374 722c  uence[Tuple[str,
-0001b4b0: 2073 7472 5d5d 293a 2053 7472 696e 6773   str]]): Strings
-0001b4c0: 2077 6869 6368 2073 686f 756c 6420 6265   which should be
-0001b4d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b4e0: 2073 656e 7420 616c 6f6e 6720 7769 7468   sent along with
-0001b4f0: 2074 6865 2072 6571 7565 7374 2061 7320   the request as 
-0001b500: 6d65 7461 6461 7461 2e0a 0a20 2020 2020  metadata...     
-0001b510: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-0001b520: 2020 2020 2020 2020 676f 6f67 6c65 2e61          google.a
-0001b530: 7070 732e 6368 6174 5f76 312e 7479 7065  pps.chat_v1.type
-0001b540: 732e 4d65 6d62 6572 7368 6970 3a0a 2020  s.Membership:.  
-0001b550: 2020 2020 2020 2020 2020 2020 2020 5265                Re
-0001b560: 7072 6573 656e 7473 2061 206d 656d 6265  presents a membe
-0001b570: 7273 6869 7020 7265 6c61 7469 6f6e 2069  rship relation i
-0001b580: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-0001b590: 2020 476f 6f67 6c65 2043 6861 742c 2073    Google Chat, s
-0001b5a0: 7563 6820 6173 2077 6865 7468 6572 2061  uch as whether a
-0001b5b0: 2075 7365 7220 6f72 0a20 2020 2020 2020   user or.       
-0001b5c0: 2020 2020 2020 2020 2043 6861 7420 6170           Chat ap
-0001b5d0: 7020 6973 2069 6e76 6974 6564 2074 6f2c  p is invited to,
-0001b5e0: 2070 6172 7420 6f66 2c20 6f72 0a20 2020   part of, or.   
-0001b5f0: 2020 2020 2020 2020 2020 2020 2061 6273               abs
-0001b600: 656e 7420 6672 6f6d 2061 2073 7061 6365  ent from a space
-0001b610: 2e0a 0a20 2020 2020 2020 2022 2222 0a20  ...        """. 
-0001b620: 2020 2020 2020 2023 2043 7265 6174 6520         # Create 
-0001b630: 6f72 2063 6f65 7263 6520 6120 7072 6f74  or coerce a prot
-0001b640: 6f62 7566 2072 6571 7565 7374 206f 626a  obuf request obj
-0001b650: 6563 742e 0a20 2020 2020 2020 2023 2051  ect..        # Q
-0001b660: 7569 636b 2063 6865 636b 3a20 4966 2077  uick check: If w
-0001b670: 6520 676f 7420 6120 7265 7175 6573 7420  e got a request 
-0001b680: 6f62 6a65 6374 2c20 7765 2073 686f 756c  object, we shoul
-0001b690: 6420 2a6e 6f74 2a20 6861 7665 0a20 2020  d *not* have.   
-0001b6a0: 2020 2020 2023 2067 6f74 7465 6e20 616e       # gotten an
-0001b6b0: 7920 6b65 7977 6f72 6420 6172 6775 6d65  y keyword argume
-0001b6c0: 6e74 7320 7468 6174 206d 6170 2074 6f20  nts that map to 
-0001b6d0: 7468 6520 7265 7175 6573 742e 0a20 2020  the request..   
-0001b6e0: 2020 2020 2068 6173 5f66 6c61 7474 656e       has_flatten
-0001b6f0: 6564 5f70 6172 616d 7320 3d20 616e 7928  ed_params = any(
-0001b700: 5b6e 616d 655d 290a 2020 2020 2020 2020  [name]).        
-0001b710: 6966 2072 6571 7565 7374 2069 7320 6e6f  if request is no
-0001b720: 7420 4e6f 6e65 2061 6e64 2068 6173 5f66  t None and has_f
-0001b730: 6c61 7474 656e 6564 5f70 6172 616d 733a  lattened_params:
-0001b740: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0001b750: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
-0001b760: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0001b770: 4966 2074 6865 2060 7265 7175 6573 7460  If the `request`
-0001b780: 2061 7267 756d 656e 7420 6973 2073 6574   argument is set
-0001b790: 2c20 7468 656e 206e 6f6e 6520 6f66 2022  , then none of "
-0001b7a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b7b0: 2022 7468 6520 696e 6469 7669 6475 616c   "the individual
-0001b7c0: 2066 6965 6c64 2061 7267 756d 656e 7473   field arguments
-0001b7d0: 2073 686f 756c 6420 6265 2073 6574 2e22   should be set."
-0001b7e0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-0001b7f0: 2020 2020 2020 2020 7265 7175 6573 7420          request 
-0001b800: 3d20 6d65 6d62 6572 7368 6970 2e44 656c  = membership.Del
-0001b810: 6574 654d 656d 6265 7273 6869 7052 6571  eteMembershipReq
-0001b820: 7565 7374 2872 6571 7565 7374 290a 0a20  uest(request).. 
-0001b830: 2020 2020 2020 2023 2049 6620 7765 2068         # If we h
-0001b840: 6176 6520 6b65 7977 6f72 6420 6172 6775  ave keyword argu
-0001b850: 6d65 6e74 7320 636f 7272 6573 706f 6e64  ments correspond
-0001b860: 696e 6720 746f 2066 6965 6c64 7320 6f6e  ing to fields on
-0001b870: 2074 6865 0a20 2020 2020 2020 2023 2072   the.        # r
-0001b880: 6571 7565 7374 2c20 6170 706c 7920 7468  equest, apply th
-0001b890: 6573 652e 0a20 2020 2020 2020 2069 6620  ese..        if 
-0001b8a0: 6e61 6d65 2069 7320 6e6f 7420 4e6f 6e65  name is not None
-0001b8b0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0001b8c0: 7175 6573 742e 6e61 6d65 203d 206e 616d  quest.name = nam
-0001b8d0: 650a 0a20 2020 2020 2020 2023 2057 7261  e..        # Wra
-0001b8e0: 7020 7468 6520 5250 4320 6d65 7468 6f64  p the RPC method
-0001b8f0: 3b20 7468 6973 2061 6464 7320 7265 7472  ; this adds retr
-0001b900: 7920 616e 6420 7469 6d65 6f75 7420 696e  y and timeout in
-0001b910: 666f 726d 6174 696f 6e2c 0a20 2020 2020  formation,.     
-0001b920: 2020 2023 2061 6e64 2066 7269 656e 646c     # and friendl
-0001b930: 7920 6572 726f 7220 6861 6e64 6c69 6e67  y error handling
-0001b940: 2e0a 2020 2020 2020 2020 7270 6320 3d20  ..        rpc = 
-0001b950: 6761 7069 635f 7631 2e6d 6574 686f 645f  gapic_v1.method_
-0001b960: 6173 796e 632e 7772 6170 5f6d 6574 686f  async.wrap_metho
-0001b970: 6428 0a20 2020 2020 2020 2020 2020 2073  d(.            s
-0001b980: 656c 662e 5f63 6c69 656e 742e 5f74 7261  elf._client._tra
-0001b990: 6e73 706f 7274 2e64 656c 6574 655f 6d65  nsport.delete_me
-0001b9a0: 6d62 6572 7368 6970 2c0a 2020 2020 2020  mbership,.      
-0001b9b0: 2020 2020 2020 6465 6661 756c 745f 7265        default_re
-0001b9c0: 7472 793d 7265 7472 6965 732e 4173 796e  try=retries.Asyn
-0001b9d0: 6352 6574 7279 280a 2020 2020 2020 2020  cRetry(.        
-0001b9e0: 2020 2020 2020 2020 696e 6974 6961 6c3d          initial=
-0001b9f0: 312e 302c 0a20 2020 2020 2020 2020 2020  1.0,.           
-0001ba00: 2020 2020 206d 6178 696d 756d 3d31 302e       maximum=10.
-0001ba10: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
-0001ba20: 2020 206d 756c 7469 706c 6965 723d 312e     multiplier=1.
-0001ba30: 332c 0a20 2020 2020 2020 2020 2020 2020  3,.             
-0001ba40: 2020 2070 7265 6469 6361 7465 3d72 6574     predicate=ret
-0001ba50: 7269 6573 2e69 665f 6578 6365 7074 696f  ries.if_exceptio
-0001ba60: 6e5f 7479 7065 280a 2020 2020 2020 2020  n_type(.        
-0001ba70: 2020 2020 2020 2020 2020 2020 636f 7265              core
-0001ba80: 5f65 7863 6570 7469 6f6e 732e 5365 7276  _exceptions.Serv
-0001ba90: 6963 6555 6e61 7661 696c 6162 6c65 2c0a  iceUnavailable,.
-0001baa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bab0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0001bac0: 2020 2064 6561 646c 696e 653d 3330 2e30     deadline=30.0
-0001bad0: 2c0a 2020 2020 2020 2020 2020 2020 292c  ,.            ),
-0001bae0: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
-0001baf0: 6175 6c74 5f74 696d 656f 7574 3d33 302e  ault_timeout=30.
-0001bb00: 302c 0a20 2020 2020 2020 2020 2020 2063  0,.            c
-0001bb10: 6c69 656e 745f 696e 666f 3d44 4546 4155  lient_info=DEFAU
-0001bb20: 4c54 5f43 4c49 454e 545f 494e 464f 2c0a  LT_CLIENT_INFO,.
-0001bb30: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0001bb40: 2020 2023 2043 6572 7461 696e 2066 6965     # Certain fie
-0001bb50: 6c64 7320 7368 6f75 6c64 2062 6520 7072  lds should be pr
-0001bb60: 6f76 6964 6564 2077 6974 6869 6e20 7468  ovided within th
-0001bb70: 6520 6d65 7461 6461 7461 2068 6561 6465  e metadata heade
-0001bb80: 723b 0a20 2020 2020 2020 2023 2061 6464  r;.        # add
-0001bb90: 2074 6865 7365 2068 6572 652e 0a20 2020   these here..   
-0001bba0: 2020 2020 206d 6574 6164 6174 6120 3d20       metadata = 
-0001bbb0: 7475 706c 6528 6d65 7461 6461 7461 2920  tuple(metadata) 
-0001bbc0: 2b20 280a 2020 2020 2020 2020 2020 2020  + (.            
-0001bbd0: 6761 7069 635f 7631 2e72 6f75 7469 6e67  gapic_v1.routing
-0001bbe0: 5f68 6561 6465 722e 746f 5f67 7270 635f  _header.to_grpc_
-0001bbf0: 6d65 7461 6461 7461 2828 2822 6e61 6d65  metadata((("name
-0001bc00: 222c 2072 6571 7565 7374 2e6e 616d 6529  ", request.name)
-0001bc10: 2c29 292c 0a20 2020 2020 2020 2029 0a0a  ,)),.        )..
-0001bc20: 2020 2020 2020 2020 2320 5661 6c69 6461          # Valida
-0001bc30: 7465 2074 6865 2075 6e69 7665 7273 6520  te the universe 
-0001bc40: 646f 6d61 696e 2e0a 2020 2020 2020 2020  domain..        
-0001bc50: 7365 6c66 2e5f 636c 6965 6e74 2e5f 7661  self._client._va
-0001bc60: 6c69 6461 7465 5f75 6e69 7665 7273 655f  lidate_universe_
-0001bc70: 646f 6d61 696e 2829 0a0a 2020 2020 2020  domain()..      
-0001bc80: 2020 2320 5365 6e64 2074 6865 2072 6571    # Send the req
-0001bc90: 7565 7374 2e0a 2020 2020 2020 2020 7265  uest..        re
-0001bca0: 7370 6f6e 7365 203d 2061 7761 6974 2072  sponse = await r
-0001bcb0: 7063 280a 2020 2020 2020 2020 2020 2020  pc(.            
-0001bcc0: 7265 7175 6573 742c 0a20 2020 2020 2020  request,.       
-0001bcd0: 2020 2020 2072 6574 7279 3d72 6574 7279       retry=retry
-0001bce0: 2c0a 2020 2020 2020 2020 2020 2020 7469  ,.            ti
-0001bcf0: 6d65 6f75 743d 7469 6d65 6f75 742c 0a20  meout=timeout,. 
-0001bd00: 2020 2020 2020 2020 2020 206d 6574 6164             metad
-0001bd10: 6174 613d 6d65 7461 6461 7461 2c0a 2020  ata=metadata,.  
-0001bd20: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0001bd30: 2023 2044 6f6e 653b 2072 6574 7572 6e20   # Done; return 
-0001bd40: 7468 6520 7265 7370 6f6e 7365 2e0a 2020  the response..  
-0001bd50: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-0001bd60: 706f 6e73 650a 0a20 2020 2061 7379 6e63  ponse..    async
-0001bd70: 2064 6566 2063 7265 6174 655f 7265 6163   def create_reac
-0001bd80: 7469 6f6e 280a 2020 2020 2020 2020 7365  tion(.        se
-0001bd90: 6c66 2c0a 2020 2020 2020 2020 7265 7175  lf,.        requ
-0001bda0: 6573 743a 204f 7074 696f 6e61 6c5b 556e  est: Optional[Un
-0001bdb0: 696f 6e5b 6763 5f72 6561 6374 696f 6e2e  ion[gc_reaction.
-0001bdc0: 4372 6561 7465 5265 6163 7469 6f6e 5265  CreateReactionRe
-0001bdd0: 7175 6573 742c 2064 6963 745d 5d20 3d20  quest, dict]] = 
-0001bde0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2a2c  None,.        *,
-0001bdf0: 0a20 2020 2020 2020 2070 6172 656e 743a  .        parent:
-0001be00: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-0001be10: 204e 6f6e 652c 0a20 2020 2020 2020 2072   None,.        r
-0001be20: 6561 6374 696f 6e3a 204f 7074 696f 6e61  eaction: Optiona
-0001be30: 6c5b 6763 5f72 6561 6374 696f 6e2e 5265  l[gc_reaction.Re
-0001be40: 6163 7469 6f6e 5d20 3d20 4e6f 6e65 2c0a  action] = None,.
-0001be50: 2020 2020 2020 2020 7265 7472 793a 204f          retry: O
-0001be60: 7074 696f 6e61 6c52 6574 7279 203d 2067  ptionalRetry = g
-0001be70: 6170 6963 5f76 312e 6d65 7468 6f64 2e44  apic_v1.method.D
-0001be80: 4546 4155 4c54 2c0a 2020 2020 2020 2020  EFAULT,.        
-0001be90: 7469 6d65 6f75 743a 2055 6e69 6f6e 5b66  timeout: Union[f
-0001bea0: 6c6f 6174 2c20 6f62 6a65 6374 5d20 3d20  loat, object] = 
-0001beb0: 6761 7069 635f 7631 2e6d 6574 686f 642e  gapic_v1.method.
-0001bec0: 4445 4641 554c 542c 0a20 2020 2020 2020  DEFAULT,.       
-0001bed0: 206d 6574 6164 6174 613a 2053 6571 7565   metadata: Seque
-0001bee0: 6e63 655b 5475 706c 655b 7374 722c 2073  nce[Tuple[str, s
-0001bef0: 7472 5d5d 203d 2028 292c 0a20 2020 2029  tr]] = (),.    )
-0001bf00: 202d 3e20 6763 5f72 6561 6374 696f 6e2e   -> gc_reaction.
-0001bf10: 5265 6163 7469 6f6e 3a0a 2020 2020 2020  Reaction:.      
-0001bf20: 2020 7222 2222 4372 6561 7465 7320 6120    r"""Creates a 
-0001bf30: 7265 6163 7469 6f6e 2061 6e64 2061 6464  reaction and add
-0001bf40: 7320 6974 2074 6f20 6120 6d65 7373 6167  s it to a messag
-0001bf50: 652e 204f 6e6c 7920 756e 6963 6f64 6520  e. Only unicode 
-0001bf60: 656d 6f6a 6973 0a20 2020 2020 2020 2061  emojis.        a
-0001bf70: 7265 2073 7570 706f 7274 6564 2e20 466f  re supported. Fo
-0001bf80: 7220 616e 2065 7861 6d70 6c65 2c20 7365  r an example, se
-0001bf90: 6520 6041 6464 2061 2072 6561 6374 696f  e `Add a reactio
-0001bfa0: 6e20 746f 2061 0a20 2020 2020 2020 206d  n to a.        m
-0001bfb0: 6573 7361 6765 203c 6874 7470 733a 2f2f  essage <https://
-0001bfc0: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
-0001bfd0: 652e 636f 6d2f 776f 726b 7370 6163 652f  e.com/workspace/
-0001bfe0: 6368 6174 2f63 7265 6174 652d 7265 6163  chat/create-reac
-0001bff0: 7469 6f6e 733e 605f 5f2e 0a20 2020 2020  tions>`__..     
-0001c000: 2020 2052 6571 7569 7265 7320 6075 7365     Requires `use
-0001c010: 720a 2020 2020 2020 2020 6175 7468 656e  r.        authen
-0001c020: 7469 6361 7469 6f6e 203c 6874 7470 733a  tication <https:
-0001c030: 2f2f 6465 7665 6c6f 7065 7273 2e67 6f6f  //developers.goo
-0001c040: 676c 652e 636f 6d2f 776f 726b 7370 6163  gle.com/workspac
-0001c050: 652f 6368 6174 2f61 7574 6865 6e74 6963  e/chat/authentic
-0001c060: 6174 652d 6175 7468 6f72 697a 652d 6368  ate-authorize-ch
-0001c070: 6174 2d75 7365 723e 605f 5f2e 0a0a 2020  at-user>`__...  
-0001c080: 2020 2020 2020 2e2e 2063 6f64 652d 626c        .. code-bl
-0001c090: 6f63 6b3a 3a20 7079 7468 6f6e 0a0a 2020  ock:: python..  
-0001c0a0: 2020 2020 2020 2020 2020 2320 5468 6973            # This
-0001c0b0: 2073 6e69 7070 6574 2068 6173 2062 6565   snippet has bee
-0001c0c0: 6e20 6175 746f 6d61 7469 6361 6c6c 7920  n automatically 
-0001c0d0: 6765 6e65 7261 7465 6420 616e 6420 7368  generated and sh
-0001c0e0: 6f75 6c64 2062 6520 7265 6761 7264 6564  ould be regarded
-0001c0f0: 2061 7320 610a 2020 2020 2020 2020 2020   as a.          
-0001c100: 2020 2320 636f 6465 2074 656d 706c 6174    # code templat
-0001c110: 6520 6f6e 6c79 2e0a 2020 2020 2020 2020  e only..        
-0001c120: 2020 2020 2320 4974 2077 696c 6c20 7265      # It will re
-0001c130: 7175 6972 6520 6d6f 6469 6669 6361 7469  quire modificati
-0001c140: 6f6e 7320 746f 2077 6f72 6b3a 0a20 2020  ons to work:.   
-0001c150: 2020 2020 2020 2020 2023 202d 2049 7420           # - It 
-0001c160: 6d61 7920 7265 7175 6972 6520 636f 7272  may require corr
-0001c170: 6563 742f 696e 2d72 616e 6765 2076 616c  ect/in-range val
-0001c180: 7565 7320 666f 7220 7265 7175 6573 7420  ues for request 
-0001c190: 696e 6974 6961 6c69 7a61 7469 6f6e 2e0a  initialization..
-0001c1a0: 2020 2020 2020 2020 2020 2020 2320 2d20              # - 
-0001c1b0: 4974 206d 6179 2072 6571 7569 7265 2073  It may require s
-0001c1c0: 7065 6369 6679 696e 6720 7265 6769 6f6e  pecifying region
-0001c1d0: 616c 2065 6e64 706f 696e 7473 2077 6865  al endpoints whe
-0001c1e0: 6e20 6372 6561 7469 6e67 2074 6865 2073  n creating the s
-0001c1f0: 6572 7669 6365 0a20 2020 2020 2020 2020  ervice.         
-0001c200: 2020 2023 2020 2063 6c69 656e 7420 6173     #   client as
-0001c210: 2073 686f 776e 2069 6e3a 0a20 2020 2020   shown in:.     
-0001c220: 2020 2020 2020 2023 2020 2068 7474 7073         #   https
-0001c230: 3a2f 2f67 6f6f 676c 6561 7069 732e 6465  ://googleapis.de
-0001c240: 762f 7079 7468 6f6e 2f67 6f6f 676c 652d  v/python/google-
-0001c250: 6170 692d 636f 7265 2f6c 6174 6573 742f  api-core/latest/
-0001c260: 636c 6965 6e74 5f6f 7074 696f 6e73 2e68  client_options.h
-0001c270: 746d 6c0a 2020 2020 2020 2020 2020 2020  tml.            
-0001c280: 6672 6f6d 2067 6f6f 676c 652e 6170 7073  from google.apps
-0001c290: 2069 6d70 6f72 7420 6368 6174 5f76 310a   import chat_v1.
-0001c2a0: 0a20 2020 2020 2020 2020 2020 2061 7379  .            asy
-0001c2b0: 6e63 2064 6566 2073 616d 706c 655f 6372  nc def sample_cr
-0001c2c0: 6561 7465 5f72 6561 6374 696f 6e28 293a  eate_reaction():
-0001c2d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c2e0: 2023 2043 7265 6174 6520 6120 636c 6965   # Create a clie
-0001c2f0: 6e74 0a20 2020 2020 2020 2020 2020 2020  nt.             
-0001c300: 2020 2063 6c69 656e 7420 3d20 6368 6174     client = chat
-0001c310: 5f76 312e 4368 6174 5365 7276 6963 6541  _v1.ChatServiceA
-0001c320: 7379 6e63 436c 6965 6e74 2829 0a0a 2020  syncClient()..  
-0001c330: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0001c340: 496e 6974 6961 6c69 7a65 2072 6571 7565  Initialize reque
-0001c350: 7374 2061 7267 756d 656e 7428 7329 0a20  st argument(s). 
-0001c360: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0001c370: 6571 7565 7374 203d 2063 6861 745f 7631  equest = chat_v1
-0001c380: 2e43 7265 6174 6552 6561 6374 696f 6e52  .CreateReactionR
-0001c390: 6571 7565 7374 280a 2020 2020 2020 2020  equest(.        
-0001c3a0: 2020 2020 2020 2020 2020 2020 7061 7265              pare
-0001c3b0: 6e74 3d22 7061 7265 6e74 5f76 616c 7565  nt="parent_value
-0001c3c0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0001c3d0: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
-0001c3e0: 2020 2020 2020 2320 4d61 6b65 2074 6865        # Make the
-0001c3f0: 2072 6571 7565 7374 0a20 2020 2020 2020   request.       
-0001c400: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
-0001c410: 6520 3d20 6177 6169 7420 636c 6965 6e74  e = await client
-0001c420: 2e63 7265 6174 655f 7265 6163 7469 6f6e  .create_reaction
-0001c430: 2872 6571 7565 7374 3d72 6571 7565 7374  (request=request
-0001c440: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-0001c450: 2020 2023 2048 616e 646c 6520 7468 6520     # Handle the 
-0001c460: 7265 7370 6f6e 7365 0a20 2020 2020 2020  response.       
-0001c470: 2020 2020 2020 2020 2070 7269 6e74 2872           print(r
-0001c480: 6573 706f 6e73 6529 0a0a 2020 2020 2020  esponse)..      
-0001c490: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-0001c4a0: 2020 2020 7265 7175 6573 7420 284f 7074      request (Opt
-0001c4b0: 696f 6e61 6c5b 556e 696f 6e5b 676f 6f67  ional[Union[goog
-0001c4c0: 6c65 2e61 7070 732e 6368 6174 5f76 312e  le.apps.chat_v1.
-0001c4d0: 7479 7065 732e 4372 6561 7465 5265 6163  types.CreateReac
-0001c4e0: 7469 6f6e 5265 7175 6573 742c 2064 6963  tionRequest, dic
-0001c4f0: 745d 5d29 3a0a 2020 2020 2020 2020 2020  t]]):.          
-0001c500: 2020 2020 2020 5468 6520 7265 7175 6573        The reques
-0001c510: 7420 6f62 6a65 6374 2e20 4372 6561 7465  t object. Create
-0001c520: 7320 6120 7265 6163 7469 6f6e 2074 6f20  s a reaction to 
-0001c530: 6120 6d65 7373 6167 652e 0a20 2020 2020  a message..     
-0001c540: 2020 2020 2020 2070 6172 656e 7420 283a         parent (:
-0001c550: 636c 6173 733a 6073 7472 6029 3a0a 2020  class:`str`):.  
-0001c560: 2020 2020 2020 2020 2020 2020 2020 5265                Re
-0001c570: 7175 6972 6564 2e20 5468 6520 6d65 7373  quired. The mess
-0001c580: 6167 6520 7768 6572 6520 7468 6520 7265  age where the re
-0001c590: 6163 7469 6f6e 2069 7320 6372 6561 7465  action is create
-0001c5a0: 642e 0a0a 2020 2020 2020 2020 2020 2020  d...            
-0001c5b0: 2020 2020 466f 726d 6174 3a20 6060 7370      Format: ``sp
-0001c5c0: 6163 6573 2f7b 7370 6163 657d 2f6d 6573  aces/{space}/mes
-0001c5d0: 7361 6765 732f 7b6d 6573 7361 6765 7d60  sages/{message}`
-0001c5e0: 600a 0a20 2020 2020 2020 2020 2020 2020  `..             
-0001c5f0: 2020 2054 6869 7320 636f 7272 6573 706f     This correspo
-0001c600: 6e64 7320 746f 2074 6865 2060 6070 6172  nds to the ``par
-0001c610: 656e 7460 6020 6669 656c 640a 2020 2020  ent`` field.    
-0001c620: 2020 2020 2020 2020 2020 2020 6f6e 2074              on t
-0001c630: 6865 2060 6072 6571 7565 7374 6060 2069  he ``request`` i
-0001c640: 6e73 7461 6e63 653b 2069 6620 6060 7265  nstance; if ``re
-0001c650: 7175 6573 7460 6020 6973 2070 726f 7669  quest`` is provi
-0001c660: 6465 642c 2074 6869 730a 2020 2020 2020  ded, this.      
-0001c670: 2020 2020 2020 2020 2020 7368 6f75 6c64            should
-0001c680: 206e 6f74 2062 6520 7365 742e 0a20 2020   not be set..   
-0001c690: 2020 2020 2020 2020 2072 6561 6374 696f           reactio
-0001c6a0: 6e20 283a 636c 6173 733a 6067 6f6f 676c  n (:class:`googl
-0001c6b0: 652e 6170 7073 2e63 6861 745f 7631 2e74  e.apps.chat_v1.t
-0001c6c0: 7970 6573 2e52 6561 6374 696f 6e60 293a  ypes.Reaction`):
-0001c6d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c6e0: 2052 6571 7569 7265 642e 2054 6865 2072   Required. The r
-0001c6f0: 6561 6374 696f 6e20 746f 2063 7265 6174  eaction to creat
-0001c700: 652e 0a20 2020 2020 2020 2020 2020 2020  e..             
-0001c710: 2020 2054 6869 7320 636f 7272 6573 706f     This correspo
-0001c720: 6e64 7320 746f 2074 6865 2060 6072 6561  nds to the ``rea
-0001c730: 6374 696f 6e60 6020 6669 656c 640a 2020  ction`` field.  
-0001c740: 2020 2020 2020 2020 2020 2020 2020 6f6e                on
-0001c750: 2074 6865 2060 6072 6571 7565 7374 6060   the ``request``
-0001c760: 2069 6e73 7461 6e63 653b 2069 6620 6060   instance; if ``
-0001c770: 7265 7175 6573 7460 6020 6973 2070 726f  request`` is pro
-0001c780: 7669 6465 642c 2074 6869 730a 2020 2020  vided, this.    
-0001c790: 2020 2020 2020 2020 2020 2020 7368 6f75              shou
-0001c7a0: 6c64 206e 6f74 2062 6520 7365 742e 0a20  ld not be set.. 
-0001c7b0: 2020 2020 2020 2020 2020 2072 6574 7279             retry
-0001c7c0: 2028 676f 6f67 6c65 2e61 7069 5f63 6f72   (google.api_cor
-0001c7d0: 652e 7265 7472 795f 6173 796e 632e 4173  e.retry_async.As
-0001c7e0: 796e 6352 6574 7279 293a 2044 6573 6967  yncRetry): Desig
-0001c7f0: 6e61 7469 6f6e 206f 6620 7768 6174 2065  nation of what e
-0001c800: 7272 6f72 732c 2069 6620 616e 792c 0a20  rrors, if any,. 
-0001c810: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001c820: 686f 756c 6420 6265 2072 6574 7269 6564  hould be retried
-0001c830: 2e0a 2020 2020 2020 2020 2020 2020 7469  ..            ti
-0001c840: 6d65 6f75 7420 2866 6c6f 6174 293a 2054  meout (float): T
-0001c850: 6865 2074 696d 656f 7574 2066 6f72 2074  he timeout for t
-0001c860: 6869 7320 7265 7175 6573 742e 0a20 2020  his request..   
-0001c870: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
-0001c880: 6120 2853 6571 7565 6e63 655b 5475 706c  a (Sequence[Tupl
-0001c890: 655b 7374 722c 2073 7472 5d5d 293a 2053  e[str, str]]): S
-0001c8a0: 7472 696e 6773 2077 6869 6368 2073 686f  trings which sho
-0001c8b0: 756c 6420 6265 0a20 2020 2020 2020 2020  uld be.         
-0001c8c0: 2020 2020 2020 2073 656e 7420 616c 6f6e         sent alon
-0001c8d0: 6720 7769 7468 2074 6865 2072 6571 7565  g with the reque
-0001c8e0: 7374 2061 7320 6d65 7461 6461 7461 2e0a  st as metadata..
-0001c8f0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-0001c900: 3a0a 2020 2020 2020 2020 2020 2020 676f  :.            go
-0001c910: 6f67 6c65 2e61 7070 732e 6368 6174 5f76  ogle.apps.chat_v
-0001c920: 312e 7479 7065 732e 5265 6163 7469 6f6e  1.types.Reaction
-0001c930: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001c940: 2020 4120 7265 6163 7469 6f6e 2074 6f20    A reaction to 
-0001c950: 6120 6d65 7373 6167 652e 0a20 2020 2020  a message..     
-0001c960: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
-0001c970: 2043 7265 6174 6520 6f72 2063 6f65 7263   Create or coerc
-0001c980: 6520 6120 7072 6f74 6f62 7566 2072 6571  e a protobuf req
-0001c990: 7565 7374 206f 626a 6563 742e 0a20 2020  uest object..   
-0001c9a0: 2020 2020 2023 2051 7569 636b 2063 6865       # Quick che
-0001c9b0: 636b 3a20 4966 2077 6520 676f 7420 6120  ck: If we got a 
-0001c9c0: 7265 7175 6573 7420 6f62 6a65 6374 2c20  request object, 
-0001c9d0: 7765 2073 686f 756c 6420 2a6e 6f74 2a20  we should *not* 
-0001c9e0: 6861 7665 0a20 2020 2020 2020 2023 2067  have.        # g
-0001c9f0: 6f74 7465 6e20 616e 7920 6b65 7977 6f72  otten any keywor
-0001ca00: 6420 6172 6775 6d65 6e74 7320 7468 6174  d arguments that
-0001ca10: 206d 6170 2074 6f20 7468 6520 7265 7175   map to the requ
-0001ca20: 6573 742e 0a20 2020 2020 2020 2068 6173  est..        has
-0001ca30: 5f66 6c61 7474 656e 6564 5f70 6172 616d  _flattened_param
-0001ca40: 7320 3d20 616e 7928 5b70 6172 656e 742c  s = any([parent,
-0001ca50: 2072 6561 6374 696f 6e5d 290a 2020 2020   reaction]).    
-0001ca60: 2020 2020 6966 2072 6571 7565 7374 2069      if request i
-0001ca70: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2068  s not None and h
-0001ca80: 6173 5f66 6c61 7474 656e 6564 5f70 6172  as_flattened_par
-0001ca90: 616d 733a 0a20 2020 2020 2020 2020 2020  ams:.           
-0001caa0: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-0001cab0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-0001cac0: 2020 2022 4966 2074 6865 2060 7265 7175     "If the `requ
-0001cad0: 6573 7460 2061 7267 756d 656e 7420 6973  est` argument is
-0001cae0: 2073 6574 2c20 7468 656e 206e 6f6e 6520   set, then none 
-0001caf0: 6f66 2022 0a20 2020 2020 2020 2020 2020  of ".           
-0001cb00: 2020 2020 2022 7468 6520 696e 6469 7669       "the indivi
-0001cb10: 6475 616c 2066 6965 6c64 2061 7267 756d  dual field argum
-0001cb20: 656e 7473 2073 686f 756c 6420 6265 2073  ents should be s
-0001cb30: 6574 2e22 0a20 2020 2020 2020 2020 2020  et.".           
-0001cb40: 2029 0a0a 2020 2020 2020 2020 7265 7175   )..        requ
-0001cb50: 6573 7420 3d20 6763 5f72 6561 6374 696f  est = gc_reactio
-0001cb60: 6e2e 4372 6561 7465 5265 6163 7469 6f6e  n.CreateReaction
-0001cb70: 5265 7175 6573 7428 7265 7175 6573 7429  Request(request)
-0001cb80: 0a0a 2020 2020 2020 2020 2320 4966 2077  ..        # If w
-0001cb90: 6520 6861 7665 206b 6579 776f 7264 2061  e have keyword a
-0001cba0: 7267 756d 656e 7473 2063 6f72 7265 7370  rguments corresp
-0001cbb0: 6f6e 6469 6e67 2074 6f20 6669 656c 6473  onding to fields
-0001cbc0: 206f 6e20 7468 650a 2020 2020 2020 2020   on the.        
-0001cbd0: 2320 7265 7175 6573 742c 2061 7070 6c79  # request, apply
-0001cbe0: 2074 6865 7365 2e0a 2020 2020 2020 2020   these..        
-0001cbf0: 6966 2070 6172 656e 7420 6973 206e 6f74  if parent is not
-0001cc00: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0001cc10: 2020 2072 6571 7565 7374 2e70 6172 656e     request.paren
-0001cc20: 7420 3d20 7061 7265 6e74 0a20 2020 2020  t = parent.     
-0001cc30: 2020 2069 6620 7265 6163 7469 6f6e 2069     if reaction i
-0001cc40: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0001cc50: 2020 2020 2020 2020 7265 7175 6573 742e          request.
-0001cc60: 7265 6163 7469 6f6e 203d 2072 6561 6374  reaction = react
-0001cc70: 696f 6e0a 0a20 2020 2020 2020 2023 2057  ion..        # W
-0001cc80: 7261 7020 7468 6520 5250 4320 6d65 7468  rap the RPC meth
-0001cc90: 6f64 3b20 7468 6973 2061 6464 7320 7265  od; this adds re
-0001cca0: 7472 7920 616e 6420 7469 6d65 6f75 7420  try and timeout 
-0001ccb0: 696e 666f 726d 6174 696f 6e2c 0a20 2020  information,.   
-0001ccc0: 2020 2020 2023 2061 6e64 2066 7269 656e       # and frien
-0001ccd0: 646c 7920 6572 726f 7220 6861 6e64 6c69  dly error handli
-0001cce0: 6e67 2e0a 2020 2020 2020 2020 7270 6320  ng..        rpc 
-0001ccf0: 3d20 6761 7069 635f 7631 2e6d 6574 686f  = gapic_v1.metho
-0001cd00: 645f 6173 796e 632e 7772 6170 5f6d 6574  d_async.wrap_met
-0001cd10: 686f 6428 0a20 2020 2020 2020 2020 2020  hod(.           
-0001cd20: 2073 656c 662e 5f63 6c69 656e 742e 5f74   self._client._t
-0001cd30: 7261 6e73 706f 7274 2e63 7265 6174 655f  ransport.create_
-0001cd40: 7265 6163 7469 6f6e 2c0a 2020 2020 2020  reaction,.      
-0001cd50: 2020 2020 2020 6465 6661 756c 745f 7265        default_re
-0001cd60: 7472 793d 7265 7472 6965 732e 4173 796e  try=retries.Asyn
-0001cd70: 6352 6574 7279 280a 2020 2020 2020 2020  cRetry(.        
-0001cd80: 2020 2020 2020 2020 696e 6974 6961 6c3d          initial=
-0001cd90: 312e 302c 0a20 2020 2020 2020 2020 2020  1.0,.           
-0001cda0: 2020 2020 206d 6178 696d 756d 3d31 302e       maximum=10.
-0001cdb0: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
-0001cdc0: 2020 206d 756c 7469 706c 6965 723d 312e     multiplier=1.
-0001cdd0: 332c 0a20 2020 2020 2020 2020 2020 2020  3,.             
-0001cde0: 2020 2070 7265 6469 6361 7465 3d72 6574     predicate=ret
-0001cdf0: 7269 6573 2e69 665f 6578 6365 7074 696f  ries.if_exceptio
-0001ce00: 6e5f 7479 7065 280a 2020 2020 2020 2020  n_type(.        
-0001ce10: 2020 2020 2020 2020 2020 2020 636f 7265              core
-0001ce20: 5f65 7863 6570 7469 6f6e 732e 5365 7276  _exceptions.Serv
-0001ce30: 6963 6555 6e61 7661 696c 6162 6c65 2c0a  iceUnavailable,.
-0001ce40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ce50: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0001ce60: 2020 2064 6561 646c 696e 653d 3330 2e30     deadline=30.0
-0001ce70: 2c0a 2020 2020 2020 2020 2020 2020 292c  ,.            ),
-0001ce80: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
-0001ce90: 6175 6c74 5f74 696d 656f 7574 3d33 302e  ault_timeout=30.
-0001cea0: 302c 0a20 2020 2020 2020 2020 2020 2063  0,.            c
-0001ceb0: 6c69 656e 745f 696e 666f 3d44 4546 4155  lient_info=DEFAU
-0001cec0: 4c54 5f43 4c49 454e 545f 494e 464f 2c0a  LT_CLIENT_INFO,.
-0001ced0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0001cee0: 2020 2023 2043 6572 7461 696e 2066 6965     # Certain fie
-0001cef0: 6c64 7320 7368 6f75 6c64 2062 6520 7072  lds should be pr
-0001cf00: 6f76 6964 6564 2077 6974 6869 6e20 7468  ovided within th
-0001cf10: 6520 6d65 7461 6461 7461 2068 6561 6465  e metadata heade
-0001cf20: 723b 0a20 2020 2020 2020 2023 2061 6464  r;.        # add
-0001cf30: 2074 6865 7365 2068 6572 652e 0a20 2020   these here..   
-0001cf40: 2020 2020 206d 6574 6164 6174 6120 3d20       metadata = 
-0001cf50: 7475 706c 6528 6d65 7461 6461 7461 2920  tuple(metadata) 
-0001cf60: 2b20 280a 2020 2020 2020 2020 2020 2020  + (.            
-0001cf70: 6761 7069 635f 7631 2e72 6f75 7469 6e67  gapic_v1.routing
-0001cf80: 5f68 6561 6465 722e 746f 5f67 7270 635f  _header.to_grpc_
-0001cf90: 6d65 7461 6461 7461 2828 2822 7061 7265  metadata((("pare
-0001cfa0: 6e74 222c 2072 6571 7565 7374 2e70 6172  nt", request.par
-0001cfb0: 656e 7429 2c29 292c 0a20 2020 2020 2020  ent),)),.       
-0001cfc0: 2029 0a0a 2020 2020 2020 2020 2320 5661   )..        # Va
-0001cfd0: 6c69 6461 7465 2074 6865 2075 6e69 7665  lidate the unive
-0001cfe0: 7273 6520 646f 6d61 696e 2e0a 2020 2020  rse domain..    
-0001cff0: 2020 2020 7365 6c66 2e5f 636c 6965 6e74      self._client
-0001d000: 2e5f 7661 6c69 6461 7465 5f75 6e69 7665  ._validate_unive
-0001d010: 7273 655f 646f 6d61 696e 2829 0a0a 2020  rse_domain()..  
-0001d020: 2020 2020 2020 2320 5365 6e64 2074 6865        # Send the
-0001d030: 2072 6571 7565 7374 2e0a 2020 2020 2020   request..      
-0001d040: 2020 7265 7370 6f6e 7365 203d 2061 7761    response = awa
-0001d050: 6974 2072 7063 280a 2020 2020 2020 2020  it rpc(.        
-0001d060: 2020 2020 7265 7175 6573 742c 0a20 2020      request,.   
-0001d070: 2020 2020 2020 2020 2072 6574 7279 3d72           retry=r
-0001d080: 6574 7279 2c0a 2020 2020 2020 2020 2020  etry,.          
-0001d090: 2020 7469 6d65 6f75 743d 7469 6d65 6f75    timeout=timeou
-0001d0a0: 742c 0a20 2020 2020 2020 2020 2020 206d  t,.            m
-0001d0b0: 6574 6164 6174 613d 6d65 7461 6461 7461  etadata=metadata
-0001d0c0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-0001d0d0: 2020 2020 2023 2044 6f6e 653b 2072 6574       # Done; ret
-0001d0e0: 7572 6e20 7468 6520 7265 7370 6f6e 7365  urn the response
-0001d0f0: 2e0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0001d100: 2072 6573 706f 6e73 650a 0a20 2020 2061   response..    a
-0001d110: 7379 6e63 2064 6566 206c 6973 745f 7265  sync def list_re
-0001d120: 6163 7469 6f6e 7328 0a20 2020 2020 2020  actions(.       
-0001d130: 2073 656c 662c 0a20 2020 2020 2020 2072   self,.        r
-0001d140: 6571 7565 7374 3a20 4f70 7469 6f6e 616c  equest: Optional
-0001d150: 5b55 6e69 6f6e 5b72 6561 6374 696f 6e2e  [Union[reaction.
-0001d160: 4c69 7374 5265 6163 7469 6f6e 7352 6571  ListReactionsReq
-0001d170: 7565 7374 2c20 6469 6374 5d5d 203d 204e  uest, dict]] = N
-0001d180: 6f6e 652c 0a20 2020 2020 2020 202a 2c0a  one,.        *,.
-0001d190: 2020 2020 2020 2020 7061 7265 6e74 3a20          parent: 
-0001d1a0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-0001d1b0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7265  None,.        re
-0001d1c0: 7472 793a 204f 7074 696f 6e61 6c52 6574  try: OptionalRet
-0001d1d0: 7279 203d 2067 6170 6963 5f76 312e 6d65  ry = gapic_v1.me
-0001d1e0: 7468 6f64 2e44 4546 4155 4c54 2c0a 2020  thod.DEFAULT,.  
-0001d1f0: 2020 2020 2020 7469 6d65 6f75 743a 2055        timeout: U
-0001d200: 6e69 6f6e 5b66 6c6f 6174 2c20 6f62 6a65  nion[float, obje
-0001d210: 6374 5d20 3d20 6761 7069 635f 7631 2e6d  ct] = gapic_v1.m
-0001d220: 6574 686f 642e 4445 4641 554c 542c 0a20  ethod.DEFAULT,. 
-0001d230: 2020 2020 2020 206d 6574 6164 6174 613a         metadata:
-0001d240: 2053 6571 7565 6e63 655b 5475 706c 655b   Sequence[Tuple[
-0001d250: 7374 722c 2073 7472 5d5d 203d 2028 292c  str, str]] = (),
-0001d260: 0a20 2020 2029 202d 3e20 7061 6765 7273  .    ) -> pagers
-0001d270: 2e4c 6973 7452 6561 6374 696f 6e73 4173  .ListReactionsAs
-0001d280: 796e 6350 6167 6572 3a0a 2020 2020 2020  yncPager:.      
-0001d290: 2020 7222 2222 4c69 7374 7320 7265 6163    r"""Lists reac
-0001d2a0: 7469 6f6e 7320 746f 2061 206d 6573 7361  tions to a messa
-0001d2b0: 6765 2e20 466f 7220 616e 2065 7861 6d70  ge. For an examp
-0001d2c0: 6c65 2c20 7365 6520 604c 6973 740a 2020  le, see `List.  
-0001d2d0: 2020 2020 2020 7265 6163 7469 6f6e 7320        reactions 
-0001d2e0: 666f 7220 610a 2020 2020 2020 2020 6d65  for a.        me
-0001d2f0: 7373 6167 6520 3c68 7474 7073 3a2f 2f64  ssage <https://d
-0001d300: 6576 656c 6f70 6572 732e 676f 6f67 6c65  evelopers.google
-0001d310: 2e63 6f6d 2f77 6f72 6b73 7061 6365 2f63  .com/workspace/c
-0001d320: 6861 742f 6c69 7374 2d72 6561 6374 696f  hat/list-reactio
-0001d330: 6e73 3e60 5f5f 2e0a 2020 2020 2020 2020  ns>`__..        
-0001d340: 5265 7175 6972 6573 2060 7573 6572 0a20  Requires `user. 
-0001d350: 2020 2020 2020 2061 7574 6865 6e74 6963         authentic
-0001d360: 6174 696f 6e20 3c68 7474 7073 3a2f 2f64  ation <https://d
-0001d370: 6576 656c 6f70 6572 732e 676f 6f67 6c65  evelopers.google
-0001d380: 2e63 6f6d 2f77 6f72 6b73 7061 6365 2f63  .com/workspace/c
-0001d390: 6861 742f 6175 7468 656e 7469 6361 7465  hat/authenticate
-0001d3a0: 2d61 7574 686f 7269 7a65 2d63 6861 742d  -authorize-chat-
-0001d3b0: 7573 6572 3e60 5f5f 2e0a 0a20 2020 2020  user>`__...     
-0001d3c0: 2020 202e 2e20 636f 6465 2d62 6c6f 636b     .. code-block
-0001d3d0: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
-0001d3e0: 2020 2020 2020 2023 2054 6869 7320 736e         # This sn
-0001d3f0: 6970 7065 7420 6861 7320 6265 656e 2061  ippet has been a
-0001d400: 7574 6f6d 6174 6963 616c 6c79 2067 656e  utomatically gen
-0001d410: 6572 6174 6564 2061 6e64 2073 686f 756c  erated and shoul
-0001d420: 6420 6265 2072 6567 6172 6465 6420 6173  d be regarded as
-0001d430: 2061 0a20 2020 2020 2020 2020 2020 2023   a.            #
-0001d440: 2063 6f64 6520 7465 6d70 6c61 7465 206f   code template o
-0001d450: 6e6c 792e 0a20 2020 2020 2020 2020 2020  nly..           
-0001d460: 2023 2049 7420 7769 6c6c 2072 6571 7569   # It will requi
-0001d470: 7265 206d 6f64 6966 6963 6174 696f 6e73  re modifications
-0001d480: 2074 6f20 776f 726b 3a0a 2020 2020 2020   to work:.      
-0001d490: 2020 2020 2020 2320 2d20 4974 206d 6179        # - It may
-0001d4a0: 2072 6571 7569 7265 2063 6f72 7265 6374   require correct
-0001d4b0: 2f69 6e2d 7261 6e67 6520 7661 6c75 6573  /in-range values
-0001d4c0: 2066 6f72 2072 6571 7565 7374 2069 6e69   for request ini
-0001d4d0: 7469 616c 697a 6174 696f 6e2e 0a20 2020  tialization..   
-0001d4e0: 2020 2020 2020 2020 2023 202d 2049 7420           # - It 
-0001d4f0: 6d61 7920 7265 7175 6972 6520 7370 6563  may require spec
-0001d500: 6966 7969 6e67 2072 6567 696f 6e61 6c20  ifying regional 
-0001d510: 656e 6470 6f69 6e74 7320 7768 656e 2063  endpoints when c
-0001d520: 7265 6174 696e 6720 7468 6520 7365 7276  reating the serv
-0001d530: 6963 650a 2020 2020 2020 2020 2020 2020  ice.            
-0001d540: 2320 2020 636c 6965 6e74 2061 7320 7368  #   client as sh
-0001d550: 6f77 6e20 696e 3a0a 2020 2020 2020 2020  own in:.        
-0001d560: 2020 2020 2320 2020 6874 7470 733a 2f2f      #   https://
-0001d570: 676f 6f67 6c65 6170 6973 2e64 6576 2f70  googleapis.dev/p
-0001d580: 7974 686f 6e2f 676f 6f67 6c65 2d61 7069  ython/google-api
-0001d590: 2d63 6f72 652f 6c61 7465 7374 2f63 6c69  -core/latest/cli
-0001d5a0: 656e 745f 6f70 7469 6f6e 732e 6874 6d6c  ent_options.html
-0001d5b0: 0a20 2020 2020 2020 2020 2020 2066 726f  .            fro
-0001d5c0: 6d20 676f 6f67 6c65 2e61 7070 7320 696d  m google.apps im
-0001d5d0: 706f 7274 2063 6861 745f 7631 0a0a 2020  port chat_v1..  
-0001d5e0: 2020 2020 2020 2020 2020 6173 796e 6320            async 
-0001d5f0: 6465 6620 7361 6d70 6c65 5f6c 6973 745f  def sample_list_
-0001d600: 7265 6163 7469 6f6e 7328 293a 0a20 2020  reactions():.   
-0001d610: 2020 2020 2020 2020 2020 2020 2023 2043               # C
-0001d620: 7265 6174 6520 6120 636c 6965 6e74 0a20  reate a client. 
-0001d630: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0001d640: 6c69 656e 7420 3d20 6368 6174 5f76 312e  lient = chat_v1.
-0001d650: 4368 6174 5365 7276 6963 6541 7379 6e63  ChatServiceAsync
-0001d660: 436c 6965 6e74 2829 0a0a 2020 2020 2020  Client()..      
-0001d670: 2020 2020 2020 2020 2020 2320 496e 6974            # Init
-0001d680: 6961 6c69 7a65 2072 6571 7565 7374 2061  ialize request a
-0001d690: 7267 756d 656e 7428 7329 0a20 2020 2020  rgument(s).     
-0001d6a0: 2020 2020 2020 2020 2020 2072 6571 7565             reque
-0001d6b0: 7374 203d 2063 6861 745f 7631 2e4c 6973  st = chat_v1.Lis
-0001d6c0: 7452 6561 6374 696f 6e73 5265 7175 6573  tReactionsReques
-0001d6d0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-0001d6e0: 2020 2020 2020 2070 6172 656e 743d 2270         parent="p
-0001d6f0: 6172 656e 745f 7661 6c75 6522 2c0a 2020  arent_value",.  
-0001d700: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0001d710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d720: 2023 204d 616b 6520 7468 6520 7265 7175   # Make the requ
-0001d730: 6573 740a 2020 2020 2020 2020 2020 2020  est.            
-0001d740: 2020 2020 7061 6765 5f72 6573 756c 7420      page_result 
-0001d750: 3d20 636c 6965 6e74 2e6c 6973 745f 7265  = client.list_re
-0001d760: 6163 7469 6f6e 7328 7265 7175 6573 743d  actions(request=
-0001d770: 7265 7175 6573 7429 0a0a 2020 2020 2020  request)..      
-0001d780: 2020 2020 2020 2020 2020 2320 4861 6e64            # Hand
-0001d790: 6c65 2074 6865 2072 6573 706f 6e73 650a  le the response.
-0001d7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d7b0: 6173 796e 6320 666f 7220 7265 7370 6f6e  async for respon
-0001d7c0: 7365 2069 6e20 7061 6765 5f72 6573 756c  se in page_resul
-0001d7d0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-0001d7e0: 2020 2020 2020 2070 7269 6e74 2872 6573         print(res
-0001d7f0: 706f 6e73 6529 0a0a 2020 2020 2020 2020  ponse)..        
-0001d800: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-0001d810: 2020 7265 7175 6573 7420 284f 7074 696f    request (Optio
-0001d820: 6e61 6c5b 556e 696f 6e5b 676f 6f67 6c65  nal[Union[google
-0001d830: 2e61 7070 732e 6368 6174 5f76 312e 7479  .apps.chat_v1.ty
-0001d840: 7065 732e 4c69 7374 5265 6163 7469 6f6e  pes.ListReaction
-0001d850: 7352 6571 7565 7374 2c20 6469 6374 5d5d  sRequest, dict]]
-0001d860: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0001d870: 2020 2054 6865 2072 6571 7565 7374 206f     The request o
-0001d880: 626a 6563 742e 204c 6973 7473 2072 6561  bject. Lists rea
-0001d890: 6374 696f 6e73 2074 6f20 6120 6d65 7373  ctions to a mess
-0001d8a0: 6167 652e 0a20 2020 2020 2020 2020 2020  age..           
-0001d8b0: 2070 6172 656e 7420 283a 636c 6173 733a   parent (:class:
-0001d8c0: 6073 7472 6029 3a0a 2020 2020 2020 2020  `str`):.        
-0001d8d0: 2020 2020 2020 2020 5265 7175 6972 6564          Required
-0001d8e0: 2e20 5468 6520 6d65 7373 6167 6520 7573  . The message us
-0001d8f0: 6572 7320 7265 6163 7465 6420 746f 2e0a  ers reacted to..
-0001d900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d910: 2046 6f72 6d61 743a 2060 6073 7061 6365   Format: ``space
-0001d920: 732f 7b73 7061 6365 7d2f 6d65 7373 6167  s/{space}/messag
-0001d930: 6573 2f7b 6d65 7373 6167 657d 6060 0a0a  es/{message}``..
-0001d940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d950: 5468 6973 2063 6f72 7265 7370 6f6e 6473  This corresponds
-0001d960: 2074 6f20 7468 6520 6060 7061 7265 6e74   to the ``parent
-0001d970: 6060 2066 6965 6c64 0a20 2020 2020 2020  `` field.       
-0001d980: 2020 2020 2020 2020 206f 6e20 7468 6520           on the 
-0001d990: 6060 7265 7175 6573 7460 6020 696e 7374  ``request`` inst
-0001d9a0: 616e 6365 3b20 6966 2060 6072 6571 7565  ance; if ``reque
-0001d9b0: 7374 6060 2069 7320 7072 6f76 6964 6564  st`` is provided
-0001d9c0: 2c20 7468 6973 0a20 2020 2020 2020 2020  , this.         
-0001d9d0: 2020 2020 2020 2073 686f 756c 6420 6e6f         should no
-0001d9e0: 7420 6265 2073 6574 2e0a 2020 2020 2020  t be set..      
-0001d9f0: 2020 2020 2020 7265 7472 7920 2867 6f6f        retry (goo
-0001da00: 676c 652e 6170 695f 636f 7265 2e72 6574  gle.api_core.ret
-0001da10: 7279 5f61 7379 6e63 2e41 7379 6e63 5265  ry_async.AsyncRe
-0001da20: 7472 7929 3a20 4465 7369 676e 6174 696f  try): Designatio
-0001da30: 6e20 6f66 2077 6861 7420 6572 726f 7273  n of what errors
-0001da40: 2c20 6966 2061 6e79 2c0a 2020 2020 2020  , if any,.      
-0001da50: 2020 2020 2020 2020 2020 7368 6f75 6c64            should
-0001da60: 2062 6520 7265 7472 6965 642e 0a20 2020   be retried..   
-0001da70: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
-0001da80: 2028 666c 6f61 7429 3a20 5468 6520 7469   (float): The ti
-0001da90: 6d65 6f75 7420 666f 7220 7468 6973 2072  meout for this r
-0001daa0: 6571 7565 7374 2e0a 2020 2020 2020 2020  equest..        
-0001dab0: 2020 2020 6d65 7461 6461 7461 2028 5365      metadata (Se
-0001dac0: 7175 656e 6365 5b54 7570 6c65 5b73 7472  quence[Tuple[str
-0001dad0: 2c20 7374 725d 5d29 3a20 5374 7269 6e67  , str]]): String
-0001dae0: 7320 7768 6963 6820 7368 6f75 6c64 2062  s which should b
-0001daf0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0001db00: 2020 7365 6e74 2061 6c6f 6e67 2077 6974    sent along wit
-0001db10: 6820 7468 6520 7265 7175 6573 7420 6173  h the request as
-0001db20: 206d 6574 6164 6174 612e 0a0a 2020 2020   metadata...    
-0001db30: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-0001db40: 2020 2020 2020 2020 2067 6f6f 676c 652e           google.
-0001db50: 6170 7073 2e63 6861 745f 7631 2e73 6572  apps.chat_v1.ser
-0001db60: 7669 6365 732e 6368 6174 5f73 6572 7669  vices.chat_servi
-0001db70: 6365 2e70 6167 6572 732e 4c69 7374 5265  ce.pagers.ListRe
-0001db80: 6163 7469 6f6e 7341 7379 6e63 5061 6765  actionsAsyncPage
-0001db90: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-0001dba0: 2020 2052 6573 706f 6e73 6520 746f 2061     Response to a
-0001dbb0: 206c 6973 7420 7265 6163 7469 6f6e 7320   list reactions 
-0001dbc0: 7265 7175 6573 742e 0a0a 2020 2020 2020  request...      
-0001dbd0: 2020 2020 2020 2020 2020 4974 6572 6174            Iterat
-0001dbe0: 696e 6720 6f76 6572 2074 6869 7320 6f62  ing over this ob
-0001dbf0: 6a65 6374 2077 696c 6c20 7969 656c 640a  ject will yield.
-0001dc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dc10: 7265 7375 6c74 7320 616e 6420 7265 736f  results and reso
-0001dc20: 6c76 6520 6164 6469 7469 6f6e 616c 2070  lve additional p
-0001dc30: 6167 6573 0a20 2020 2020 2020 2020 2020  ages.           
-0001dc40: 2020 2020 2061 7574 6f6d 6174 6963 616c       automatical
-0001dc50: 6c79 2e0a 0a20 2020 2020 2020 2022 2222  ly...        """
-0001dc60: 0a20 2020 2020 2020 2023 2043 7265 6174  .        # Creat
-0001dc70: 6520 6f72 2063 6f65 7263 6520 6120 7072  e or coerce a pr
-0001dc80: 6f74 6f62 7566 2072 6571 7565 7374 206f  otobuf request o
-0001dc90: 626a 6563 742e 0a20 2020 2020 2020 2023  bject..        #
-0001dca0: 2051 7569 636b 2063 6865 636b 3a20 4966   Quick check: If
-0001dcb0: 2077 6520 676f 7420 6120 7265 7175 6573   we got a reques
-0001dcc0: 7420 6f62 6a65 6374 2c20 7765 2073 686f  t object, we sho
-0001dcd0: 756c 6420 2a6e 6f74 2a20 6861 7665 0a20  uld *not* have. 
-0001dce0: 2020 2020 2020 2023 2067 6f74 7465 6e20         # gotten 
-0001dcf0: 616e 7920 6b65 7977 6f72 6420 6172 6775  any keyword argu
-0001dd00: 6d65 6e74 7320 7468 6174 206d 6170 2074  ments that map t
-0001dd10: 6f20 7468 6520 7265 7175 6573 742e 0a20  o the request.. 
-0001dd20: 2020 2020 2020 2068 6173 5f66 6c61 7474         has_flatt
-0001dd30: 656e 6564 5f70 6172 616d 7320 3d20 616e  ened_params = an
-0001dd40: 7928 5b70 6172 656e 745d 290a 2020 2020  y([parent]).    
-0001dd50: 2020 2020 6966 2072 6571 7565 7374 2069      if request i
-0001dd60: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2068  s not None and h
-0001dd70: 6173 5f66 6c61 7474 656e 6564 5f70 6172  as_flattened_par
-0001dd80: 616d 733a 0a20 2020 2020 2020 2020 2020  ams:.           
-0001dd90: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-0001dda0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-0001ddb0: 2020 2022 4966 2074 6865 2060 7265 7175     "If the `requ
-0001ddc0: 6573 7460 2061 7267 756d 656e 7420 6973  est` argument is
-0001ddd0: 2073 6574 2c20 7468 656e 206e 6f6e 6520   set, then none 
-0001dde0: 6f66 2022 0a20 2020 2020 2020 2020 2020  of ".           
-0001ddf0: 2020 2020 2022 7468 6520 696e 6469 7669       "the indivi
-0001de00: 6475 616c 2066 6965 6c64 2061 7267 756d  dual field argum
-0001de10: 656e 7473 2073 686f 756c 6420 6265 2073  ents should be s
-0001de20: 6574 2e22 0a20 2020 2020 2020 2020 2020  et.".           
-0001de30: 2029 0a0a 2020 2020 2020 2020 7265 7175   )..        requ
-0001de40: 6573 7420 3d20 7265 6163 7469 6f6e 2e4c  est = reaction.L
-0001de50: 6973 7452 6561 6374 696f 6e73 5265 7175  istReactionsRequ
-0001de60: 6573 7428 7265 7175 6573 7429 0a0a 2020  est(request)..  
-0001de70: 2020 2020 2020 2320 4966 2077 6520 6861        # If we ha
-0001de80: 7665 206b 6579 776f 7264 2061 7267 756d  ve keyword argum
-0001de90: 656e 7473 2063 6f72 7265 7370 6f6e 6469  ents correspondi
-0001dea0: 6e67 2074 6f20 6669 656c 6473 206f 6e20  ng to fields on 
-0001deb0: 7468 650a 2020 2020 2020 2020 2320 7265  the.        # re
-0001dec0: 7175 6573 742c 2061 7070 6c79 2074 6865  quest, apply the
-0001ded0: 7365 2e0a 2020 2020 2020 2020 6966 2070  se..        if p
-0001dee0: 6172 656e 7420 6973 206e 6f74 204e 6f6e  arent is not Non
-0001def0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0001df00: 6571 7565 7374 2e70 6172 656e 7420 3d20  equest.parent = 
-0001df10: 7061 7265 6e74 0a0a 2020 2020 2020 2020  parent..        
-0001df20: 2320 5772 6170 2074 6865 2052 5043 206d  # Wrap the RPC m
-0001df30: 6574 686f 643b 2074 6869 7320 6164 6473  ethod; this adds
-0001df40: 2072 6574 7279 2061 6e64 2074 696d 656f   retry and timeo
-0001df50: 7574 2069 6e66 6f72 6d61 7469 6f6e 2c0a  ut information,.
-0001df60: 2020 2020 2020 2020 2320 616e 6420 6672          # and fr
-0001df70: 6965 6e64 6c79 2065 7272 6f72 2068 616e  iendly error han
-0001df80: 646c 696e 672e 0a20 2020 2020 2020 2072  dling..        r
-0001df90: 7063 203d 2067 6170 6963 5f76 312e 6d65  pc = gapic_v1.me
-0001dfa0: 7468 6f64 5f61 7379 6e63 2e77 7261 705f  thod_async.wrap_
-0001dfb0: 6d65 7468 6f64 280a 2020 2020 2020 2020  method(.        
-0001dfc0: 2020 2020 7365 6c66 2e5f 636c 6965 6e74      self._client
-0001dfd0: 2e5f 7472 616e 7370 6f72 742e 6c69 7374  ._transport.list
-0001dfe0: 5f72 6561 6374 696f 6e73 2c0a 2020 2020  _reactions,.    
-0001dff0: 2020 2020 2020 2020 6465 6661 756c 745f          default_
-0001e000: 7265 7472 793d 7265 7472 6965 732e 4173  retry=retries.As
-0001e010: 796e 6352 6574 7279 280a 2020 2020 2020  yncRetry(.      
-0001e020: 2020 2020 2020 2020 2020 696e 6974 6961            initia
-0001e030: 6c3d 312e 302c 0a20 2020 2020 2020 2020  l=1.0,.         
-0001e040: 2020 2020 2020 206d 6178 696d 756d 3d31         maximum=1
-0001e050: 302e 302c 0a20 2020 2020 2020 2020 2020  0.0,.           
-0001e060: 2020 2020 206d 756c 7469 706c 6965 723d       multiplier=
-0001e070: 312e 332c 0a20 2020 2020 2020 2020 2020  1.3,.           
-0001e080: 2020 2020 2070 7265 6469 6361 7465 3d72       predicate=r
-0001e090: 6574 7269 6573 2e69 665f 6578 6365 7074  etries.if_except
-0001e0a0: 696f 6e5f 7479 7065 280a 2020 2020 2020  ion_type(.      
-0001e0b0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0001e0c0: 7265 5f65 7863 6570 7469 6f6e 732e 5365  re_exceptions.Se
-0001e0d0: 7276 6963 6555 6e61 7661 696c 6162 6c65  rviceUnavailable
-0001e0e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001e0f0: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
-0001e100: 2020 2020 2064 6561 646c 696e 653d 3330       deadline=30
-0001e110: 2e30 2c0a 2020 2020 2020 2020 2020 2020  .0,.            
-0001e120: 292c 0a20 2020 2020 2020 2020 2020 2064  ),.            d
-0001e130: 6566 6175 6c74 5f74 696d 656f 7574 3d33  efault_timeout=3
-0001e140: 302e 302c 0a20 2020 2020 2020 2020 2020  0.0,.           
-0001e150: 2063 6c69 656e 745f 696e 666f 3d44 4546   client_info=DEF
-0001e160: 4155 4c54 5f43 4c49 454e 545f 494e 464f  AULT_CLIENT_INFO
-0001e170: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-0001e180: 2020 2020 2023 2043 6572 7461 696e 2066       # Certain f
-0001e190: 6965 6c64 7320 7368 6f75 6c64 2062 6520  ields should be 
-0001e1a0: 7072 6f76 6964 6564 2077 6974 6869 6e20  provided within 
-0001e1b0: 7468 6520 6d65 7461 6461 7461 2068 6561  the metadata hea
-0001e1c0: 6465 723b 0a20 2020 2020 2020 2023 2061  der;.        # a
-0001e1d0: 6464 2074 6865 7365 2068 6572 652e 0a20  dd these here.. 
-0001e1e0: 2020 2020 2020 206d 6574 6164 6174 6120         metadata 
-0001e1f0: 3d20 7475 706c 6528 6d65 7461 6461 7461  = tuple(metadata
-0001e200: 2920 2b20 280a 2020 2020 2020 2020 2020  ) + (.          
-0001e210: 2020 6761 7069 635f 7631 2e72 6f75 7469    gapic_v1.routi
-0001e220: 6e67 5f68 6561 6465 722e 746f 5f67 7270  ng_header.to_grp
-0001e230: 635f 6d65 7461 6461 7461 2828 2822 7061  c_metadata((("pa
-0001e240: 7265 6e74 222c 2072 6571 7565 7374 2e70  rent", request.p
-0001e250: 6172 656e 7429 2c29 292c 0a20 2020 2020  arent),)),.     
-0001e260: 2020 2029 0a0a 2020 2020 2020 2020 2320     )..        # 
-0001e270: 5661 6c69 6461 7465 2074 6865 2075 6e69  Validate the uni
-0001e280: 7665 7273 6520 646f 6d61 696e 2e0a 2020  verse domain..  
-0001e290: 2020 2020 2020 7365 6c66 2e5f 636c 6965        self._clie
-0001e2a0: 6e74 2e5f 7661 6c69 6461 7465 5f75 6e69  nt._validate_uni
-0001e2b0: 7665 7273 655f 646f 6d61 696e 2829 0a0a  verse_domain()..
-0001e2c0: 2020 2020 2020 2020 2320 5365 6e64 2074          # Send t
-0001e2d0: 6865 2072 6571 7565 7374 2e0a 2020 2020  he request..    
-0001e2e0: 2020 2020 7265 7370 6f6e 7365 203d 2061      response = a
-0001e2f0: 7761 6974 2072 7063 280a 2020 2020 2020  wait rpc(.      
-0001e300: 2020 2020 2020 7265 7175 6573 742c 0a20        request,. 
-0001e310: 2020 2020 2020 2020 2020 2072 6574 7279             retry
-0001e320: 3d72 6574 7279 2c0a 2020 2020 2020 2020  =retry,.        
-0001e330: 2020 2020 7469 6d65 6f75 743d 7469 6d65      timeout=time
-0001e340: 6f75 742c 0a20 2020 2020 2020 2020 2020  out,.           
-0001e350: 206d 6574 6164 6174 613d 6d65 7461 6461   metadata=metada
-0001e360: 7461 2c0a 2020 2020 2020 2020 290a 0a20  ta,.        ).. 
-0001e370: 2020 2020 2020 2023 2054 6869 7320 6d65         # This me
-0001e380: 7468 6f64 2069 7320 7061 6765 643b 2077  thod is paged; w
-0001e390: 7261 7020 7468 6520 7265 7370 6f6e 7365  rap the response
-0001e3a0: 2069 6e20 6120 7061 6765 722c 2077 6869   in a pager, whi
-0001e3b0: 6368 2070 726f 7669 6465 730a 2020 2020  ch provides.    
-0001e3c0: 2020 2020 2320 616e 2060 5f5f 6169 7465      # an `__aite
-0001e3d0: 725f 5f60 2063 6f6e 7665 6e69 656e 6365  r__` convenience
-0001e3e0: 206d 6574 686f 642e 0a20 2020 2020 2020   method..       
-0001e3f0: 2072 6573 706f 6e73 6520 3d20 7061 6765   response = page
-0001e400: 7273 2e4c 6973 7452 6561 6374 696f 6e73  rs.ListReactions
-0001e410: 4173 796e 6350 6167 6572 280a 2020 2020  AsyncPager(.    
-0001e420: 2020 2020 2020 2020 6d65 7468 6f64 3d72          method=r
-0001e430: 7063 2c0a 2020 2020 2020 2020 2020 2020  pc,.            
-0001e440: 7265 7175 6573 743d 7265 7175 6573 742c  request=request,
-0001e450: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0001e460: 706f 6e73 653d 7265 7370 6f6e 7365 2c0a  ponse=response,.
-0001e470: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
-0001e480: 6461 7461 3d6d 6574 6164 6174 612c 0a20  data=metadata,. 
-0001e490: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-0001e4a0: 2020 2320 446f 6e65 3b20 7265 7475 726e    # Done; return
-0001e4b0: 2074 6865 2072 6573 706f 6e73 652e 0a20   the response.. 
-0001e4c0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0001e4d0: 7370 6f6e 7365 0a0a 2020 2020 6173 796e  sponse..    asyn
-0001e4e0: 6320 6465 6620 6465 6c65 7465 5f72 6561  c def delete_rea
-0001e4f0: 6374 696f 6e28 0a20 2020 2020 2020 2073  ction(.        s
-0001e500: 656c 662c 0a20 2020 2020 2020 2072 6571  elf,.        req
-0001e510: 7565 7374 3a20 4f70 7469 6f6e 616c 5b55  uest: Optional[U
-0001e520: 6e69 6f6e 5b72 6561 6374 696f 6e2e 4465  nion[reaction.De
-0001e530: 6c65 7465 5265 6163 7469 6f6e 5265 7175  leteReactionRequ
-0001e540: 6573 742c 2064 6963 745d 5d20 3d20 4e6f  est, dict]] = No
-0001e550: 6e65 2c0a 2020 2020 2020 2020 2a2c 0a20  ne,.        *,. 
-0001e560: 2020 2020 2020 206e 616d 653a 204f 7074         name: Opt
-0001e570: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0001e580: 652c 0a20 2020 2020 2020 2072 6574 7279  e,.        retry
-0001e590: 3a20 4f70 7469 6f6e 616c 5265 7472 7920  : OptionalRetry 
-0001e5a0: 3d20 6761 7069 635f 7631 2e6d 6574 686f  = gapic_v1.metho
-0001e5b0: 642e 4445 4641 554c 542c 0a20 2020 2020  d.DEFAULT,.     
-0001e5c0: 2020 2074 696d 656f 7574 3a20 556e 696f     timeout: Unio
-0001e5d0: 6e5b 666c 6f61 742c 206f 626a 6563 745d  n[float, object]
-0001e5e0: 203d 2067 6170 6963 5f76 312e 6d65 7468   = gapic_v1.meth
-0001e5f0: 6f64 2e44 4546 4155 4c54 2c0a 2020 2020  od.DEFAULT,.    
-0001e600: 2020 2020 6d65 7461 6461 7461 3a20 5365      metadata: Se
-0001e610: 7175 656e 6365 5b54 7570 6c65 5b73 7472  quence[Tuple[str
-0001e620: 2c20 7374 725d 5d20 3d20 2829 2c0a 2020  , str]] = (),.  
-0001e630: 2020 2920 2d3e 204e 6f6e 653a 0a20 2020    ) -> None:.   
-0001e640: 2020 2020 2072 2222 2244 656c 6574 6573       r"""Deletes
-0001e650: 2061 2072 6561 6374 696f 6e20 746f 2061   a reaction to a
-0001e660: 206d 6573 7361 6765 2e20 4f6e 6c79 2075   message. Only u
-0001e670: 6e69 636f 6465 2065 6d6f 6a69 7320 6172  nicode emojis ar
-0001e680: 650a 2020 2020 2020 2020 7375 7070 6f72  e.        suppor
-0001e690: 7465 642e 2046 6f72 2061 6e20 6578 616d  ted. For an exam
-0001e6a0: 706c 652c 2073 6565 2060 4465 6c65 7465  ple, see `Delete
-0001e6b0: 2061 0a20 2020 2020 2020 2072 6561 6374   a.        react
-0001e6c0: 696f 6e20 3c68 7474 7073 3a2f 2f64 6576  ion <https://dev
-0001e6d0: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
-0001e6e0: 6f6d 2f77 6f72 6b73 7061 6365 2f63 6861  om/workspace/cha
-0001e6f0: 742f 6465 6c65 7465 2d72 6561 6374 696f  t/delete-reactio
-0001e700: 6e73 3e60 5f5f 2e0a 2020 2020 2020 2020  ns>`__..        
-0001e710: 5265 7175 6972 6573 2060 7573 6572 0a20  Requires `user. 
-0001e720: 2020 2020 2020 2061 7574 6865 6e74 6963         authentic
-0001e730: 6174 696f 6e20 3c68 7474 7073 3a2f 2f64  ation <https://d
-0001e740: 6576 656c 6f70 6572 732e 676f 6f67 6c65  evelopers.google
-0001e750: 2e63 6f6d 2f77 6f72 6b73 7061 6365 2f63  .com/workspace/c
-0001e760: 6861 742f 6175 7468 656e 7469 6361 7465  hat/authenticate
-0001e770: 2d61 7574 686f 7269 7a65 2d63 6861 742d  -authorize-chat-
-0001e780: 7573 6572 3e60 5f5f 2e0a 0a20 2020 2020  user>`__...     
-0001e790: 2020 202e 2e20 636f 6465 2d62 6c6f 636b     .. code-block
-0001e7a0: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
-0001e7b0: 2020 2020 2020 2023 2054 6869 7320 736e         # This sn
-0001e7c0: 6970 7065 7420 6861 7320 6265 656e 2061  ippet has been a
-0001e7d0: 7574 6f6d 6174 6963 616c 6c79 2067 656e  utomatically gen
-0001e7e0: 6572 6174 6564 2061 6e64 2073 686f 756c  erated and shoul
-0001e7f0: 6420 6265 2072 6567 6172 6465 6420 6173  d be regarded as
-0001e800: 2061 0a20 2020 2020 2020 2020 2020 2023   a.            #
-0001e810: 2063 6f64 6520 7465 6d70 6c61 7465 206f   code template o
-0001e820: 6e6c 792e 0a20 2020 2020 2020 2020 2020  nly..           
-0001e830: 2023 2049 7420 7769 6c6c 2072 6571 7569   # It will requi
-0001e840: 7265 206d 6f64 6966 6963 6174 696f 6e73  re modifications
-0001e850: 2074 6f20 776f 726b 3a0a 2020 2020 2020   to work:.      
-0001e860: 2020 2020 2020 2320 2d20 4974 206d 6179        # - It may
-0001e870: 2072 6571 7569 7265 2063 6f72 7265 6374   require correct
-0001e880: 2f69 6e2d 7261 6e67 6520 7661 6c75 6573  /in-range values
-0001e890: 2066 6f72 2072 6571 7565 7374 2069 6e69   for request ini
-0001e8a0: 7469 616c 697a 6174 696f 6e2e 0a20 2020  tialization..   
-0001e8b0: 2020 2020 2020 2020 2023 202d 2049 7420           # - It 
-0001e8c0: 6d61 7920 7265 7175 6972 6520 7370 6563  may require spec
-0001e8d0: 6966 7969 6e67 2072 6567 696f 6e61 6c20  ifying regional 
-0001e8e0: 656e 6470 6f69 6e74 7320 7768 656e 2063  endpoints when c
-0001e8f0: 7265 6174 696e 6720 7468 6520 7365 7276  reating the serv
-0001e900: 6963 650a 2020 2020 2020 2020 2020 2020  ice.            
-0001e910: 2320 2020 636c 6965 6e74 2061 7320 7368  #   client as sh
-0001e920: 6f77 6e20 696e 3a0a 2020 2020 2020 2020  own in:.        
-0001e930: 2020 2020 2320 2020 6874 7470 733a 2f2f      #   https://
-0001e940: 676f 6f67 6c65 6170 6973 2e64 6576 2f70  googleapis.dev/p
-0001e950: 7974 686f 6e2f 676f 6f67 6c65 2d61 7069  ython/google-api
-0001e960: 2d63 6f72 652f 6c61 7465 7374 2f63 6c69  -core/latest/cli
-0001e970: 656e 745f 6f70 7469 6f6e 732e 6874 6d6c  ent_options.html
-0001e980: 0a20 2020 2020 2020 2020 2020 2066 726f  .            fro
-0001e990: 6d20 676f 6f67 6c65 2e61 7070 7320 696d  m google.apps im
-0001e9a0: 706f 7274 2063 6861 745f 7631 0a0a 2020  port chat_v1..  
-0001e9b0: 2020 2020 2020 2020 2020 6173 796e 6320            async 
-0001e9c0: 6465 6620 7361 6d70 6c65 5f64 656c 6574  def sample_delet
-0001e9d0: 655f 7265 6163 7469 6f6e 2829 3a0a 2020  e_reaction():.  
-0001e9e0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0001e9f0: 4372 6561 7465 2061 2063 6c69 656e 740a  Create a client.
-0001ea00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ea10: 636c 6965 6e74 203d 2063 6861 745f 7631  client = chat_v1
-0001ea20: 2e43 6861 7453 6572 7669 6365 4173 796e  .ChatServiceAsyn
-0001ea30: 6343 6c69 656e 7428 290a 0a20 2020 2020  cClient()..     
-0001ea40: 2020 2020 2020 2020 2020 2023 2049 6e69             # Ini
-0001ea50: 7469 616c 697a 6520 7265 7175 6573 7420  tialize request 
-0001ea60: 6172 6775 6d65 6e74 2873 290a 2020 2020  argument(s).    
-0001ea70: 2020 2020 2020 2020 2020 2020 7265 7175              requ
-0001ea80: 6573 7420 3d20 6368 6174 5f76 312e 4465  est = chat_v1.De
-0001ea90: 6c65 7465 5265 6163 7469 6f6e 5265 7175  leteReactionRequ
-0001eaa0: 6573 7428 0a20 2020 2020 2020 2020 2020  est(.           
-0001eab0: 2020 2020 2020 2020 206e 616d 653d 226e           name="n
-0001eac0: 616d 655f 7661 6c75 6522 2c0a 2020 2020  ame_value",.    
-0001ead0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-0001eae0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0001eaf0: 204d 616b 6520 7468 6520 7265 7175 6573   Make the reques
-0001eb00: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-0001eb10: 2020 6177 6169 7420 636c 6965 6e74 2e64    await client.d
-0001eb20: 656c 6574 655f 7265 6163 7469 6f6e 2872  elete_reaction(r
-0001eb30: 6571 7565 7374 3d72 6571 7565 7374 290a  equest=request).
-0001eb40: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-0001eb50: 2020 2020 2020 2020 2020 2072 6571 7565             reque
-0001eb60: 7374 2028 4f70 7469 6f6e 616c 5b55 6e69  st (Optional[Uni
-0001eb70: 6f6e 5b67 6f6f 676c 652e 6170 7073 2e63  on[google.apps.c
-0001eb80: 6861 745f 7631 2e74 7970 6573 2e44 656c  hat_v1.types.Del
-0001eb90: 6574 6552 6561 6374 696f 6e52 6571 7565  eteReactionReque
-0001eba0: 7374 2c20 6469 6374 5d5d 293a 0a20 2020  st, dict]]):.   
-0001ebb0: 2020 2020 2020 2020 2020 2020 2054 6865               The
-0001ebc0: 2072 6571 7565 7374 206f 626a 6563 742e   request object.
-0001ebd0: 2044 656c 6574 6573 2061 2072 6561 6374   Deletes a react
-0001ebe0: 696f 6e20 746f 2061 206d 6573 7361 6765  ion to a message
-0001ebf0: 2e0a 2020 2020 2020 2020 2020 2020 6e61  ..            na
-0001ec00: 6d65 2028 3a63 6c61 7373 3a60 7374 7260  me (:class:`str`
-0001ec10: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0001ec20: 2020 2052 6571 7569 7265 642e 204e 616d     Required. Nam
-0001ec30: 6520 6f66 2074 6865 2072 6561 6374 696f  e of the reactio
-0001ec40: 6e20 746f 2064 656c 6574 652e 0a0a 2020  n to delete...  
-0001ec50: 2020 2020 2020 2020 2020 2020 2020 466f                Fo
-0001ec60: 726d 6174 3a0a 2020 2020 2020 2020 2020  rmat:.          
-0001ec70: 2020 2020 2020 6060 7370 6163 6573 2f7b        ``spaces/{
-0001ec80: 7370 6163 657d 2f6d 6573 7361 6765 732f  space}/messages/
-0001ec90: 7b6d 6573 7361 6765 7d2f 7265 6163 7469  {message}/reacti
-0001eca0: 6f6e 732f 7b72 6561 6374 696f 6e7d 6060  ons/{reaction}``
-0001ecb0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001ecc0: 2020 5468 6973 2063 6f72 7265 7370 6f6e    This correspon
-0001ecd0: 6473 2074 6f20 7468 6520 6060 6e61 6d65  ds to the ``name
-0001ece0: 6060 2066 6965 6c64 0a20 2020 2020 2020  `` field.       
-0001ecf0: 2020 2020 2020 2020 206f 6e20 7468 6520           on the 
-0001ed00: 6060 7265 7175 6573 7460 6020 696e 7374  ``request`` inst
-0001ed10: 616e 6365 3b20 6966 2060 6072 6571 7565  ance; if ``reque
-0001ed20: 7374 6060 2069 7320 7072 6f76 6964 6564  st`` is provided
-0001ed30: 2c20 7468 6973 0a20 2020 2020 2020 2020  , this.         
-0001ed40: 2020 2020 2020 2073 686f 756c 6420 6e6f         should no
-0001ed50: 7420 6265 2073 6574 2e0a 2020 2020 2020  t be set..      
-0001ed60: 2020 2020 2020 7265 7472 7920 2867 6f6f        retry (goo
-0001ed70: 676c 652e 6170 695f 636f 7265 2e72 6574  gle.api_core.ret
-0001ed80: 7279 5f61 7379 6e63 2e41 7379 6e63 5265  ry_async.AsyncRe
-0001ed90: 7472 7929 3a20 4465 7369 676e 6174 696f  try): Designatio
-0001eda0: 6e20 6f66 2077 6861 7420 6572 726f 7273  n of what errors
-0001edb0: 2c20 6966 2061 6e79 2c0a 2020 2020 2020  , if any,.      
-0001edc0: 2020 2020 2020 2020 2020 7368 6f75 6c64            should
-0001edd0: 2062 6520 7265 7472 6965 642e 0a20 2020   be retried..   
-0001ede0: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
-0001edf0: 2028 666c 6f61 7429 3a20 5468 6520 7469   (float): The ti
-0001ee00: 6d65 6f75 7420 666f 7220 7468 6973 2072  meout for this r
-0001ee10: 6571 7565 7374 2e0a 2020 2020 2020 2020  equest..        
-0001ee20: 2020 2020 6d65 7461 6461 7461 2028 5365      metadata (Se
-0001ee30: 7175 656e 6365 5b54 7570 6c65 5b73 7472  quence[Tuple[str
-0001ee40: 2c20 7374 725d 5d29 3a20 5374 7269 6e67  , str]]): String
-0001ee50: 7320 7768 6963 6820 7368 6f75 6c64 2062  s which should b
-0001ee60: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0001ee70: 2020 7365 6e74 2061 6c6f 6e67 2077 6974    sent along wit
-0001ee80: 6820 7468 6520 7265 7175 6573 7420 6173  h the request as
-0001ee90: 206d 6574 6164 6174 612e 0a20 2020 2020   metadata..     
-0001eea0: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
-0001eeb0: 2043 7265 6174 6520 6f72 2063 6f65 7263   Create or coerc
-0001eec0: 6520 6120 7072 6f74 6f62 7566 2072 6571  e a protobuf req
-0001eed0: 7565 7374 206f 626a 6563 742e 0a20 2020  uest object..   
-0001eee0: 2020 2020 2023 2051 7569 636b 2063 6865       # Quick che
-0001eef0: 636b 3a20 4966 2077 6520 676f 7420 6120  ck: If we got a 
-0001ef00: 7265 7175 6573 7420 6f62 6a65 6374 2c20  request object, 
-0001ef10: 7765 2073 686f 756c 6420 2a6e 6f74 2a20  we should *not* 
-0001ef20: 6861 7665 0a20 2020 2020 2020 2023 2067  have.        # g
-0001ef30: 6f74 7465 6e20 616e 7920 6b65 7977 6f72  otten any keywor
-0001ef40: 6420 6172 6775 6d65 6e74 7320 7468 6174  d arguments that
-0001ef50: 206d 6170 2074 6f20 7468 6520 7265 7175   map to the requ
-0001ef60: 6573 742e 0a20 2020 2020 2020 2068 6173  est..        has
-0001ef70: 5f66 6c61 7474 656e 6564 5f70 6172 616d  _flattened_param
-0001ef80: 7320 3d20 616e 7928 5b6e 616d 655d 290a  s = any([name]).
-0001ef90: 2020 2020 2020 2020 6966 2072 6571 7565          if reque
-0001efa0: 7374 2069 7320 6e6f 7420 4e6f 6e65 2061  st is not None a
-0001efb0: 6e64 2068 6173 5f66 6c61 7474 656e 6564  nd has_flattened
-0001efc0: 5f70 6172 616d 733a 0a20 2020 2020 2020  _params:.       
-0001efd0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-0001efe0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-0001eff0: 2020 2020 2020 2022 4966 2074 6865 2060         "If the `
-0001f000: 7265 7175 6573 7460 2061 7267 756d 656e  request` argumen
-0001f010: 7420 6973 2073 6574 2c20 7468 656e 206e  t is set, then n
-0001f020: 6f6e 6520 6f66 2022 0a20 2020 2020 2020  one of ".       
-0001f030: 2020 2020 2020 2020 2022 7468 6520 696e           "the in
-0001f040: 6469 7669 6475 616c 2066 6965 6c64 2061  dividual field a
-0001f050: 7267 756d 656e 7473 2073 686f 756c 6420  rguments should 
-0001f060: 6265 2073 6574 2e22 0a20 2020 2020 2020  be set.".       
-0001f070: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0001f080: 7265 7175 6573 7420 3d20 7265 6163 7469  request = reacti
-0001f090: 6f6e 2e44 656c 6574 6552 6561 6374 696f  on.DeleteReactio
-0001f0a0: 6e52 6571 7565 7374 2872 6571 7565 7374  nRequest(request
-0001f0b0: 290a 0a20 2020 2020 2020 2023 2049 6620  )..        # If 
-0001f0c0: 7765 2068 6176 6520 6b65 7977 6f72 6420  we have keyword 
-0001f0d0: 6172 6775 6d65 6e74 7320 636f 7272 6573  arguments corres
-0001f0e0: 706f 6e64 696e 6720 746f 2066 6965 6c64  ponding to field
-0001f0f0: 7320 6f6e 2074 6865 0a20 2020 2020 2020  s on the.       
-0001f100: 2023 2072 6571 7565 7374 2c20 6170 706c   # request, appl
-0001f110: 7920 7468 6573 652e 0a20 2020 2020 2020  y these..       
-0001f120: 2069 6620 6e61 6d65 2069 7320 6e6f 7420   if name is not 
-0001f130: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0001f140: 2020 7265 7175 6573 742e 6e61 6d65 203d    request.name =
-0001f150: 206e 616d 650a 0a20 2020 2020 2020 2023   name..        #
-0001f160: 2057 7261 7020 7468 6520 5250 4320 6d65   Wrap the RPC me
-0001f170: 7468 6f64 3b20 7468 6973 2061 6464 7320  thod; this adds 
-0001f180: 7265 7472 7920 616e 6420 7469 6d65 6f75  retry and timeou
-0001f190: 7420 696e 666f 726d 6174 696f 6e2c 0a20  t information,. 
-0001f1a0: 2020 2020 2020 2023 2061 6e64 2066 7269         # and fri
-0001f1b0: 656e 646c 7920 6572 726f 7220 6861 6e64  endly error hand
-0001f1c0: 6c69 6e67 2e0a 2020 2020 2020 2020 7270  ling..        rp
-0001f1d0: 6320 3d20 6761 7069 635f 7631 2e6d 6574  c = gapic_v1.met
-0001f1e0: 686f 645f 6173 796e 632e 7772 6170 5f6d  hod_async.wrap_m
-0001f1f0: 6574 686f 6428 0a20 2020 2020 2020 2020  ethod(.         
-0001f200: 2020 2073 656c 662e 5f63 6c69 656e 742e     self._client.
-0001f210: 5f74 7261 6e73 706f 7274 2e64 656c 6574  _transport.delet
-0001f220: 655f 7265 6163 7469 6f6e 2c0a 2020 2020  e_reaction,.    
-0001f230: 2020 2020 2020 2020 6465 6661 756c 745f          default_
-0001f240: 7265 7472 793d 7265 7472 6965 732e 4173  retry=retries.As
-0001f250: 796e 6352 6574 7279 280a 2020 2020 2020  yncRetry(.      
-0001f260: 2020 2020 2020 2020 2020 696e 6974 6961            initia
-0001f270: 6c3d 312e 302c 0a20 2020 2020 2020 2020  l=1.0,.         
-0001f280: 2020 2020 2020 206d 6178 696d 756d 3d31         maximum=1
-0001f290: 302e 302c 0a20 2020 2020 2020 2020 2020  0.0,.           
-0001f2a0: 2020 2020 206d 756c 7469 706c 6965 723d       multiplier=
-0001f2b0: 312e 332c 0a20 2020 2020 2020 2020 2020  1.3,.           
-0001f2c0: 2020 2020 2070 7265 6469 6361 7465 3d72       predicate=r
-0001f2d0: 6574 7269 6573 2e69 665f 6578 6365 7074  etries.if_except
-0001f2e0: 696f 6e5f 7479 7065 280a 2020 2020 2020  ion_type(.      
-0001f2f0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0001f300: 7265 5f65 7863 6570 7469 6f6e 732e 5365  re_exceptions.Se
-0001f310: 7276 6963 6555 6e61 7661 696c 6162 6c65  rviceUnavailable
-0001f320: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001f330: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
-0001f340: 2020 2020 2064 6561 646c 696e 653d 3330       deadline=30
-0001f350: 2e30 2c0a 2020 2020 2020 2020 2020 2020  .0,.            
-0001f360: 292c 0a20 2020 2020 2020 2020 2020 2064  ),.            d
-0001f370: 6566 6175 6c74 5f74 696d 656f 7574 3d33  efault_timeout=3
-0001f380: 302e 302c 0a20 2020 2020 2020 2020 2020  0.0,.           
-0001f390: 2063 6c69 656e 745f 696e 666f 3d44 4546   client_info=DEF
-0001f3a0: 4155 4c54 5f43 4c49 454e 545f 494e 464f  AULT_CLIENT_INFO
-0001f3b0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-0001f3c0: 2020 2020 2023 2043 6572 7461 696e 2066       # Certain f
-0001f3d0: 6965 6c64 7320 7368 6f75 6c64 2062 6520  ields should be 
-0001f3e0: 7072 6f76 6964 6564 2077 6974 6869 6e20  provided within 
-0001f3f0: 7468 6520 6d65 7461 6461 7461 2068 6561  the metadata hea
-0001f400: 6465 723b 0a20 2020 2020 2020 2023 2061  der;.        # a
-0001f410: 6464 2074 6865 7365 2068 6572 652e 0a20  dd these here.. 
-0001f420: 2020 2020 2020 206d 6574 6164 6174 6120         metadata 
-0001f430: 3d20 7475 706c 6528 6d65 7461 6461 7461  = tuple(metadata
-0001f440: 2920 2b20 280a 2020 2020 2020 2020 2020  ) + (.          
-0001f450: 2020 6761 7069 635f 7631 2e72 6f75 7469    gapic_v1.routi
-0001f460: 6e67 5f68 6561 6465 722e 746f 5f67 7270  ng_header.to_grp
-0001f470: 635f 6d65 7461 6461 7461 2828 2822 6e61  c_metadata((("na
-0001f480: 6d65 222c 2072 6571 7565 7374 2e6e 616d  me", request.nam
-0001f490: 6529 2c29 292c 0a20 2020 2020 2020 2029  e),)),.        )
-0001f4a0: 0a0a 2020 2020 2020 2020 2320 5661 6c69  ..        # Vali
-0001f4b0: 6461 7465 2074 6865 2075 6e69 7665 7273  date the univers
-0001f4c0: 6520 646f 6d61 696e 2e0a 2020 2020 2020  e domain..      
-0001f4d0: 2020 7365 6c66 2e5f 636c 6965 6e74 2e5f    self._client._
-0001f4e0: 7661 6c69 6461 7465 5f75 6e69 7665 7273  validate_univers
-0001f4f0: 655f 646f 6d61 696e 2829 0a0a 2020 2020  e_domain()..    
-0001f500: 2020 2020 2320 5365 6e64 2074 6865 2072      # Send the r
-0001f510: 6571 7565 7374 2e0a 2020 2020 2020 2020  equest..        
-0001f520: 6177 6169 7420 7270 6328 0a20 2020 2020  await rpc(.     
-0001f530: 2020 2020 2020 2072 6571 7565 7374 2c0a         request,.
-0001f540: 2020 2020 2020 2020 2020 2020 7265 7472              retr
-0001f550: 793d 7265 7472 792c 0a20 2020 2020 2020  y=retry,.       
-0001f560: 2020 2020 2074 696d 656f 7574 3d74 696d       timeout=tim
-0001f570: 656f 7574 2c0a 2020 2020 2020 2020 2020  eout,.          
-0001f580: 2020 6d65 7461 6461 7461 3d6d 6574 6164    metadata=metad
-0001f590: 6174 612c 0a20 2020 2020 2020 2029 0a0a  ata,.        )..
-0001f5a0: 2020 2020 6173 796e 6320 6465 6620 5f5f      async def __
-0001f5b0: 6165 6e74 6572 5f5f 2873 656c 6629 202d  aenter__(self) -
-0001f5c0: 3e20 2243 6861 7453 6572 7669 6365 4173  > "ChatServiceAs
-0001f5d0: 796e 6343 6c69 656e 7422 3a0a 2020 2020  yncClient":.    
-0001f5e0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-0001f5f0: 0a20 2020 2061 7379 6e63 2064 6566 205f  .    async def _
-0001f600: 5f61 6578 6974 5f5f 2873 656c 662c 2065  _aexit__(self, e
-0001f610: 7863 5f74 7970 652c 2065 7863 2c20 7462  xc_type, exc, tb
-0001f620: 293a 0a20 2020 2020 2020 2061 7761 6974  ):.        await
-0001f630: 2073 656c 662e 7472 616e 7370 6f72 742e   self.transport.
-0001f640: 636c 6f73 6528 290a 0a0a 4445 4641 554c  close()...DEFAUL
-0001f650: 545f 434c 4945 4e54 5f49 4e46 4f20 3d20  T_CLIENT_INFO = 
-0001f660: 6761 7069 635f 7631 2e63 6c69 656e 745f  gapic_v1.client_
-0001f670: 696e 666f 2e43 6c69 656e 7449 6e66 6f28  info.ClientInfo(
-0001f680: 0a20 2020 2067 6170 6963 5f76 6572 7369  .    gapic_versi
-0001f690: 6f6e 3d70 6163 6b61 6765 5f76 6572 7369  on=package_versi
-0001f6a0: 6f6e 2e5f 5f76 6572 7369 6f6e 5f5f 0a29  on.__version__.)
-0001f6b0: 0a0a 0a5f 5f61 6c6c 5f5f 203d 2028 2243  ...__all__ = ("C
-0001f6c0: 6861 7453 6572 7669 6365 4173 796e 6343  hatServiceAsyncC
-0001f6d0: 6c69 656e 7422 2c29 0a                   lient",).
+0001a820: 6e69 6f6e 5b67 635f 6d65 6d62 6572 7368  nion[gc_membersh
+0001a830: 6970 2e55 7064 6174 654d 656d 6265 7273  ip.UpdateMembers
+0001a840: 6869 7052 6571 7565 7374 2c20 6469 6374  hipRequest, dict
+0001a850: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
+0001a860: 2020 202a 2c0a 2020 2020 2020 2020 6d65     *,.        me
+0001a870: 6d62 6572 7368 6970 3a20 4f70 7469 6f6e  mbership: Option
+0001a880: 616c 5b67 635f 6d65 6d62 6572 7368 6970  al[gc_membership
+0001a890: 2e4d 656d 6265 7273 6869 705d 203d 204e  .Membership] = N
+0001a8a0: 6f6e 652c 0a20 2020 2020 2020 2075 7064  one,.        upd
+0001a8b0: 6174 655f 6d61 736b 3a20 4f70 7469 6f6e  ate_mask: Option
+0001a8c0: 616c 5b66 6965 6c64 5f6d 6173 6b5f 7062  al[field_mask_pb
+0001a8d0: 322e 4669 656c 644d 6173 6b5d 203d 204e  2.FieldMask] = N
+0001a8e0: 6f6e 652c 0a20 2020 2020 2020 2072 6574  one,.        ret
+0001a8f0: 7279 3a20 4f70 7469 6f6e 616c 5265 7472  ry: OptionalRetr
+0001a900: 7920 3d20 6761 7069 635f 7631 2e6d 6574  y = gapic_v1.met
+0001a910: 686f 642e 4445 4641 554c 542c 0a20 2020  hod.DEFAULT,.   
+0001a920: 2020 2020 2074 696d 656f 7574 3a20 556e       timeout: Un
+0001a930: 696f 6e5b 666c 6f61 742c 206f 626a 6563  ion[float, objec
+0001a940: 745d 203d 2067 6170 6963 5f76 312e 6d65  t] = gapic_v1.me
+0001a950: 7468 6f64 2e44 4546 4155 4c54 2c0a 2020  thod.DEFAULT,.  
+0001a960: 2020 2020 2020 6d65 7461 6461 7461 3a20        metadata: 
+0001a970: 5365 7175 656e 6365 5b54 7570 6c65 5b73  Sequence[Tuple[s
+0001a980: 7472 2c20 7374 725d 5d20 3d20 2829 2c0a  tr, str]] = (),.
+0001a990: 2020 2020 2920 2d3e 2067 635f 6d65 6d62      ) -> gc_memb
+0001a9a0: 6572 7368 6970 2e4d 656d 6265 7273 6869  ership.Membershi
+0001a9b0: 703a 0a20 2020 2020 2020 2072 2222 2255  p:.        r"""U
+0001a9c0: 7064 6174 6573 2061 206d 656d 6265 7273  pdates a members
+0001a9d0: 6869 702e 2052 6571 7569 7265 7320 6075  hip. Requires `u
+0001a9e0: 7365 720a 2020 2020 2020 2020 6175 7468  ser.        auth
+0001a9f0: 656e 7469 6361 7469 6f6e 203c 6874 7470  entication <http
+0001aa00: 733a 2f2f 6465 7665 6c6f 7065 7273 2e67  s://developers.g
+0001aa10: 6f6f 676c 652e 636f 6d2f 6368 6174 2f61  oogle.com/chat/a
+0001aa20: 7069 2f67 7569 6465 732f 6175 7468 2f75  pi/guides/auth/u
+0001aa30: 7365 7273 3e60 5f5f 2e0a 0a20 2020 2020  sers>`__...     
+0001aa40: 2020 202e 2e20 636f 6465 2d62 6c6f 636b     .. code-block
+0001aa50: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
+0001aa60: 2020 2020 2020 2023 2054 6869 7320 736e         # This sn
+0001aa70: 6970 7065 7420 6861 7320 6265 656e 2061  ippet has been a
+0001aa80: 7574 6f6d 6174 6963 616c 6c79 2067 656e  utomatically gen
+0001aa90: 6572 6174 6564 2061 6e64 2073 686f 756c  erated and shoul
+0001aaa0: 6420 6265 2072 6567 6172 6465 6420 6173  d be regarded as
+0001aab0: 2061 0a20 2020 2020 2020 2020 2020 2023   a.            #
+0001aac0: 2063 6f64 6520 7465 6d70 6c61 7465 206f   code template o
+0001aad0: 6e6c 792e 0a20 2020 2020 2020 2020 2020  nly..           
+0001aae0: 2023 2049 7420 7769 6c6c 2072 6571 7569   # It will requi
+0001aaf0: 7265 206d 6f64 6966 6963 6174 696f 6e73  re modifications
+0001ab00: 2074 6f20 776f 726b 3a0a 2020 2020 2020   to work:.      
+0001ab10: 2020 2020 2020 2320 2d20 4974 206d 6179        # - It may
+0001ab20: 2072 6571 7569 7265 2063 6f72 7265 6374   require correct
+0001ab30: 2f69 6e2d 7261 6e67 6520 7661 6c75 6573  /in-range values
+0001ab40: 2066 6f72 2072 6571 7565 7374 2069 6e69   for request ini
+0001ab50: 7469 616c 697a 6174 696f 6e2e 0a20 2020  tialization..   
+0001ab60: 2020 2020 2020 2020 2023 202d 2049 7420           # - It 
+0001ab70: 6d61 7920 7265 7175 6972 6520 7370 6563  may require spec
+0001ab80: 6966 7969 6e67 2072 6567 696f 6e61 6c20  ifying regional 
+0001ab90: 656e 6470 6f69 6e74 7320 7768 656e 2063  endpoints when c
+0001aba0: 7265 6174 696e 6720 7468 6520 7365 7276  reating the serv
+0001abb0: 6963 650a 2020 2020 2020 2020 2020 2020  ice.            
+0001abc0: 2320 2020 636c 6965 6e74 2061 7320 7368  #   client as sh
+0001abd0: 6f77 6e20 696e 3a0a 2020 2020 2020 2020  own in:.        
+0001abe0: 2020 2020 2320 2020 6874 7470 733a 2f2f      #   https://
+0001abf0: 676f 6f67 6c65 6170 6973 2e64 6576 2f70  googleapis.dev/p
+0001ac00: 7974 686f 6e2f 676f 6f67 6c65 2d61 7069  ython/google-api
+0001ac10: 2d63 6f72 652f 6c61 7465 7374 2f63 6c69  -core/latest/cli
+0001ac20: 656e 745f 6f70 7469 6f6e 732e 6874 6d6c  ent_options.html
+0001ac30: 0a20 2020 2020 2020 2020 2020 2066 726f  .            fro
+0001ac40: 6d20 676f 6f67 6c65 2e61 7070 7320 696d  m google.apps im
+0001ac50: 706f 7274 2063 6861 745f 7631 0a0a 2020  port chat_v1..  
+0001ac60: 2020 2020 2020 2020 2020 6173 796e 6320            async 
+0001ac70: 6465 6620 7361 6d70 6c65 5f75 7064 6174  def sample_updat
+0001ac80: 655f 6d65 6d62 6572 7368 6970 2829 3a0a  e_membership():.
+0001ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aca0: 2320 4372 6561 7465 2061 2063 6c69 656e  # Create a clien
+0001acb0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+0001acc0: 2020 636c 6965 6e74 203d 2063 6861 745f    client = chat_
+0001acd0: 7631 2e43 6861 7453 6572 7669 6365 4173  v1.ChatServiceAs
+0001ace0: 796e 6343 6c69 656e 7428 290a 0a20 2020  yncClient()..   
+0001acf0: 2020 2020 2020 2020 2020 2020 2023 2049               # I
+0001ad00: 6e69 7469 616c 697a 6520 7265 7175 6573  nitialize reques
+0001ad10: 7420 6172 6775 6d65 6e74 2873 290a 2020  t argument(s).  
+0001ad20: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0001ad30: 7175 6573 7420 3d20 6368 6174 5f76 312e  quest = chat_v1.
+0001ad40: 5570 6461 7465 4d65 6d62 6572 7368 6970  UpdateMembership
+0001ad50: 5265 7175 6573 7428 0a20 2020 2020 2020  Request(.       
+0001ad60: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+0001ad70: 2020 2020 2020 2020 2020 2020 2320 4d61              # Ma
+0001ad80: 6b65 2074 6865 2072 6571 7565 7374 0a20  ke the request. 
+0001ad90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0001ada0: 6573 706f 6e73 6520 3d20 6177 6169 7420  esponse = await 
+0001adb0: 636c 6965 6e74 2e75 7064 6174 655f 6d65  client.update_me
+0001adc0: 6d62 6572 7368 6970 2872 6571 7565 7374  mbership(request
+0001add0: 3d72 6571 7565 7374 290a 0a20 2020 2020  =request)..     
+0001ade0: 2020 2020 2020 2020 2020 2023 2048 616e             # Han
+0001adf0: 646c 6520 7468 6520 7265 7370 6f6e 7365  dle the response
+0001ae00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ae10: 2070 7269 6e74 2872 6573 706f 6e73 6529   print(response)
+0001ae20: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+0001ae30: 2020 2020 2020 2020 2020 2020 7265 7175              requ
+0001ae40: 6573 7420 284f 7074 696f 6e61 6c5b 556e  est (Optional[Un
+0001ae50: 696f 6e5b 676f 6f67 6c65 2e61 7070 732e  ion[google.apps.
+0001ae60: 6368 6174 5f76 312e 7479 7065 732e 5570  chat_v1.types.Up
+0001ae70: 6461 7465 4d65 6d62 6572 7368 6970 5265  dateMembershipRe
+0001ae80: 7175 6573 742c 2064 6963 745d 5d29 3a0a  quest, dict]]):.
+0001ae90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aea0: 5468 6520 7265 7175 6573 7420 6f62 6a65  The request obje
+0001aeb0: 6374 2e20 5265 7175 6573 7420 6d65 7373  ct. Request mess
+0001aec0: 6167 6520 666f 7220 7570 6461 7469 6e67  age for updating
+0001aed0: 2061 0a20 2020 2020 2020 2020 2020 2020   a.             
+0001aee0: 2020 206d 656d 6265 7273 6869 702e 0a20     membership.. 
+0001aef0: 2020 2020 2020 2020 2020 206d 656d 6265             membe
+0001af00: 7273 6869 7020 283a 636c 6173 733a 6067  rship (:class:`g
+0001af10: 6f6f 676c 652e 6170 7073 2e63 6861 745f  oogle.apps.chat_
+0001af20: 7631 2e74 7970 6573 2e4d 656d 6265 7273  v1.types.Members
+0001af30: 6869 7060 293a 0a20 2020 2020 2020 2020  hip`):.         
+0001af40: 2020 2020 2020 2052 6571 7569 7265 642e         Required.
+0001af50: 2054 6865 206d 656d 6265 7273 6869 7020   The membership 
+0001af60: 746f 2075 7064 6174 652e 204f 6e6c 7920  to update. Only 
+0001af70: 6669 656c 6473 0a20 2020 2020 2020 2020  fields.         
+0001af80: 2020 2020 2020 2073 7065 6369 6669 6564         specified
+0001af90: 2062 7920 6060 7570 6461 7465 5f6d 6173   by ``update_mas
+0001afa0: 6b60 6020 6172 6520 7570 6461 7465 642e  k`` are updated.
+0001afb0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001afc0: 2020 5468 6973 2063 6f72 7265 7370 6f6e    This correspon
+0001afd0: 6473 2074 6f20 7468 6520 6060 6d65 6d62  ds to the ``memb
+0001afe0: 6572 7368 6970 6060 2066 6965 6c64 0a20  ership`` field. 
+0001aff0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0001b000: 6e20 7468 6520 6060 7265 7175 6573 7460  n the ``request`
+0001b010: 6020 696e 7374 616e 6365 3b20 6966 2060  ` instance; if `
+0001b020: 6072 6571 7565 7374 6060 2069 7320 7072  `request`` is pr
+0001b030: 6f76 6964 6564 2c20 7468 6973 0a20 2020  ovided, this.   
+0001b040: 2020 2020 2020 2020 2020 2020 2073 686f               sho
+0001b050: 756c 6420 6e6f 7420 6265 2073 6574 2e0a  uld not be set..
+0001b060: 2020 2020 2020 2020 2020 2020 7570 6461              upda
+0001b070: 7465 5f6d 6173 6b20 283a 636c 6173 733a  te_mask (:class:
+0001b080: 6067 6f6f 676c 652e 7072 6f74 6f62 7566  `google.protobuf
+0001b090: 2e66 6965 6c64 5f6d 6173 6b5f 7062 322e  .field_mask_pb2.
+0001b0a0: 4669 656c 644d 6173 6b60 293a 0a20 2020  FieldMask`):.   
+0001b0b0: 2020 2020 2020 2020 2020 2020 2052 6571               Req
+0001b0c0: 7569 7265 642e 2054 6865 2066 6965 6c64  uired. The field
+0001b0d0: 2070 6174 6873 2074 6f20 7570 6461 7465   paths to update
+0001b0e0: 2e20 5365 7061 7261 7465 206d 756c 7469  . Separate multi
+0001b0f0: 706c 650a 2020 2020 2020 2020 2020 2020  ple.            
+0001b100: 2020 2020 7661 6c75 6573 2077 6974 6820      values with 
+0001b110: 636f 6d6d 6173 206f 7220 7573 6520 6060  commas or use ``
+0001b120: 2a60 6020 746f 2075 7064 6174 6520 616c  *`` to update al
+0001b130: 6c20 6669 656c 640a 2020 2020 2020 2020  l field.        
+0001b140: 2020 2020 2020 2020 7061 7468 732e 0a0a          paths...
+0001b150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b160: 4375 7272 656e 746c 7920 7375 7070 6f72  Currently suppor
+0001b170: 7465 6420 6669 656c 6420 7061 7468 733a  ted field paths:
+0001b180: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001b190: 2020 2d20 2060 6072 6f6c 6560 600a 0a20    -  ``role``.. 
+0001b1a0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+0001b1b0: 6869 7320 636f 7272 6573 706f 6e64 7320  his corresponds 
+0001b1c0: 746f 2074 6865 2060 6075 7064 6174 655f  to the ``update_
+0001b1d0: 6d61 736b 6060 2066 6965 6c64 0a20 2020  mask`` field.   
+0001b1e0: 2020 2020 2020 2020 2020 2020 206f 6e20               on 
+0001b1f0: 7468 6520 6060 7265 7175 6573 7460 6020  the ``request`` 
+0001b200: 696e 7374 616e 6365 3b20 6966 2060 6072  instance; if ``r
+0001b210: 6571 7565 7374 6060 2069 7320 7072 6f76  equest`` is prov
+0001b220: 6964 6564 2c20 7468 6973 0a20 2020 2020  ided, this.     
+0001b230: 2020 2020 2020 2020 2020 2073 686f 756c             shoul
+0001b240: 6420 6e6f 7420 6265 2073 6574 2e0a 2020  d not be set..  
+0001b250: 2020 2020 2020 2020 2020 7265 7472 7920            retry 
+0001b260: 2867 6f6f 676c 652e 6170 695f 636f 7265  (google.api_core
+0001b270: 2e72 6574 7279 5f61 7379 6e63 2e41 7379  .retry_async.Asy
+0001b280: 6e63 5265 7472 7929 3a20 4465 7369 676e  ncRetry): Design
+0001b290: 6174 696f 6e20 6f66 2077 6861 7420 6572  ation of what er
+0001b2a0: 726f 7273 2c20 6966 2061 6e79 2c0a 2020  rors, if any,.  
+0001b2b0: 2020 2020 2020 2020 2020 2020 2020 7368                sh
+0001b2c0: 6f75 6c64 2062 6520 7265 7472 6965 642e  ould be retried.
+0001b2d0: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
+0001b2e0: 656f 7574 2028 666c 6f61 7429 3a20 5468  eout (float): Th
+0001b2f0: 6520 7469 6d65 6f75 7420 666f 7220 7468  e timeout for th
+0001b300: 6973 2072 6571 7565 7374 2e0a 2020 2020  is request..    
+0001b310: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
+0001b320: 2028 5365 7175 656e 6365 5b54 7570 6c65   (Sequence[Tuple
+0001b330: 5b73 7472 2c20 7374 725d 5d29 3a20 5374  [str, str]]): St
+0001b340: 7269 6e67 7320 7768 6963 6820 7368 6f75  rings which shou
+0001b350: 6c64 2062 650a 2020 2020 2020 2020 2020  ld be.          
+0001b360: 2020 2020 2020 7365 6e74 2061 6c6f 6e67        sent along
+0001b370: 2077 6974 6820 7468 6520 7265 7175 6573   with the reques
+0001b380: 7420 6173 206d 6574 6164 6174 612e 0a0a  t as metadata...
+0001b390: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+0001b3a0: 0a20 2020 2020 2020 2020 2020 2067 6f6f  .            goo
+0001b3b0: 676c 652e 6170 7073 2e63 6861 745f 7631  gle.apps.chat_v1
+0001b3c0: 2e74 7970 6573 2e4d 656d 6265 7273 6869  .types.Membershi
+0001b3d0: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
+0001b3e0: 2020 2052 6570 7265 7365 6e74 7320 6120     Represents a 
+0001b3f0: 6d65 6d62 6572 7368 6970 2072 656c 6174  membership relat
+0001b400: 696f 6e20 696e 0a20 2020 2020 2020 2020  ion in.         
+0001b410: 2020 2020 2020 2047 6f6f 676c 6520 4368         Google Ch
+0001b420: 6174 2c20 7375 6368 2061 7320 7768 6574  at, such as whet
+0001b430: 6865 7220 6120 7573 6572 206f 720a 2020  her a user or.  
+0001b440: 2020 2020 2020 2020 2020 2020 2020 4368                Ch
+0001b450: 6174 2061 7070 2069 7320 696e 7669 7465  at app is invite
+0001b460: 6420 746f 2c20 7061 7274 206f 662c 206f  d to, part of, o
+0001b470: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+0001b480: 2020 6162 7365 6e74 2066 726f 6d20 6120    absent from a 
+0001b490: 7370 6163 652e 0a0a 2020 2020 2020 2020  space...        
+0001b4a0: 2222 220a 2020 2020 2020 2020 2320 4372  """.        # Cr
+0001b4b0: 6561 7465 206f 7220 636f 6572 6365 2061  eate or coerce a
+0001b4c0: 2070 726f 746f 6275 6620 7265 7175 6573   protobuf reques
+0001b4d0: 7420 6f62 6a65 6374 2e0a 2020 2020 2020  t object..      
+0001b4e0: 2020 2320 5175 6963 6b20 6368 6563 6b3a    # Quick check:
+0001b4f0: 2049 6620 7765 2067 6f74 2061 2072 6571   If we got a req
+0001b500: 7565 7374 206f 626a 6563 742c 2077 6520  uest object, we 
+0001b510: 7368 6f75 6c64 202a 6e6f 742a 2068 6176  should *not* hav
+0001b520: 650a 2020 2020 2020 2020 2320 676f 7474  e.        # gott
+0001b530: 656e 2061 6e79 206b 6579 776f 7264 2061  en any keyword a
+0001b540: 7267 756d 656e 7473 2074 6861 7420 6d61  rguments that ma
+0001b550: 7020 746f 2074 6865 2072 6571 7565 7374  p to the request
+0001b560: 2e0a 2020 2020 2020 2020 6861 735f 666c  ..        has_fl
+0001b570: 6174 7465 6e65 645f 7061 7261 6d73 203d  attened_params =
+0001b580: 2061 6e79 285b 6d65 6d62 6572 7368 6970   any([membership
+0001b590: 2c20 7570 6461 7465 5f6d 6173 6b5d 290a  , update_mask]).
+0001b5a0: 2020 2020 2020 2020 6966 2072 6571 7565          if reque
+0001b5b0: 7374 2069 7320 6e6f 7420 4e6f 6e65 2061  st is not None a
+0001b5c0: 6e64 2068 6173 5f66 6c61 7474 656e 6564  nd has_flattened
+0001b5d0: 5f70 6172 616d 733a 0a20 2020 2020 2020  _params:.       
+0001b5e0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+0001b5f0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+0001b600: 2020 2020 2020 2022 4966 2074 6865 2060         "If the `
+0001b610: 7265 7175 6573 7460 2061 7267 756d 656e  request` argumen
+0001b620: 7420 6973 2073 6574 2c20 7468 656e 206e  t is set, then n
+0001b630: 6f6e 6520 6f66 2022 0a20 2020 2020 2020  one of ".       
+0001b640: 2020 2020 2020 2020 2022 7468 6520 696e           "the in
+0001b650: 6469 7669 6475 616c 2066 6965 6c64 2061  dividual field a
+0001b660: 7267 756d 656e 7473 2073 686f 756c 6420  rguments should 
+0001b670: 6265 2073 6574 2e22 0a20 2020 2020 2020  be set.".       
+0001b680: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0001b690: 7265 7175 6573 7420 3d20 6763 5f6d 656d  request = gc_mem
+0001b6a0: 6265 7273 6869 702e 5570 6461 7465 4d65  bership.UpdateMe
+0001b6b0: 6d62 6572 7368 6970 5265 7175 6573 7428  mbershipRequest(
+0001b6c0: 7265 7175 6573 7429 0a0a 2020 2020 2020  request)..      
+0001b6d0: 2020 2320 4966 2077 6520 6861 7665 206b    # If we have k
+0001b6e0: 6579 776f 7264 2061 7267 756d 656e 7473  eyword arguments
+0001b6f0: 2063 6f72 7265 7370 6f6e 6469 6e67 2074   corresponding t
+0001b700: 6f20 6669 656c 6473 206f 6e20 7468 650a  o fields on the.
+0001b710: 2020 2020 2020 2020 2320 7265 7175 6573          # reques
+0001b720: 742c 2061 7070 6c79 2074 6865 7365 2e0a  t, apply these..
+0001b730: 2020 2020 2020 2020 6966 206d 656d 6265          if membe
+0001b740: 7273 6869 7020 6973 206e 6f74 204e 6f6e  rship is not Non
+0001b750: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0001b760: 6571 7565 7374 2e6d 656d 6265 7273 6869  equest.membershi
+0001b770: 7020 3d20 6d65 6d62 6572 7368 6970 0a20  p = membership. 
+0001b780: 2020 2020 2020 2069 6620 7570 6461 7465         if update
+0001b790: 5f6d 6173 6b20 6973 206e 6f74 204e 6f6e  _mask is not Non
+0001b7a0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0001b7b0: 6571 7565 7374 2e75 7064 6174 655f 6d61  equest.update_ma
+0001b7c0: 736b 203d 2075 7064 6174 655f 6d61 736b  sk = update_mask
+0001b7d0: 0a0a 2020 2020 2020 2020 2320 5772 6170  ..        # Wrap
+0001b7e0: 2074 6865 2052 5043 206d 6574 686f 643b   the RPC method;
+0001b7f0: 2074 6869 7320 6164 6473 2072 6574 7279   this adds retry
+0001b800: 2061 6e64 2074 696d 656f 7574 2069 6e66   and timeout inf
+0001b810: 6f72 6d61 7469 6f6e 2c0a 2020 2020 2020  ormation,.      
+0001b820: 2020 2320 616e 6420 6672 6965 6e64 6c79    # and friendly
+0001b830: 2065 7272 6f72 2068 616e 646c 696e 672e   error handling.
+0001b840: 0a20 2020 2020 2020 2072 7063 203d 2067  .        rpc = g
+0001b850: 6170 6963 5f76 312e 6d65 7468 6f64 5f61  apic_v1.method_a
+0001b860: 7379 6e63 2e77 7261 705f 6d65 7468 6f64  sync.wrap_method
+0001b870: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
+0001b880: 6c66 2e5f 636c 6965 6e74 2e5f 7472 616e  lf._client._tran
+0001b890: 7370 6f72 742e 7570 6461 7465 5f6d 656d  sport.update_mem
+0001b8a0: 6265 7273 6869 702c 0a20 2020 2020 2020  bership,.       
+0001b8b0: 2020 2020 2064 6566 6175 6c74 5f72 6574       default_ret
+0001b8c0: 7279 3d72 6574 7269 6573 2e41 7379 6e63  ry=retries.Async
+0001b8d0: 5265 7472 7928 0a20 2020 2020 2020 2020  Retry(.         
+0001b8e0: 2020 2020 2020 2069 6e69 7469 616c 3d31         initial=1
+0001b8f0: 2e30 2c0a 2020 2020 2020 2020 2020 2020  .0,.            
+0001b900: 2020 2020 6d61 7869 6d75 6d3d 3130 2e30      maximum=10.0
+0001b910: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001b920: 2020 6d75 6c74 6970 6c69 6572 3d31 2e33    multiplier=1.3
+0001b930: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001b940: 2020 7072 6564 6963 6174 653d 7265 7472    predicate=retr
+0001b950: 6965 732e 6966 5f65 7863 6570 7469 6f6e  ies.if_exception
+0001b960: 5f74 7970 6528 0a20 2020 2020 2020 2020  _type(.         
+0001b970: 2020 2020 2020 2020 2020 2063 6f72 655f             core_
+0001b980: 6578 6365 7074 696f 6e73 2e53 6572 7669  exceptions.Servi
+0001b990: 6365 556e 6176 6169 6c61 626c 652c 0a20  ceUnavailable,. 
+0001b9a0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0001b9b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001b9c0: 2020 6465 6164 6c69 6e65 3d33 302e 302c    deadline=30.0,
+0001b9d0: 0a20 2020 2020 2020 2020 2020 2029 2c0a  .            ),.
+0001b9e0: 2020 2020 2020 2020 2020 2020 6465 6661              defa
+0001b9f0: 756c 745f 7469 6d65 6f75 743d 3330 2e30  ult_timeout=30.0
+0001ba00: 2c0a 2020 2020 2020 2020 2020 2020 636c  ,.            cl
+0001ba10: 6965 6e74 5f69 6e66 6f3d 4445 4641 554c  ient_info=DEFAUL
+0001ba20: 545f 434c 4945 4e54 5f49 4e46 4f2c 0a20  T_CLIENT_INFO,. 
+0001ba30: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+0001ba40: 2020 2320 4365 7274 6169 6e20 6669 656c    # Certain fiel
+0001ba50: 6473 2073 686f 756c 6420 6265 2070 726f  ds should be pro
+0001ba60: 7669 6465 6420 7769 7468 696e 2074 6865  vided within the
+0001ba70: 206d 6574 6164 6174 6120 6865 6164 6572   metadata header
+0001ba80: 3b0a 2020 2020 2020 2020 2320 6164 6420  ;.        # add 
+0001ba90: 7468 6573 6520 6865 7265 2e0a 2020 2020  these here..    
+0001baa0: 2020 2020 6d65 7461 6461 7461 203d 2074      metadata = t
+0001bab0: 7570 6c65 286d 6574 6164 6174 6129 202b  uple(metadata) +
+0001bac0: 2028 0a20 2020 2020 2020 2020 2020 2067   (.            g
+0001bad0: 6170 6963 5f76 312e 726f 7574 696e 675f  apic_v1.routing_
+0001bae0: 6865 6164 6572 2e74 6f5f 6772 7063 5f6d  header.to_grpc_m
+0001baf0: 6574 6164 6174 6128 0a20 2020 2020 2020  etadata(.       
+0001bb00: 2020 2020 2020 2020 2028 2822 6d65 6d62           (("memb
+0001bb10: 6572 7368 6970 2e6e 616d 6522 2c20 7265  ership.name", re
+0001bb20: 7175 6573 742e 6d65 6d62 6572 7368 6970  quest.membership
+0001bb30: 2e6e 616d 6529 2c29 0a20 2020 2020 2020  .name),).       
+0001bb40: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
+0001bb50: 290a 0a20 2020 2020 2020 2023 2056 616c  )..        # Val
+0001bb60: 6964 6174 6520 7468 6520 756e 6976 6572  idate the univer
+0001bb70: 7365 2064 6f6d 6169 6e2e 0a20 2020 2020  se domain..     
+0001bb80: 2020 2073 656c 662e 5f63 6c69 656e 742e     self._client.
+0001bb90: 5f76 616c 6964 6174 655f 756e 6976 6572  _validate_univer
+0001bba0: 7365 5f64 6f6d 6169 6e28 290a 0a20 2020  se_domain()..   
+0001bbb0: 2020 2020 2023 2053 656e 6420 7468 6520       # Send the 
+0001bbc0: 7265 7175 6573 742e 0a20 2020 2020 2020  request..       
+0001bbd0: 2072 6573 706f 6e73 6520 3d20 6177 6169   response = awai
+0001bbe0: 7420 7270 6328 0a20 2020 2020 2020 2020  t rpc(.         
+0001bbf0: 2020 2072 6571 7565 7374 2c0a 2020 2020     request,.    
+0001bc00: 2020 2020 2020 2020 7265 7472 793d 7265          retry=re
+0001bc10: 7472 792c 0a20 2020 2020 2020 2020 2020  try,.           
+0001bc20: 2074 696d 656f 7574 3d74 696d 656f 7574   timeout=timeout
+0001bc30: 2c0a 2020 2020 2020 2020 2020 2020 6d65  ,.            me
+0001bc40: 7461 6461 7461 3d6d 6574 6164 6174 612c  tadata=metadata,
+0001bc50: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+0001bc60: 2020 2020 2320 446f 6e65 3b20 7265 7475      # Done; retu
+0001bc70: 726e 2074 6865 2072 6573 706f 6e73 652e  rn the response.
+0001bc80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001bc90: 7265 7370 6f6e 7365 0a0a 2020 2020 6173  response..    as
+0001bca0: 796e 6320 6465 6620 6465 6c65 7465 5f6d  ync def delete_m
+0001bcb0: 656d 6265 7273 6869 7028 0a20 2020 2020  embership(.     
+0001bcc0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0001bcd0: 2072 6571 7565 7374 3a20 4f70 7469 6f6e   request: Option
+0001bce0: 616c 5b55 6e69 6f6e 5b6d 656d 6265 7273  al[Union[members
+0001bcf0: 6869 702e 4465 6c65 7465 4d65 6d62 6572  hip.DeleteMember
+0001bd00: 7368 6970 5265 7175 6573 742c 2064 6963  shipRequest, dic
+0001bd10: 745d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  t]] = None,.    
+0001bd20: 2020 2020 2a2c 0a20 2020 2020 2020 206e      *,.        n
+0001bd30: 616d 653a 204f 7074 696f 6e61 6c5b 7374  ame: Optional[st
+0001bd40: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+0001bd50: 2020 2072 6574 7279 3a20 4f70 7469 6f6e     retry: Option
+0001bd60: 616c 5265 7472 7920 3d20 6761 7069 635f  alRetry = gapic_
+0001bd70: 7631 2e6d 6574 686f 642e 4445 4641 554c  v1.method.DEFAUL
+0001bd80: 542c 0a20 2020 2020 2020 2074 696d 656f  T,.        timeo
+0001bd90: 7574 3a20 556e 696f 6e5b 666c 6f61 742c  ut: Union[float,
+0001bda0: 206f 626a 6563 745d 203d 2067 6170 6963   object] = gapic
+0001bdb0: 5f76 312e 6d65 7468 6f64 2e44 4546 4155  _v1.method.DEFAU
+0001bdc0: 4c54 2c0a 2020 2020 2020 2020 6d65 7461  LT,.        meta
+0001bdd0: 6461 7461 3a20 5365 7175 656e 6365 5b54  data: Sequence[T
+0001bde0: 7570 6c65 5b73 7472 2c20 7374 725d 5d20  uple[str, str]] 
+0001bdf0: 3d20 2829 2c0a 2020 2020 2920 2d3e 206d  = (),.    ) -> m
+0001be00: 656d 6265 7273 6869 702e 4d65 6d62 6572  embership.Member
+0001be10: 7368 6970 3a0a 2020 2020 2020 2020 7222  ship:.        r"
+0001be20: 2222 4465 6c65 7465 7320 6120 6d65 6d62  ""Deletes a memb
+0001be30: 6572 7368 6970 2e20 466f 7220 616e 2065  ership. For an e
+0001be40: 7861 6d70 6c65 2c20 7365 6520 6052 656d  xample, see `Rem
+0001be50: 6f76 6520 6120 7573 6572 206f 7220 610a  ove a user or a.
+0001be60: 2020 2020 2020 2020 476f 6f67 6c65 2043          Google C
+0001be70: 6861 7420 6170 7020 6672 6f6d 2061 0a20  hat app from a. 
+0001be80: 2020 2020 2020 2073 7061 6365 203c 6874         space <ht
+0001be90: 7470 733a 2f2f 6465 7665 6c6f 7065 7273  tps://developers
+0001bea0: 2e67 6f6f 676c 652e 636f 6d2f 776f 726b  .google.com/work
+0001beb0: 7370 6163 652f 6368 6174 2f64 656c 6574  space/chat/delet
+0001bec0: 652d 6d65 6d62 6572 733e 605f 5f2e 0a0a  e-members>`__...
+0001bed0: 2020 2020 2020 2020 5265 7175 6972 6573          Requires
+0001bee0: 2060 7573 6572 0a20 2020 2020 2020 2061   `user.        a
+0001bef0: 7574 6865 6e74 6963 6174 696f 6e20 3c68  uthentication <h
+0001bf00: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
+0001bf10: 732e 676f 6f67 6c65 2e63 6f6d 2f77 6f72  s.google.com/wor
+0001bf20: 6b73 7061 6365 2f63 6861 742f 6175 7468  kspace/chat/auth
+0001bf30: 656e 7469 6361 7465 2d61 7574 686f 7269  enticate-authori
+0001bf40: 7a65 2d63 6861 742d 7573 6572 3e60 5f5f  ze-chat-user>`__
+0001bf50: 2e0a 0a20 2020 2020 2020 202e 2e20 636f  ...        .. co
+0001bf60: 6465 2d62 6c6f 636b 3a3a 2070 7974 686f  de-block:: pytho
+0001bf70: 6e0a 0a20 2020 2020 2020 2020 2020 2023  n..            #
+0001bf80: 2054 6869 7320 736e 6970 7065 7420 6861   This snippet ha
+0001bf90: 7320 6265 656e 2061 7574 6f6d 6174 6963  s been automatic
+0001bfa0: 616c 6c79 2067 656e 6572 6174 6564 2061  ally generated a
+0001bfb0: 6e64 2073 686f 756c 6420 6265 2072 6567  nd should be reg
+0001bfc0: 6172 6465 6420 6173 2061 0a20 2020 2020  arded as a.     
+0001bfd0: 2020 2020 2020 2023 2063 6f64 6520 7465         # code te
+0001bfe0: 6d70 6c61 7465 206f 6e6c 792e 0a20 2020  mplate only..   
+0001bff0: 2020 2020 2020 2020 2023 2049 7420 7769           # It wi
+0001c000: 6c6c 2072 6571 7569 7265 206d 6f64 6966  ll require modif
+0001c010: 6963 6174 696f 6e73 2074 6f20 776f 726b  ications to work
+0001c020: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+0001c030: 2d20 4974 206d 6179 2072 6571 7569 7265  - It may require
+0001c040: 2063 6f72 7265 6374 2f69 6e2d 7261 6e67   correct/in-rang
+0001c050: 6520 7661 6c75 6573 2066 6f72 2072 6571  e values for req
+0001c060: 7565 7374 2069 6e69 7469 616c 697a 6174  uest initializat
+0001c070: 696f 6e2e 0a20 2020 2020 2020 2020 2020  ion..           
+0001c080: 2023 202d 2049 7420 6d61 7920 7265 7175   # - It may requ
+0001c090: 6972 6520 7370 6563 6966 7969 6e67 2072  ire specifying r
+0001c0a0: 6567 696f 6e61 6c20 656e 6470 6f69 6e74  egional endpoint
+0001c0b0: 7320 7768 656e 2063 7265 6174 696e 6720  s when creating 
+0001c0c0: 7468 6520 7365 7276 6963 650a 2020 2020  the service.    
+0001c0d0: 2020 2020 2020 2020 2320 2020 636c 6965          #   clie
+0001c0e0: 6e74 2061 7320 7368 6f77 6e20 696e 3a0a  nt as shown in:.
+0001c0f0: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+0001c100: 6874 7470 733a 2f2f 676f 6f67 6c65 6170  https://googleap
+0001c110: 6973 2e64 6576 2f70 7974 686f 6e2f 676f  is.dev/python/go
+0001c120: 6f67 6c65 2d61 7069 2d63 6f72 652f 6c61  ogle-api-core/la
+0001c130: 7465 7374 2f63 6c69 656e 745f 6f70 7469  test/client_opti
+0001c140: 6f6e 732e 6874 6d6c 0a20 2020 2020 2020  ons.html.       
+0001c150: 2020 2020 2066 726f 6d20 676f 6f67 6c65       from google
+0001c160: 2e61 7070 7320 696d 706f 7274 2063 6861  .apps import cha
+0001c170: 745f 7631 0a0a 2020 2020 2020 2020 2020  t_v1..          
+0001c180: 2020 6173 796e 6320 6465 6620 7361 6d70    async def samp
+0001c190: 6c65 5f64 656c 6574 655f 6d65 6d62 6572  le_delete_member
+0001c1a0: 7368 6970 2829 3a0a 2020 2020 2020 2020  ship():.        
+0001c1b0: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
+0001c1c0: 2061 2063 6c69 656e 740a 2020 2020 2020   a client.      
+0001c1d0: 2020 2020 2020 2020 2020 636c 6965 6e74            client
+0001c1e0: 203d 2063 6861 745f 7631 2e43 6861 7453   = chat_v1.ChatS
+0001c1f0: 6572 7669 6365 4173 796e 6343 6c69 656e  erviceAsyncClien
+0001c200: 7428 290a 0a20 2020 2020 2020 2020 2020  t()..           
+0001c210: 2020 2020 2023 2049 6e69 7469 616c 697a       # Initializ
+0001c220: 6520 7265 7175 6573 7420 6172 6775 6d65  e request argume
+0001c230: 6e74 2873 290a 2020 2020 2020 2020 2020  nt(s).          
+0001c240: 2020 2020 2020 7265 7175 6573 7420 3d20        request = 
+0001c250: 6368 6174 5f76 312e 4465 6c65 7465 4d65  chat_v1.DeleteMe
+0001c260: 6d62 6572 7368 6970 5265 7175 6573 7428  mbershipRequest(
+0001c270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c280: 2020 2020 206e 616d 653d 226e 616d 655f       name="name_
+0001c290: 7661 6c75 6522 2c0a 2020 2020 2020 2020  value",.        
+0001c2a0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0001c2b0: 2020 2020 2020 2020 2020 2023 204d 616b             # Mak
+0001c2c0: 6520 7468 6520 7265 7175 6573 740a 2020  e the request.  
+0001c2d0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0001c2e0: 7370 6f6e 7365 203d 2061 7761 6974 2063  sponse = await c
+0001c2f0: 6c69 656e 742e 6465 6c65 7465 5f6d 656d  lient.delete_mem
+0001c300: 6265 7273 6869 7028 7265 7175 6573 743d  bership(request=
+0001c310: 7265 7175 6573 7429 0a0a 2020 2020 2020  request)..      
+0001c320: 2020 2020 2020 2020 2020 2320 4861 6e64            # Hand
+0001c330: 6c65 2074 6865 2072 6573 706f 6e73 650a  le the response.
+0001c340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c350: 7072 696e 7428 7265 7370 6f6e 7365 290a  print(response).
+0001c360: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+0001c370: 2020 2020 2020 2020 2020 2072 6571 7565             reque
+0001c380: 7374 2028 4f70 7469 6f6e 616c 5b55 6e69  st (Optional[Uni
+0001c390: 6f6e 5b67 6f6f 676c 652e 6170 7073 2e63  on[google.apps.c
+0001c3a0: 6861 745f 7631 2e74 7970 6573 2e44 656c  hat_v1.types.Del
+0001c3b0: 6574 654d 656d 6265 7273 6869 7052 6571  eteMembershipReq
+0001c3c0: 7565 7374 2c20 6469 6374 5d5d 293a 0a20  uest, dict]]):. 
+0001c3d0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+0001c3e0: 6865 2072 6571 7565 7374 206f 626a 6563  he request objec
+0001c3f0: 742e 2052 6571 7565 7374 2074 6f20 6465  t. Request to de
+0001c400: 6c65 7465 2061 206d 656d 6265 7273 6869  lete a membershi
+0001c410: 7020 696e 2061 0a20 2020 2020 2020 2020  p in a.         
+0001c420: 2020 2020 2020 2073 7061 6365 2e0a 2020         space..  
+0001c430: 2020 2020 2020 2020 2020 6e61 6d65 2028            name (
+0001c440: 3a63 6c61 7373 3a60 7374 7260 293a 0a20  :class:`str`):. 
+0001c450: 2020 2020 2020 2020 2020 2020 2020 2052                 R
+0001c460: 6571 7569 7265 642e 2052 6573 6f75 7263  equired. Resourc
+0001c470: 6520 6e61 6d65 206f 6620 7468 6520 6d65  e name of the me
+0001c480: 6d62 6572 7368 6970 2074 6f20 6465 6c65  mbership to dele
+0001c490: 7465 2e0a 2020 2020 2020 2020 2020 2020  te..            
+0001c4a0: 2020 2020 4368 6174 2061 7070 7320 6361      Chat apps ca
+0001c4b0: 6e20 6465 6c65 7465 2068 756d 616e 2075  n delete human u
+0001c4c0: 7365 7273 2720 6f72 2074 6865 6972 206f  sers' or their o
+0001c4d0: 776e 0a20 2020 2020 2020 2020 2020 2020  wn.             
+0001c4e0: 2020 206d 656d 6265 7273 6869 7073 2e20     memberships. 
+0001c4f0: 4368 6174 2061 7070 7320 6361 6e27 7420  Chat apps can't 
+0001c500: 6465 6c65 7465 206f 7468 6572 2061 7070  delete other app
+0001c510: 7327 0a20 2020 2020 2020 2020 2020 2020  s'.             
+0001c520: 2020 206d 656d 6265 7273 6869 7073 2e0a     memberships..
+0001c530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c540: 2057 6865 6e20 6465 6c65 7469 6e67 2061   When deleting a
+0001c550: 2068 756d 616e 206d 656d 6265 7273 6869   human membershi
+0001c560: 702c 2072 6571 7569 7265 7320 7468 650a  p, requires the.
+0001c570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c580: 6060 6368 6174 2e6d 656d 6265 7273 6869  ``chat.membershi
+0001c590: 7073 6060 2073 636f 7065 2061 6e64 0a20  ps`` scope and. 
+0001c5a0: 2020 2020 2020 2020 2020 2020 2020 2060                 `
+0001c5b0: 6073 7061 6365 732f 7b73 7061 6365 7d2f  `spaces/{space}/
+0001c5c0: 6d65 6d62 6572 732f 7b6d 656d 6265 727d  members/{member}
+0001c5d0: 6060 2066 6f72 6d61 742e 2059 6f75 2063  `` format. You c
+0001c5e0: 616e 2075 7365 0a20 2020 2020 2020 2020  an use.         
+0001c5f0: 2020 2020 2020 2074 6865 2065 6d61 696c         the email
+0001c600: 2061 7320 616e 2061 6c69 6173 2066 6f72   as an alias for
+0001c610: 2060 607b 6d65 6d62 6572 7d60 602e 2046   ``{member}``. F
+0001c620: 6f72 2065 7861 6d70 6c65 2c0a 2020 2020  or example,.    
+0001c630: 2020 2020 2020 2020 2020 2020 6060 7370              ``sp
+0001c640: 6163 6573 2f7b 7370 6163 657d 2f6d 656d  aces/{space}/mem
+0001c650: 6265 7273 2f65 7861 6d70 6c65 4067 6d61  bers/example@gma
+0001c660: 696c 2e63 6f6d 6060 2077 6865 7265 0a20  il.com`` where. 
+0001c670: 2020 2020 2020 2020 2020 2020 2020 2060                 `
+0001c680: 6065 7861 6d70 6c65 4067 6d61 696c 2e63  `example@gmail.c
+0001c690: 6f6d 6060 2069 7320 7468 6520 656d 6169  om`` is the emai
+0001c6a0: 6c20 6f66 2074 6865 2047 6f6f 676c 6520  l of the Google 
+0001c6b0: 4368 6174 0a20 2020 2020 2020 2020 2020  Chat.           
+0001c6c0: 2020 2020 2075 7365 722e 0a0a 2020 2020       user...    
+0001c6d0: 2020 2020 2020 2020 2020 2020 5768 656e              When
+0001c6e0: 2064 656c 6574 696e 6720 616e 2061 7070   deleting an app
+0001c6f0: 206d 656d 6265 7273 6869 702c 2072 6571   membership, req
+0001c700: 7569 7265 7320 7468 650a 2020 2020 2020  uires the.      
+0001c710: 2020 2020 2020 2020 2020 6060 6368 6174            ``chat
+0001c720: 2e6d 656d 6265 7273 6869 7073 2e61 7070  .memberships.app
+0001c730: 6060 2073 636f 7065 2061 6e64 0a20 2020  `` scope and.   
+0001c740: 2020 2020 2020 2020 2020 2020 2060 6073               ``s
+0001c750: 7061 6365 732f 7b73 7061 6365 7d2f 6d65  paces/{space}/me
+0001c760: 6d62 6572 732f 6170 7060 6020 666f 726d  mbers/app`` form
+0001c770: 6174 2e0a 0a20 2020 2020 2020 2020 2020  at...           
+0001c780: 2020 2020 2046 6f72 6d61 743a 2060 6073       Format: ``s
+0001c790: 7061 6365 732f 7b73 7061 6365 7d2f 6d65  paces/{space}/me
+0001c7a0: 6d62 6572 732f 7b6d 656d 6265 727d 6060  mbers/{member}``
+0001c7b0: 206f 720a 2020 2020 2020 2020 2020 2020   or.            
+0001c7c0: 2020 2020 6060 7370 6163 6573 2f7b 7370      ``spaces/{sp
+0001c7d0: 6163 657d 2f6d 656d 6265 7273 2f61 7070  ace}/members/app
+0001c7e0: 6060 2e0a 0a20 2020 2020 2020 2020 2020  ``...           
+0001c7f0: 2020 2020 2054 6869 7320 636f 7272 6573       This corres
+0001c800: 706f 6e64 7320 746f 2074 6865 2060 606e  ponds to the ``n
+0001c810: 616d 6560 6020 6669 656c 640a 2020 2020  ame`` field.    
+0001c820: 2020 2020 2020 2020 2020 2020 6f6e 2074              on t
+0001c830: 6865 2060 6072 6571 7565 7374 6060 2069  he ``request`` i
+0001c840: 6e73 7461 6e63 653b 2069 6620 6060 7265  nstance; if ``re
+0001c850: 7175 6573 7460 6020 6973 2070 726f 7669  quest`` is provi
+0001c860: 6465 642c 2074 6869 730a 2020 2020 2020  ded, this.      
+0001c870: 2020 2020 2020 2020 2020 7368 6f75 6c64            should
+0001c880: 206e 6f74 2062 6520 7365 742e 0a20 2020   not be set..   
+0001c890: 2020 2020 2020 2020 2072 6574 7279 2028           retry (
+0001c8a0: 676f 6f67 6c65 2e61 7069 5f63 6f72 652e  google.api_core.
+0001c8b0: 7265 7472 795f 6173 796e 632e 4173 796e  retry_async.Asyn
+0001c8c0: 6352 6574 7279 293a 2044 6573 6967 6e61  cRetry): Designa
+0001c8d0: 7469 6f6e 206f 6620 7768 6174 2065 7272  tion of what err
+0001c8e0: 6f72 732c 2069 6620 616e 792c 0a20 2020  ors, if any,.   
+0001c8f0: 2020 2020 2020 2020 2020 2020 2073 686f               sho
+0001c900: 756c 6420 6265 2072 6574 7269 6564 2e0a  uld be retried..
+0001c910: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+0001c920: 6f75 7420 2866 6c6f 6174 293a 2054 6865  out (float): The
+0001c930: 2074 696d 656f 7574 2066 6f72 2074 6869   timeout for thi
+0001c940: 7320 7265 7175 6573 742e 0a20 2020 2020  s request..     
+0001c950: 2020 2020 2020 206d 6574 6164 6174 6120         metadata 
+0001c960: 2853 6571 7565 6e63 655b 5475 706c 655b  (Sequence[Tuple[
+0001c970: 7374 722c 2073 7472 5d5d 293a 2053 7472  str, str]]): Str
+0001c980: 696e 6773 2077 6869 6368 2073 686f 756c  ings which shoul
+0001c990: 6420 6265 0a20 2020 2020 2020 2020 2020  d be.           
+0001c9a0: 2020 2020 2073 656e 7420 616c 6f6e 6720       sent along 
+0001c9b0: 7769 7468 2074 6865 2072 6571 7565 7374  with the request
+0001c9c0: 2061 7320 6d65 7461 6461 7461 2e0a 0a20   as metadata... 
+0001c9d0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+0001c9e0: 2020 2020 2020 2020 2020 2020 676f 6f67              goog
+0001c9f0: 6c65 2e61 7070 732e 6368 6174 5f76 312e  le.apps.chat_v1.
+0001ca00: 7479 7065 732e 4d65 6d62 6572 7368 6970  types.Membership
+0001ca10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001ca20: 2020 5265 7072 6573 656e 7473 2061 206d    Represents a m
+0001ca30: 656d 6265 7273 6869 7020 7265 6c61 7469  embership relati
+0001ca40: 6f6e 2069 6e0a 2020 2020 2020 2020 2020  on in.          
+0001ca50: 2020 2020 2020 476f 6f67 6c65 2043 6861        Google Cha
+0001ca60: 742c 2073 7563 6820 6173 2077 6865 7468  t, such as wheth
+0001ca70: 6572 2061 2075 7365 7220 6f72 0a20 2020  er a user or.   
+0001ca80: 2020 2020 2020 2020 2020 2020 2043 6861               Cha
+0001ca90: 7420 6170 7020 6973 2069 6e76 6974 6564  t app is invited
+0001caa0: 2074 6f2c 2070 6172 7420 6f66 2c20 6f72   to, part of, or
+0001cab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001cac0: 2061 6273 656e 7420 6672 6f6d 2061 2073   absent from a s
+0001cad0: 7061 6365 2e0a 0a20 2020 2020 2020 2022  pace...        "
+0001cae0: 2222 0a20 2020 2020 2020 2023 2043 7265  "".        # Cre
+0001caf0: 6174 6520 6f72 2063 6f65 7263 6520 6120  ate or coerce a 
+0001cb00: 7072 6f74 6f62 7566 2072 6571 7565 7374  protobuf request
+0001cb10: 206f 626a 6563 742e 0a20 2020 2020 2020   object..       
+0001cb20: 2023 2051 7569 636b 2063 6865 636b 3a20   # Quick check: 
+0001cb30: 4966 2077 6520 676f 7420 6120 7265 7175  If we got a requ
+0001cb40: 6573 7420 6f62 6a65 6374 2c20 7765 2073  est object, we s
+0001cb50: 686f 756c 6420 2a6e 6f74 2a20 6861 7665  hould *not* have
+0001cb60: 0a20 2020 2020 2020 2023 2067 6f74 7465  .        # gotte
+0001cb70: 6e20 616e 7920 6b65 7977 6f72 6420 6172  n any keyword ar
+0001cb80: 6775 6d65 6e74 7320 7468 6174 206d 6170  guments that map
+0001cb90: 2074 6f20 7468 6520 7265 7175 6573 742e   to the request.
+0001cba0: 0a20 2020 2020 2020 2068 6173 5f66 6c61  .        has_fla
+0001cbb0: 7474 656e 6564 5f70 6172 616d 7320 3d20  ttened_params = 
+0001cbc0: 616e 7928 5b6e 616d 655d 290a 2020 2020  any([name]).    
+0001cbd0: 2020 2020 6966 2072 6571 7565 7374 2069      if request i
+0001cbe0: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2068  s not None and h
+0001cbf0: 6173 5f66 6c61 7474 656e 6564 5f70 6172  as_flattened_par
+0001cc00: 616d 733a 0a20 2020 2020 2020 2020 2020  ams:.           
+0001cc10: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+0001cc20: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+0001cc30: 2020 2022 4966 2074 6865 2060 7265 7175     "If the `requ
+0001cc40: 6573 7460 2061 7267 756d 656e 7420 6973  est` argument is
+0001cc50: 2073 6574 2c20 7468 656e 206e 6f6e 6520   set, then none 
+0001cc60: 6f66 2022 0a20 2020 2020 2020 2020 2020  of ".           
+0001cc70: 2020 2020 2022 7468 6520 696e 6469 7669       "the indivi
+0001cc80: 6475 616c 2066 6965 6c64 2061 7267 756d  dual field argum
+0001cc90: 656e 7473 2073 686f 756c 6420 6265 2073  ents should be s
+0001cca0: 6574 2e22 0a20 2020 2020 2020 2020 2020  et.".           
+0001ccb0: 2029 0a0a 2020 2020 2020 2020 7265 7175   )..        requ
+0001ccc0: 6573 7420 3d20 6d65 6d62 6572 7368 6970  est = membership
+0001ccd0: 2e44 656c 6574 654d 656d 6265 7273 6869  .DeleteMembershi
+0001cce0: 7052 6571 7565 7374 2872 6571 7565 7374  pRequest(request
+0001ccf0: 290a 0a20 2020 2020 2020 2023 2049 6620  )..        # If 
+0001cd00: 7765 2068 6176 6520 6b65 7977 6f72 6420  we have keyword 
+0001cd10: 6172 6775 6d65 6e74 7320 636f 7272 6573  arguments corres
+0001cd20: 706f 6e64 696e 6720 746f 2066 6965 6c64  ponding to field
+0001cd30: 7320 6f6e 2074 6865 0a20 2020 2020 2020  s on the.       
+0001cd40: 2023 2072 6571 7565 7374 2c20 6170 706c   # request, appl
+0001cd50: 7920 7468 6573 652e 0a20 2020 2020 2020  y these..       
+0001cd60: 2069 6620 6e61 6d65 2069 7320 6e6f 7420   if name is not 
+0001cd70: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0001cd80: 2020 7265 7175 6573 742e 6e61 6d65 203d    request.name =
+0001cd90: 206e 616d 650a 0a20 2020 2020 2020 2023   name..        #
+0001cda0: 2057 7261 7020 7468 6520 5250 4320 6d65   Wrap the RPC me
+0001cdb0: 7468 6f64 3b20 7468 6973 2061 6464 7320  thod; this adds 
+0001cdc0: 7265 7472 7920 616e 6420 7469 6d65 6f75  retry and timeou
+0001cdd0: 7420 696e 666f 726d 6174 696f 6e2c 0a20  t information,. 
+0001cde0: 2020 2020 2020 2023 2061 6e64 2066 7269         # and fri
+0001cdf0: 656e 646c 7920 6572 726f 7220 6861 6e64  endly error hand
+0001ce00: 6c69 6e67 2e0a 2020 2020 2020 2020 7270  ling..        rp
+0001ce10: 6320 3d20 6761 7069 635f 7631 2e6d 6574  c = gapic_v1.met
+0001ce20: 686f 645f 6173 796e 632e 7772 6170 5f6d  hod_async.wrap_m
+0001ce30: 6574 686f 6428 0a20 2020 2020 2020 2020  ethod(.         
+0001ce40: 2020 2073 656c 662e 5f63 6c69 656e 742e     self._client.
+0001ce50: 5f74 7261 6e73 706f 7274 2e64 656c 6574  _transport.delet
+0001ce60: 655f 6d65 6d62 6572 7368 6970 2c0a 2020  e_membership,.  
+0001ce70: 2020 2020 2020 2020 2020 6465 6661 756c            defaul
+0001ce80: 745f 7265 7472 793d 7265 7472 6965 732e  t_retry=retries.
+0001ce90: 4173 796e 6352 6574 7279 280a 2020 2020  AsyncRetry(.    
+0001cea0: 2020 2020 2020 2020 2020 2020 696e 6974              init
+0001ceb0: 6961 6c3d 312e 302c 0a20 2020 2020 2020  ial=1.0,.       
+0001cec0: 2020 2020 2020 2020 206d 6178 696d 756d           maximum
+0001ced0: 3d31 302e 302c 0a20 2020 2020 2020 2020  =10.0,.         
+0001cee0: 2020 2020 2020 206d 756c 7469 706c 6965         multiplie
+0001cef0: 723d 312e 332c 0a20 2020 2020 2020 2020  r=1.3,.         
+0001cf00: 2020 2020 2020 2070 7265 6469 6361 7465         predicate
+0001cf10: 3d72 6574 7269 6573 2e69 665f 6578 6365  =retries.if_exce
+0001cf20: 7074 696f 6e5f 7479 7065 280a 2020 2020  ption_type(.    
+0001cf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cf40: 636f 7265 5f65 7863 6570 7469 6f6e 732e  core_exceptions.
+0001cf50: 5365 7276 6963 6555 6e61 7661 696c 6162  ServiceUnavailab
+0001cf60: 6c65 2c0a 2020 2020 2020 2020 2020 2020  le,.            
+0001cf70: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+0001cf80: 2020 2020 2020 2064 6561 646c 696e 653d         deadline=
+0001cf90: 3330 2e30 2c0a 2020 2020 2020 2020 2020  30.0,.          
+0001cfa0: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
+0001cfb0: 2064 6566 6175 6c74 5f74 696d 656f 7574   default_timeout
+0001cfc0: 3d33 302e 302c 0a20 2020 2020 2020 2020  =30.0,.         
+0001cfd0: 2020 2063 6c69 656e 745f 696e 666f 3d44     client_info=D
+0001cfe0: 4546 4155 4c54 5f43 4c49 454e 545f 494e  EFAULT_CLIENT_IN
+0001cff0: 464f 2c0a 2020 2020 2020 2020 290a 0a20  FO,.        ).. 
+0001d000: 2020 2020 2020 2023 2043 6572 7461 696e         # Certain
+0001d010: 2066 6965 6c64 7320 7368 6f75 6c64 2062   fields should b
+0001d020: 6520 7072 6f76 6964 6564 2077 6974 6869  e provided withi
+0001d030: 6e20 7468 6520 6d65 7461 6461 7461 2068  n the metadata h
+0001d040: 6561 6465 723b 0a20 2020 2020 2020 2023  eader;.        #
+0001d050: 2061 6464 2074 6865 7365 2068 6572 652e   add these here.
+0001d060: 0a20 2020 2020 2020 206d 6574 6164 6174  .        metadat
+0001d070: 6120 3d20 7475 706c 6528 6d65 7461 6461  a = tuple(metada
+0001d080: 7461 2920 2b20 280a 2020 2020 2020 2020  ta) + (.        
+0001d090: 2020 2020 6761 7069 635f 7631 2e72 6f75      gapic_v1.rou
+0001d0a0: 7469 6e67 5f68 6561 6465 722e 746f 5f67  ting_header.to_g
+0001d0b0: 7270 635f 6d65 7461 6461 7461 2828 2822  rpc_metadata((("
+0001d0c0: 6e61 6d65 222c 2072 6571 7565 7374 2e6e  name", request.n
+0001d0d0: 616d 6529 2c29 292c 0a20 2020 2020 2020  ame),)),.       
+0001d0e0: 2029 0a0a 2020 2020 2020 2020 2320 5661   )..        # Va
+0001d0f0: 6c69 6461 7465 2074 6865 2075 6e69 7665  lidate the unive
+0001d100: 7273 6520 646f 6d61 696e 2e0a 2020 2020  rse domain..    
+0001d110: 2020 2020 7365 6c66 2e5f 636c 6965 6e74      self._client
+0001d120: 2e5f 7661 6c69 6461 7465 5f75 6e69 7665  ._validate_unive
+0001d130: 7273 655f 646f 6d61 696e 2829 0a0a 2020  rse_domain()..  
+0001d140: 2020 2020 2020 2320 5365 6e64 2074 6865        # Send the
+0001d150: 2072 6571 7565 7374 2e0a 2020 2020 2020   request..      
+0001d160: 2020 7265 7370 6f6e 7365 203d 2061 7761    response = awa
+0001d170: 6974 2072 7063 280a 2020 2020 2020 2020  it rpc(.        
+0001d180: 2020 2020 7265 7175 6573 742c 0a20 2020      request,.   
+0001d190: 2020 2020 2020 2020 2072 6574 7279 3d72           retry=r
+0001d1a0: 6574 7279 2c0a 2020 2020 2020 2020 2020  etry,.          
+0001d1b0: 2020 7469 6d65 6f75 743d 7469 6d65 6f75    timeout=timeou
+0001d1c0: 742c 0a20 2020 2020 2020 2020 2020 206d  t,.            m
+0001d1d0: 6574 6164 6174 613d 6d65 7461 6461 7461  etadata=metadata
+0001d1e0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+0001d1f0: 2020 2020 2023 2044 6f6e 653b 2072 6574       # Done; ret
+0001d200: 7572 6e20 7468 6520 7265 7370 6f6e 7365  urn the response
+0001d210: 2e0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0001d220: 2072 6573 706f 6e73 650a 0a20 2020 2061   response..    a
+0001d230: 7379 6e63 2064 6566 2063 7265 6174 655f  sync def create_
+0001d240: 7265 6163 7469 6f6e 280a 2020 2020 2020  reaction(.      
+0001d250: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+0001d260: 7265 7175 6573 743a 204f 7074 696f 6e61  request: Optiona
+0001d270: 6c5b 556e 696f 6e5b 6763 5f72 6561 6374  l[Union[gc_react
+0001d280: 696f 6e2e 4372 6561 7465 5265 6163 7469  ion.CreateReacti
+0001d290: 6f6e 5265 7175 6573 742c 2064 6963 745d  onRequest, dict]
+0001d2a0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0001d2b0: 2020 2a2c 0a20 2020 2020 2020 2070 6172    *,.        par
+0001d2c0: 656e 743a 204f 7074 696f 6e61 6c5b 7374  ent: Optional[st
+0001d2d0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+0001d2e0: 2020 2072 6561 6374 696f 6e3a 204f 7074     reaction: Opt
+0001d2f0: 696f 6e61 6c5b 6763 5f72 6561 6374 696f  ional[gc_reactio
+0001d300: 6e2e 5265 6163 7469 6f6e 5d20 3d20 4e6f  n.Reaction] = No
+0001d310: 6e65 2c0a 2020 2020 2020 2020 7265 7472  ne,.        retr
+0001d320: 793a 204f 7074 696f 6e61 6c52 6574 7279  y: OptionalRetry
+0001d330: 203d 2067 6170 6963 5f76 312e 6d65 7468   = gapic_v1.meth
+0001d340: 6f64 2e44 4546 4155 4c54 2c0a 2020 2020  od.DEFAULT,.    
+0001d350: 2020 2020 7469 6d65 6f75 743a 2055 6e69      timeout: Uni
+0001d360: 6f6e 5b66 6c6f 6174 2c20 6f62 6a65 6374  on[float, object
+0001d370: 5d20 3d20 6761 7069 635f 7631 2e6d 6574  ] = gapic_v1.met
+0001d380: 686f 642e 4445 4641 554c 542c 0a20 2020  hod.DEFAULT,.   
+0001d390: 2020 2020 206d 6574 6164 6174 613a 2053       metadata: S
+0001d3a0: 6571 7565 6e63 655b 5475 706c 655b 7374  equence[Tuple[st
+0001d3b0: 722c 2073 7472 5d5d 203d 2028 292c 0a20  r, str]] = (),. 
+0001d3c0: 2020 2029 202d 3e20 6763 5f72 6561 6374     ) -> gc_react
+0001d3d0: 696f 6e2e 5265 6163 7469 6f6e 3a0a 2020  ion.Reaction:.  
+0001d3e0: 2020 2020 2020 7222 2222 4372 6561 7465        r"""Create
+0001d3f0: 7320 6120 7265 6163 7469 6f6e 2061 6e64  s a reaction and
+0001d400: 2061 6464 7320 6974 2074 6f20 6120 6d65   adds it to a me
+0001d410: 7373 6167 652e 204f 6e6c 7920 756e 6963  ssage. Only unic
+0001d420: 6f64 6520 656d 6f6a 6973 0a20 2020 2020  ode emojis.     
+0001d430: 2020 2061 7265 2073 7570 706f 7274 6564     are supported
+0001d440: 2e20 466f 7220 616e 2065 7861 6d70 6c65  . For an example
+0001d450: 2c20 7365 6520 6041 6464 2061 2072 6561  , see `Add a rea
+0001d460: 6374 696f 6e20 746f 2061 0a20 2020 2020  ction to a.     
+0001d470: 2020 206d 6573 7361 6765 203c 6874 7470     message <http
+0001d480: 733a 2f2f 6465 7665 6c6f 7065 7273 2e67  s://developers.g
+0001d490: 6f6f 676c 652e 636f 6d2f 776f 726b 7370  oogle.com/worksp
+0001d4a0: 6163 652f 6368 6174 2f63 7265 6174 652d  ace/chat/create-
+0001d4b0: 7265 6163 7469 6f6e 733e 605f 5f2e 0a20  reactions>`__.. 
+0001d4c0: 2020 2020 2020 2052 6571 7569 7265 7320         Requires 
+0001d4d0: 6075 7365 720a 2020 2020 2020 2020 6175  `user.        au
+0001d4e0: 7468 656e 7469 6361 7469 6f6e 203c 6874  thentication <ht
+0001d4f0: 7470 733a 2f2f 6465 7665 6c6f 7065 7273  tps://developers
+0001d500: 2e67 6f6f 676c 652e 636f 6d2f 776f 726b  .google.com/work
+0001d510: 7370 6163 652f 6368 6174 2f61 7574 6865  space/chat/authe
+0001d520: 6e74 6963 6174 652d 6175 7468 6f72 697a  nticate-authoriz
+0001d530: 652d 6368 6174 2d75 7365 723e 605f 5f2e  e-chat-user>`__.
+0001d540: 0a0a 2020 2020 2020 2020 2e2e 2063 6f64  ..        .. cod
+0001d550: 652d 626c 6f63 6b3a 3a20 7079 7468 6f6e  e-block:: python
+0001d560: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0001d570: 5468 6973 2073 6e69 7070 6574 2068 6173  This snippet has
+0001d580: 2062 6565 6e20 6175 746f 6d61 7469 6361   been automatica
+0001d590: 6c6c 7920 6765 6e65 7261 7465 6420 616e  lly generated an
+0001d5a0: 6420 7368 6f75 6c64 2062 6520 7265 6761  d should be rega
+0001d5b0: 7264 6564 2061 7320 610a 2020 2020 2020  rded as a.      
+0001d5c0: 2020 2020 2020 2320 636f 6465 2074 656d        # code tem
+0001d5d0: 706c 6174 6520 6f6e 6c79 2e0a 2020 2020  plate only..    
+0001d5e0: 2020 2020 2020 2020 2320 4974 2077 696c          # It wil
+0001d5f0: 6c20 7265 7175 6972 6520 6d6f 6469 6669  l require modifi
+0001d600: 6361 7469 6f6e 7320 746f 2077 6f72 6b3a  cations to work:
+0001d610: 0a20 2020 2020 2020 2020 2020 2023 202d  .            # -
+0001d620: 2049 7420 6d61 7920 7265 7175 6972 6520   It may require 
+0001d630: 636f 7272 6563 742f 696e 2d72 616e 6765  correct/in-range
+0001d640: 2076 616c 7565 7320 666f 7220 7265 7175   values for requ
+0001d650: 6573 7420 696e 6974 6961 6c69 7a61 7469  est initializati
+0001d660: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
+0001d670: 2320 2d20 4974 206d 6179 2072 6571 7569  # - It may requi
+0001d680: 7265 2073 7065 6369 6679 696e 6720 7265  re specifying re
+0001d690: 6769 6f6e 616c 2065 6e64 706f 696e 7473  gional endpoints
+0001d6a0: 2077 6865 6e20 6372 6561 7469 6e67 2074   when creating t
+0001d6b0: 6865 2073 6572 7669 6365 0a20 2020 2020  he service.     
+0001d6c0: 2020 2020 2020 2023 2020 2063 6c69 656e         #   clien
+0001d6d0: 7420 6173 2073 686f 776e 2069 6e3a 0a20  t as shown in:. 
+0001d6e0: 2020 2020 2020 2020 2020 2023 2020 2068             #   h
+0001d6f0: 7474 7073 3a2f 2f67 6f6f 676c 6561 7069  ttps://googleapi
+0001d700: 732e 6465 762f 7079 7468 6f6e 2f67 6f6f  s.dev/python/goo
+0001d710: 676c 652d 6170 692d 636f 7265 2f6c 6174  gle-api-core/lat
+0001d720: 6573 742f 636c 6965 6e74 5f6f 7074 696f  est/client_optio
+0001d730: 6e73 2e68 746d 6c0a 2020 2020 2020 2020  ns.html.        
+0001d740: 2020 2020 6672 6f6d 2067 6f6f 676c 652e      from google.
+0001d750: 6170 7073 2069 6d70 6f72 7420 6368 6174  apps import chat
+0001d760: 5f76 310a 0a20 2020 2020 2020 2020 2020  _v1..           
+0001d770: 2061 7379 6e63 2064 6566 2073 616d 706c   async def sampl
+0001d780: 655f 6372 6561 7465 5f72 6561 6374 696f  e_create_reactio
+0001d790: 6e28 293a 0a20 2020 2020 2020 2020 2020  n():.           
+0001d7a0: 2020 2020 2023 2043 7265 6174 6520 6120       # Create a 
+0001d7b0: 636c 6965 6e74 0a20 2020 2020 2020 2020  client.         
+0001d7c0: 2020 2020 2020 2063 6c69 656e 7420 3d20         client = 
+0001d7d0: 6368 6174 5f76 312e 4368 6174 5365 7276  chat_v1.ChatServ
+0001d7e0: 6963 6541 7379 6e63 436c 6965 6e74 2829  iceAsyncClient()
+0001d7f0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001d800: 2020 2320 496e 6974 6961 6c69 7a65 2072    # Initialize r
+0001d810: 6571 7565 7374 2061 7267 756d 656e 7428  equest argument(
+0001d820: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
+0001d830: 2020 2072 6571 7565 7374 203d 2063 6861     request = cha
+0001d840: 745f 7631 2e43 7265 6174 6552 6561 6374  t_v1.CreateReact
+0001d850: 696f 6e52 6571 7565 7374 280a 2020 2020  ionRequest(.    
+0001d860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d870: 7061 7265 6e74 3d22 7061 7265 6e74 5f76  parent="parent_v
+0001d880: 616c 7565 222c 0a20 2020 2020 2020 2020  alue",.         
+0001d890: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+0001d8a0: 2020 2020 2020 2020 2020 2320 4d61 6b65            # Make
+0001d8b0: 2074 6865 2072 6571 7565 7374 0a20 2020   the request.   
+0001d8c0: 2020 2020 2020 2020 2020 2020 2072 6573               res
+0001d8d0: 706f 6e73 6520 3d20 6177 6169 7420 636c  ponse = await cl
+0001d8e0: 6965 6e74 2e63 7265 6174 655f 7265 6163  ient.create_reac
+0001d8f0: 7469 6f6e 2872 6571 7565 7374 3d72 6571  tion(request=req
+0001d900: 7565 7374 290a 0a20 2020 2020 2020 2020  uest)..         
+0001d910: 2020 2020 2020 2023 2048 616e 646c 6520         # Handle 
+0001d920: 7468 6520 7265 7370 6f6e 7365 0a20 2020  the response.   
+0001d930: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+0001d940: 6e74 2872 6573 706f 6e73 6529 0a0a 2020  nt(response)..  
+0001d950: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+0001d960: 2020 2020 2020 2020 7265 7175 6573 7420          request 
+0001d970: 284f 7074 696f 6e61 6c5b 556e 696f 6e5b  (Optional[Union[
+0001d980: 676f 6f67 6c65 2e61 7070 732e 6368 6174  google.apps.chat
+0001d990: 5f76 312e 7479 7065 732e 4372 6561 7465  _v1.types.Create
+0001d9a0: 5265 6163 7469 6f6e 5265 7175 6573 742c  ReactionRequest,
+0001d9b0: 2064 6963 745d 5d29 3a0a 2020 2020 2020   dict]]):.      
+0001d9c0: 2020 2020 2020 2020 2020 5468 6520 7265            The re
+0001d9d0: 7175 6573 7420 6f62 6a65 6374 2e20 4372  quest object. Cr
+0001d9e0: 6561 7465 7320 6120 7265 6163 7469 6f6e  eates a reaction
+0001d9f0: 2074 6f20 6120 6d65 7373 6167 652e 0a20   to a message.. 
+0001da00: 2020 2020 2020 2020 2020 2070 6172 656e             paren
+0001da10: 7420 283a 636c 6173 733a 6073 7472 6029  t (:class:`str`)
+0001da20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001da30: 2020 5265 7175 6972 6564 2e20 5468 6520    Required. The 
+0001da40: 6d65 7373 6167 6520 7768 6572 6520 7468  message where th
+0001da50: 6520 7265 6163 7469 6f6e 2069 7320 6372  e reaction is cr
+0001da60: 6561 7465 642e 0a0a 2020 2020 2020 2020  eated...        
+0001da70: 2020 2020 2020 2020 466f 726d 6174 3a20          Format: 
+0001da80: 6060 7370 6163 6573 2f7b 7370 6163 657d  ``spaces/{space}
+0001da90: 2f6d 6573 7361 6765 732f 7b6d 6573 7361  /messages/{messa
+0001daa0: 6765 7d60 600a 0a20 2020 2020 2020 2020  ge}``..         
+0001dab0: 2020 2020 2020 2054 6869 7320 636f 7272         This corr
+0001dac0: 6573 706f 6e64 7320 746f 2074 6865 2060  esponds to the `
+0001dad0: 6070 6172 656e 7460 6020 6669 656c 640a  `parent`` field.
+0001dae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001daf0: 6f6e 2074 6865 2060 6072 6571 7565 7374  on the ``request
+0001db00: 6060 2069 6e73 7461 6e63 653b 2069 6620  `` instance; if 
+0001db10: 6060 7265 7175 6573 7460 6020 6973 2070  ``request`` is p
+0001db20: 726f 7669 6465 642c 2074 6869 730a 2020  rovided, this.  
+0001db30: 2020 2020 2020 2020 2020 2020 2020 7368                sh
+0001db40: 6f75 6c64 206e 6f74 2062 6520 7365 742e  ould not be set.
+0001db50: 0a20 2020 2020 2020 2020 2020 2072 6561  .            rea
+0001db60: 6374 696f 6e20 283a 636c 6173 733a 6067  ction (:class:`g
+0001db70: 6f6f 676c 652e 6170 7073 2e63 6861 745f  oogle.apps.chat_
+0001db80: 7631 2e74 7970 6573 2e52 6561 6374 696f  v1.types.Reactio
+0001db90: 6e60 293a 0a20 2020 2020 2020 2020 2020  n`):.           
+0001dba0: 2020 2020 2052 6571 7569 7265 642e 2054       Required. T
+0001dbb0: 6865 2072 6561 6374 696f 6e20 746f 2063  he reaction to c
+0001dbc0: 7265 6174 652e 0a20 2020 2020 2020 2020  reate..         
+0001dbd0: 2020 2020 2020 2054 6869 7320 636f 7272         This corr
+0001dbe0: 6573 706f 6e64 7320 746f 2074 6865 2060  esponds to the `
+0001dbf0: 6072 6561 6374 696f 6e60 6020 6669 656c  `reaction`` fiel
+0001dc00: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+0001dc10: 2020 6f6e 2074 6865 2060 6072 6571 7565    on the ``reque
+0001dc20: 7374 6060 2069 6e73 7461 6e63 653b 2069  st`` instance; i
+0001dc30: 6620 6060 7265 7175 6573 7460 6020 6973  f ``request`` is
+0001dc40: 2070 726f 7669 6465 642c 2074 6869 730a   provided, this.
+0001dc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dc60: 7368 6f75 6c64 206e 6f74 2062 6520 7365  should not be se
+0001dc70: 742e 0a20 2020 2020 2020 2020 2020 2072  t..            r
+0001dc80: 6574 7279 2028 676f 6f67 6c65 2e61 7069  etry (google.api
+0001dc90: 5f63 6f72 652e 7265 7472 795f 6173 796e  _core.retry_asyn
+0001dca0: 632e 4173 796e 6352 6574 7279 293a 2044  c.AsyncRetry): D
+0001dcb0: 6573 6967 6e61 7469 6f6e 206f 6620 7768  esignation of wh
+0001dcc0: 6174 2065 7272 6f72 732c 2069 6620 616e  at errors, if an
+0001dcd0: 792c 0a20 2020 2020 2020 2020 2020 2020  y,.             
+0001dce0: 2020 2073 686f 756c 6420 6265 2072 6574     should be ret
+0001dcf0: 7269 6564 2e0a 2020 2020 2020 2020 2020  ried..          
+0001dd00: 2020 7469 6d65 6f75 7420 2866 6c6f 6174    timeout (float
+0001dd10: 293a 2054 6865 2074 696d 656f 7574 2066  ): The timeout f
+0001dd20: 6f72 2074 6869 7320 7265 7175 6573 742e  or this request.
+0001dd30: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
+0001dd40: 6164 6174 6120 2853 6571 7565 6e63 655b  adata (Sequence[
+0001dd50: 5475 706c 655b 7374 722c 2073 7472 5d5d  Tuple[str, str]]
+0001dd60: 293a 2053 7472 696e 6773 2077 6869 6368  ): Strings which
+0001dd70: 2073 686f 756c 6420 6265 0a20 2020 2020   should be.     
+0001dd80: 2020 2020 2020 2020 2020 2073 656e 7420             sent 
+0001dd90: 616c 6f6e 6720 7769 7468 2074 6865 2072  along with the r
+0001dda0: 6571 7565 7374 2061 7320 6d65 7461 6461  equest as metada
+0001ddb0: 7461 2e0a 0a20 2020 2020 2020 2052 6574  ta...        Ret
+0001ddc0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+0001ddd0: 2020 676f 6f67 6c65 2e61 7070 732e 6368    google.apps.ch
+0001dde0: 6174 5f76 312e 7479 7065 732e 5265 6163  at_v1.types.Reac
+0001ddf0: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
+0001de00: 2020 2020 2020 4120 7265 6163 7469 6f6e        A reaction
+0001de10: 2074 6f20 6120 6d65 7373 6167 652e 0a20   to a message.. 
+0001de20: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0001de30: 2020 2023 2043 7265 6174 6520 6f72 2063     # Create or c
+0001de40: 6f65 7263 6520 6120 7072 6f74 6f62 7566  oerce a protobuf
+0001de50: 2072 6571 7565 7374 206f 626a 6563 742e   request object.
+0001de60: 0a20 2020 2020 2020 2023 2051 7569 636b  .        # Quick
+0001de70: 2063 6865 636b 3a20 4966 2077 6520 676f   check: If we go
+0001de80: 7420 6120 7265 7175 6573 7420 6f62 6a65  t a request obje
+0001de90: 6374 2c20 7765 2073 686f 756c 6420 2a6e  ct, we should *n
+0001dea0: 6f74 2a20 6861 7665 0a20 2020 2020 2020  ot* have.       
+0001deb0: 2023 2067 6f74 7465 6e20 616e 7920 6b65   # gotten any ke
+0001dec0: 7977 6f72 6420 6172 6775 6d65 6e74 7320  yword arguments 
+0001ded0: 7468 6174 206d 6170 2074 6f20 7468 6520  that map to the 
+0001dee0: 7265 7175 6573 742e 0a20 2020 2020 2020  request..       
+0001def0: 2068 6173 5f66 6c61 7474 656e 6564 5f70   has_flattened_p
+0001df00: 6172 616d 7320 3d20 616e 7928 5b70 6172  arams = any([par
+0001df10: 656e 742c 2072 6561 6374 696f 6e5d 290a  ent, reaction]).
+0001df20: 2020 2020 2020 2020 6966 2072 6571 7565          if reque
+0001df30: 7374 2069 7320 6e6f 7420 4e6f 6e65 2061  st is not None a
+0001df40: 6e64 2068 6173 5f66 6c61 7474 656e 6564  nd has_flattened
+0001df50: 5f70 6172 616d 733a 0a20 2020 2020 2020  _params:.       
+0001df60: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+0001df70: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+0001df80: 2020 2020 2020 2022 4966 2074 6865 2060         "If the `
+0001df90: 7265 7175 6573 7460 2061 7267 756d 656e  request` argumen
+0001dfa0: 7420 6973 2073 6574 2c20 7468 656e 206e  t is set, then n
+0001dfb0: 6f6e 6520 6f66 2022 0a20 2020 2020 2020  one of ".       
+0001dfc0: 2020 2020 2020 2020 2022 7468 6520 696e           "the in
+0001dfd0: 6469 7669 6475 616c 2066 6965 6c64 2061  dividual field a
+0001dfe0: 7267 756d 656e 7473 2073 686f 756c 6420  rguments should 
+0001dff0: 6265 2073 6574 2e22 0a20 2020 2020 2020  be set.".       
+0001e000: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0001e010: 7265 7175 6573 7420 3d20 6763 5f72 6561  request = gc_rea
+0001e020: 6374 696f 6e2e 4372 6561 7465 5265 6163  ction.CreateReac
+0001e030: 7469 6f6e 5265 7175 6573 7428 7265 7175  tionRequest(requ
+0001e040: 6573 7429 0a0a 2020 2020 2020 2020 2320  est)..        # 
+0001e050: 4966 2077 6520 6861 7665 206b 6579 776f  If we have keywo
+0001e060: 7264 2061 7267 756d 656e 7473 2063 6f72  rd arguments cor
+0001e070: 7265 7370 6f6e 6469 6e67 2074 6f20 6669  responding to fi
+0001e080: 656c 6473 206f 6e20 7468 650a 2020 2020  elds on the.    
+0001e090: 2020 2020 2320 7265 7175 6573 742c 2061      # request, a
+0001e0a0: 7070 6c79 2074 6865 7365 2e0a 2020 2020  pply these..    
+0001e0b0: 2020 2020 6966 2070 6172 656e 7420 6973      if parent is
+0001e0c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0001e0d0: 2020 2020 2020 2072 6571 7565 7374 2e70         request.p
+0001e0e0: 6172 656e 7420 3d20 7061 7265 6e74 0a20  arent = parent. 
+0001e0f0: 2020 2020 2020 2069 6620 7265 6163 7469         if reacti
+0001e100: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  on is not None:.
+0001e110: 2020 2020 2020 2020 2020 2020 7265 7175              requ
+0001e120: 6573 742e 7265 6163 7469 6f6e 203d 2072  est.reaction = r
+0001e130: 6561 6374 696f 6e0a 0a20 2020 2020 2020  eaction..       
+0001e140: 2023 2057 7261 7020 7468 6520 5250 4320   # Wrap the RPC 
+0001e150: 6d65 7468 6f64 3b20 7468 6973 2061 6464  method; this add
+0001e160: 7320 7265 7472 7920 616e 6420 7469 6d65  s retry and time
+0001e170: 6f75 7420 696e 666f 726d 6174 696f 6e2c  out information,
+0001e180: 0a20 2020 2020 2020 2023 2061 6e64 2066  .        # and f
+0001e190: 7269 656e 646c 7920 6572 726f 7220 6861  riendly error ha
+0001e1a0: 6e64 6c69 6e67 2e0a 2020 2020 2020 2020  ndling..        
+0001e1b0: 7270 6320 3d20 6761 7069 635f 7631 2e6d  rpc = gapic_v1.m
+0001e1c0: 6574 686f 645f 6173 796e 632e 7772 6170  ethod_async.wrap
+0001e1d0: 5f6d 6574 686f 6428 0a20 2020 2020 2020  _method(.       
+0001e1e0: 2020 2020 2073 656c 662e 5f63 6c69 656e       self._clien
+0001e1f0: 742e 5f74 7261 6e73 706f 7274 2e63 7265  t._transport.cre
+0001e200: 6174 655f 7265 6163 7469 6f6e 2c0a 2020  ate_reaction,.  
+0001e210: 2020 2020 2020 2020 2020 6465 6661 756c            defaul
+0001e220: 745f 7265 7472 793d 7265 7472 6965 732e  t_retry=retries.
+0001e230: 4173 796e 6352 6574 7279 280a 2020 2020  AsyncRetry(.    
+0001e240: 2020 2020 2020 2020 2020 2020 696e 6974              init
+0001e250: 6961 6c3d 312e 302c 0a20 2020 2020 2020  ial=1.0,.       
+0001e260: 2020 2020 2020 2020 206d 6178 696d 756d           maximum
+0001e270: 3d31 302e 302c 0a20 2020 2020 2020 2020  =10.0,.         
+0001e280: 2020 2020 2020 206d 756c 7469 706c 6965         multiplie
+0001e290: 723d 312e 332c 0a20 2020 2020 2020 2020  r=1.3,.         
+0001e2a0: 2020 2020 2020 2070 7265 6469 6361 7465         predicate
+0001e2b0: 3d72 6574 7269 6573 2e69 665f 6578 6365  =retries.if_exce
+0001e2c0: 7074 696f 6e5f 7479 7065 280a 2020 2020  ption_type(.    
+0001e2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e2e0: 636f 7265 5f65 7863 6570 7469 6f6e 732e  core_exceptions.
+0001e2f0: 5365 7276 6963 6555 6e61 7661 696c 6162  ServiceUnavailab
+0001e300: 6c65 2c0a 2020 2020 2020 2020 2020 2020  le,.            
+0001e310: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+0001e320: 2020 2020 2020 2064 6561 646c 696e 653d         deadline=
+0001e330: 3330 2e30 2c0a 2020 2020 2020 2020 2020  30.0,.          
+0001e340: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
+0001e350: 2064 6566 6175 6c74 5f74 696d 656f 7574   default_timeout
+0001e360: 3d33 302e 302c 0a20 2020 2020 2020 2020  =30.0,.         
+0001e370: 2020 2063 6c69 656e 745f 696e 666f 3d44     client_info=D
+0001e380: 4546 4155 4c54 5f43 4c49 454e 545f 494e  EFAULT_CLIENT_IN
+0001e390: 464f 2c0a 2020 2020 2020 2020 290a 0a20  FO,.        ).. 
+0001e3a0: 2020 2020 2020 2023 2043 6572 7461 696e         # Certain
+0001e3b0: 2066 6965 6c64 7320 7368 6f75 6c64 2062   fields should b
+0001e3c0: 6520 7072 6f76 6964 6564 2077 6974 6869  e provided withi
+0001e3d0: 6e20 7468 6520 6d65 7461 6461 7461 2068  n the metadata h
+0001e3e0: 6561 6465 723b 0a20 2020 2020 2020 2023  eader;.        #
+0001e3f0: 2061 6464 2074 6865 7365 2068 6572 652e   add these here.
+0001e400: 0a20 2020 2020 2020 206d 6574 6164 6174  .        metadat
+0001e410: 6120 3d20 7475 706c 6528 6d65 7461 6461  a = tuple(metada
+0001e420: 7461 2920 2b20 280a 2020 2020 2020 2020  ta) + (.        
+0001e430: 2020 2020 6761 7069 635f 7631 2e72 6f75      gapic_v1.rou
+0001e440: 7469 6e67 5f68 6561 6465 722e 746f 5f67  ting_header.to_g
+0001e450: 7270 635f 6d65 7461 6461 7461 2828 2822  rpc_metadata((("
+0001e460: 7061 7265 6e74 222c 2072 6571 7565 7374  parent", request
+0001e470: 2e70 6172 656e 7429 2c29 292c 0a20 2020  .parent),)),.   
+0001e480: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0001e490: 2320 5661 6c69 6461 7465 2074 6865 2075  # Validate the u
+0001e4a0: 6e69 7665 7273 6520 646f 6d61 696e 2e0a  niverse domain..
+0001e4b0: 2020 2020 2020 2020 7365 6c66 2e5f 636c          self._cl
+0001e4c0: 6965 6e74 2e5f 7661 6c69 6461 7465 5f75  ient._validate_u
+0001e4d0: 6e69 7665 7273 655f 646f 6d61 696e 2829  niverse_domain()
+0001e4e0: 0a0a 2020 2020 2020 2020 2320 5365 6e64  ..        # Send
+0001e4f0: 2074 6865 2072 6571 7565 7374 2e0a 2020   the request..  
+0001e500: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
+0001e510: 2061 7761 6974 2072 7063 280a 2020 2020   await rpc(.    
+0001e520: 2020 2020 2020 2020 7265 7175 6573 742c          request,
+0001e530: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0001e540: 7279 3d72 6574 7279 2c0a 2020 2020 2020  ry=retry,.      
+0001e550: 2020 2020 2020 7469 6d65 6f75 743d 7469        timeout=ti
+0001e560: 6d65 6f75 742c 0a20 2020 2020 2020 2020  meout,.         
+0001e570: 2020 206d 6574 6164 6174 613d 6d65 7461     metadata=meta
+0001e580: 6461 7461 2c0a 2020 2020 2020 2020 290a  data,.        ).
+0001e590: 0a20 2020 2020 2020 2023 2044 6f6e 653b  .        # Done;
+0001e5a0: 2072 6574 7572 6e20 7468 6520 7265 7370   return the resp
+0001e5b0: 6f6e 7365 2e0a 2020 2020 2020 2020 7265  onse..        re
+0001e5c0: 7475 726e 2072 6573 706f 6e73 650a 0a20  turn response.. 
+0001e5d0: 2020 2061 7379 6e63 2064 6566 206c 6973     async def lis
+0001e5e0: 745f 7265 6163 7469 6f6e 7328 0a20 2020  t_reactions(.   
+0001e5f0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0001e600: 2020 2072 6571 7565 7374 3a20 4f70 7469     request: Opti
+0001e610: 6f6e 616c 5b55 6e69 6f6e 5b72 6561 6374  onal[Union[react
+0001e620: 696f 6e2e 4c69 7374 5265 6163 7469 6f6e  ion.ListReaction
+0001e630: 7352 6571 7565 7374 2c20 6469 6374 5d5d  sRequest, dict]]
+0001e640: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0001e650: 202a 2c0a 2020 2020 2020 2020 7061 7265   *,.        pare
+0001e660: 6e74 3a20 4f70 7469 6f6e 616c 5b73 7472  nt: Optional[str
+0001e670: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0001e680: 2020 7265 7472 793a 204f 7074 696f 6e61    retry: Optiona
+0001e690: 6c52 6574 7279 203d 2067 6170 6963 5f76  lRetry = gapic_v
+0001e6a0: 312e 6d65 7468 6f64 2e44 4546 4155 4c54  1.method.DEFAULT
+0001e6b0: 2c0a 2020 2020 2020 2020 7469 6d65 6f75  ,.        timeou
+0001e6c0: 743a 2055 6e69 6f6e 5b66 6c6f 6174 2c20  t: Union[float, 
+0001e6d0: 6f62 6a65 6374 5d20 3d20 6761 7069 635f  object] = gapic_
+0001e6e0: 7631 2e6d 6574 686f 642e 4445 4641 554c  v1.method.DEFAUL
+0001e6f0: 542c 0a20 2020 2020 2020 206d 6574 6164  T,.        metad
+0001e700: 6174 613a 2053 6571 7565 6e63 655b 5475  ata: Sequence[Tu
+0001e710: 706c 655b 7374 722c 2073 7472 5d5d 203d  ple[str, str]] =
+0001e720: 2028 292c 0a20 2020 2029 202d 3e20 7061   (),.    ) -> pa
+0001e730: 6765 7273 2e4c 6973 7452 6561 6374 696f  gers.ListReactio
+0001e740: 6e73 4173 796e 6350 6167 6572 3a0a 2020  nsAsyncPager:.  
+0001e750: 2020 2020 2020 7222 2222 4c69 7374 7320        r"""Lists 
+0001e760: 7265 6163 7469 6f6e 7320 746f 2061 206d  reactions to a m
+0001e770: 6573 7361 6765 2e20 466f 7220 616e 2065  essage. For an e
+0001e780: 7861 6d70 6c65 2c20 7365 6520 604c 6973  xample, see `Lis
+0001e790: 740a 2020 2020 2020 2020 7265 6163 7469  t.        reacti
+0001e7a0: 6f6e 7320 666f 7220 610a 2020 2020 2020  ons for a.      
+0001e7b0: 2020 6d65 7373 6167 6520 3c68 7474 7073    message <https
+0001e7c0: 3a2f 2f64 6576 656c 6f70 6572 732e 676f  ://developers.go
+0001e7d0: 6f67 6c65 2e63 6f6d 2f77 6f72 6b73 7061  ogle.com/workspa
+0001e7e0: 6365 2f63 6861 742f 6c69 7374 2d72 6561  ce/chat/list-rea
+0001e7f0: 6374 696f 6e73 3e60 5f5f 2e0a 2020 2020  ctions>`__..    
+0001e800: 2020 2020 5265 7175 6972 6573 2060 7573      Requires `us
+0001e810: 6572 0a20 2020 2020 2020 2061 7574 6865  er.        authe
+0001e820: 6e74 6963 6174 696f 6e20 3c68 7474 7073  ntication <https
+0001e830: 3a2f 2f64 6576 656c 6f70 6572 732e 676f  ://developers.go
+0001e840: 6f67 6c65 2e63 6f6d 2f77 6f72 6b73 7061  ogle.com/workspa
+0001e850: 6365 2f63 6861 742f 6175 7468 656e 7469  ce/chat/authenti
+0001e860: 6361 7465 2d61 7574 686f 7269 7a65 2d63  cate-authorize-c
+0001e870: 6861 742d 7573 6572 3e60 5f5f 2e0a 0a20  hat-user>`__... 
+0001e880: 2020 2020 2020 202e 2e20 636f 6465 2d62         .. code-b
+0001e890: 6c6f 636b 3a3a 2070 7974 686f 6e0a 0a20  lock:: python.. 
+0001e8a0: 2020 2020 2020 2020 2020 2023 2054 6869             # Thi
+0001e8b0: 7320 736e 6970 7065 7420 6861 7320 6265  s snippet has be
+0001e8c0: 656e 2061 7574 6f6d 6174 6963 616c 6c79  en automatically
+0001e8d0: 2067 656e 6572 6174 6564 2061 6e64 2073   generated and s
+0001e8e0: 686f 756c 6420 6265 2072 6567 6172 6465  hould be regarde
+0001e8f0: 6420 6173 2061 0a20 2020 2020 2020 2020  d as a.         
+0001e900: 2020 2023 2063 6f64 6520 7465 6d70 6c61     # code templa
+0001e910: 7465 206f 6e6c 792e 0a20 2020 2020 2020  te only..       
+0001e920: 2020 2020 2023 2049 7420 7769 6c6c 2072       # It will r
+0001e930: 6571 7569 7265 206d 6f64 6966 6963 6174  equire modificat
+0001e940: 696f 6e73 2074 6f20 776f 726b 3a0a 2020  ions to work:.  
+0001e950: 2020 2020 2020 2020 2020 2320 2d20 4974            # - It
+0001e960: 206d 6179 2072 6571 7569 7265 2063 6f72   may require cor
+0001e970: 7265 6374 2f69 6e2d 7261 6e67 6520 7661  rect/in-range va
+0001e980: 6c75 6573 2066 6f72 2072 6571 7565 7374  lues for request
+0001e990: 2069 6e69 7469 616c 697a 6174 696f 6e2e   initialization.
+0001e9a0: 0a20 2020 2020 2020 2020 2020 2023 202d  .            # -
+0001e9b0: 2049 7420 6d61 7920 7265 7175 6972 6520   It may require 
+0001e9c0: 7370 6563 6966 7969 6e67 2072 6567 696f  specifying regio
+0001e9d0: 6e61 6c20 656e 6470 6f69 6e74 7320 7768  nal endpoints wh
+0001e9e0: 656e 2063 7265 6174 696e 6720 7468 6520  en creating the 
+0001e9f0: 7365 7276 6963 650a 2020 2020 2020 2020  service.        
+0001ea00: 2020 2020 2320 2020 636c 6965 6e74 2061      #   client a
+0001ea10: 7320 7368 6f77 6e20 696e 3a0a 2020 2020  s shown in:.    
+0001ea20: 2020 2020 2020 2020 2320 2020 6874 7470          #   http
+0001ea30: 733a 2f2f 676f 6f67 6c65 6170 6973 2e64  s://googleapis.d
+0001ea40: 6576 2f70 7974 686f 6e2f 676f 6f67 6c65  ev/python/google
+0001ea50: 2d61 7069 2d63 6f72 652f 6c61 7465 7374  -api-core/latest
+0001ea60: 2f63 6c69 656e 745f 6f70 7469 6f6e 732e  /client_options.
+0001ea70: 6874 6d6c 0a20 2020 2020 2020 2020 2020  html.           
+0001ea80: 2066 726f 6d20 676f 6f67 6c65 2e61 7070   from google.app
+0001ea90: 7320 696d 706f 7274 2063 6861 745f 7631  s import chat_v1
+0001eaa0: 0a0a 2020 2020 2020 2020 2020 2020 6173  ..            as
+0001eab0: 796e 6320 6465 6620 7361 6d70 6c65 5f6c  ync def sample_l
+0001eac0: 6973 745f 7265 6163 7469 6f6e 7328 293a  ist_reactions():
+0001ead0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001eae0: 2023 2043 7265 6174 6520 6120 636c 6965   # Create a clie
+0001eaf0: 6e74 0a20 2020 2020 2020 2020 2020 2020  nt.             
+0001eb00: 2020 2063 6c69 656e 7420 3d20 6368 6174     client = chat
+0001eb10: 5f76 312e 4368 6174 5365 7276 6963 6541  _v1.ChatServiceA
+0001eb20: 7379 6e63 436c 6965 6e74 2829 0a0a 2020  syncClient()..  
+0001eb30: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0001eb40: 496e 6974 6961 6c69 7a65 2072 6571 7565  Initialize reque
+0001eb50: 7374 2061 7267 756d 656e 7428 7329 0a20  st argument(s). 
+0001eb60: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0001eb70: 6571 7565 7374 203d 2063 6861 745f 7631  equest = chat_v1
+0001eb80: 2e4c 6973 7452 6561 6374 696f 6e73 5265  .ListReactionsRe
+0001eb90: 7175 6573 7428 0a20 2020 2020 2020 2020  quest(.         
+0001eba0: 2020 2020 2020 2020 2020 2070 6172 656e             paren
+0001ebb0: 743d 2270 6172 656e 745f 7661 6c75 6522  t="parent_value"
+0001ebc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001ebd0: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
+0001ebe0: 2020 2020 2023 204d 616b 6520 7468 6520       # Make the 
+0001ebf0: 7265 7175 6573 740a 2020 2020 2020 2020  request.        
+0001ec00: 2020 2020 2020 2020 7061 6765 5f72 6573          page_res
+0001ec10: 756c 7420 3d20 636c 6965 6e74 2e6c 6973  ult = client.lis
+0001ec20: 745f 7265 6163 7469 6f6e 7328 7265 7175  t_reactions(requ
+0001ec30: 6573 743d 7265 7175 6573 7429 0a0a 2020  est=request)..  
+0001ec40: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0001ec50: 4861 6e64 6c65 2074 6865 2072 6573 706f  Handle the respo
+0001ec60: 6e73 650a 2020 2020 2020 2020 2020 2020  nse.            
+0001ec70: 2020 2020 6173 796e 6320 666f 7220 7265      async for re
+0001ec80: 7370 6f6e 7365 2069 6e20 7061 6765 5f72  sponse in page_r
+0001ec90: 6573 756c 743a 0a20 2020 2020 2020 2020  esult:.         
+0001eca0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0001ecb0: 2872 6573 706f 6e73 6529 0a0a 2020 2020  (response)..    
+0001ecc0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+0001ecd0: 2020 2020 2020 7265 7175 6573 7420 284f        request (O
+0001ece0: 7074 696f 6e61 6c5b 556e 696f 6e5b 676f  ptional[Union[go
+0001ecf0: 6f67 6c65 2e61 7070 732e 6368 6174 5f76  ogle.apps.chat_v
+0001ed00: 312e 7479 7065 732e 4c69 7374 5265 6163  1.types.ListReac
+0001ed10: 7469 6f6e 7352 6571 7565 7374 2c20 6469  tionsRequest, di
+0001ed20: 6374 5d5d 293a 0a20 2020 2020 2020 2020  ct]]):.         
+0001ed30: 2020 2020 2020 2054 6865 2072 6571 7565         The reque
+0001ed40: 7374 206f 626a 6563 742e 204c 6973 7473  st object. Lists
+0001ed50: 2072 6561 6374 696f 6e73 2074 6f20 6120   reactions to a 
+0001ed60: 6d65 7373 6167 652e 0a20 2020 2020 2020  message..       
+0001ed70: 2020 2020 2070 6172 656e 7420 283a 636c       parent (:cl
+0001ed80: 6173 733a 6073 7472 6029 3a0a 2020 2020  ass:`str`):.    
+0001ed90: 2020 2020 2020 2020 2020 2020 5265 7175              Requ
+0001eda0: 6972 6564 2e20 5468 6520 6d65 7373 6167  ired. The messag
+0001edb0: 6520 7573 6572 7320 7265 6163 7465 6420  e users reacted 
+0001edc0: 746f 2e0a 0a20 2020 2020 2020 2020 2020  to...           
+0001edd0: 2020 2020 2046 6f72 6d61 743a 2060 6073       Format: ``s
+0001ede0: 7061 6365 732f 7b73 7061 6365 7d2f 6d65  paces/{space}/me
+0001edf0: 7373 6167 6573 2f7b 6d65 7373 6167 657d  ssages/{message}
+0001ee00: 6060 0a0a 2020 2020 2020 2020 2020 2020  ``..            
+0001ee10: 2020 2020 5468 6973 2063 6f72 7265 7370      This corresp
+0001ee20: 6f6e 6473 2074 6f20 7468 6520 6060 7061  onds to the ``pa
+0001ee30: 7265 6e74 6060 2066 6965 6c64 0a20 2020  rent`` field.   
+0001ee40: 2020 2020 2020 2020 2020 2020 206f 6e20               on 
+0001ee50: 7468 6520 6060 7265 7175 6573 7460 6020  the ``request`` 
+0001ee60: 696e 7374 616e 6365 3b20 6966 2060 6072  instance; if ``r
+0001ee70: 6571 7565 7374 6060 2069 7320 7072 6f76  equest`` is prov
+0001ee80: 6964 6564 2c20 7468 6973 0a20 2020 2020  ided, this.     
+0001ee90: 2020 2020 2020 2020 2020 2073 686f 756c             shoul
+0001eea0: 6420 6e6f 7420 6265 2073 6574 2e0a 2020  d not be set..  
+0001eeb0: 2020 2020 2020 2020 2020 7265 7472 7920            retry 
+0001eec0: 2867 6f6f 676c 652e 6170 695f 636f 7265  (google.api_core
+0001eed0: 2e72 6574 7279 5f61 7379 6e63 2e41 7379  .retry_async.Asy
+0001eee0: 6e63 5265 7472 7929 3a20 4465 7369 676e  ncRetry): Design
+0001eef0: 6174 696f 6e20 6f66 2077 6861 7420 6572  ation of what er
+0001ef00: 726f 7273 2c20 6966 2061 6e79 2c0a 2020  rors, if any,.  
+0001ef10: 2020 2020 2020 2020 2020 2020 2020 7368                sh
+0001ef20: 6f75 6c64 2062 6520 7265 7472 6965 642e  ould be retried.
+0001ef30: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
+0001ef40: 656f 7574 2028 666c 6f61 7429 3a20 5468  eout (float): Th
+0001ef50: 6520 7469 6d65 6f75 7420 666f 7220 7468  e timeout for th
+0001ef60: 6973 2072 6571 7565 7374 2e0a 2020 2020  is request..    
+0001ef70: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
+0001ef80: 2028 5365 7175 656e 6365 5b54 7570 6c65   (Sequence[Tuple
+0001ef90: 5b73 7472 2c20 7374 725d 5d29 3a20 5374  [str, str]]): St
+0001efa0: 7269 6e67 7320 7768 6963 6820 7368 6f75  rings which shou
+0001efb0: 6c64 2062 650a 2020 2020 2020 2020 2020  ld be.          
+0001efc0: 2020 2020 2020 7365 6e74 2061 6c6f 6e67        sent along
+0001efd0: 2077 6974 6820 7468 6520 7265 7175 6573   with the reques
+0001efe0: 7420 6173 206d 6574 6164 6174 612e 0a0a  t as metadata...
+0001eff0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+0001f000: 0a20 2020 2020 2020 2020 2020 2067 6f6f  .            goo
+0001f010: 676c 652e 6170 7073 2e63 6861 745f 7631  gle.apps.chat_v1
+0001f020: 2e73 6572 7669 6365 732e 6368 6174 5f73  .services.chat_s
+0001f030: 6572 7669 6365 2e70 6167 6572 732e 4c69  ervice.pagers.Li
+0001f040: 7374 5265 6163 7469 6f6e 7341 7379 6e63  stReactionsAsync
+0001f050: 5061 6765 723a 0a20 2020 2020 2020 2020  Pager:.         
+0001f060: 2020 2020 2020 2052 6573 706f 6e73 6520         Response 
+0001f070: 746f 2061 206c 6973 7420 7265 6163 7469  to a list reacti
+0001f080: 6f6e 7320 7265 7175 6573 742e 0a0a 2020  ons request...  
+0001f090: 2020 2020 2020 2020 2020 2020 2020 4974                It
+0001f0a0: 6572 6174 696e 6720 6f76 6572 2074 6869  erating over thi
+0001f0b0: 7320 6f62 6a65 6374 2077 696c 6c20 7969  s object will yi
+0001f0c0: 656c 640a 2020 2020 2020 2020 2020 2020  eld.            
+0001f0d0: 2020 2020 7265 7375 6c74 7320 616e 6420      results and 
+0001f0e0: 7265 736f 6c76 6520 6164 6469 7469 6f6e  resolve addition
+0001f0f0: 616c 2070 6167 6573 0a20 2020 2020 2020  al pages.       
+0001f100: 2020 2020 2020 2020 2061 7574 6f6d 6174           automat
+0001f110: 6963 616c 6c79 2e0a 0a20 2020 2020 2020  ically...       
+0001f120: 2022 2222 0a20 2020 2020 2020 2023 2043   """.        # C
+0001f130: 7265 6174 6520 6f72 2063 6f65 7263 6520  reate or coerce 
+0001f140: 6120 7072 6f74 6f62 7566 2072 6571 7565  a protobuf reque
+0001f150: 7374 206f 626a 6563 742e 0a20 2020 2020  st object..     
+0001f160: 2020 2023 2051 7569 636b 2063 6865 636b     # Quick check
+0001f170: 3a20 4966 2077 6520 676f 7420 6120 7265  : If we got a re
+0001f180: 7175 6573 7420 6f62 6a65 6374 2c20 7765  quest object, we
+0001f190: 2073 686f 756c 6420 2a6e 6f74 2a20 6861   should *not* ha
+0001f1a0: 7665 0a20 2020 2020 2020 2023 2067 6f74  ve.        # got
+0001f1b0: 7465 6e20 616e 7920 6b65 7977 6f72 6420  ten any keyword 
+0001f1c0: 6172 6775 6d65 6e74 7320 7468 6174 206d  arguments that m
+0001f1d0: 6170 2074 6f20 7468 6520 7265 7175 6573  ap to the reques
+0001f1e0: 742e 0a20 2020 2020 2020 2068 6173 5f66  t..        has_f
+0001f1f0: 6c61 7474 656e 6564 5f70 6172 616d 7320  lattened_params 
+0001f200: 3d20 616e 7928 5b70 6172 656e 745d 290a  = any([parent]).
+0001f210: 2020 2020 2020 2020 6966 2072 6571 7565          if reque
+0001f220: 7374 2069 7320 6e6f 7420 4e6f 6e65 2061  st is not None a
+0001f230: 6e64 2068 6173 5f66 6c61 7474 656e 6564  nd has_flattened
+0001f240: 5f70 6172 616d 733a 0a20 2020 2020 2020  _params:.       
+0001f250: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+0001f260: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+0001f270: 2020 2020 2020 2022 4966 2074 6865 2060         "If the `
+0001f280: 7265 7175 6573 7460 2061 7267 756d 656e  request` argumen
+0001f290: 7420 6973 2073 6574 2c20 7468 656e 206e  t is set, then n
+0001f2a0: 6f6e 6520 6f66 2022 0a20 2020 2020 2020  one of ".       
+0001f2b0: 2020 2020 2020 2020 2022 7468 6520 696e           "the in
+0001f2c0: 6469 7669 6475 616c 2066 6965 6c64 2061  dividual field a
+0001f2d0: 7267 756d 656e 7473 2073 686f 756c 6420  rguments should 
+0001f2e0: 6265 2073 6574 2e22 0a20 2020 2020 2020  be set.".       
+0001f2f0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0001f300: 7265 7175 6573 7420 3d20 7265 6163 7469  request = reacti
+0001f310: 6f6e 2e4c 6973 7452 6561 6374 696f 6e73  on.ListReactions
+0001f320: 5265 7175 6573 7428 7265 7175 6573 7429  Request(request)
+0001f330: 0a0a 2020 2020 2020 2020 2320 4966 2077  ..        # If w
+0001f340: 6520 6861 7665 206b 6579 776f 7264 2061  e have keyword a
+0001f350: 7267 756d 656e 7473 2063 6f72 7265 7370  rguments corresp
+0001f360: 6f6e 6469 6e67 2074 6f20 6669 656c 6473  onding to fields
+0001f370: 206f 6e20 7468 650a 2020 2020 2020 2020   on the.        
+0001f380: 2320 7265 7175 6573 742c 2061 7070 6c79  # request, apply
+0001f390: 2074 6865 7365 2e0a 2020 2020 2020 2020   these..        
+0001f3a0: 6966 2070 6172 656e 7420 6973 206e 6f74  if parent is not
+0001f3b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0001f3c0: 2020 2072 6571 7565 7374 2e70 6172 656e     request.paren
+0001f3d0: 7420 3d20 7061 7265 6e74 0a0a 2020 2020  t = parent..    
+0001f3e0: 2020 2020 2320 5772 6170 2074 6865 2052      # Wrap the R
+0001f3f0: 5043 206d 6574 686f 643b 2074 6869 7320  PC method; this 
+0001f400: 6164 6473 2072 6574 7279 2061 6e64 2074  adds retry and t
+0001f410: 696d 656f 7574 2069 6e66 6f72 6d61 7469  imeout informati
+0001f420: 6f6e 2c0a 2020 2020 2020 2020 2320 616e  on,.        # an
+0001f430: 6420 6672 6965 6e64 6c79 2065 7272 6f72  d friendly error
+0001f440: 2068 616e 646c 696e 672e 0a20 2020 2020   handling..     
+0001f450: 2020 2072 7063 203d 2067 6170 6963 5f76     rpc = gapic_v
+0001f460: 312e 6d65 7468 6f64 5f61 7379 6e63 2e77  1.method_async.w
+0001f470: 7261 705f 6d65 7468 6f64 280a 2020 2020  rap_method(.    
+0001f480: 2020 2020 2020 2020 7365 6c66 2e5f 636c          self._cl
+0001f490: 6965 6e74 2e5f 7472 616e 7370 6f72 742e  ient._transport.
+0001f4a0: 6c69 7374 5f72 6561 6374 696f 6e73 2c0a  list_reactions,.
+0001f4b0: 2020 2020 2020 2020 2020 2020 6465 6661              defa
+0001f4c0: 756c 745f 7265 7472 793d 7265 7472 6965  ult_retry=retrie
+0001f4d0: 732e 4173 796e 6352 6574 7279 280a 2020  s.AsyncRetry(.  
+0001f4e0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+0001f4f0: 6974 6961 6c3d 312e 302c 0a20 2020 2020  itial=1.0,.     
+0001f500: 2020 2020 2020 2020 2020 206d 6178 696d             maxim
+0001f510: 756d 3d31 302e 302c 0a20 2020 2020 2020  um=10.0,.       
+0001f520: 2020 2020 2020 2020 206d 756c 7469 706c           multipl
+0001f530: 6965 723d 312e 332c 0a20 2020 2020 2020  ier=1.3,.       
+0001f540: 2020 2020 2020 2020 2070 7265 6469 6361           predica
+0001f550: 7465 3d72 6574 7269 6573 2e69 665f 6578  te=retries.if_ex
+0001f560: 6365 7074 696f 6e5f 7479 7065 280a 2020  ception_type(.  
+0001f570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f580: 2020 636f 7265 5f65 7863 6570 7469 6f6e    core_exception
+0001f590: 732e 5365 7276 6963 6555 6e61 7661 696c  s.ServiceUnavail
+0001f5a0: 6162 6c65 2c0a 2020 2020 2020 2020 2020  able,.          
+0001f5b0: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+0001f5c0: 2020 2020 2020 2020 2064 6561 646c 696e           deadlin
+0001f5d0: 653d 3330 2e30 2c0a 2020 2020 2020 2020  e=30.0,.        
+0001f5e0: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+0001f5f0: 2020 2064 6566 6175 6c74 5f74 696d 656f     default_timeo
+0001f600: 7574 3d33 302e 302c 0a20 2020 2020 2020  ut=30.0,.       
+0001f610: 2020 2020 2063 6c69 656e 745f 696e 666f       client_info
+0001f620: 3d44 4546 4155 4c54 5f43 4c49 454e 545f  =DEFAULT_CLIENT_
+0001f630: 494e 464f 2c0a 2020 2020 2020 2020 290a  INFO,.        ).
+0001f640: 0a20 2020 2020 2020 2023 2043 6572 7461  .        # Certa
+0001f650: 696e 2066 6965 6c64 7320 7368 6f75 6c64  in fields should
+0001f660: 2062 6520 7072 6f76 6964 6564 2077 6974   be provided wit
+0001f670: 6869 6e20 7468 6520 6d65 7461 6461 7461  hin the metadata
+0001f680: 2068 6561 6465 723b 0a20 2020 2020 2020   header;.       
+0001f690: 2023 2061 6464 2074 6865 7365 2068 6572   # add these her
+0001f6a0: 652e 0a20 2020 2020 2020 206d 6574 6164  e..        metad
+0001f6b0: 6174 6120 3d20 7475 706c 6528 6d65 7461  ata = tuple(meta
+0001f6c0: 6461 7461 2920 2b20 280a 2020 2020 2020  data) + (.      
+0001f6d0: 2020 2020 2020 6761 7069 635f 7631 2e72        gapic_v1.r
+0001f6e0: 6f75 7469 6e67 5f68 6561 6465 722e 746f  outing_header.to
+0001f6f0: 5f67 7270 635f 6d65 7461 6461 7461 2828  _grpc_metadata((
+0001f700: 2822 7061 7265 6e74 222c 2072 6571 7565  ("parent", reque
+0001f710: 7374 2e70 6172 656e 7429 2c29 292c 0a20  st.parent),)),. 
+0001f720: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+0001f730: 2020 2320 5661 6c69 6461 7465 2074 6865    # Validate the
+0001f740: 2075 6e69 7665 7273 6520 646f 6d61 696e   universe domain
+0001f750: 2e0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+0001f760: 636c 6965 6e74 2e5f 7661 6c69 6461 7465  client._validate
+0001f770: 5f75 6e69 7665 7273 655f 646f 6d61 696e  _universe_domain
+0001f780: 2829 0a0a 2020 2020 2020 2020 2320 5365  ()..        # Se
+0001f790: 6e64 2074 6865 2072 6571 7565 7374 2e0a  nd the request..
+0001f7a0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+0001f7b0: 203d 2061 7761 6974 2072 7063 280a 2020   = await rpc(.  
+0001f7c0: 2020 2020 2020 2020 2020 7265 7175 6573            reques
+0001f7d0: 742c 0a20 2020 2020 2020 2020 2020 2072  t,.            r
+0001f7e0: 6574 7279 3d72 6574 7279 2c0a 2020 2020  etry=retry,.    
+0001f7f0: 2020 2020 2020 2020 7469 6d65 6f75 743d          timeout=
+0001f800: 7469 6d65 6f75 742c 0a20 2020 2020 2020  timeout,.       
+0001f810: 2020 2020 206d 6574 6164 6174 613d 6d65       metadata=me
+0001f820: 7461 6461 7461 2c0a 2020 2020 2020 2020  tadata,.        
+0001f830: 290a 0a20 2020 2020 2020 2023 2054 6869  )..        # Thi
+0001f840: 7320 6d65 7468 6f64 2069 7320 7061 6765  s method is page
+0001f850: 643b 2077 7261 7020 7468 6520 7265 7370  d; wrap the resp
+0001f860: 6f6e 7365 2069 6e20 6120 7061 6765 722c  onse in a pager,
+0001f870: 2077 6869 6368 2070 726f 7669 6465 730a   which provides.
+0001f880: 2020 2020 2020 2020 2320 616e 2060 5f5f          # an `__
+0001f890: 6169 7465 725f 5f60 2063 6f6e 7665 6e69  aiter__` conveni
+0001f8a0: 656e 6365 206d 6574 686f 642e 0a20 2020  ence method..   
+0001f8b0: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
+0001f8c0: 7061 6765 7273 2e4c 6973 7452 6561 6374  pagers.ListReact
+0001f8d0: 696f 6e73 4173 796e 6350 6167 6572 280a  ionsAsyncPager(.
+0001f8e0: 2020 2020 2020 2020 2020 2020 6d65 7468              meth
+0001f8f0: 6f64 3d72 7063 2c0a 2020 2020 2020 2020  od=rpc,.        
+0001f900: 2020 2020 7265 7175 6573 743d 7265 7175      request=requ
+0001f910: 6573 742c 0a20 2020 2020 2020 2020 2020  est,.           
+0001f920: 2072 6573 706f 6e73 653d 7265 7370 6f6e   response=respon
+0001f930: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+0001f940: 6d65 7461 6461 7461 3d6d 6574 6164 6174  metadata=metadat
+0001f950: 612c 0a20 2020 2020 2020 2029 0a0a 2020  a,.        )..  
+0001f960: 2020 2020 2020 2320 446f 6e65 3b20 7265        # Done; re
+0001f970: 7475 726e 2074 6865 2072 6573 706f 6e73  turn the respons
+0001f980: 652e 0a20 2020 2020 2020 2072 6574 7572  e..        retur
+0001f990: 6e20 7265 7370 6f6e 7365 0a0a 2020 2020  n response..    
+0001f9a0: 6173 796e 6320 6465 6620 6465 6c65 7465  async def delete
+0001f9b0: 5f72 6561 6374 696f 6e28 0a20 2020 2020  _reaction(.     
+0001f9c0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0001f9d0: 2072 6571 7565 7374 3a20 4f70 7469 6f6e   request: Option
+0001f9e0: 616c 5b55 6e69 6f6e 5b72 6561 6374 696f  al[Union[reactio
+0001f9f0: 6e2e 4465 6c65 7465 5265 6163 7469 6f6e  n.DeleteReaction
+0001fa00: 5265 7175 6573 742c 2064 6963 745d 5d20  Request, dict]] 
+0001fa10: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0001fa20: 2a2c 0a20 2020 2020 2020 206e 616d 653a  *,.        name:
+0001fa30: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+0001fa40: 204e 6f6e 652c 0a20 2020 2020 2020 2072   None,.        r
+0001fa50: 6574 7279 3a20 4f70 7469 6f6e 616c 5265  etry: OptionalRe
+0001fa60: 7472 7920 3d20 6761 7069 635f 7631 2e6d  try = gapic_v1.m
+0001fa70: 6574 686f 642e 4445 4641 554c 542c 0a20  ethod.DEFAULT,. 
+0001fa80: 2020 2020 2020 2074 696d 656f 7574 3a20         timeout: 
+0001fa90: 556e 696f 6e5b 666c 6f61 742c 206f 626a  Union[float, obj
+0001faa0: 6563 745d 203d 2067 6170 6963 5f76 312e  ect] = gapic_v1.
+0001fab0: 6d65 7468 6f64 2e44 4546 4155 4c54 2c0a  method.DEFAULT,.
+0001fac0: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
+0001fad0: 3a20 5365 7175 656e 6365 5b54 7570 6c65  : Sequence[Tuple
+0001fae0: 5b73 7472 2c20 7374 725d 5d20 3d20 2829  [str, str]] = ()
+0001faf0: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
+0001fb00: 0a20 2020 2020 2020 2072 2222 2244 656c  .        r"""Del
+0001fb10: 6574 6573 2061 2072 6561 6374 696f 6e20  etes a reaction 
+0001fb20: 746f 2061 206d 6573 7361 6765 2e20 4f6e  to a message. On
+0001fb30: 6c79 2075 6e69 636f 6465 2065 6d6f 6a69  ly unicode emoji
+0001fb40: 7320 6172 650a 2020 2020 2020 2020 7375  s are.        su
+0001fb50: 7070 6f72 7465 642e 2046 6f72 2061 6e20  pported. For an 
+0001fb60: 6578 616d 706c 652c 2073 6565 2060 4465  example, see `De
+0001fb70: 6c65 7465 2061 0a20 2020 2020 2020 2072  lete a.        r
+0001fb80: 6561 6374 696f 6e20 3c68 7474 7073 3a2f  eaction <https:/
+0001fb90: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
+0001fba0: 6c65 2e63 6f6d 2f77 6f72 6b73 7061 6365  le.com/workspace
+0001fbb0: 2f63 6861 742f 6465 6c65 7465 2d72 6561  /chat/delete-rea
+0001fbc0: 6374 696f 6e73 3e60 5f5f 2e0a 2020 2020  ctions>`__..    
+0001fbd0: 2020 2020 5265 7175 6972 6573 2060 7573      Requires `us
+0001fbe0: 6572 0a20 2020 2020 2020 2061 7574 6865  er.        authe
+0001fbf0: 6e74 6963 6174 696f 6e20 3c68 7474 7073  ntication <https
+0001fc00: 3a2f 2f64 6576 656c 6f70 6572 732e 676f  ://developers.go
+0001fc10: 6f67 6c65 2e63 6f6d 2f77 6f72 6b73 7061  ogle.com/workspa
+0001fc20: 6365 2f63 6861 742f 6175 7468 656e 7469  ce/chat/authenti
+0001fc30: 6361 7465 2d61 7574 686f 7269 7a65 2d63  cate-authorize-c
+0001fc40: 6861 742d 7573 6572 3e60 5f5f 2e0a 0a20  hat-user>`__... 
+0001fc50: 2020 2020 2020 202e 2e20 636f 6465 2d62         .. code-b
+0001fc60: 6c6f 636b 3a3a 2070 7974 686f 6e0a 0a20  lock:: python.. 
+0001fc70: 2020 2020 2020 2020 2020 2023 2054 6869             # Thi
+0001fc80: 7320 736e 6970 7065 7420 6861 7320 6265  s snippet has be
+0001fc90: 656e 2061 7574 6f6d 6174 6963 616c 6c79  en automatically
+0001fca0: 2067 656e 6572 6174 6564 2061 6e64 2073   generated and s
+0001fcb0: 686f 756c 6420 6265 2072 6567 6172 6465  hould be regarde
+0001fcc0: 6420 6173 2061 0a20 2020 2020 2020 2020  d as a.         
+0001fcd0: 2020 2023 2063 6f64 6520 7465 6d70 6c61     # code templa
+0001fce0: 7465 206f 6e6c 792e 0a20 2020 2020 2020  te only..       
+0001fcf0: 2020 2020 2023 2049 7420 7769 6c6c 2072       # It will r
+0001fd00: 6571 7569 7265 206d 6f64 6966 6963 6174  equire modificat
+0001fd10: 696f 6e73 2074 6f20 776f 726b 3a0a 2020  ions to work:.  
+0001fd20: 2020 2020 2020 2020 2020 2320 2d20 4974            # - It
+0001fd30: 206d 6179 2072 6571 7569 7265 2063 6f72   may require cor
+0001fd40: 7265 6374 2f69 6e2d 7261 6e67 6520 7661  rect/in-range va
+0001fd50: 6c75 6573 2066 6f72 2072 6571 7565 7374  lues for request
+0001fd60: 2069 6e69 7469 616c 697a 6174 696f 6e2e   initialization.
+0001fd70: 0a20 2020 2020 2020 2020 2020 2023 202d  .            # -
+0001fd80: 2049 7420 6d61 7920 7265 7175 6972 6520   It may require 
+0001fd90: 7370 6563 6966 7969 6e67 2072 6567 696f  specifying regio
+0001fda0: 6e61 6c20 656e 6470 6f69 6e74 7320 7768  nal endpoints wh
+0001fdb0: 656e 2063 7265 6174 696e 6720 7468 6520  en creating the 
+0001fdc0: 7365 7276 6963 650a 2020 2020 2020 2020  service.        
+0001fdd0: 2020 2020 2320 2020 636c 6965 6e74 2061      #   client a
+0001fde0: 7320 7368 6f77 6e20 696e 3a0a 2020 2020  s shown in:.    
+0001fdf0: 2020 2020 2020 2020 2320 2020 6874 7470          #   http
+0001fe00: 733a 2f2f 676f 6f67 6c65 6170 6973 2e64  s://googleapis.d
+0001fe10: 6576 2f70 7974 686f 6e2f 676f 6f67 6c65  ev/python/google
+0001fe20: 2d61 7069 2d63 6f72 652f 6c61 7465 7374  -api-core/latest
+0001fe30: 2f63 6c69 656e 745f 6f70 7469 6f6e 732e  /client_options.
+0001fe40: 6874 6d6c 0a20 2020 2020 2020 2020 2020  html.           
+0001fe50: 2066 726f 6d20 676f 6f67 6c65 2e61 7070   from google.app
+0001fe60: 7320 696d 706f 7274 2063 6861 745f 7631  s import chat_v1
+0001fe70: 0a0a 2020 2020 2020 2020 2020 2020 6173  ..            as
+0001fe80: 796e 6320 6465 6620 7361 6d70 6c65 5f64  ync def sample_d
+0001fe90: 656c 6574 655f 7265 6163 7469 6f6e 2829  elete_reaction()
+0001fea0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001feb0: 2020 2320 4372 6561 7465 2061 2063 6c69    # Create a cli
+0001fec0: 656e 740a 2020 2020 2020 2020 2020 2020  ent.            
+0001fed0: 2020 2020 636c 6965 6e74 203d 2063 6861      client = cha
+0001fee0: 745f 7631 2e43 6861 7453 6572 7669 6365  t_v1.ChatService
+0001fef0: 4173 796e 6343 6c69 656e 7428 290a 0a20  AsyncClient().. 
+0001ff00: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0001ff10: 2049 6e69 7469 616c 697a 6520 7265 7175   Initialize requ
+0001ff20: 6573 7420 6172 6775 6d65 6e74 2873 290a  est argument(s).
+0001ff30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ff40: 7265 7175 6573 7420 3d20 6368 6174 5f76  request = chat_v
+0001ff50: 312e 4465 6c65 7465 5265 6163 7469 6f6e  1.DeleteReaction
+0001ff60: 5265 7175 6573 7428 0a20 2020 2020 2020  Request(.       
+0001ff70: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+0001ff80: 653d 226e 616d 655f 7661 6c75 6522 2c0a  e="name_value",.
+0001ff90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ffa0: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001ffb0: 2020 2023 204d 616b 6520 7468 6520 7265     # Make the re
+0001ffc0: 7175 6573 740a 2020 2020 2020 2020 2020  quest.          
+0001ffd0: 2020 2020 2020 6177 6169 7420 636c 6965        await clie
+0001ffe0: 6e74 2e64 656c 6574 655f 7265 6163 7469  nt.delete_reacti
+0001fff0: 6f6e 2872 6571 7565 7374 3d72 6571 7565  on(request=reque
+00020000: 7374 290a 0a20 2020 2020 2020 2041 7267  st)..        Arg
+00020010: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
+00020020: 6571 7565 7374 2028 4f70 7469 6f6e 616c  equest (Optional
+00020030: 5b55 6e69 6f6e 5b67 6f6f 676c 652e 6170  [Union[google.ap
+00020040: 7073 2e63 6861 745f 7631 2e74 7970 6573  ps.chat_v1.types
+00020050: 2e44 656c 6574 6552 6561 6374 696f 6e52  .DeleteReactionR
+00020060: 6571 7565 7374 2c20 6469 6374 5d5d 293a  equest, dict]]):
+00020070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020080: 2054 6865 2072 6571 7565 7374 206f 626a   The request obj
+00020090: 6563 742e 2044 656c 6574 6573 2061 2072  ect. Deletes a r
+000200a0: 6561 6374 696f 6e20 746f 2061 206d 6573  eaction to a mes
+000200b0: 7361 6765 2e0a 2020 2020 2020 2020 2020  sage..          
+000200c0: 2020 6e61 6d65 2028 3a63 6c61 7373 3a60    name (:class:`
+000200d0: 7374 7260 293a 0a20 2020 2020 2020 2020  str`):.         
+000200e0: 2020 2020 2020 2052 6571 7569 7265 642e         Required.
+000200f0: 204e 616d 6520 6f66 2074 6865 2072 6561   Name of the rea
+00020100: 6374 696f 6e20 746f 2064 656c 6574 652e  ction to delete.
+00020110: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00020120: 2020 466f 726d 6174 3a0a 2020 2020 2020    Format:.      
+00020130: 2020 2020 2020 2020 2020 6060 7370 6163            ``spac
+00020140: 6573 2f7b 7370 6163 657d 2f6d 6573 7361  es/{space}/messa
+00020150: 6765 732f 7b6d 6573 7361 6765 7d2f 7265  ges/{message}/re
+00020160: 6163 7469 6f6e 732f 7b72 6561 6374 696f  actions/{reactio
+00020170: 6e7d 6060 0a0a 2020 2020 2020 2020 2020  n}``..          
+00020180: 2020 2020 2020 5468 6973 2063 6f72 7265        This corre
+00020190: 7370 6f6e 6473 2074 6f20 7468 6520 6060  sponds to the ``
+000201a0: 6e61 6d65 6060 2066 6965 6c64 0a20 2020  name`` field.   
+000201b0: 2020 2020 2020 2020 2020 2020 206f 6e20               on 
+000201c0: 7468 6520 6060 7265 7175 6573 7460 6020  the ``request`` 
+000201d0: 696e 7374 616e 6365 3b20 6966 2060 6072  instance; if ``r
+000201e0: 6571 7565 7374 6060 2069 7320 7072 6f76  equest`` is prov
+000201f0: 6964 6564 2c20 7468 6973 0a20 2020 2020  ided, this.     
+00020200: 2020 2020 2020 2020 2020 2073 686f 756c             shoul
+00020210: 6420 6e6f 7420 6265 2073 6574 2e0a 2020  d not be set..  
+00020220: 2020 2020 2020 2020 2020 7265 7472 7920            retry 
+00020230: 2867 6f6f 676c 652e 6170 695f 636f 7265  (google.api_core
+00020240: 2e72 6574 7279 5f61 7379 6e63 2e41 7379  .retry_async.Asy
+00020250: 6e63 5265 7472 7929 3a20 4465 7369 676e  ncRetry): Design
+00020260: 6174 696f 6e20 6f66 2077 6861 7420 6572  ation of what er
+00020270: 726f 7273 2c20 6966 2061 6e79 2c0a 2020  rors, if any,.  
+00020280: 2020 2020 2020 2020 2020 2020 2020 7368                sh
+00020290: 6f75 6c64 2062 6520 7265 7472 6965 642e  ould be retried.
+000202a0: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
+000202b0: 656f 7574 2028 666c 6f61 7429 3a20 5468  eout (float): Th
+000202c0: 6520 7469 6d65 6f75 7420 666f 7220 7468  e timeout for th
+000202d0: 6973 2072 6571 7565 7374 2e0a 2020 2020  is request..    
+000202e0: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
+000202f0: 2028 5365 7175 656e 6365 5b54 7570 6c65   (Sequence[Tuple
+00020300: 5b73 7472 2c20 7374 725d 5d29 3a20 5374  [str, str]]): St
+00020310: 7269 6e67 7320 7768 6963 6820 7368 6f75  rings which shou
+00020320: 6c64 2062 650a 2020 2020 2020 2020 2020  ld be.          
+00020330: 2020 2020 2020 7365 6e74 2061 6c6f 6e67        sent along
+00020340: 2077 6974 6820 7468 6520 7265 7175 6573   with the reques
+00020350: 7420 6173 206d 6574 6164 6174 612e 0a20  t as metadata.. 
+00020360: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00020370: 2020 2023 2043 7265 6174 6520 6f72 2063     # Create or c
+00020380: 6f65 7263 6520 6120 7072 6f74 6f62 7566  oerce a protobuf
+00020390: 2072 6571 7565 7374 206f 626a 6563 742e   request object.
+000203a0: 0a20 2020 2020 2020 2023 2051 7569 636b  .        # Quick
+000203b0: 2063 6865 636b 3a20 4966 2077 6520 676f   check: If we go
+000203c0: 7420 6120 7265 7175 6573 7420 6f62 6a65  t a request obje
+000203d0: 6374 2c20 7765 2073 686f 756c 6420 2a6e  ct, we should *n
+000203e0: 6f74 2a20 6861 7665 0a20 2020 2020 2020  ot* have.       
+000203f0: 2023 2067 6f74 7465 6e20 616e 7920 6b65   # gotten any ke
+00020400: 7977 6f72 6420 6172 6775 6d65 6e74 7320  yword arguments 
+00020410: 7468 6174 206d 6170 2074 6f20 7468 6520  that map to the 
+00020420: 7265 7175 6573 742e 0a20 2020 2020 2020  request..       
+00020430: 2068 6173 5f66 6c61 7474 656e 6564 5f70   has_flattened_p
+00020440: 6172 616d 7320 3d20 616e 7928 5b6e 616d  arams = any([nam
+00020450: 655d 290a 2020 2020 2020 2020 6966 2072  e]).        if r
+00020460: 6571 7565 7374 2069 7320 6e6f 7420 4e6f  equest is not No
+00020470: 6e65 2061 6e64 2068 6173 5f66 6c61 7474  ne and has_flatt
+00020480: 656e 6564 5f70 6172 616d 733a 0a20 2020  ened_params:.   
+00020490: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+000204a0: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
+000204b0: 2020 2020 2020 2020 2020 2022 4966 2074             "If t
+000204c0: 6865 2060 7265 7175 6573 7460 2061 7267  he `request` arg
+000204d0: 756d 656e 7420 6973 2073 6574 2c20 7468  ument is set, th
+000204e0: 656e 206e 6f6e 6520 6f66 2022 0a20 2020  en none of ".   
+000204f0: 2020 2020 2020 2020 2020 2020 2022 7468               "th
+00020500: 6520 696e 6469 7669 6475 616c 2066 6965  e individual fie
+00020510: 6c64 2061 7267 756d 656e 7473 2073 686f  ld arguments sho
+00020520: 756c 6420 6265 2073 6574 2e22 0a20 2020  uld be set.".   
+00020530: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00020540: 2020 2020 7265 7175 6573 7420 3d20 7265      request = re
+00020550: 6163 7469 6f6e 2e44 656c 6574 6552 6561  action.DeleteRea
+00020560: 6374 696f 6e52 6571 7565 7374 2872 6571  ctionRequest(req
+00020570: 7565 7374 290a 0a20 2020 2020 2020 2023  uest)..        #
+00020580: 2049 6620 7765 2068 6176 6520 6b65 7977   If we have keyw
+00020590: 6f72 6420 6172 6775 6d65 6e74 7320 636f  ord arguments co
+000205a0: 7272 6573 706f 6e64 696e 6720 746f 2066  rresponding to f
+000205b0: 6965 6c64 7320 6f6e 2074 6865 0a20 2020  ields on the.   
+000205c0: 2020 2020 2023 2072 6571 7565 7374 2c20       # request, 
+000205d0: 6170 706c 7920 7468 6573 652e 0a20 2020  apply these..   
+000205e0: 2020 2020 2069 6620 6e61 6d65 2069 7320       if name is 
+000205f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00020600: 2020 2020 2020 7265 7175 6573 742e 6e61        request.na
+00020610: 6d65 203d 206e 616d 650a 0a20 2020 2020  me = name..     
+00020620: 2020 2023 2057 7261 7020 7468 6520 5250     # Wrap the RP
+00020630: 4320 6d65 7468 6f64 3b20 7468 6973 2061  C method; this a
+00020640: 6464 7320 7265 7472 7920 616e 6420 7469  dds retry and ti
+00020650: 6d65 6f75 7420 696e 666f 726d 6174 696f  meout informatio
+00020660: 6e2c 0a20 2020 2020 2020 2023 2061 6e64  n,.        # and
+00020670: 2066 7269 656e 646c 7920 6572 726f 7220   friendly error 
+00020680: 6861 6e64 6c69 6e67 2e0a 2020 2020 2020  handling..      
+00020690: 2020 7270 6320 3d20 6761 7069 635f 7631    rpc = gapic_v1
+000206a0: 2e6d 6574 686f 645f 6173 796e 632e 7772  .method_async.wr
+000206b0: 6170 5f6d 6574 686f 6428 0a20 2020 2020  ap_method(.     
+000206c0: 2020 2020 2020 2073 656c 662e 5f63 6c69         self._cli
+000206d0: 656e 742e 5f74 7261 6e73 706f 7274 2e64  ent._transport.d
+000206e0: 656c 6574 655f 7265 6163 7469 6f6e 2c0a  elete_reaction,.
+000206f0: 2020 2020 2020 2020 2020 2020 6465 6661              defa
+00020700: 756c 745f 7265 7472 793d 7265 7472 6965  ult_retry=retrie
+00020710: 732e 4173 796e 6352 6574 7279 280a 2020  s.AsyncRetry(.  
+00020720: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00020730: 6974 6961 6c3d 312e 302c 0a20 2020 2020  itial=1.0,.     
+00020740: 2020 2020 2020 2020 2020 206d 6178 696d             maxim
+00020750: 756d 3d31 302e 302c 0a20 2020 2020 2020  um=10.0,.       
+00020760: 2020 2020 2020 2020 206d 756c 7469 706c           multipl
+00020770: 6965 723d 312e 332c 0a20 2020 2020 2020  ier=1.3,.       
+00020780: 2020 2020 2020 2020 2070 7265 6469 6361           predica
+00020790: 7465 3d72 6574 7269 6573 2e69 665f 6578  te=retries.if_ex
+000207a0: 6365 7074 696f 6e5f 7479 7065 280a 2020  ception_type(.  
+000207b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000207c0: 2020 636f 7265 5f65 7863 6570 7469 6f6e    core_exception
+000207d0: 732e 5365 7276 6963 6555 6e61 7661 696c  s.ServiceUnavail
+000207e0: 6162 6c65 2c0a 2020 2020 2020 2020 2020  able,.          
+000207f0: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+00020800: 2020 2020 2020 2020 2064 6561 646c 696e           deadlin
+00020810: 653d 3330 2e30 2c0a 2020 2020 2020 2020  e=30.0,.        
+00020820: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+00020830: 2020 2064 6566 6175 6c74 5f74 696d 656f     default_timeo
+00020840: 7574 3d33 302e 302c 0a20 2020 2020 2020  ut=30.0,.       
+00020850: 2020 2020 2063 6c69 656e 745f 696e 666f       client_info
+00020860: 3d44 4546 4155 4c54 5f43 4c49 454e 545f  =DEFAULT_CLIENT_
+00020870: 494e 464f 2c0a 2020 2020 2020 2020 290a  INFO,.        ).
+00020880: 0a20 2020 2020 2020 2023 2043 6572 7461  .        # Certa
+00020890: 696e 2066 6965 6c64 7320 7368 6f75 6c64  in fields should
+000208a0: 2062 6520 7072 6f76 6964 6564 2077 6974   be provided wit
+000208b0: 6869 6e20 7468 6520 6d65 7461 6461 7461  hin the metadata
+000208c0: 2068 6561 6465 723b 0a20 2020 2020 2020   header;.       
+000208d0: 2023 2061 6464 2074 6865 7365 2068 6572   # add these her
+000208e0: 652e 0a20 2020 2020 2020 206d 6574 6164  e..        metad
+000208f0: 6174 6120 3d20 7475 706c 6528 6d65 7461  ata = tuple(meta
+00020900: 6461 7461 2920 2b20 280a 2020 2020 2020  data) + (.      
+00020910: 2020 2020 2020 6761 7069 635f 7631 2e72        gapic_v1.r
+00020920: 6f75 7469 6e67 5f68 6561 6465 722e 746f  outing_header.to
+00020930: 5f67 7270 635f 6d65 7461 6461 7461 2828  _grpc_metadata((
+00020940: 2822 6e61 6d65 222c 2072 6571 7565 7374  ("name", request
+00020950: 2e6e 616d 6529 2c29 292c 0a20 2020 2020  .name),)),.     
+00020960: 2020 2029 0a0a 2020 2020 2020 2020 2320     )..        # 
+00020970: 5661 6c69 6461 7465 2074 6865 2075 6e69  Validate the uni
+00020980: 7665 7273 6520 646f 6d61 696e 2e0a 2020  verse domain..  
+00020990: 2020 2020 2020 7365 6c66 2e5f 636c 6965        self._clie
+000209a0: 6e74 2e5f 7661 6c69 6461 7465 5f75 6e69  nt._validate_uni
+000209b0: 7665 7273 655f 646f 6d61 696e 2829 0a0a  verse_domain()..
+000209c0: 2020 2020 2020 2020 2320 5365 6e64 2074          # Send t
+000209d0: 6865 2072 6571 7565 7374 2e0a 2020 2020  he request..    
+000209e0: 2020 2020 6177 6169 7420 7270 6328 0a20      await rpc(. 
+000209f0: 2020 2020 2020 2020 2020 2072 6571 7565             reque
+00020a00: 7374 2c0a 2020 2020 2020 2020 2020 2020  st,.            
+00020a10: 7265 7472 793d 7265 7472 792c 0a20 2020  retry=retry,.   
+00020a20: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
+00020a30: 3d74 696d 656f 7574 2c0a 2020 2020 2020  =timeout,.      
+00020a40: 2020 2020 2020 6d65 7461 6461 7461 3d6d        metadata=m
+00020a50: 6574 6164 6174 612c 0a20 2020 2020 2020  etadata,.       
+00020a60: 2029 0a0a 2020 2020 6173 796e 6320 6465   )..    async de
+00020a70: 6620 5f5f 6165 6e74 6572 5f5f 2873 656c  f __aenter__(sel
+00020a80: 6629 202d 3e20 2243 6861 7453 6572 7669  f) -> "ChatServi
+00020a90: 6365 4173 796e 6343 6c69 656e 7422 3a0a  ceAsyncClient":.
+00020aa0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00020ab0: 656c 660a 0a20 2020 2061 7379 6e63 2064  elf..    async d
+00020ac0: 6566 205f 5f61 6578 6974 5f5f 2873 656c  ef __aexit__(sel
+00020ad0: 662c 2065 7863 5f74 7970 652c 2065 7863  f, exc_type, exc
+00020ae0: 2c20 7462 293a 0a20 2020 2020 2020 2061  , tb):.        a
+00020af0: 7761 6974 2073 656c 662e 7472 616e 7370  wait self.transp
+00020b00: 6f72 742e 636c 6f73 6528 290a 0a0a 4445  ort.close()...DE
+00020b10: 4641 554c 545f 434c 4945 4e54 5f49 4e46  FAULT_CLIENT_INF
+00020b20: 4f20 3d20 6761 7069 635f 7631 2e63 6c69  O = gapic_v1.cli
+00020b30: 656e 745f 696e 666f 2e43 6c69 656e 7449  ent_info.ClientI
+00020b40: 6e66 6f28 0a20 2020 2067 6170 6963 5f76  nfo(.    gapic_v
+00020b50: 6572 7369 6f6e 3d70 6163 6b61 6765 5f76  ersion=package_v
+00020b60: 6572 7369 6f6e 2e5f 5f76 6572 7369 6f6e  ersion.__version
+00020b70: 5f5f 0a29 0a0a 0a5f 5f61 6c6c 5f5f 203d  __.)...__all__ =
+00020b80: 2028 2243 6861 7453 6572 7669 6365 4173   ("ChatServiceAs
+00020b90: 796e 6343 6c69 656e 7422 2c29 0a         yncClient",).
```

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/services/chat_service/client.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/services/chat_service/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -7752,1246 +7752,1569 @@
 0001e470: 696d 656f 7574 2c0a 2020 2020 2020 2020  imeout,.        
 0001e480: 2020 2020 6d65 7461 6461 7461 3d6d 6574      metadata=met
 0001e490: 6164 6174 612c 0a20 2020 2020 2020 2029  adata,.        )
 0001e4a0: 0a0a 2020 2020 2020 2020 2320 446f 6e65  ..        # Done
 0001e4b0: 3b20 7265 7475 726e 2074 6865 2072 6573  ; return the res
 0001e4c0: 706f 6e73 652e 0a20 2020 2020 2020 2072  ponse..        r
 0001e4d0: 6574 7572 6e20 7265 7370 6f6e 7365 0a0a  eturn response..
-0001e4e0: 2020 2020 6465 6620 6465 6c65 7465 5f6d      def delete_m
+0001e4e0: 2020 2020 6465 6620 7570 6461 7465 5f6d      def update_m
 0001e4f0: 656d 6265 7273 6869 7028 0a20 2020 2020  embership(.     
 0001e500: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
 0001e510: 2072 6571 7565 7374 3a20 4f70 7469 6f6e   request: Option
-0001e520: 616c 5b55 6e69 6f6e 5b6d 656d 6265 7273  al[Union[members
-0001e530: 6869 702e 4465 6c65 7465 4d65 6d62 6572  hip.DeleteMember
-0001e540: 7368 6970 5265 7175 6573 742c 2064 6963  shipRequest, dic
-0001e550: 745d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  t]] = None,.    
-0001e560: 2020 2020 2a2c 0a20 2020 2020 2020 206e      *,.        n
-0001e570: 616d 653a 204f 7074 696f 6e61 6c5b 7374  ame: Optional[st
-0001e580: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-0001e590: 2020 2072 6574 7279 3a20 4f70 7469 6f6e     retry: Option
-0001e5a0: 616c 5265 7472 7920 3d20 6761 7069 635f  alRetry = gapic_
-0001e5b0: 7631 2e6d 6574 686f 642e 4445 4641 554c  v1.method.DEFAUL
-0001e5c0: 542c 0a20 2020 2020 2020 2074 696d 656f  T,.        timeo
-0001e5d0: 7574 3a20 556e 696f 6e5b 666c 6f61 742c  ut: Union[float,
-0001e5e0: 206f 626a 6563 745d 203d 2067 6170 6963   object] = gapic
-0001e5f0: 5f76 312e 6d65 7468 6f64 2e44 4546 4155  _v1.method.DEFAU
-0001e600: 4c54 2c0a 2020 2020 2020 2020 6d65 7461  LT,.        meta
-0001e610: 6461 7461 3a20 5365 7175 656e 6365 5b54  data: Sequence[T
-0001e620: 7570 6c65 5b73 7472 2c20 7374 725d 5d20  uple[str, str]] 
-0001e630: 3d20 2829 2c0a 2020 2020 2920 2d3e 206d  = (),.    ) -> m
-0001e640: 656d 6265 7273 6869 702e 4d65 6d62 6572  embership.Member
-0001e650: 7368 6970 3a0a 2020 2020 2020 2020 7222  ship:.        r"
-0001e660: 2222 4465 6c65 7465 7320 6120 6d65 6d62  ""Deletes a memb
-0001e670: 6572 7368 6970 2e20 466f 7220 616e 2065  ership. For an e
-0001e680: 7861 6d70 6c65 2c20 7365 6520 6052 656d  xample, see `Rem
-0001e690: 6f76 6520 6120 7573 6572 206f 7220 610a  ove a user or a.
-0001e6a0: 2020 2020 2020 2020 476f 6f67 6c65 2043          Google C
-0001e6b0: 6861 7420 6170 7020 6672 6f6d 2061 0a20  hat app from a. 
-0001e6c0: 2020 2020 2020 2073 7061 6365 203c 6874         space <ht
-0001e6d0: 7470 733a 2f2f 6465 7665 6c6f 7065 7273  tps://developers
-0001e6e0: 2e67 6f6f 676c 652e 636f 6d2f 776f 726b  .google.com/work
-0001e6f0: 7370 6163 652f 6368 6174 2f64 656c 6574  space/chat/delet
-0001e700: 652d 6d65 6d62 6572 733e 605f 5f2e 0a0a  e-members>`__...
-0001e710: 2020 2020 2020 2020 5265 7175 6972 6573          Requires
-0001e720: 2060 7573 6572 0a20 2020 2020 2020 2061   `user.        a
-0001e730: 7574 6865 6e74 6963 6174 696f 6e20 3c68  uthentication <h
-0001e740: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
-0001e750: 732e 676f 6f67 6c65 2e63 6f6d 2f77 6f72  s.google.com/wor
-0001e760: 6b73 7061 6365 2f63 6861 742f 6175 7468  kspace/chat/auth
-0001e770: 656e 7469 6361 7465 2d61 7574 686f 7269  enticate-authori
-0001e780: 7a65 2d63 6861 742d 7573 6572 3e60 5f5f  ze-chat-user>`__
-0001e790: 2e0a 0a20 2020 2020 2020 202e 2e20 636f  ...        .. co
-0001e7a0: 6465 2d62 6c6f 636b 3a3a 2070 7974 686f  de-block:: pytho
-0001e7b0: 6e0a 0a20 2020 2020 2020 2020 2020 2023  n..            #
-0001e7c0: 2054 6869 7320 736e 6970 7065 7420 6861   This snippet ha
-0001e7d0: 7320 6265 656e 2061 7574 6f6d 6174 6963  s been automatic
-0001e7e0: 616c 6c79 2067 656e 6572 6174 6564 2061  ally generated a
-0001e7f0: 6e64 2073 686f 756c 6420 6265 2072 6567  nd should be reg
-0001e800: 6172 6465 6420 6173 2061 0a20 2020 2020  arded as a.     
-0001e810: 2020 2020 2020 2023 2063 6f64 6520 7465         # code te
-0001e820: 6d70 6c61 7465 206f 6e6c 792e 0a20 2020  mplate only..   
-0001e830: 2020 2020 2020 2020 2023 2049 7420 7769           # It wi
-0001e840: 6c6c 2072 6571 7569 7265 206d 6f64 6966  ll require modif
-0001e850: 6963 6174 696f 6e73 2074 6f20 776f 726b  ications to work
-0001e860: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-0001e870: 2d20 4974 206d 6179 2072 6571 7569 7265  - It may require
-0001e880: 2063 6f72 7265 6374 2f69 6e2d 7261 6e67   correct/in-rang
-0001e890: 6520 7661 6c75 6573 2066 6f72 2072 6571  e values for req
-0001e8a0: 7565 7374 2069 6e69 7469 616c 697a 6174  uest initializat
-0001e8b0: 696f 6e2e 0a20 2020 2020 2020 2020 2020  ion..           
-0001e8c0: 2023 202d 2049 7420 6d61 7920 7265 7175   # - It may requ
-0001e8d0: 6972 6520 7370 6563 6966 7969 6e67 2072  ire specifying r
-0001e8e0: 6567 696f 6e61 6c20 656e 6470 6f69 6e74  egional endpoint
-0001e8f0: 7320 7768 656e 2063 7265 6174 696e 6720  s when creating 
-0001e900: 7468 6520 7365 7276 6963 650a 2020 2020  the service.    
-0001e910: 2020 2020 2020 2020 2320 2020 636c 6965          #   clie
-0001e920: 6e74 2061 7320 7368 6f77 6e20 696e 3a0a  nt as shown in:.
-0001e930: 2020 2020 2020 2020 2020 2020 2320 2020              #   
-0001e940: 6874 7470 733a 2f2f 676f 6f67 6c65 6170  https://googleap
-0001e950: 6973 2e64 6576 2f70 7974 686f 6e2f 676f  is.dev/python/go
-0001e960: 6f67 6c65 2d61 7069 2d63 6f72 652f 6c61  ogle-api-core/la
-0001e970: 7465 7374 2f63 6c69 656e 745f 6f70 7469  test/client_opti
-0001e980: 6f6e 732e 6874 6d6c 0a20 2020 2020 2020  ons.html.       
-0001e990: 2020 2020 2066 726f 6d20 676f 6f67 6c65       from google
-0001e9a0: 2e61 7070 7320 696d 706f 7274 2063 6861  .apps import cha
-0001e9b0: 745f 7631 0a0a 2020 2020 2020 2020 2020  t_v1..          
-0001e9c0: 2020 6465 6620 7361 6d70 6c65 5f64 656c    def sample_del
-0001e9d0: 6574 655f 6d65 6d62 6572 7368 6970 2829  ete_membership()
-0001e9e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001e9f0: 2020 2320 4372 6561 7465 2061 2063 6c69    # Create a cli
-0001ea00: 656e 740a 2020 2020 2020 2020 2020 2020  ent.            
-0001ea10: 2020 2020 636c 6965 6e74 203d 2063 6861      client = cha
-0001ea20: 745f 7631 2e43 6861 7453 6572 7669 6365  t_v1.ChatService
-0001ea30: 436c 6965 6e74 2829 0a0a 2020 2020 2020  Client()..      
-0001ea40: 2020 2020 2020 2020 2020 2320 496e 6974            # Init
-0001ea50: 6961 6c69 7a65 2072 6571 7565 7374 2061  ialize request a
-0001ea60: 7267 756d 656e 7428 7329 0a20 2020 2020  rgument(s).     
-0001ea70: 2020 2020 2020 2020 2020 2072 6571 7565             reque
-0001ea80: 7374 203d 2063 6861 745f 7631 2e44 656c  st = chat_v1.Del
-0001ea90: 6574 654d 656d 6265 7273 6869 7052 6571  eteMembershipReq
-0001eaa0: 7565 7374 280a 2020 2020 2020 2020 2020  uest(.          
-0001eab0: 2020 2020 2020 2020 2020 6e61 6d65 3d22            name="
-0001eac0: 6e61 6d65 5f76 616c 7565 222c 0a20 2020  name_value",.   
-0001ead0: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
-0001eae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eaf0: 2320 4d61 6b65 2074 6865 2072 6571 7565  # Make the reque
-0001eb00: 7374 0a20 2020 2020 2020 2020 2020 2020  st.             
-0001eb10: 2020 2072 6573 706f 6e73 6520 3d20 636c     response = cl
-0001eb20: 6965 6e74 2e64 656c 6574 655f 6d65 6d62  ient.delete_memb
-0001eb30: 6572 7368 6970 2872 6571 7565 7374 3d72  ership(request=r
-0001eb40: 6571 7565 7374 290a 0a20 2020 2020 2020  equest)..       
-0001eb50: 2020 2020 2020 2020 2023 2048 616e 646c           # Handl
-0001eb60: 6520 7468 6520 7265 7370 6f6e 7365 0a20  e the response. 
-0001eb70: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0001eb80: 7269 6e74 2872 6573 706f 6e73 6529 0a0a  rint(response)..
-0001eb90: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-0001eba0: 2020 2020 2020 2020 2020 7265 7175 6573            reques
-0001ebb0: 7420 2855 6e69 6f6e 5b67 6f6f 676c 652e  t (Union[google.
-0001ebc0: 6170 7073 2e63 6861 745f 7631 2e74 7970  apps.chat_v1.typ
-0001ebd0: 6573 2e44 656c 6574 654d 656d 6265 7273  es.DeleteMembers
-0001ebe0: 6869 7052 6571 7565 7374 2c20 6469 6374  hipRequest, dict
-0001ebf0: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
-0001ec00: 2020 2020 5468 6520 7265 7175 6573 7420      The request 
-0001ec10: 6f62 6a65 6374 2e20 5265 7175 6573 7420  object. Request 
-0001ec20: 746f 2064 656c 6574 6520 6120 6d65 6d62  to delete a memb
-0001ec30: 6572 7368 6970 2069 6e20 610a 2020 2020  ership in a.    
-0001ec40: 2020 2020 2020 2020 2020 2020 7370 6163              spac
-0001ec50: 652e 0a20 2020 2020 2020 2020 2020 206e  e..            n
-0001ec60: 616d 6520 2873 7472 293a 0a20 2020 2020  ame (str):.     
-0001ec70: 2020 2020 2020 2020 2020 2052 6571 7569             Requi
-0001ec80: 7265 642e 2052 6573 6f75 7263 6520 6e61  red. Resource na
-0001ec90: 6d65 206f 6620 7468 6520 6d65 6d62 6572  me of the member
-0001eca0: 7368 6970 2074 6f20 6465 6c65 7465 2e0a  ship to delete..
-0001ecb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ecc0: 4368 6174 2061 7070 7320 6361 6e20 6465  Chat apps can de
-0001ecd0: 6c65 7465 2068 756d 616e 2075 7365 7273  lete human users
-0001ece0: 2720 6f72 2074 6865 6972 206f 776e 0a20  ' or their own. 
-0001ecf0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0001ed00: 656d 6265 7273 6869 7073 2e20 4368 6174  emberships. Chat
-0001ed10: 2061 7070 7320 6361 6e27 7420 6465 6c65   apps can't dele
-0001ed20: 7465 206f 7468 6572 2061 7070 7327 0a20  te other apps'. 
-0001ed30: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0001ed40: 656d 6265 7273 6869 7073 2e0a 0a20 2020  emberships...   
-0001ed50: 2020 2020 2020 2020 2020 2020 2057 6865               Whe
-0001ed60: 6e20 6465 6c65 7469 6e67 2061 2068 756d  n deleting a hum
-0001ed70: 616e 206d 656d 6265 7273 6869 702c 2072  an membership, r
-0001ed80: 6571 7569 7265 7320 7468 650a 2020 2020  equires the.    
-0001ed90: 2020 2020 2020 2020 2020 2020 6060 6368              ``ch
-0001eda0: 6174 2e6d 656d 6265 7273 6869 7073 6060  at.memberships``
-0001edb0: 2073 636f 7065 2061 6e64 0a20 2020 2020   scope and.     
-0001edc0: 2020 2020 2020 2020 2020 2060 6073 7061             ``spa
-0001edd0: 6365 732f 7b73 7061 6365 7d2f 6d65 6d62  ces/{space}/memb
-0001ede0: 6572 732f 7b6d 656d 6265 727d 6060 2066  ers/{member}`` f
-0001edf0: 6f72 6d61 742e 2059 6f75 2063 616e 2075  ormat. You can u
-0001ee00: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
-0001ee10: 2020 2074 6865 2065 6d61 696c 2061 7320     the email as 
-0001ee20: 616e 2061 6c69 6173 2066 6f72 2060 607b  an alias for ``{
-0001ee30: 6d65 6d62 6572 7d60 602e 2046 6f72 2065  member}``. For e
-0001ee40: 7861 6d70 6c65 2c0a 2020 2020 2020 2020  xample,.        
-0001ee50: 2020 2020 2020 2020 6060 7370 6163 6573          ``spaces
-0001ee60: 2f7b 7370 6163 657d 2f6d 656d 6265 7273  /{space}/members
-0001ee70: 2f65 7861 6d70 6c65 4067 6d61 696c 2e63  /example@gmail.c
-0001ee80: 6f6d 6060 2077 6865 7265 0a20 2020 2020  om`` where.     
-0001ee90: 2020 2020 2020 2020 2020 2060 6065 7861             ``exa
-0001eea0: 6d70 6c65 4067 6d61 696c 2e63 6f6d 6060  mple@gmail.com``
-0001eeb0: 2069 7320 7468 6520 656d 6169 6c20 6f66   is the email of
-0001eec0: 2074 6865 2047 6f6f 676c 6520 4368 6174   the Google Chat
-0001eed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001eee0: 2075 7365 722e 0a0a 2020 2020 2020 2020   user...        
-0001eef0: 2020 2020 2020 2020 5768 656e 2064 656c          When del
-0001ef00: 6574 696e 6720 616e 2061 7070 206d 656d  eting an app mem
-0001ef10: 6265 7273 6869 702c 2072 6571 7569 7265  bership, require
-0001ef20: 7320 7468 650a 2020 2020 2020 2020 2020  s the.          
-0001ef30: 2020 2020 2020 6060 6368 6174 2e6d 656d        ``chat.mem
-0001ef40: 6265 7273 6869 7073 2e61 7070 6060 2073  berships.app`` s
-0001ef50: 636f 7065 2061 6e64 0a20 2020 2020 2020  cope and.       
-0001ef60: 2020 2020 2020 2020 2060 6073 7061 6365           ``space
-0001ef70: 732f 7b73 7061 6365 7d2f 6d65 6d62 6572  s/{space}/member
-0001ef80: 732f 6170 7060 6020 666f 726d 6174 2e0a  s/app`` format..
-0001ef90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001efa0: 2046 6f72 6d61 743a 2060 6073 7061 6365   Format: ``space
-0001efb0: 732f 7b73 7061 6365 7d2f 6d65 6d62 6572  s/{space}/member
-0001efc0: 732f 7b6d 656d 6265 727d 6060 206f 720a  s/{member}`` or.
-0001efd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001efe0: 6060 7370 6163 6573 2f7b 7370 6163 657d  ``spaces/{space}
-0001eff0: 2f6d 656d 6265 7273 2f61 7070 6060 2e0a  /members/app``..
-0001f000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001f010: 2054 6869 7320 636f 7272 6573 706f 6e64   This correspond
-0001f020: 7320 746f 2074 6865 2060 606e 616d 6560  s to the ``name`
-0001f030: 6020 6669 656c 640a 2020 2020 2020 2020  ` field.        
-0001f040: 2020 2020 2020 2020 6f6e 2074 6865 2060          on the `
-0001f050: 6072 6571 7565 7374 6060 2069 6e73 7461  `request`` insta
-0001f060: 6e63 653b 2069 6620 6060 7265 7175 6573  nce; if ``reques
-0001f070: 7460 6020 6973 2070 726f 7669 6465 642c  t`` is provided,
-0001f080: 2074 6869 730a 2020 2020 2020 2020 2020   this.          
-0001f090: 2020 2020 2020 7368 6f75 6c64 206e 6f74        should not
-0001f0a0: 2062 6520 7365 742e 0a20 2020 2020 2020   be set..       
-0001f0b0: 2020 2020 2072 6574 7279 2028 676f 6f67       retry (goog
-0001f0c0: 6c65 2e61 7069 5f63 6f72 652e 7265 7472  le.api_core.retr
-0001f0d0: 792e 5265 7472 7929 3a20 4465 7369 676e  y.Retry): Design
-0001f0e0: 6174 696f 6e20 6f66 2077 6861 7420 6572  ation of what er
-0001f0f0: 726f 7273 2c20 6966 2061 6e79 2c0a 2020  rors, if any,.  
-0001f100: 2020 2020 2020 2020 2020 2020 2020 7368                sh
-0001f110: 6f75 6c64 2062 6520 7265 7472 6965 642e  ould be retried.
-0001f120: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
-0001f130: 656f 7574 2028 666c 6f61 7429 3a20 5468  eout (float): Th
-0001f140: 6520 7469 6d65 6f75 7420 666f 7220 7468  e timeout for th
-0001f150: 6973 2072 6571 7565 7374 2e0a 2020 2020  is request..    
-0001f160: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
-0001f170: 2028 5365 7175 656e 6365 5b54 7570 6c65   (Sequence[Tuple
-0001f180: 5b73 7472 2c20 7374 725d 5d29 3a20 5374  [str, str]]): St
-0001f190: 7269 6e67 7320 7768 6963 6820 7368 6f75  rings which shou
-0001f1a0: 6c64 2062 650a 2020 2020 2020 2020 2020  ld be.          
-0001f1b0: 2020 2020 2020 7365 6e74 2061 6c6f 6e67        sent along
-0001f1c0: 2077 6974 6820 7468 6520 7265 7175 6573   with the reques
-0001f1d0: 7420 6173 206d 6574 6164 6174 612e 0a0a  t as metadata...
-0001f1e0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-0001f1f0: 0a20 2020 2020 2020 2020 2020 2067 6f6f  .            goo
-0001f200: 676c 652e 6170 7073 2e63 6861 745f 7631  gle.apps.chat_v1
-0001f210: 2e74 7970 6573 2e4d 656d 6265 7273 6869  .types.Membershi
-0001f220: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
-0001f230: 2020 2052 6570 7265 7365 6e74 7320 6120     Represents a 
-0001f240: 6d65 6d62 6572 7368 6970 2072 656c 6174  membership relat
-0001f250: 696f 6e20 696e 0a20 2020 2020 2020 2020  ion in.         
-0001f260: 2020 2020 2020 2047 6f6f 676c 6520 4368         Google Ch
-0001f270: 6174 2c20 7375 6368 2061 7320 7768 6574  at, such as whet
-0001f280: 6865 7220 6120 7573 6572 206f 720a 2020  her a user or.  
-0001f290: 2020 2020 2020 2020 2020 2020 2020 4368                Ch
-0001f2a0: 6174 2061 7070 2069 7320 696e 7669 7465  at app is invite
-0001f2b0: 6420 746f 2c20 7061 7274 206f 662c 206f  d to, part of, o
-0001f2c0: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-0001f2d0: 2020 6162 7365 6e74 2066 726f 6d20 6120    absent from a 
-0001f2e0: 7370 6163 652e 0a0a 2020 2020 2020 2020  space...        
-0001f2f0: 2222 220a 2020 2020 2020 2020 2320 4372  """.        # Cr
-0001f300: 6561 7465 206f 7220 636f 6572 6365 2061  eate or coerce a
-0001f310: 2070 726f 746f 6275 6620 7265 7175 6573   protobuf reques
-0001f320: 7420 6f62 6a65 6374 2e0a 2020 2020 2020  t object..      
-0001f330: 2020 2320 5175 6963 6b20 6368 6563 6b3a    # Quick check:
-0001f340: 2049 6620 7765 2067 6f74 2061 2072 6571   If we got a req
-0001f350: 7565 7374 206f 626a 6563 742c 2077 6520  uest object, we 
-0001f360: 7368 6f75 6c64 202a 6e6f 742a 2068 6176  should *not* hav
-0001f370: 650a 2020 2020 2020 2020 2320 676f 7474  e.        # gott
-0001f380: 656e 2061 6e79 206b 6579 776f 7264 2061  en any keyword a
-0001f390: 7267 756d 656e 7473 2074 6861 7420 6d61  rguments that ma
-0001f3a0: 7020 746f 2074 6865 2072 6571 7565 7374  p to the request
-0001f3b0: 2e0a 2020 2020 2020 2020 6861 735f 666c  ..        has_fl
-0001f3c0: 6174 7465 6e65 645f 7061 7261 6d73 203d  attened_params =
-0001f3d0: 2061 6e79 285b 6e61 6d65 5d29 0a20 2020   any([name]).   
-0001f3e0: 2020 2020 2069 6620 7265 7175 6573 7420       if request 
-0001f3f0: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
-0001f400: 6861 735f 666c 6174 7465 6e65 645f 7061  has_flattened_pa
-0001f410: 7261 6d73 3a0a 2020 2020 2020 2020 2020  rams:.          
-0001f420: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-0001f430: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-0001f440: 2020 2020 2249 6620 7468 6520 6072 6571      "If the `req
-0001f450: 7565 7374 6020 6172 6775 6d65 6e74 2069  uest` argument i
-0001f460: 7320 7365 742c 2074 6865 6e20 6e6f 6e65  s set, then none
-0001f470: 206f 6620 220a 2020 2020 2020 2020 2020   of ".          
-0001f480: 2020 2020 2020 2274 6865 2069 6e64 6976        "the indiv
-0001f490: 6964 7561 6c20 6669 656c 6420 6172 6775  idual field argu
-0001f4a0: 6d65 6e74 7320 7368 6f75 6c64 2062 6520  ments should be 
-0001f4b0: 7365 742e 220a 2020 2020 2020 2020 2020  set.".          
-0001f4c0: 2020 290a 0a20 2020 2020 2020 2023 204d    )..        # M
-0001f4d0: 696e 6f72 206f 7074 696d 697a 6174 696f  inor optimizatio
-0001f4e0: 6e20 746f 2061 766f 6964 206d 616b 696e  n to avoid makin
-0001f4f0: 6720 6120 636f 7079 2069 6620 7468 6520  g a copy if the 
-0001f500: 7573 6572 2070 6173 7365 730a 2020 2020  user passes.    
-0001f510: 2020 2020 2320 696e 2061 206d 656d 6265      # in a membe
-0001f520: 7273 6869 702e 4465 6c65 7465 4d65 6d62  rship.DeleteMemb
-0001f530: 6572 7368 6970 5265 7175 6573 742e 0a20  ershipRequest.. 
-0001f540: 2020 2020 2020 2023 2054 6865 7265 2773         # There's
-0001f550: 206e 6f20 7269 736b 206f 6620 6d6f 6469   no risk of modi
-0001f560: 6679 696e 6720 7468 6520 696e 7075 7420  fying the input 
-0001f570: 6173 2077 6527 7665 2061 6c72 6561 6479  as we've already
-0001f580: 2076 6572 6966 6965 640a 2020 2020 2020   verified.      
-0001f590: 2020 2320 7468 6572 6520 6172 6520 6e6f    # there are no
-0001f5a0: 2066 6c61 7474 656e 6564 2066 6965 6c64   flattened field
-0001f5b0: 732e 0a20 2020 2020 2020 2069 6620 6e6f  s..        if no
-0001f5c0: 7420 6973 696e 7374 616e 6365 2872 6571  t isinstance(req
-0001f5d0: 7565 7374 2c20 6d65 6d62 6572 7368 6970  uest, membership
-0001f5e0: 2e44 656c 6574 654d 656d 6265 7273 6869  .DeleteMembershi
-0001f5f0: 7052 6571 7565 7374 293a 0a20 2020 2020  pRequest):.     
-0001f600: 2020 2020 2020 2072 6571 7565 7374 203d         request =
-0001f610: 206d 656d 6265 7273 6869 702e 4465 6c65   membership.Dele
-0001f620: 7465 4d65 6d62 6572 7368 6970 5265 7175  teMembershipRequ
-0001f630: 6573 7428 7265 7175 6573 7429 0a20 2020  est(request).   
-0001f640: 2020 2020 2020 2020 2023 2049 6620 7765           # If we
-0001f650: 2068 6176 6520 6b65 7977 6f72 6420 6172   have keyword ar
-0001f660: 6775 6d65 6e74 7320 636f 7272 6573 706f  guments correspo
-0001f670: 6e64 696e 6720 746f 2066 6965 6c64 7320  nding to fields 
-0001f680: 6f6e 2074 6865 0a20 2020 2020 2020 2020  on the.         
-0001f690: 2020 2023 2072 6571 7565 7374 2c20 6170     # request, ap
-0001f6a0: 706c 7920 7468 6573 652e 0a20 2020 2020  ply these..     
-0001f6b0: 2020 2020 2020 2069 6620 6e61 6d65 2069         if name i
-0001f6c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0001f6d0: 2020 2020 2020 2020 2020 2020 7265 7175              requ
-0001f6e0: 6573 742e 6e61 6d65 203d 206e 616d 650a  est.name = name.
-0001f6f0: 0a20 2020 2020 2020 2023 2057 7261 7020  .        # Wrap 
-0001f700: 7468 6520 5250 4320 6d65 7468 6f64 3b20  the RPC method; 
-0001f710: 7468 6973 2061 6464 7320 7265 7472 7920  this adds retry 
-0001f720: 616e 6420 7469 6d65 6f75 7420 696e 666f  and timeout info
-0001f730: 726d 6174 696f 6e2c 0a20 2020 2020 2020  rmation,.       
-0001f740: 2023 2061 6e64 2066 7269 656e 646c 7920   # and friendly 
-0001f750: 6572 726f 7220 6861 6e64 6c69 6e67 2e0a  error handling..
-0001f760: 2020 2020 2020 2020 7270 6320 3d20 7365          rpc = se
-0001f770: 6c66 2e5f 7472 616e 7370 6f72 742e 5f77  lf._transport._w
-0001f780: 7261 7070 6564 5f6d 6574 686f 6473 5b73  rapped_methods[s
-0001f790: 656c 662e 5f74 7261 6e73 706f 7274 2e64  elf._transport.d
-0001f7a0: 656c 6574 655f 6d65 6d62 6572 7368 6970  elete_membership
-0001f7b0: 5d0a 0a20 2020 2020 2020 2023 2043 6572  ]..        # Cer
-0001f7c0: 7461 696e 2066 6965 6c64 7320 7368 6f75  tain fields shou
-0001f7d0: 6c64 2062 6520 7072 6f76 6964 6564 2077  ld be provided w
-0001f7e0: 6974 6869 6e20 7468 6520 6d65 7461 6461  ithin the metada
-0001f7f0: 7461 2068 6561 6465 723b 0a20 2020 2020  ta header;.     
-0001f800: 2020 2023 2061 6464 2074 6865 7365 2068     # add these h
-0001f810: 6572 652e 0a20 2020 2020 2020 206d 6574  ere..        met
-0001f820: 6164 6174 6120 3d20 7475 706c 6528 6d65  adata = tuple(me
-0001f830: 7461 6461 7461 2920 2b20 280a 2020 2020  tadata) + (.    
-0001f840: 2020 2020 2020 2020 6761 7069 635f 7631          gapic_v1
-0001f850: 2e72 6f75 7469 6e67 5f68 6561 6465 722e  .routing_header.
-0001f860: 746f 5f67 7270 635f 6d65 7461 6461 7461  to_grpc_metadata
-0001f870: 2828 2822 6e61 6d65 222c 2072 6571 7565  ((("name", reque
-0001f880: 7374 2e6e 616d 6529 2c29 292c 0a20 2020  st.name),)),.   
-0001f890: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0001f8a0: 2320 5661 6c69 6461 7465 2074 6865 2075  # Validate the u
-0001f8b0: 6e69 7665 7273 6520 646f 6d61 696e 2e0a  niverse domain..
-0001f8c0: 2020 2020 2020 2020 7365 6c66 2e5f 7661          self._va
-0001f8d0: 6c69 6461 7465 5f75 6e69 7665 7273 655f  lidate_universe_
-0001f8e0: 646f 6d61 696e 2829 0a0a 2020 2020 2020  domain()..      
-0001f8f0: 2020 2320 5365 6e64 2074 6865 2072 6571    # Send the req
-0001f900: 7565 7374 2e0a 2020 2020 2020 2020 7265  uest..        re
-0001f910: 7370 6f6e 7365 203d 2072 7063 280a 2020  sponse = rpc(.  
-0001f920: 2020 2020 2020 2020 2020 7265 7175 6573            reques
-0001f930: 742c 0a20 2020 2020 2020 2020 2020 2072  t,.            r
-0001f940: 6574 7279 3d72 6574 7279 2c0a 2020 2020  etry=retry,.    
-0001f950: 2020 2020 2020 2020 7469 6d65 6f75 743d          timeout=
-0001f960: 7469 6d65 6f75 742c 0a20 2020 2020 2020  timeout,.       
-0001f970: 2020 2020 206d 6574 6164 6174 613d 6d65       metadata=me
-0001f980: 7461 6461 7461 2c0a 2020 2020 2020 2020  tadata,.        
-0001f990: 290a 0a20 2020 2020 2020 2023 2044 6f6e  )..        # Don
-0001f9a0: 653b 2072 6574 7572 6e20 7468 6520 7265  e; return the re
-0001f9b0: 7370 6f6e 7365 2e0a 2020 2020 2020 2020  sponse..        
-0001f9c0: 7265 7475 726e 2072 6573 706f 6e73 650a  return response.
-0001f9d0: 0a20 2020 2064 6566 2063 7265 6174 655f  .    def create_
-0001f9e0: 7265 6163 7469 6f6e 280a 2020 2020 2020  reaction(.      
-0001f9f0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0001fa00: 7265 7175 6573 743a 204f 7074 696f 6e61  request: Optiona
-0001fa10: 6c5b 556e 696f 6e5b 6763 5f72 6561 6374  l[Union[gc_react
-0001fa20: 696f 6e2e 4372 6561 7465 5265 6163 7469  ion.CreateReacti
-0001fa30: 6f6e 5265 7175 6573 742c 2064 6963 745d  onRequest, dict]
-0001fa40: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0001fa50: 2020 2a2c 0a20 2020 2020 2020 2070 6172    *,.        par
-0001fa60: 656e 743a 204f 7074 696f 6e61 6c5b 7374  ent: Optional[st
-0001fa70: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-0001fa80: 2020 2072 6561 6374 696f 6e3a 204f 7074     reaction: Opt
-0001fa90: 696f 6e61 6c5b 6763 5f72 6561 6374 696f  ional[gc_reactio
-0001faa0: 6e2e 5265 6163 7469 6f6e 5d20 3d20 4e6f  n.Reaction] = No
-0001fab0: 6e65 2c0a 2020 2020 2020 2020 7265 7472  ne,.        retr
-0001fac0: 793a 204f 7074 696f 6e61 6c52 6574 7279  y: OptionalRetry
-0001fad0: 203d 2067 6170 6963 5f76 312e 6d65 7468   = gapic_v1.meth
-0001fae0: 6f64 2e44 4546 4155 4c54 2c0a 2020 2020  od.DEFAULT,.    
-0001faf0: 2020 2020 7469 6d65 6f75 743a 2055 6e69      timeout: Uni
-0001fb00: 6f6e 5b66 6c6f 6174 2c20 6f62 6a65 6374  on[float, object
-0001fb10: 5d20 3d20 6761 7069 635f 7631 2e6d 6574  ] = gapic_v1.met
-0001fb20: 686f 642e 4445 4641 554c 542c 0a20 2020  hod.DEFAULT,.   
-0001fb30: 2020 2020 206d 6574 6164 6174 613a 2053       metadata: S
-0001fb40: 6571 7565 6e63 655b 5475 706c 655b 7374  equence[Tuple[st
-0001fb50: 722c 2073 7472 5d5d 203d 2028 292c 0a20  r, str]] = (),. 
-0001fb60: 2020 2029 202d 3e20 6763 5f72 6561 6374     ) -> gc_react
-0001fb70: 696f 6e2e 5265 6163 7469 6f6e 3a0a 2020  ion.Reaction:.  
-0001fb80: 2020 2020 2020 7222 2222 4372 6561 7465        r"""Create
-0001fb90: 7320 6120 7265 6163 7469 6f6e 2061 6e64  s a reaction and
-0001fba0: 2061 6464 7320 6974 2074 6f20 6120 6d65   adds it to a me
-0001fbb0: 7373 6167 652e 204f 6e6c 7920 756e 6963  ssage. Only unic
-0001fbc0: 6f64 6520 656d 6f6a 6973 0a20 2020 2020  ode emojis.     
-0001fbd0: 2020 2061 7265 2073 7570 706f 7274 6564     are supported
-0001fbe0: 2e20 466f 7220 616e 2065 7861 6d70 6c65  . For an example
-0001fbf0: 2c20 7365 6520 6041 6464 2061 2072 6561  , see `Add a rea
-0001fc00: 6374 696f 6e20 746f 2061 0a20 2020 2020  ction to a.     
-0001fc10: 2020 206d 6573 7361 6765 203c 6874 7470     message <http
-0001fc20: 733a 2f2f 6465 7665 6c6f 7065 7273 2e67  s://developers.g
-0001fc30: 6f6f 676c 652e 636f 6d2f 776f 726b 7370  oogle.com/worksp
-0001fc40: 6163 652f 6368 6174 2f63 7265 6174 652d  ace/chat/create-
-0001fc50: 7265 6163 7469 6f6e 733e 605f 5f2e 0a20  reactions>`__.. 
-0001fc60: 2020 2020 2020 2052 6571 7569 7265 7320         Requires 
-0001fc70: 6075 7365 720a 2020 2020 2020 2020 6175  `user.        au
-0001fc80: 7468 656e 7469 6361 7469 6f6e 203c 6874  thentication <ht
-0001fc90: 7470 733a 2f2f 6465 7665 6c6f 7065 7273  tps://developers
-0001fca0: 2e67 6f6f 676c 652e 636f 6d2f 776f 726b  .google.com/work
-0001fcb0: 7370 6163 652f 6368 6174 2f61 7574 6865  space/chat/authe
-0001fcc0: 6e74 6963 6174 652d 6175 7468 6f72 697a  nticate-authoriz
-0001fcd0: 652d 6368 6174 2d75 7365 723e 605f 5f2e  e-chat-user>`__.
-0001fce0: 0a0a 2020 2020 2020 2020 2e2e 2063 6f64  ..        .. cod
-0001fcf0: 652d 626c 6f63 6b3a 3a20 7079 7468 6f6e  e-block:: python
-0001fd00: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0001fd10: 5468 6973 2073 6e69 7070 6574 2068 6173  This snippet has
-0001fd20: 2062 6565 6e20 6175 746f 6d61 7469 6361   been automatica
-0001fd30: 6c6c 7920 6765 6e65 7261 7465 6420 616e  lly generated an
-0001fd40: 6420 7368 6f75 6c64 2062 6520 7265 6761  d should be rega
-0001fd50: 7264 6564 2061 7320 610a 2020 2020 2020  rded as a.      
-0001fd60: 2020 2020 2020 2320 636f 6465 2074 656d        # code tem
-0001fd70: 706c 6174 6520 6f6e 6c79 2e0a 2020 2020  plate only..    
-0001fd80: 2020 2020 2020 2020 2320 4974 2077 696c          # It wil
-0001fd90: 6c20 7265 7175 6972 6520 6d6f 6469 6669  l require modifi
-0001fda0: 6361 7469 6f6e 7320 746f 2077 6f72 6b3a  cations to work:
-0001fdb0: 0a20 2020 2020 2020 2020 2020 2023 202d  .            # -
-0001fdc0: 2049 7420 6d61 7920 7265 7175 6972 6520   It may require 
-0001fdd0: 636f 7272 6563 742f 696e 2d72 616e 6765  correct/in-range
-0001fde0: 2076 616c 7565 7320 666f 7220 7265 7175   values for requ
-0001fdf0: 6573 7420 696e 6974 6961 6c69 7a61 7469  est initializati
-0001fe00: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
-0001fe10: 2320 2d20 4974 206d 6179 2072 6571 7569  # - It may requi
-0001fe20: 7265 2073 7065 6369 6679 696e 6720 7265  re specifying re
-0001fe30: 6769 6f6e 616c 2065 6e64 706f 696e 7473  gional endpoints
-0001fe40: 2077 6865 6e20 6372 6561 7469 6e67 2074   when creating t
-0001fe50: 6865 2073 6572 7669 6365 0a20 2020 2020  he service.     
-0001fe60: 2020 2020 2020 2023 2020 2063 6c69 656e         #   clien
-0001fe70: 7420 6173 2073 686f 776e 2069 6e3a 0a20  t as shown in:. 
-0001fe80: 2020 2020 2020 2020 2020 2023 2020 2068             #   h
-0001fe90: 7474 7073 3a2f 2f67 6f6f 676c 6561 7069  ttps://googleapi
-0001fea0: 732e 6465 762f 7079 7468 6f6e 2f67 6f6f  s.dev/python/goo
-0001feb0: 676c 652d 6170 692d 636f 7265 2f6c 6174  gle-api-core/lat
-0001fec0: 6573 742f 636c 6965 6e74 5f6f 7074 696f  est/client_optio
-0001fed0: 6e73 2e68 746d 6c0a 2020 2020 2020 2020  ns.html.        
-0001fee0: 2020 2020 6672 6f6d 2067 6f6f 676c 652e      from google.
-0001fef0: 6170 7073 2069 6d70 6f72 7420 6368 6174  apps import chat
-0001ff00: 5f76 310a 0a20 2020 2020 2020 2020 2020  _v1..           
-0001ff10: 2064 6566 2073 616d 706c 655f 6372 6561   def sample_crea
-0001ff20: 7465 5f72 6561 6374 696f 6e28 293a 0a20  te_reaction():. 
-0001ff30: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0001ff40: 2043 7265 6174 6520 6120 636c 6965 6e74   Create a client
-0001ff50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ff60: 2063 6c69 656e 7420 3d20 6368 6174 5f76   client = chat_v
-0001ff70: 312e 4368 6174 5365 7276 6963 6543 6c69  1.ChatServiceCli
-0001ff80: 656e 7428 290a 0a20 2020 2020 2020 2020  ent()..         
-0001ff90: 2020 2020 2020 2023 2049 6e69 7469 616c         # Initial
-0001ffa0: 697a 6520 7265 7175 6573 7420 6172 6775  ize request argu
-0001ffb0: 6d65 6e74 2873 290a 2020 2020 2020 2020  ment(s).        
-0001ffc0: 2020 2020 2020 2020 7265 7175 6573 7420          request 
-0001ffd0: 3d20 6368 6174 5f76 312e 4372 6561 7465  = chat_v1.Create
-0001ffe0: 5265 6163 7469 6f6e 5265 7175 6573 7428  ReactionRequest(
-0001fff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020000: 2020 2020 2070 6172 656e 743d 2270 6172       parent="par
-00020010: 656e 745f 7661 6c75 6522 2c0a 2020 2020  ent_value",.    
-00020020: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00020030: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00020040: 204d 616b 6520 7468 6520 7265 7175 6573   Make the reques
-00020050: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-00020060: 2020 7265 7370 6f6e 7365 203d 2063 6c69    response = cli
-00020070: 656e 742e 6372 6561 7465 5f72 6561 6374  ent.create_react
-00020080: 696f 6e28 7265 7175 6573 743d 7265 7175  ion(request=requ
-00020090: 6573 7429 0a0a 2020 2020 2020 2020 2020  est)..          
-000200a0: 2020 2020 2020 2320 4861 6e64 6c65 2074        # Handle t
-000200b0: 6865 2072 6573 706f 6e73 650a 2020 2020  he response.    
-000200c0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-000200d0: 7428 7265 7370 6f6e 7365 290a 0a20 2020  t(response)..   
-000200e0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-000200f0: 2020 2020 2020 2072 6571 7565 7374 2028         request (
-00020100: 556e 696f 6e5b 676f 6f67 6c65 2e61 7070  Union[google.app
-00020110: 732e 6368 6174 5f76 312e 7479 7065 732e  s.chat_v1.types.
-00020120: 4372 6561 7465 5265 6163 7469 6f6e 5265  CreateReactionRe
-00020130: 7175 6573 742c 2064 6963 745d 293a 0a20  quest, dict]):. 
-00020140: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-00020150: 6865 2072 6571 7565 7374 206f 626a 6563  he request objec
-00020160: 742e 2043 7265 6174 6573 2061 2072 6561  t. Creates a rea
-00020170: 6374 696f 6e20 746f 2061 206d 6573 7361  ction to a messa
-00020180: 6765 2e0a 2020 2020 2020 2020 2020 2020  ge..            
-00020190: 7061 7265 6e74 2028 7374 7229 3a0a 2020  parent (str):.  
-000201a0: 2020 2020 2020 2020 2020 2020 2020 5265                Re
-000201b0: 7175 6972 6564 2e20 5468 6520 6d65 7373  quired. The mess
-000201c0: 6167 6520 7768 6572 6520 7468 6520 7265  age where the re
-000201d0: 6163 7469 6f6e 2069 7320 6372 6561 7465  action is create
-000201e0: 642e 0a0a 2020 2020 2020 2020 2020 2020  d...            
-000201f0: 2020 2020 466f 726d 6174 3a20 6060 7370      Format: ``sp
-00020200: 6163 6573 2f7b 7370 6163 657d 2f6d 6573  aces/{space}/mes
-00020210: 7361 6765 732f 7b6d 6573 7361 6765 7d60  sages/{message}`
-00020220: 600a 0a20 2020 2020 2020 2020 2020 2020  `..             
-00020230: 2020 2054 6869 7320 636f 7272 6573 706f     This correspo
-00020240: 6e64 7320 746f 2074 6865 2060 6070 6172  nds to the ``par
-00020250: 656e 7460 6020 6669 656c 640a 2020 2020  ent`` field.    
-00020260: 2020 2020 2020 2020 2020 2020 6f6e 2074              on t
-00020270: 6865 2060 6072 6571 7565 7374 6060 2069  he ``request`` i
-00020280: 6e73 7461 6e63 653b 2069 6620 6060 7265  nstance; if ``re
-00020290: 7175 6573 7460 6020 6973 2070 726f 7669  quest`` is provi
-000202a0: 6465 642c 2074 6869 730a 2020 2020 2020  ded, this.      
-000202b0: 2020 2020 2020 2020 2020 7368 6f75 6c64            should
-000202c0: 206e 6f74 2062 6520 7365 742e 0a20 2020   not be set..   
-000202d0: 2020 2020 2020 2020 2072 6561 6374 696f           reactio
-000202e0: 6e20 2867 6f6f 676c 652e 6170 7073 2e63  n (google.apps.c
-000202f0: 6861 745f 7631 2e74 7970 6573 2e52 6561  hat_v1.types.Rea
-00020300: 6374 696f 6e29 3a0a 2020 2020 2020 2020  ction):.        
-00020310: 2020 2020 2020 2020 5265 7175 6972 6564          Required
-00020320: 2e20 5468 6520 7265 6163 7469 6f6e 2074  . The reaction t
-00020330: 6f20 6372 6561 7465 2e0a 2020 2020 2020  o create..      
-00020340: 2020 2020 2020 2020 2020 5468 6973 2063            This c
-00020350: 6f72 7265 7370 6f6e 6473 2074 6f20 7468  orresponds to th
-00020360: 6520 6060 7265 6163 7469 6f6e 6060 2066  e ``reaction`` f
-00020370: 6965 6c64 0a20 2020 2020 2020 2020 2020  ield.           
-00020380: 2020 2020 206f 6e20 7468 6520 6060 7265       on the ``re
-00020390: 7175 6573 7460 6020 696e 7374 616e 6365  quest`` instance
-000203a0: 3b20 6966 2060 6072 6571 7565 7374 6060  ; if ``request``
-000203b0: 2069 7320 7072 6f76 6964 6564 2c20 7468   is provided, th
-000203c0: 6973 0a20 2020 2020 2020 2020 2020 2020  is.             
-000203d0: 2020 2073 686f 756c 6420 6e6f 7420 6265     should not be
-000203e0: 2073 6574 2e0a 2020 2020 2020 2020 2020   set..          
-000203f0: 2020 7265 7472 7920 2867 6f6f 676c 652e    retry (google.
-00020400: 6170 695f 636f 7265 2e72 6574 7279 2e52  api_core.retry.R
-00020410: 6574 7279 293a 2044 6573 6967 6e61 7469  etry): Designati
-00020420: 6f6e 206f 6620 7768 6174 2065 7272 6f72  on of what error
-00020430: 732c 2069 6620 616e 792c 0a20 2020 2020  s, if any,.     
-00020440: 2020 2020 2020 2020 2020 2073 686f 756c             shoul
-00020450: 6420 6265 2072 6574 7269 6564 2e0a 2020  d be retried..  
-00020460: 2020 2020 2020 2020 2020 7469 6d65 6f75            timeou
-00020470: 7420 2866 6c6f 6174 293a 2054 6865 2074  t (float): The t
-00020480: 696d 656f 7574 2066 6f72 2074 6869 7320  imeout for this 
-00020490: 7265 7175 6573 742e 0a20 2020 2020 2020  request..       
-000204a0: 2020 2020 206d 6574 6164 6174 6120 2853       metadata (S
-000204b0: 6571 7565 6e63 655b 5475 706c 655b 7374  equence[Tuple[st
-000204c0: 722c 2073 7472 5d5d 293a 2053 7472 696e  r, str]]): Strin
-000204d0: 6773 2077 6869 6368 2073 686f 756c 6420  gs which should 
-000204e0: 6265 0a20 2020 2020 2020 2020 2020 2020  be.             
-000204f0: 2020 2073 656e 7420 616c 6f6e 6720 7769     sent along wi
-00020500: 7468 2074 6865 2072 6571 7565 7374 2061  th the request a
-00020510: 7320 6d65 7461 6461 7461 2e0a 0a20 2020  s metadata...   
-00020520: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00020530: 2020 2020 2020 2020 2020 676f 6f67 6c65            google
-00020540: 2e61 7070 732e 6368 6174 5f76 312e 7479  .apps.chat_v1.ty
-00020550: 7065 732e 5265 6163 7469 6f6e 3a0a 2020  pes.Reaction:.  
-00020560: 2020 2020 2020 2020 2020 2020 2020 4120                A 
-00020570: 7265 6163 7469 6f6e 2074 6f20 6120 6d65  reaction to a me
-00020580: 7373 6167 652e 0a20 2020 2020 2020 2022  ssage..        "
-00020590: 2222 0a20 2020 2020 2020 2023 2043 7265  "".        # Cre
-000205a0: 6174 6520 6f72 2063 6f65 7263 6520 6120  ate or coerce a 
-000205b0: 7072 6f74 6f62 7566 2072 6571 7565 7374  protobuf request
-000205c0: 206f 626a 6563 742e 0a20 2020 2020 2020   object..       
-000205d0: 2023 2051 7569 636b 2063 6865 636b 3a20   # Quick check: 
-000205e0: 4966 2077 6520 676f 7420 6120 7265 7175  If we got a requ
-000205f0: 6573 7420 6f62 6a65 6374 2c20 7765 2073  est object, we s
-00020600: 686f 756c 6420 2a6e 6f74 2a20 6861 7665  hould *not* have
-00020610: 0a20 2020 2020 2020 2023 2067 6f74 7465  .        # gotte
-00020620: 6e20 616e 7920 6b65 7977 6f72 6420 6172  n any keyword ar
-00020630: 6775 6d65 6e74 7320 7468 6174 206d 6170  guments that map
-00020640: 2074 6f20 7468 6520 7265 7175 6573 742e   to the request.
-00020650: 0a20 2020 2020 2020 2068 6173 5f66 6c61  .        has_fla
-00020660: 7474 656e 6564 5f70 6172 616d 7320 3d20  ttened_params = 
-00020670: 616e 7928 5b70 6172 656e 742c 2072 6561  any([parent, rea
-00020680: 6374 696f 6e5d 290a 2020 2020 2020 2020  ction]).        
-00020690: 6966 2072 6571 7565 7374 2069 7320 6e6f  if request is no
-000206a0: 7420 4e6f 6e65 2061 6e64 2068 6173 5f66  t None and has_f
-000206b0: 6c61 7474 656e 6564 5f70 6172 616d 733a  lattened_params:
-000206c0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-000206d0: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
-000206e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000206f0: 4966 2074 6865 2060 7265 7175 6573 7460  If the `request`
-00020700: 2061 7267 756d 656e 7420 6973 2073 6574   argument is set
-00020710: 2c20 7468 656e 206e 6f6e 6520 6f66 2022  , then none of "
-00020720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020730: 2022 7468 6520 696e 6469 7669 6475 616c   "the individual
-00020740: 2066 6965 6c64 2061 7267 756d 656e 7473   field arguments
-00020750: 2073 686f 756c 6420 6265 2073 6574 2e22   should be set."
-00020760: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-00020770: 2020 2020 2020 2020 2320 4d69 6e6f 7220          # Minor 
-00020780: 6f70 7469 6d69 7a61 7469 6f6e 2074 6f20  optimization to 
-00020790: 6176 6f69 6420 6d61 6b69 6e67 2061 2063  avoid making a c
-000207a0: 6f70 7920 6966 2074 6865 2075 7365 7220  opy if the user 
-000207b0: 7061 7373 6573 0a20 2020 2020 2020 2023  passes.        #
-000207c0: 2069 6e20 6120 6763 5f72 6561 6374 696f   in a gc_reactio
-000207d0: 6e2e 4372 6561 7465 5265 6163 7469 6f6e  n.CreateReaction
-000207e0: 5265 7175 6573 742e 0a20 2020 2020 2020  Request..       
-000207f0: 2023 2054 6865 7265 2773 206e 6f20 7269   # There's no ri
-00020800: 736b 206f 6620 6d6f 6469 6679 696e 6720  sk of modifying 
-00020810: 7468 6520 696e 7075 7420 6173 2077 6527  the input as we'
-00020820: 7665 2061 6c72 6561 6479 2076 6572 6966  ve already verif
-00020830: 6965 640a 2020 2020 2020 2020 2320 7468  ied.        # th
-00020840: 6572 6520 6172 6520 6e6f 2066 6c61 7474  ere are no flatt
-00020850: 656e 6564 2066 6965 6c64 732e 0a20 2020  ened fields..   
-00020860: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
-00020870: 7374 616e 6365 2872 6571 7565 7374 2c20  stance(request, 
-00020880: 6763 5f72 6561 6374 696f 6e2e 4372 6561  gc_reaction.Crea
-00020890: 7465 5265 6163 7469 6f6e 5265 7175 6573  teReactionReques
-000208a0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-000208b0: 7265 7175 6573 7420 3d20 6763 5f72 6561  request = gc_rea
-000208c0: 6374 696f 6e2e 4372 6561 7465 5265 6163  ction.CreateReac
-000208d0: 7469 6f6e 5265 7175 6573 7428 7265 7175  tionRequest(requ
-000208e0: 6573 7429 0a20 2020 2020 2020 2020 2020  est).           
-000208f0: 2023 2049 6620 7765 2068 6176 6520 6b65   # If we have ke
-00020900: 7977 6f72 6420 6172 6775 6d65 6e74 7320  yword arguments 
-00020910: 636f 7272 6573 706f 6e64 696e 6720 746f  corresponding to
-00020920: 2066 6965 6c64 7320 6f6e 2074 6865 0a20   fields on the. 
-00020930: 2020 2020 2020 2020 2020 2023 2072 6571             # req
-00020940: 7565 7374 2c20 6170 706c 7920 7468 6573  uest, apply thes
-00020950: 652e 0a20 2020 2020 2020 2020 2020 2069  e..            i
-00020960: 6620 7061 7265 6e74 2069 7320 6e6f 7420  f parent is not 
-00020970: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00020980: 2020 2020 2020 7265 7175 6573 742e 7061        request.pa
-00020990: 7265 6e74 203d 2070 6172 656e 740a 2020  rent = parent.  
-000209a0: 2020 2020 2020 2020 2020 6966 2072 6561            if rea
-000209b0: 6374 696f 6e20 6973 206e 6f74 204e 6f6e  ction is not Non
-000209c0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000209d0: 2020 2072 6571 7565 7374 2e72 6561 6374     request.react
-000209e0: 696f 6e20 3d20 7265 6163 7469 6f6e 0a0a  ion = reaction..
-000209f0: 2020 2020 2020 2020 2320 5772 6170 2074          # Wrap t
-00020a00: 6865 2052 5043 206d 6574 686f 643b 2074  he RPC method; t
-00020a10: 6869 7320 6164 6473 2072 6574 7279 2061  his adds retry a
-00020a20: 6e64 2074 696d 656f 7574 2069 6e66 6f72  nd timeout infor
-00020a30: 6d61 7469 6f6e 2c0a 2020 2020 2020 2020  mation,.        
-00020a40: 2320 616e 6420 6672 6965 6e64 6c79 2065  # and friendly e
-00020a50: 7272 6f72 2068 616e 646c 696e 672e 0a20  rror handling.. 
-00020a60: 2020 2020 2020 2072 7063 203d 2073 656c         rpc = sel
-00020a70: 662e 5f74 7261 6e73 706f 7274 2e5f 7772  f._transport._wr
-00020a80: 6170 7065 645f 6d65 7468 6f64 735b 7365  apped_methods[se
-00020a90: 6c66 2e5f 7472 616e 7370 6f72 742e 6372  lf._transport.cr
-00020aa0: 6561 7465 5f72 6561 6374 696f 6e5d 0a0a  eate_reaction]..
-00020ab0: 2020 2020 2020 2020 2320 4365 7274 6169          # Certai
-00020ac0: 6e20 6669 656c 6473 2073 686f 756c 6420  n fields should 
-00020ad0: 6265 2070 726f 7669 6465 6420 7769 7468  be provided with
-00020ae0: 696e 2074 6865 206d 6574 6164 6174 6120  in the metadata 
-00020af0: 6865 6164 6572 3b0a 2020 2020 2020 2020  header;.        
-00020b00: 2320 6164 6420 7468 6573 6520 6865 7265  # add these here
-00020b10: 2e0a 2020 2020 2020 2020 6d65 7461 6461  ..        metada
-00020b20: 7461 203d 2074 7570 6c65 286d 6574 6164  ta = tuple(metad
-00020b30: 6174 6129 202b 2028 0a20 2020 2020 2020  ata) + (.       
-00020b40: 2020 2020 2067 6170 6963 5f76 312e 726f       gapic_v1.ro
-00020b50: 7574 696e 675f 6865 6164 6572 2e74 6f5f  uting_header.to_
-00020b60: 6772 7063 5f6d 6574 6164 6174 6128 2828  grpc_metadata(((
-00020b70: 2270 6172 656e 7422 2c20 7265 7175 6573  "parent", reques
-00020b80: 742e 7061 7265 6e74 292c 2929 2c0a 2020  t.parent),)),.  
-00020b90: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00020ba0: 2023 2056 616c 6964 6174 6520 7468 6520   # Validate the 
-00020bb0: 756e 6976 6572 7365 2064 6f6d 6169 6e2e  universe domain.
-00020bc0: 0a20 2020 2020 2020 2073 656c 662e 5f76  .        self._v
-00020bd0: 616c 6964 6174 655f 756e 6976 6572 7365  alidate_universe
-00020be0: 5f64 6f6d 6169 6e28 290a 0a20 2020 2020  _domain()..     
-00020bf0: 2020 2023 2053 656e 6420 7468 6520 7265     # Send the re
-00020c00: 7175 6573 742e 0a20 2020 2020 2020 2072  quest..        r
-00020c10: 6573 706f 6e73 6520 3d20 7270 6328 0a20  esponse = rpc(. 
-00020c20: 2020 2020 2020 2020 2020 2072 6571 7565             reque
-00020c30: 7374 2c0a 2020 2020 2020 2020 2020 2020  st,.            
-00020c40: 7265 7472 793d 7265 7472 792c 0a20 2020  retry=retry,.   
-00020c50: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
-00020c60: 3d74 696d 656f 7574 2c0a 2020 2020 2020  =timeout,.      
-00020c70: 2020 2020 2020 6d65 7461 6461 7461 3d6d        metadata=m
-00020c80: 6574 6164 6174 612c 0a20 2020 2020 2020  etadata,.       
-00020c90: 2029 0a0a 2020 2020 2020 2020 2320 446f   )..        # Do
-00020ca0: 6e65 3b20 7265 7475 726e 2074 6865 2072  ne; return the r
-00020cb0: 6573 706f 6e73 652e 0a20 2020 2020 2020  esponse..       
-00020cc0: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
-00020cd0: 0a0a 2020 2020 6465 6620 6c69 7374 5f72  ..    def list_r
-00020ce0: 6561 6374 696f 6e73 280a 2020 2020 2020  eactions(.      
-00020cf0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00020d00: 7265 7175 6573 743a 204f 7074 696f 6e61  request: Optiona
-00020d10: 6c5b 556e 696f 6e5b 7265 6163 7469 6f6e  l[Union[reaction
-00020d20: 2e4c 6973 7452 6561 6374 696f 6e73 5265  .ListReactionsRe
-00020d30: 7175 6573 742c 2064 6963 745d 5d20 3d20  quest, dict]] = 
-00020d40: 4e6f 6e65 2c0a 2020 2020 2020 2020 2a2c  None,.        *,
-00020d50: 0a20 2020 2020 2020 2070 6172 656e 743a  .        parent:
-00020d60: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-00020d70: 204e 6f6e 652c 0a20 2020 2020 2020 2072   None,.        r
-00020d80: 6574 7279 3a20 4f70 7469 6f6e 616c 5265  etry: OptionalRe
-00020d90: 7472 7920 3d20 6761 7069 635f 7631 2e6d  try = gapic_v1.m
-00020da0: 6574 686f 642e 4445 4641 554c 542c 0a20  ethod.DEFAULT,. 
-00020db0: 2020 2020 2020 2074 696d 656f 7574 3a20         timeout: 
-00020dc0: 556e 696f 6e5b 666c 6f61 742c 206f 626a  Union[float, obj
-00020dd0: 6563 745d 203d 2067 6170 6963 5f76 312e  ect] = gapic_v1.
-00020de0: 6d65 7468 6f64 2e44 4546 4155 4c54 2c0a  method.DEFAULT,.
-00020df0: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
-00020e00: 3a20 5365 7175 656e 6365 5b54 7570 6c65  : Sequence[Tuple
-00020e10: 5b73 7472 2c20 7374 725d 5d20 3d20 2829  [str, str]] = ()
-00020e20: 2c0a 2020 2020 2920 2d3e 2070 6167 6572  ,.    ) -> pager
-00020e30: 732e 4c69 7374 5265 6163 7469 6f6e 7350  s.ListReactionsP
-00020e40: 6167 6572 3a0a 2020 2020 2020 2020 7222  ager:.        r"
-00020e50: 2222 4c69 7374 7320 7265 6163 7469 6f6e  ""Lists reaction
-00020e60: 7320 746f 2061 206d 6573 7361 6765 2e20  s to a message. 
-00020e70: 466f 7220 616e 2065 7861 6d70 6c65 2c20  For an example, 
-00020e80: 7365 6520 604c 6973 740a 2020 2020 2020  see `List.      
-00020e90: 2020 7265 6163 7469 6f6e 7320 666f 7220    reactions for 
-00020ea0: 610a 2020 2020 2020 2020 6d65 7373 6167  a.        messag
-00020eb0: 6520 3c68 7474 7073 3a2f 2f64 6576 656c  e <https://devel
-00020ec0: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
-00020ed0: 2f77 6f72 6b73 7061 6365 2f63 6861 742f  /workspace/chat/
-00020ee0: 6c69 7374 2d72 6561 6374 696f 6e73 3e60  list-reactions>`
-00020ef0: 5f5f 2e0a 2020 2020 2020 2020 5265 7175  __..        Requ
-00020f00: 6972 6573 2060 7573 6572 0a20 2020 2020  ires `user.     
-00020f10: 2020 2061 7574 6865 6e74 6963 6174 696f     authenticatio
-00020f20: 6e20 3c68 7474 7073 3a2f 2f64 6576 656c  n <https://devel
-00020f30: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
-00020f40: 2f77 6f72 6b73 7061 6365 2f63 6861 742f  /workspace/chat/
-00020f50: 6175 7468 656e 7469 6361 7465 2d61 7574  authenticate-aut
-00020f60: 686f 7269 7a65 2d63 6861 742d 7573 6572  horize-chat-user
-00020f70: 3e60 5f5f 2e0a 0a20 2020 2020 2020 202e  >`__...        .
-00020f80: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2070  . code-block:: p
-00020f90: 7974 686f 6e0a 0a20 2020 2020 2020 2020  ython..         
-00020fa0: 2020 2023 2054 6869 7320 736e 6970 7065     # This snippe
-00020fb0: 7420 6861 7320 6265 656e 2061 7574 6f6d  t has been autom
-00020fc0: 6174 6963 616c 6c79 2067 656e 6572 6174  atically generat
-00020fd0: 6564 2061 6e64 2073 686f 756c 6420 6265  ed and should be
-00020fe0: 2072 6567 6172 6465 6420 6173 2061 0a20   regarded as a. 
-00020ff0: 2020 2020 2020 2020 2020 2023 2063 6f64             # cod
-00021000: 6520 7465 6d70 6c61 7465 206f 6e6c 792e  e template only.
-00021010: 0a20 2020 2020 2020 2020 2020 2023 2049  .            # I
-00021020: 7420 7769 6c6c 2072 6571 7569 7265 206d  t will require m
-00021030: 6f64 6966 6963 6174 696f 6e73 2074 6f20  odifications to 
-00021040: 776f 726b 3a0a 2020 2020 2020 2020 2020  work:.          
-00021050: 2020 2320 2d20 4974 206d 6179 2072 6571    # - It may req
-00021060: 7569 7265 2063 6f72 7265 6374 2f69 6e2d  uire correct/in-
-00021070: 7261 6e67 6520 7661 6c75 6573 2066 6f72  range values for
-00021080: 2072 6571 7565 7374 2069 6e69 7469 616c   request initial
-00021090: 697a 6174 696f 6e2e 0a20 2020 2020 2020  ization..       
-000210a0: 2020 2020 2023 202d 2049 7420 6d61 7920       # - It may 
-000210b0: 7265 7175 6972 6520 7370 6563 6966 7969  require specifyi
-000210c0: 6e67 2072 6567 696f 6e61 6c20 656e 6470  ng regional endp
-000210d0: 6f69 6e74 7320 7768 656e 2063 7265 6174  oints when creat
-000210e0: 696e 6720 7468 6520 7365 7276 6963 650a  ing the service.
-000210f0: 2020 2020 2020 2020 2020 2020 2320 2020              #   
-00021100: 636c 6965 6e74 2061 7320 7368 6f77 6e20  client as shown 
-00021110: 696e 3a0a 2020 2020 2020 2020 2020 2020  in:.            
-00021120: 2320 2020 6874 7470 733a 2f2f 676f 6f67  #   https://goog
-00021130: 6c65 6170 6973 2e64 6576 2f70 7974 686f  leapis.dev/pytho
-00021140: 6e2f 676f 6f67 6c65 2d61 7069 2d63 6f72  n/google-api-cor
-00021150: 652f 6c61 7465 7374 2f63 6c69 656e 745f  e/latest/client_
-00021160: 6f70 7469 6f6e 732e 6874 6d6c 0a20 2020  options.html.   
-00021170: 2020 2020 2020 2020 2066 726f 6d20 676f           from go
-00021180: 6f67 6c65 2e61 7070 7320 696d 706f 7274  ogle.apps import
-00021190: 2063 6861 745f 7631 0a0a 2020 2020 2020   chat_v1..      
-000211a0: 2020 2020 2020 6465 6620 7361 6d70 6c65        def sample
-000211b0: 5f6c 6973 745f 7265 6163 7469 6f6e 7328  _list_reactions(
-000211c0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000211d0: 2020 2023 2043 7265 6174 6520 6120 636c     # Create a cl
-000211e0: 6965 6e74 0a20 2020 2020 2020 2020 2020  ient.           
-000211f0: 2020 2020 2063 6c69 656e 7420 3d20 6368       client = ch
-00021200: 6174 5f76 312e 4368 6174 5365 7276 6963  at_v1.ChatServic
-00021210: 6543 6c69 656e 7428 290a 0a20 2020 2020  eClient()..     
-00021220: 2020 2020 2020 2020 2020 2023 2049 6e69             # Ini
-00021230: 7469 616c 697a 6520 7265 7175 6573 7420  tialize request 
-00021240: 6172 6775 6d65 6e74 2873 290a 2020 2020  argument(s).    
-00021250: 2020 2020 2020 2020 2020 2020 7265 7175              requ
-00021260: 6573 7420 3d20 6368 6174 5f76 312e 4c69  est = chat_v1.Li
-00021270: 7374 5265 6163 7469 6f6e 7352 6571 7565  stReactionsReque
-00021280: 7374 280a 2020 2020 2020 2020 2020 2020  st(.            
-00021290: 2020 2020 2020 2020 7061 7265 6e74 3d22          parent="
-000212a0: 7061 7265 6e74 5f76 616c 7565 222c 0a20  parent_value",. 
-000212b0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000212c0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000212d0: 2020 2320 4d61 6b65 2074 6865 2072 6571    # Make the req
-000212e0: 7565 7374 0a20 2020 2020 2020 2020 2020  uest.           
-000212f0: 2020 2020 2070 6167 655f 7265 7375 6c74       page_result
-00021300: 203d 2063 6c69 656e 742e 6c69 7374 5f72   = client.list_r
-00021310: 6561 6374 696f 6e73 2872 6571 7565 7374  eactions(request
-00021320: 3d72 6571 7565 7374 290a 0a20 2020 2020  =request)..     
-00021330: 2020 2020 2020 2020 2020 2023 2048 616e             # Han
-00021340: 646c 6520 7468 6520 7265 7370 6f6e 7365  dle the response
-00021350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021360: 2066 6f72 2072 6573 706f 6e73 6520 696e   for response in
-00021370: 2070 6167 655f 7265 7375 6c74 3a0a 2020   page_result:.  
-00021380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021390: 2020 7072 696e 7428 7265 7370 6f6e 7365    print(response
-000213a0: 290a 0a20 2020 2020 2020 2041 7267 733a  )..        Args:
-000213b0: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
-000213c0: 7565 7374 2028 556e 696f 6e5b 676f 6f67  uest (Union[goog
-000213d0: 6c65 2e61 7070 732e 6368 6174 5f76 312e  le.apps.chat_v1.
-000213e0: 7479 7065 732e 4c69 7374 5265 6163 7469  types.ListReacti
-000213f0: 6f6e 7352 6571 7565 7374 2c20 6469 6374  onsRequest, dict
-00021400: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
-00021410: 2020 2020 5468 6520 7265 7175 6573 7420      The request 
-00021420: 6f62 6a65 6374 2e20 4c69 7374 7320 7265  object. Lists re
-00021430: 6163 7469 6f6e 7320 746f 2061 206d 6573  actions to a mes
-00021440: 7361 6765 2e0a 2020 2020 2020 2020 2020  sage..          
-00021450: 2020 7061 7265 6e74 2028 7374 7229 3a0a    parent (str):.
-00021460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021470: 5265 7175 6972 6564 2e20 5468 6520 6d65  Required. The me
-00021480: 7373 6167 6520 7573 6572 7320 7265 6163  ssage users reac
-00021490: 7465 6420 746f 2e0a 0a20 2020 2020 2020  ted to...       
-000214a0: 2020 2020 2020 2020 2046 6f72 6d61 743a           Format:
-000214b0: 2060 6073 7061 6365 732f 7b73 7061 6365   ``spaces/{space
-000214c0: 7d2f 6d65 7373 6167 6573 2f7b 6d65 7373  }/messages/{mess
-000214d0: 6167 657d 6060 0a0a 2020 2020 2020 2020  age}``..        
-000214e0: 2020 2020 2020 2020 5468 6973 2063 6f72          This cor
-000214f0: 7265 7370 6f6e 6473 2074 6f20 7468 6520  responds to the 
-00021500: 6060 7061 7265 6e74 6060 2066 6965 6c64  ``parent`` field
-00021510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021520: 206f 6e20 7468 6520 6060 7265 7175 6573   on the ``reques
-00021530: 7460 6020 696e 7374 616e 6365 3b20 6966  t`` instance; if
-00021540: 2060 6072 6571 7565 7374 6060 2069 7320   ``request`` is 
-00021550: 7072 6f76 6964 6564 2c20 7468 6973 0a20  provided, this. 
-00021560: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00021570: 686f 756c 6420 6e6f 7420 6265 2073 6574  hould not be set
-00021580: 2e0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00021590: 7472 7920 2867 6f6f 676c 652e 6170 695f  try (google.api_
-000215a0: 636f 7265 2e72 6574 7279 2e52 6574 7279  core.retry.Retry
-000215b0: 293a 2044 6573 6967 6e61 7469 6f6e 206f  ): Designation o
-000215c0: 6620 7768 6174 2065 7272 6f72 732c 2069  f what errors, i
-000215d0: 6620 616e 792c 0a20 2020 2020 2020 2020  f any,.         
-000215e0: 2020 2020 2020 2073 686f 756c 6420 6265         should be
-000215f0: 2072 6574 7269 6564 2e0a 2020 2020 2020   retried..      
-00021600: 2020 2020 2020 7469 6d65 6f75 7420 2866        timeout (f
-00021610: 6c6f 6174 293a 2054 6865 2074 696d 656f  loat): The timeo
-00021620: 7574 2066 6f72 2074 6869 7320 7265 7175  ut for this requ
-00021630: 6573 742e 0a20 2020 2020 2020 2020 2020  est..           
-00021640: 206d 6574 6164 6174 6120 2853 6571 7565   metadata (Seque
-00021650: 6e63 655b 5475 706c 655b 7374 722c 2073  nce[Tuple[str, s
-00021660: 7472 5d5d 293a 2053 7472 696e 6773 2077  tr]]): Strings w
-00021670: 6869 6368 2073 686f 756c 6420 6265 0a20  hich should be. 
-00021680: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00021690: 656e 7420 616c 6f6e 6720 7769 7468 2074  ent along with t
-000216a0: 6865 2072 6571 7565 7374 2061 7320 6d65  he request as me
-000216b0: 7461 6461 7461 2e0a 0a20 2020 2020 2020  tadata...       
-000216c0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-000216d0: 2020 2020 2020 676f 6f67 6c65 2e61 7070        google.app
-000216e0: 732e 6368 6174 5f76 312e 7365 7276 6963  s.chat_v1.servic
-000216f0: 6573 2e63 6861 745f 7365 7276 6963 652e  es.chat_service.
-00021700: 7061 6765 7273 2e4c 6973 7452 6561 6374  pagers.ListReact
-00021710: 696f 6e73 5061 6765 723a 0a20 2020 2020  ionsPager:.     
-00021720: 2020 2020 2020 2020 2020 2052 6573 706f             Respo
-00021730: 6e73 6520 746f 2061 206c 6973 7420 7265  nse to a list re
-00021740: 6163 7469 6f6e 7320 7265 7175 6573 742e  actions request.
-00021750: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00021760: 2020 4974 6572 6174 696e 6720 6f76 6572    Iterating over
-00021770: 2074 6869 7320 6f62 6a65 6374 2077 696c   this object wil
-00021780: 6c20 7969 656c 640a 2020 2020 2020 2020  l yield.        
-00021790: 2020 2020 2020 2020 7265 7375 6c74 7320          results 
-000217a0: 616e 6420 7265 736f 6c76 6520 6164 6469  and resolve addi
-000217b0: 7469 6f6e 616c 2070 6167 6573 0a20 2020  tional pages.   
-000217c0: 2020 2020 2020 2020 2020 2020 2061 7574               aut
-000217d0: 6f6d 6174 6963 616c 6c79 2e0a 0a20 2020  omatically...   
-000217e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000217f0: 2023 2043 7265 6174 6520 6f72 2063 6f65   # Create or coe
-00021800: 7263 6520 6120 7072 6f74 6f62 7566 2072  rce a protobuf r
-00021810: 6571 7565 7374 206f 626a 6563 742e 0a20  equest object.. 
-00021820: 2020 2020 2020 2023 2051 7569 636b 2063         # Quick c
-00021830: 6865 636b 3a20 4966 2077 6520 676f 7420  heck: If we got 
-00021840: 6120 7265 7175 6573 7420 6f62 6a65 6374  a request object
-00021850: 2c20 7765 2073 686f 756c 6420 2a6e 6f74  , we should *not
-00021860: 2a20 6861 7665 0a20 2020 2020 2020 2023  * have.        #
-00021870: 2067 6f74 7465 6e20 616e 7920 6b65 7977   gotten any keyw
-00021880: 6f72 6420 6172 6775 6d65 6e74 7320 7468  ord arguments th
-00021890: 6174 206d 6170 2074 6f20 7468 6520 7265  at map to the re
-000218a0: 7175 6573 742e 0a20 2020 2020 2020 2068  quest..        h
-000218b0: 6173 5f66 6c61 7474 656e 6564 5f70 6172  as_flattened_par
-000218c0: 616d 7320 3d20 616e 7928 5b70 6172 656e  ams = any([paren
-000218d0: 745d 290a 2020 2020 2020 2020 6966 2072  t]).        if r
-000218e0: 6571 7565 7374 2069 7320 6e6f 7420 4e6f  equest is not No
-000218f0: 6e65 2061 6e64 2068 6173 5f66 6c61 7474  ne and has_flatt
-00021900: 656e 6564 5f70 6172 616d 733a 0a20 2020  ened_params:.   
-00021910: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-00021920: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
-00021930: 2020 2020 2020 2020 2020 2022 4966 2074             "If t
-00021940: 6865 2060 7265 7175 6573 7460 2061 7267  he `request` arg
-00021950: 756d 656e 7420 6973 2073 6574 2c20 7468  ument is set, th
-00021960: 656e 206e 6f6e 6520 6f66 2022 0a20 2020  en none of ".   
-00021970: 2020 2020 2020 2020 2020 2020 2022 7468               "th
-00021980: 6520 696e 6469 7669 6475 616c 2066 6965  e individual fie
-00021990: 6c64 2061 7267 756d 656e 7473 2073 686f  ld arguments sho
-000219a0: 756c 6420 6265 2073 6574 2e22 0a20 2020  uld be set.".   
-000219b0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-000219c0: 2020 2020 2320 4d69 6e6f 7220 6f70 7469      # Minor opti
-000219d0: 6d69 7a61 7469 6f6e 2074 6f20 6176 6f69  mization to avoi
-000219e0: 6420 6d61 6b69 6e67 2061 2063 6f70 7920  d making a copy 
-000219f0: 6966 2074 6865 2075 7365 7220 7061 7373  if the user pass
-00021a00: 6573 0a20 2020 2020 2020 2023 2069 6e20  es.        # in 
-00021a10: 6120 7265 6163 7469 6f6e 2e4c 6973 7452  a reaction.ListR
-00021a20: 6561 6374 696f 6e73 5265 7175 6573 742e  eactionsRequest.
-00021a30: 0a20 2020 2020 2020 2023 2054 6865 7265  .        # There
-00021a40: 2773 206e 6f20 7269 736b 206f 6620 6d6f  's no risk of mo
-00021a50: 6469 6679 696e 6720 7468 6520 696e 7075  difying the inpu
-00021a60: 7420 6173 2077 6527 7665 2061 6c72 6561  t as we've alrea
-00021a70: 6479 2076 6572 6966 6965 640a 2020 2020  dy verified.    
-00021a80: 2020 2020 2320 7468 6572 6520 6172 6520      # there are 
-00021a90: 6e6f 2066 6c61 7474 656e 6564 2066 6965  no flattened fie
-00021aa0: 6c64 732e 0a20 2020 2020 2020 2069 6620  lds..        if 
-00021ab0: 6e6f 7420 6973 696e 7374 616e 6365 2872  not isinstance(r
-00021ac0: 6571 7565 7374 2c20 7265 6163 7469 6f6e  equest, reaction
-00021ad0: 2e4c 6973 7452 6561 6374 696f 6e73 5265  .ListReactionsRe
-00021ae0: 7175 6573 7429 3a0a 2020 2020 2020 2020  quest):.        
-00021af0: 2020 2020 7265 7175 6573 7420 3d20 7265      request = re
-00021b00: 6163 7469 6f6e 2e4c 6973 7452 6561 6374  action.ListReact
-00021b10: 696f 6e73 5265 7175 6573 7428 7265 7175  ionsRequest(requ
-00021b20: 6573 7429 0a20 2020 2020 2020 2020 2020  est).           
-00021b30: 2023 2049 6620 7765 2068 6176 6520 6b65   # If we have ke
-00021b40: 7977 6f72 6420 6172 6775 6d65 6e74 7320  yword arguments 
-00021b50: 636f 7272 6573 706f 6e64 696e 6720 746f  corresponding to
-00021b60: 2066 6965 6c64 7320 6f6e 2074 6865 0a20   fields on the. 
-00021b70: 2020 2020 2020 2020 2020 2023 2072 6571             # req
-00021b80: 7565 7374 2c20 6170 706c 7920 7468 6573  uest, apply thes
-00021b90: 652e 0a20 2020 2020 2020 2020 2020 2069  e..            i
-00021ba0: 6620 7061 7265 6e74 2069 7320 6e6f 7420  f parent is not 
-00021bb0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00021bc0: 2020 2020 2020 7265 7175 6573 742e 7061        request.pa
-00021bd0: 7265 6e74 203d 2070 6172 656e 740a 0a20  rent = parent.. 
-00021be0: 2020 2020 2020 2023 2057 7261 7020 7468         # Wrap th
-00021bf0: 6520 5250 4320 6d65 7468 6f64 3b20 7468  e RPC method; th
-00021c00: 6973 2061 6464 7320 7265 7472 7920 616e  is adds retry an
-00021c10: 6420 7469 6d65 6f75 7420 696e 666f 726d  d timeout inform
-00021c20: 6174 696f 6e2c 0a20 2020 2020 2020 2023  ation,.        #
-00021c30: 2061 6e64 2066 7269 656e 646c 7920 6572   and friendly er
-00021c40: 726f 7220 6861 6e64 6c69 6e67 2e0a 2020  ror handling..  
-00021c50: 2020 2020 2020 7270 6320 3d20 7365 6c66        rpc = self
-00021c60: 2e5f 7472 616e 7370 6f72 742e 5f77 7261  ._transport._wra
-00021c70: 7070 6564 5f6d 6574 686f 6473 5b73 656c  pped_methods[sel
-00021c80: 662e 5f74 7261 6e73 706f 7274 2e6c 6973  f._transport.lis
-00021c90: 745f 7265 6163 7469 6f6e 735d 0a0a 2020  t_reactions]..  
-00021ca0: 2020 2020 2020 2320 4365 7274 6169 6e20        # Certain 
-00021cb0: 6669 656c 6473 2073 686f 756c 6420 6265  fields should be
-00021cc0: 2070 726f 7669 6465 6420 7769 7468 696e   provided within
-00021cd0: 2074 6865 206d 6574 6164 6174 6120 6865   the metadata he
-00021ce0: 6164 6572 3b0a 2020 2020 2020 2020 2320  ader;.        # 
-00021cf0: 6164 6420 7468 6573 6520 6865 7265 2e0a  add these here..
-00021d00: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
-00021d10: 203d 2074 7570 6c65 286d 6574 6164 6174   = tuple(metadat
-00021d20: 6129 202b 2028 0a20 2020 2020 2020 2020  a) + (.         
-00021d30: 2020 2067 6170 6963 5f76 312e 726f 7574     gapic_v1.rout
-00021d40: 696e 675f 6865 6164 6572 2e74 6f5f 6772  ing_header.to_gr
-00021d50: 7063 5f6d 6574 6164 6174 6128 2828 2270  pc_metadata((("p
-00021d60: 6172 656e 7422 2c20 7265 7175 6573 742e  arent", request.
-00021d70: 7061 7265 6e74 292c 2929 2c0a 2020 2020  parent),)),.    
-00021d80: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
-00021d90: 2056 616c 6964 6174 6520 7468 6520 756e   Validate the un
-00021da0: 6976 6572 7365 2064 6f6d 6169 6e2e 0a20  iverse domain.. 
-00021db0: 2020 2020 2020 2073 656c 662e 5f76 616c         self._val
-00021dc0: 6964 6174 655f 756e 6976 6572 7365 5f64  idate_universe_d
-00021dd0: 6f6d 6169 6e28 290a 0a20 2020 2020 2020  omain()..       
-00021de0: 2023 2053 656e 6420 7468 6520 7265 7175   # Send the requ
-00021df0: 6573 742e 0a20 2020 2020 2020 2072 6573  est..        res
-00021e00: 706f 6e73 6520 3d20 7270 6328 0a20 2020  ponse = rpc(.   
-00021e10: 2020 2020 2020 2020 2072 6571 7565 7374           request
-00021e20: 2c0a 2020 2020 2020 2020 2020 2020 7265  ,.            re
-00021e30: 7472 793d 7265 7472 792c 0a20 2020 2020  try=retry,.     
-00021e40: 2020 2020 2020 2074 696d 656f 7574 3d74         timeout=t
-00021e50: 696d 656f 7574 2c0a 2020 2020 2020 2020  imeout,.        
-00021e60: 2020 2020 6d65 7461 6461 7461 3d6d 6574      metadata=met
-00021e70: 6164 6174 612c 0a20 2020 2020 2020 2029  adata,.        )
-00021e80: 0a0a 2020 2020 2020 2020 2320 5468 6973  ..        # This
-00021e90: 206d 6574 686f 6420 6973 2070 6167 6564   method is paged
-00021ea0: 3b20 7772 6170 2074 6865 2072 6573 706f  ; wrap the respo
-00021eb0: 6e73 6520 696e 2061 2070 6167 6572 2c20  nse in a pager, 
-00021ec0: 7768 6963 6820 7072 6f76 6964 6573 0a20  which provides. 
-00021ed0: 2020 2020 2020 2023 2061 6e20 605f 5f69         # an `__i
-00021ee0: 7465 725f 5f60 2063 6f6e 7665 6e69 656e  ter__` convenien
-00021ef0: 6365 206d 6574 686f 642e 0a20 2020 2020  ce method..     
-00021f00: 2020 2072 6573 706f 6e73 6520 3d20 7061     response = pa
-00021f10: 6765 7273 2e4c 6973 7452 6561 6374 696f  gers.ListReactio
-00021f20: 6e73 5061 6765 7228 0a20 2020 2020 2020  nsPager(.       
-00021f30: 2020 2020 206d 6574 686f 643d 7270 632c       method=rpc,
-00021f40: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
-00021f50: 7565 7374 3d72 6571 7565 7374 2c0a 2020  uest=request,.  
-00021f60: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
-00021f70: 7365 3d72 6573 706f 6e73 652c 0a20 2020  se=response,.   
-00021f80: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
-00021f90: 613d 6d65 7461 6461 7461 2c0a 2020 2020  a=metadata,.    
-00021fa0: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
-00021fb0: 2044 6f6e 653b 2072 6574 7572 6e20 7468   Done; return th
-00021fc0: 6520 7265 7370 6f6e 7365 2e0a 2020 2020  e response..    
-00021fd0: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
-00021fe0: 6e73 650a 0a20 2020 2064 6566 2064 656c  nse..    def del
-00021ff0: 6574 655f 7265 6163 7469 6f6e 280a 2020  ete_reaction(.  
-00022000: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00022010: 2020 2020 7265 7175 6573 743a 204f 7074      request: Opt
-00022020: 696f 6e61 6c5b 556e 696f 6e5b 7265 6163  ional[Union[reac
-00022030: 7469 6f6e 2e44 656c 6574 6552 6561 6374  tion.DeleteReact
-00022040: 696f 6e52 6571 7565 7374 2c20 6469 6374  ionRequest, dict
-00022050: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
-00022060: 2020 202a 2c0a 2020 2020 2020 2020 6e61     *,.        na
-00022070: 6d65 3a20 4f70 7469 6f6e 616c 5b73 7472  me: Optional[str
-00022080: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-00022090: 2020 7265 7472 793a 204f 7074 696f 6e61    retry: Optiona
-000220a0: 6c52 6574 7279 203d 2067 6170 6963 5f76  lRetry = gapic_v
-000220b0: 312e 6d65 7468 6f64 2e44 4546 4155 4c54  1.method.DEFAULT
-000220c0: 2c0a 2020 2020 2020 2020 7469 6d65 6f75  ,.        timeou
-000220d0: 743a 2055 6e69 6f6e 5b66 6c6f 6174 2c20  t: Union[float, 
-000220e0: 6f62 6a65 6374 5d20 3d20 6761 7069 635f  object] = gapic_
-000220f0: 7631 2e6d 6574 686f 642e 4445 4641 554c  v1.method.DEFAUL
-00022100: 542c 0a20 2020 2020 2020 206d 6574 6164  T,.        metad
-00022110: 6174 613a 2053 6571 7565 6e63 655b 5475  ata: Sequence[Tu
-00022120: 706c 655b 7374 722c 2073 7472 5d5d 203d  ple[str, str]] =
-00022130: 2028 292c 0a20 2020 2029 202d 3e20 4e6f   (),.    ) -> No
-00022140: 6e65 3a0a 2020 2020 2020 2020 7222 2222  ne:.        r"""
-00022150: 4465 6c65 7465 7320 6120 7265 6163 7469  Deletes a reacti
-00022160: 6f6e 2074 6f20 6120 6d65 7373 6167 652e  on to a message.
-00022170: 204f 6e6c 7920 756e 6963 6f64 6520 656d   Only unicode em
-00022180: 6f6a 6973 2061 7265 0a20 2020 2020 2020  ojis are.       
-00022190: 2073 7570 706f 7274 6564 2e20 466f 7220   supported. For 
-000221a0: 616e 2065 7861 6d70 6c65 2c20 7365 6520  an example, see 
-000221b0: 6044 656c 6574 6520 610a 2020 2020 2020  `Delete a.      
-000221c0: 2020 7265 6163 7469 6f6e 203c 6874 7470    reaction <http
-000221d0: 733a 2f2f 6465 7665 6c6f 7065 7273 2e67  s://developers.g
-000221e0: 6f6f 676c 652e 636f 6d2f 776f 726b 7370  oogle.com/worksp
-000221f0: 6163 652f 6368 6174 2f64 656c 6574 652d  ace/chat/delete-
-00022200: 7265 6163 7469 6f6e 733e 605f 5f2e 0a20  reactions>`__.. 
-00022210: 2020 2020 2020 2052 6571 7569 7265 7320         Requires 
-00022220: 6075 7365 720a 2020 2020 2020 2020 6175  `user.        au
-00022230: 7468 656e 7469 6361 7469 6f6e 203c 6874  thentication <ht
-00022240: 7470 733a 2f2f 6465 7665 6c6f 7065 7273  tps://developers
-00022250: 2e67 6f6f 676c 652e 636f 6d2f 776f 726b  .google.com/work
-00022260: 7370 6163 652f 6368 6174 2f61 7574 6865  space/chat/authe
-00022270: 6e74 6963 6174 652d 6175 7468 6f72 697a  nticate-authoriz
-00022280: 652d 6368 6174 2d75 7365 723e 605f 5f2e  e-chat-user>`__.
-00022290: 0a0a 2020 2020 2020 2020 2e2e 2063 6f64  ..        .. cod
-000222a0: 652d 626c 6f63 6b3a 3a20 7079 7468 6f6e  e-block:: python
-000222b0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-000222c0: 5468 6973 2073 6e69 7070 6574 2068 6173  This snippet has
-000222d0: 2062 6565 6e20 6175 746f 6d61 7469 6361   been automatica
-000222e0: 6c6c 7920 6765 6e65 7261 7465 6420 616e  lly generated an
-000222f0: 6420 7368 6f75 6c64 2062 6520 7265 6761  d should be rega
-00022300: 7264 6564 2061 7320 610a 2020 2020 2020  rded as a.      
-00022310: 2020 2020 2020 2320 636f 6465 2074 656d        # code tem
-00022320: 706c 6174 6520 6f6e 6c79 2e0a 2020 2020  plate only..    
-00022330: 2020 2020 2020 2020 2320 4974 2077 696c          # It wil
-00022340: 6c20 7265 7175 6972 6520 6d6f 6469 6669  l require modifi
-00022350: 6361 7469 6f6e 7320 746f 2077 6f72 6b3a  cations to work:
-00022360: 0a20 2020 2020 2020 2020 2020 2023 202d  .            # -
-00022370: 2049 7420 6d61 7920 7265 7175 6972 6520   It may require 
-00022380: 636f 7272 6563 742f 696e 2d72 616e 6765  correct/in-range
-00022390: 2076 616c 7565 7320 666f 7220 7265 7175   values for requ
-000223a0: 6573 7420 696e 6974 6961 6c69 7a61 7469  est initializati
-000223b0: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
-000223c0: 2320 2d20 4974 206d 6179 2072 6571 7569  # - It may requi
-000223d0: 7265 2073 7065 6369 6679 696e 6720 7265  re specifying re
-000223e0: 6769 6f6e 616c 2065 6e64 706f 696e 7473  gional endpoints
-000223f0: 2077 6865 6e20 6372 6561 7469 6e67 2074   when creating t
-00022400: 6865 2073 6572 7669 6365 0a20 2020 2020  he service.     
-00022410: 2020 2020 2020 2023 2020 2063 6c69 656e         #   clien
-00022420: 7420 6173 2073 686f 776e 2069 6e3a 0a20  t as shown in:. 
-00022430: 2020 2020 2020 2020 2020 2023 2020 2068             #   h
-00022440: 7474 7073 3a2f 2f67 6f6f 676c 6561 7069  ttps://googleapi
-00022450: 732e 6465 762f 7079 7468 6f6e 2f67 6f6f  s.dev/python/goo
-00022460: 676c 652d 6170 692d 636f 7265 2f6c 6174  gle-api-core/lat
-00022470: 6573 742f 636c 6965 6e74 5f6f 7074 696f  est/client_optio
-00022480: 6e73 2e68 746d 6c0a 2020 2020 2020 2020  ns.html.        
-00022490: 2020 2020 6672 6f6d 2067 6f6f 676c 652e      from google.
-000224a0: 6170 7073 2069 6d70 6f72 7420 6368 6174  apps import chat
-000224b0: 5f76 310a 0a20 2020 2020 2020 2020 2020  _v1..           
-000224c0: 2064 6566 2073 616d 706c 655f 6465 6c65   def sample_dele
-000224d0: 7465 5f72 6561 6374 696f 6e28 293a 0a20  te_reaction():. 
-000224e0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000224f0: 2043 7265 6174 6520 6120 636c 6965 6e74   Create a client
-00022500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022510: 2063 6c69 656e 7420 3d20 6368 6174 5f76   client = chat_v
-00022520: 312e 4368 6174 5365 7276 6963 6543 6c69  1.ChatServiceCli
-00022530: 656e 7428 290a 0a20 2020 2020 2020 2020  ent()..         
-00022540: 2020 2020 2020 2023 2049 6e69 7469 616c         # Initial
-00022550: 697a 6520 7265 7175 6573 7420 6172 6775  ize request argu
-00022560: 6d65 6e74 2873 290a 2020 2020 2020 2020  ment(s).        
-00022570: 2020 2020 2020 2020 7265 7175 6573 7420          request 
-00022580: 3d20 6368 6174 5f76 312e 4465 6c65 7465  = chat_v1.Delete
-00022590: 5265 6163 7469 6f6e 5265 7175 6573 7428  ReactionRequest(
-000225a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000225b0: 2020 2020 206e 616d 653d 226e 616d 655f       name="name_
-000225c0: 7661 6c75 6522 2c0a 2020 2020 2020 2020  value",.        
-000225d0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-000225e0: 2020 2020 2020 2020 2020 2023 204d 616b             # Mak
-000225f0: 6520 7468 6520 7265 7175 6573 740a 2020  e the request.  
-00022600: 2020 2020 2020 2020 2020 2020 2020 636c                cl
-00022610: 6965 6e74 2e64 656c 6574 655f 7265 6163  ient.delete_reac
-00022620: 7469 6f6e 2872 6571 7565 7374 3d72 6571  tion(request=req
-00022630: 7565 7374 290a 0a20 2020 2020 2020 2041  uest)..        A
-00022640: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00022650: 2072 6571 7565 7374 2028 556e 696f 6e5b   request (Union[
-00022660: 676f 6f67 6c65 2e61 7070 732e 6368 6174  google.apps.chat
-00022670: 5f76 312e 7479 7065 732e 4465 6c65 7465  _v1.types.Delete
-00022680: 5265 6163 7469 6f6e 5265 7175 6573 742c  ReactionRequest,
-00022690: 2064 6963 745d 293a 0a20 2020 2020 2020   dict]):.       
-000226a0: 2020 2020 2020 2020 2054 6865 2072 6571           The req
-000226b0: 7565 7374 206f 626a 6563 742e 2044 656c  uest object. Del
-000226c0: 6574 6573 2061 2072 6561 6374 696f 6e20  etes a reaction 
-000226d0: 746f 2061 206d 6573 7361 6765 2e0a 2020  to a message..  
-000226e0: 2020 2020 2020 2020 2020 6e61 6d65 2028            name (
-000226f0: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-00022700: 2020 2020 2020 5265 7175 6972 6564 2e20        Required. 
-00022710: 4e61 6d65 206f 6620 7468 6520 7265 6163  Name of the reac
-00022720: 7469 6f6e 2074 6f20 6465 6c65 7465 2e0a  tion to delete..
-00022730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022740: 2046 6f72 6d61 743a 0a20 2020 2020 2020   Format:.       
-00022750: 2020 2020 2020 2020 2060 6073 7061 6365           ``space
-00022760: 732f 7b73 7061 6365 7d2f 6d65 7373 6167  s/{space}/messag
-00022770: 6573 2f7b 6d65 7373 6167 657d 2f72 6561  es/{message}/rea
-00022780: 6374 696f 6e73 2f7b 7265 6163 7469 6f6e  ctions/{reaction
-00022790: 7d60 600a 0a20 2020 2020 2020 2020 2020  }``..           
-000227a0: 2020 2020 2054 6869 7320 636f 7272 6573       This corres
-000227b0: 706f 6e64 7320 746f 2074 6865 2060 606e  ponds to the ``n
-000227c0: 616d 6560 6020 6669 656c 640a 2020 2020  ame`` field.    
-000227d0: 2020 2020 2020 2020 2020 2020 6f6e 2074              on t
-000227e0: 6865 2060 6072 6571 7565 7374 6060 2069  he ``request`` i
-000227f0: 6e73 7461 6e63 653b 2069 6620 6060 7265  nstance; if ``re
-00022800: 7175 6573 7460 6020 6973 2070 726f 7669  quest`` is provi
-00022810: 6465 642c 2074 6869 730a 2020 2020 2020  ded, this.      
-00022820: 2020 2020 2020 2020 2020 7368 6f75 6c64            should
-00022830: 206e 6f74 2062 6520 7365 742e 0a20 2020   not be set..   
-00022840: 2020 2020 2020 2020 2072 6574 7279 2028           retry (
-00022850: 676f 6f67 6c65 2e61 7069 5f63 6f72 652e  google.api_core.
-00022860: 7265 7472 792e 5265 7472 7929 3a20 4465  retry.Retry): De
-00022870: 7369 676e 6174 696f 6e20 6f66 2077 6861  signation of wha
-00022880: 7420 6572 726f 7273 2c20 6966 2061 6e79  t errors, if any
-00022890: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000228a0: 2020 7368 6f75 6c64 2062 6520 7265 7472    should be retr
-000228b0: 6965 642e 0a20 2020 2020 2020 2020 2020  ied..           
-000228c0: 2074 696d 656f 7574 2028 666c 6f61 7429   timeout (float)
-000228d0: 3a20 5468 6520 7469 6d65 6f75 7420 666f  : The timeout fo
-000228e0: 7220 7468 6973 2072 6571 7565 7374 2e0a  r this request..
-000228f0: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
-00022900: 6461 7461 2028 5365 7175 656e 6365 5b54  data (Sequence[T
-00022910: 7570 6c65 5b73 7472 2c20 7374 725d 5d29  uple[str, str]])
-00022920: 3a20 5374 7269 6e67 7320 7768 6963 6820  : Strings which 
-00022930: 7368 6f75 6c64 2062 650a 2020 2020 2020  should be.      
-00022940: 2020 2020 2020 2020 2020 7365 6e74 2061            sent a
-00022950: 6c6f 6e67 2077 6974 6820 7468 6520 7265  long with the re
-00022960: 7175 6573 7420 6173 206d 6574 6164 6174  quest as metadat
-00022970: 612e 0a20 2020 2020 2020 2022 2222 0a20  a..        """. 
-00022980: 2020 2020 2020 2023 2043 7265 6174 6520         # Create 
-00022990: 6f72 2063 6f65 7263 6520 6120 7072 6f74  or coerce a prot
-000229a0: 6f62 7566 2072 6571 7565 7374 206f 626a  obuf request obj
-000229b0: 6563 742e 0a20 2020 2020 2020 2023 2051  ect..        # Q
-000229c0: 7569 636b 2063 6865 636b 3a20 4966 2077  uick check: If w
-000229d0: 6520 676f 7420 6120 7265 7175 6573 7420  e got a request 
-000229e0: 6f62 6a65 6374 2c20 7765 2073 686f 756c  object, we shoul
-000229f0: 6420 2a6e 6f74 2a20 6861 7665 0a20 2020  d *not* have.   
-00022a00: 2020 2020 2023 2067 6f74 7465 6e20 616e       # gotten an
-00022a10: 7920 6b65 7977 6f72 6420 6172 6775 6d65  y keyword argume
-00022a20: 6e74 7320 7468 6174 206d 6170 2074 6f20  nts that map to 
-00022a30: 7468 6520 7265 7175 6573 742e 0a20 2020  the request..   
-00022a40: 2020 2020 2068 6173 5f66 6c61 7474 656e       has_flatten
-00022a50: 6564 5f70 6172 616d 7320 3d20 616e 7928  ed_params = any(
-00022a60: 5b6e 616d 655d 290a 2020 2020 2020 2020  [name]).        
-00022a70: 6966 2072 6571 7565 7374 2069 7320 6e6f  if request is no
-00022a80: 7420 4e6f 6e65 2061 6e64 2068 6173 5f66  t None and has_f
-00022a90: 6c61 7474 656e 6564 5f70 6172 616d 733a  lattened_params:
-00022aa0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00022ab0: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
-00022ac0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00022ad0: 4966 2074 6865 2060 7265 7175 6573 7460  If the `request`
-00022ae0: 2061 7267 756d 656e 7420 6973 2073 6574   argument is set
-00022af0: 2c20 7468 656e 206e 6f6e 6520 6f66 2022  , then none of "
-00022b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022b10: 2022 7468 6520 696e 6469 7669 6475 616c   "the individual
-00022b20: 2066 6965 6c64 2061 7267 756d 656e 7473   field arguments
-00022b30: 2073 686f 756c 6420 6265 2073 6574 2e22   should be set."
-00022b40: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-00022b50: 2020 2020 2020 2020 2320 4d69 6e6f 7220          # Minor 
-00022b60: 6f70 7469 6d69 7a61 7469 6f6e 2074 6f20  optimization to 
-00022b70: 6176 6f69 6420 6d61 6b69 6e67 2061 2063  avoid making a c
-00022b80: 6f70 7920 6966 2074 6865 2075 7365 7220  opy if the user 
-00022b90: 7061 7373 6573 0a20 2020 2020 2020 2023  passes.        #
-00022ba0: 2069 6e20 6120 7265 6163 7469 6f6e 2e44   in a reaction.D
-00022bb0: 656c 6574 6552 6561 6374 696f 6e52 6571  eleteReactionReq
-00022bc0: 7565 7374 2e0a 2020 2020 2020 2020 2320  uest..        # 
-00022bd0: 5468 6572 6527 7320 6e6f 2072 6973 6b20  There's no risk 
-00022be0: 6f66 206d 6f64 6966 7969 6e67 2074 6865  of modifying the
-00022bf0: 2069 6e70 7574 2061 7320 7765 2776 6520   input as we've 
-00022c00: 616c 7265 6164 7920 7665 7269 6669 6564  already verified
-00022c10: 0a20 2020 2020 2020 2023 2074 6865 7265  .        # there
-00022c20: 2061 7265 206e 6f20 666c 6174 7465 6e65   are no flattene
-00022c30: 6420 6669 656c 6473 2e0a 2020 2020 2020  d fields..      
-00022c40: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
-00022c50: 6e63 6528 7265 7175 6573 742c 2072 6561  nce(request, rea
-00022c60: 6374 696f 6e2e 4465 6c65 7465 5265 6163  ction.DeleteReac
-00022c70: 7469 6f6e 5265 7175 6573 7429 3a0a 2020  tionRequest):.  
-00022c80: 2020 2020 2020 2020 2020 7265 7175 6573            reques
-00022c90: 7420 3d20 7265 6163 7469 6f6e 2e44 656c  t = reaction.Del
-00022ca0: 6574 6552 6561 6374 696f 6e52 6571 7565  eteReactionReque
-00022cb0: 7374 2872 6571 7565 7374 290a 2020 2020  st(request).    
-00022cc0: 2020 2020 2020 2020 2320 4966 2077 6520          # If we 
-00022cd0: 6861 7665 206b 6579 776f 7264 2061 7267  have keyword arg
-00022ce0: 756d 656e 7473 2063 6f72 7265 7370 6f6e  uments correspon
-00022cf0: 6469 6e67 2074 6f20 6669 656c 6473 206f  ding to fields o
-00022d00: 6e20 7468 650a 2020 2020 2020 2020 2020  n the.          
-00022d10: 2020 2320 7265 7175 6573 742c 2061 7070    # request, app
-00022d20: 6c79 2074 6865 7365 2e0a 2020 2020 2020  ly these..      
-00022d30: 2020 2020 2020 6966 206e 616d 6520 6973        if name is
-00022d40: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00022d50: 2020 2020 2020 2020 2020 2072 6571 7565             reque
-00022d60: 7374 2e6e 616d 6520 3d20 6e61 6d65 0a0a  st.name = name..
-00022d70: 2020 2020 2020 2020 2320 5772 6170 2074          # Wrap t
-00022d80: 6865 2052 5043 206d 6574 686f 643b 2074  he RPC method; t
-00022d90: 6869 7320 6164 6473 2072 6574 7279 2061  his adds retry a
-00022da0: 6e64 2074 696d 656f 7574 2069 6e66 6f72  nd timeout infor
-00022db0: 6d61 7469 6f6e 2c0a 2020 2020 2020 2020  mation,.        
-00022dc0: 2320 616e 6420 6672 6965 6e64 6c79 2065  # and friendly e
-00022dd0: 7272 6f72 2068 616e 646c 696e 672e 0a20  rror handling.. 
-00022de0: 2020 2020 2020 2072 7063 203d 2073 656c         rpc = sel
-00022df0: 662e 5f74 7261 6e73 706f 7274 2e5f 7772  f._transport._wr
-00022e00: 6170 7065 645f 6d65 7468 6f64 735b 7365  apped_methods[se
-00022e10: 6c66 2e5f 7472 616e 7370 6f72 742e 6465  lf._transport.de
-00022e20: 6c65 7465 5f72 6561 6374 696f 6e5d 0a0a  lete_reaction]..
-00022e30: 2020 2020 2020 2020 2320 4365 7274 6169          # Certai
-00022e40: 6e20 6669 656c 6473 2073 686f 756c 6420  n fields should 
-00022e50: 6265 2070 726f 7669 6465 6420 7769 7468  be provided with
-00022e60: 696e 2074 6865 206d 6574 6164 6174 6120  in the metadata 
-00022e70: 6865 6164 6572 3b0a 2020 2020 2020 2020  header;.        
-00022e80: 2320 6164 6420 7468 6573 6520 6865 7265  # add these here
-00022e90: 2e0a 2020 2020 2020 2020 6d65 7461 6461  ..        metada
-00022ea0: 7461 203d 2074 7570 6c65 286d 6574 6164  ta = tuple(metad
-00022eb0: 6174 6129 202b 2028 0a20 2020 2020 2020  ata) + (.       
-00022ec0: 2020 2020 2067 6170 6963 5f76 312e 726f       gapic_v1.ro
-00022ed0: 7574 696e 675f 6865 6164 6572 2e74 6f5f  uting_header.to_
-00022ee0: 6772 7063 5f6d 6574 6164 6174 6128 2828  grpc_metadata(((
-00022ef0: 226e 616d 6522 2c20 7265 7175 6573 742e  "name", request.
-00022f00: 6e61 6d65 292c 2929 2c0a 2020 2020 2020  name),)),.      
-00022f10: 2020 290a 0a20 2020 2020 2020 2023 2056    )..        # V
-00022f20: 616c 6964 6174 6520 7468 6520 756e 6976  alidate the univ
-00022f30: 6572 7365 2064 6f6d 6169 6e2e 0a20 2020  erse domain..   
-00022f40: 2020 2020 2073 656c 662e 5f76 616c 6964       self._valid
-00022f50: 6174 655f 756e 6976 6572 7365 5f64 6f6d  ate_universe_dom
-00022f60: 6169 6e28 290a 0a20 2020 2020 2020 2023  ain()..        #
-00022f70: 2053 656e 6420 7468 6520 7265 7175 6573   Send the reques
-00022f80: 742e 0a20 2020 2020 2020 2072 7063 280a  t..        rpc(.
-00022f90: 2020 2020 2020 2020 2020 2020 7265 7175              requ
-00022fa0: 6573 742c 0a20 2020 2020 2020 2020 2020  est,.           
-00022fb0: 2072 6574 7279 3d72 6574 7279 2c0a 2020   retry=retry,.  
-00022fc0: 2020 2020 2020 2020 2020 7469 6d65 6f75            timeou
-00022fd0: 743d 7469 6d65 6f75 742c 0a20 2020 2020  t=timeout,.     
-00022fe0: 2020 2020 2020 206d 6574 6164 6174 613d         metadata=
-00022ff0: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
-00023000: 2020 290a 0a20 2020 2064 6566 205f 5f65    )..    def __e
-00023010: 6e74 6572 5f5f 2873 656c 6629 202d 3e20  nter__(self) -> 
-00023020: 2243 6861 7453 6572 7669 6365 436c 6965  "ChatServiceClie
-00023030: 6e74 223a 0a20 2020 2020 2020 2072 6574  nt":.        ret
-00023040: 7572 6e20 7365 6c66 0a0a 2020 2020 6465  urn self..    de
-00023050: 6620 5f5f 6578 6974 5f5f 2873 656c 662c  f __exit__(self,
-00023060: 2074 7970 652c 2076 616c 7565 2c20 7472   type, value, tr
-00023070: 6163 6562 6163 6b29 3a0a 2020 2020 2020  aceback):.      
-00023080: 2020 2222 2252 656c 6561 7365 7320 756e    """Releases un
-00023090: 6465 726c 7969 6e67 2074 7261 6e73 706f  derlying transpo
-000230a0: 7274 2773 2072 6573 6f75 7263 6573 2e0a  rt's resources..
-000230b0: 0a20 2020 2020 2020 202e 2e20 7761 726e  .        .. warn
-000230c0: 696e 673a 3a0a 2020 2020 2020 2020 2020  ing::.          
-000230d0: 2020 4f4e 4c59 2075 7365 2061 7320 6120    ONLY use as a 
-000230e0: 636f 6e74 6578 7420 6d61 6e61 6765 7220  context manager 
-000230f0: 6966 2074 6865 2074 7261 6e73 706f 7274  if the transport
-00023100: 2069 7320 4e4f 5420 7368 6172 6564 0a20   is NOT shared. 
-00023110: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00023120: 6f74 6865 7220 636c 6965 6e74 7321 2045  other clients! E
-00023130: 7869 7469 6e67 2074 6865 2077 6974 6820  xiting the with 
-00023140: 626c 6f63 6b20 7769 6c6c 2043 4c4f 5345  block will CLOSE
-00023150: 2074 6865 2074 7261 6e73 706f 7274 0a20   the transport. 
-00023160: 2020 2020 2020 2020 2020 2061 6e64 206d             and m
-00023170: 6179 2063 6175 7365 2065 7272 6f72 7320  ay cause errors 
-00023180: 696e 206f 7468 6572 2063 6c69 656e 7473  in other clients
-00023190: 210a 2020 2020 2020 2020 2222 220a 2020  !.        """.  
-000231a0: 2020 2020 2020 7365 6c66 2e74 7261 6e73        self.trans
-000231b0: 706f 7274 2e63 6c6f 7365 2829 0a0a 0a44  port.close()...D
-000231c0: 4546 4155 4c54 5f43 4c49 454e 545f 494e  EFAULT_CLIENT_IN
-000231d0: 464f 203d 2067 6170 6963 5f76 312e 636c  FO = gapic_v1.cl
-000231e0: 6965 6e74 5f69 6e66 6f2e 436c 6965 6e74  ient_info.Client
-000231f0: 496e 666f 280a 2020 2020 6761 7069 635f  Info(.    gapic_
-00023200: 7665 7273 696f 6e3d 7061 636b 6167 655f  version=package_
-00023210: 7665 7273 696f 6e2e 5f5f 7665 7273 696f  version.__versio
-00023220: 6e5f 5f0a 290a 0a0a 5f5f 616c 6c5f 5f20  n__.)...__all__ 
-00023230: 3d20 2822 4368 6174 5365 7276 6963 6543  = ("ChatServiceC
-00023240: 6c69 656e 7422 2c29 0a                   lient",).
+0001e520: 616c 5b55 6e69 6f6e 5b67 635f 6d65 6d62  al[Union[gc_memb
+0001e530: 6572 7368 6970 2e55 7064 6174 654d 656d  ership.UpdateMem
+0001e540: 6265 7273 6869 7052 6571 7565 7374 2c20  bershipRequest, 
+0001e550: 6469 6374 5d5d 203d 204e 6f6e 652c 0a20  dict]] = None,. 
+0001e560: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
+0001e570: 2020 6d65 6d62 6572 7368 6970 3a20 4f70    membership: Op
+0001e580: 7469 6f6e 616c 5b67 635f 6d65 6d62 6572  tional[gc_member
+0001e590: 7368 6970 2e4d 656d 6265 7273 6869 705d  ship.Membership]
+0001e5a0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0001e5b0: 2075 7064 6174 655f 6d61 736b 3a20 4f70   update_mask: Op
+0001e5c0: 7469 6f6e 616c 5b66 6965 6c64 5f6d 6173  tional[field_mas
+0001e5d0: 6b5f 7062 322e 4669 656c 644d 6173 6b5d  k_pb2.FieldMask]
+0001e5e0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0001e5f0: 2072 6574 7279 3a20 4f70 7469 6f6e 616c   retry: Optional
+0001e600: 5265 7472 7920 3d20 6761 7069 635f 7631  Retry = gapic_v1
+0001e610: 2e6d 6574 686f 642e 4445 4641 554c 542c  .method.DEFAULT,
+0001e620: 0a20 2020 2020 2020 2074 696d 656f 7574  .        timeout
+0001e630: 3a20 556e 696f 6e5b 666c 6f61 742c 206f  : Union[float, o
+0001e640: 626a 6563 745d 203d 2067 6170 6963 5f76  bject] = gapic_v
+0001e650: 312e 6d65 7468 6f64 2e44 4546 4155 4c54  1.method.DEFAULT
+0001e660: 2c0a 2020 2020 2020 2020 6d65 7461 6461  ,.        metada
+0001e670: 7461 3a20 5365 7175 656e 6365 5b54 7570  ta: Sequence[Tup
+0001e680: 6c65 5b73 7472 2c20 7374 725d 5d20 3d20  le[str, str]] = 
+0001e690: 2829 2c0a 2020 2020 2920 2d3e 2067 635f  (),.    ) -> gc_
+0001e6a0: 6d65 6d62 6572 7368 6970 2e4d 656d 6265  membership.Membe
+0001e6b0: 7273 6869 703a 0a20 2020 2020 2020 2072  rship:.        r
+0001e6c0: 2222 2255 7064 6174 6573 2061 206d 656d  """Updates a mem
+0001e6d0: 6265 7273 6869 702e 2052 6571 7569 7265  bership. Require
+0001e6e0: 7320 6075 7365 720a 2020 2020 2020 2020  s `user.        
+0001e6f0: 6175 7468 656e 7469 6361 7469 6f6e 203c  authentication <
+0001e700: 6874 7470 733a 2f2f 6465 7665 6c6f 7065  https://develope
+0001e710: 7273 2e67 6f6f 676c 652e 636f 6d2f 6368  rs.google.com/ch
+0001e720: 6174 2f61 7069 2f67 7569 6465 732f 6175  at/api/guides/au
+0001e730: 7468 2f75 7365 7273 3e60 5f5f 2e0a 0a20  th/users>`__... 
+0001e740: 2020 2020 2020 202e 2e20 636f 6465 2d62         .. code-b
+0001e750: 6c6f 636b 3a3a 2070 7974 686f 6e0a 0a20  lock:: python.. 
+0001e760: 2020 2020 2020 2020 2020 2023 2054 6869             # Thi
+0001e770: 7320 736e 6970 7065 7420 6861 7320 6265  s snippet has be
+0001e780: 656e 2061 7574 6f6d 6174 6963 616c 6c79  en automatically
+0001e790: 2067 656e 6572 6174 6564 2061 6e64 2073   generated and s
+0001e7a0: 686f 756c 6420 6265 2072 6567 6172 6465  hould be regarde
+0001e7b0: 6420 6173 2061 0a20 2020 2020 2020 2020  d as a.         
+0001e7c0: 2020 2023 2063 6f64 6520 7465 6d70 6c61     # code templa
+0001e7d0: 7465 206f 6e6c 792e 0a20 2020 2020 2020  te only..       
+0001e7e0: 2020 2020 2023 2049 7420 7769 6c6c 2072       # It will r
+0001e7f0: 6571 7569 7265 206d 6f64 6966 6963 6174  equire modificat
+0001e800: 696f 6e73 2074 6f20 776f 726b 3a0a 2020  ions to work:.  
+0001e810: 2020 2020 2020 2020 2020 2320 2d20 4974            # - It
+0001e820: 206d 6179 2072 6571 7569 7265 2063 6f72   may require cor
+0001e830: 7265 6374 2f69 6e2d 7261 6e67 6520 7661  rect/in-range va
+0001e840: 6c75 6573 2066 6f72 2072 6571 7565 7374  lues for request
+0001e850: 2069 6e69 7469 616c 697a 6174 696f 6e2e   initialization.
+0001e860: 0a20 2020 2020 2020 2020 2020 2023 202d  .            # -
+0001e870: 2049 7420 6d61 7920 7265 7175 6972 6520   It may require 
+0001e880: 7370 6563 6966 7969 6e67 2072 6567 696f  specifying regio
+0001e890: 6e61 6c20 656e 6470 6f69 6e74 7320 7768  nal endpoints wh
+0001e8a0: 656e 2063 7265 6174 696e 6720 7468 6520  en creating the 
+0001e8b0: 7365 7276 6963 650a 2020 2020 2020 2020  service.        
+0001e8c0: 2020 2020 2320 2020 636c 6965 6e74 2061      #   client a
+0001e8d0: 7320 7368 6f77 6e20 696e 3a0a 2020 2020  s shown in:.    
+0001e8e0: 2020 2020 2020 2020 2320 2020 6874 7470          #   http
+0001e8f0: 733a 2f2f 676f 6f67 6c65 6170 6973 2e64  s://googleapis.d
+0001e900: 6576 2f70 7974 686f 6e2f 676f 6f67 6c65  ev/python/google
+0001e910: 2d61 7069 2d63 6f72 652f 6c61 7465 7374  -api-core/latest
+0001e920: 2f63 6c69 656e 745f 6f70 7469 6f6e 732e  /client_options.
+0001e930: 6874 6d6c 0a20 2020 2020 2020 2020 2020  html.           
+0001e940: 2066 726f 6d20 676f 6f67 6c65 2e61 7070   from google.app
+0001e950: 7320 696d 706f 7274 2063 6861 745f 7631  s import chat_v1
+0001e960: 0a0a 2020 2020 2020 2020 2020 2020 6465  ..            de
+0001e970: 6620 7361 6d70 6c65 5f75 7064 6174 655f  f sample_update_
+0001e980: 6d65 6d62 6572 7368 6970 2829 3a0a 2020  membership():.  
+0001e990: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0001e9a0: 4372 6561 7465 2061 2063 6c69 656e 740a  Create a client.
+0001e9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e9c0: 636c 6965 6e74 203d 2063 6861 745f 7631  client = chat_v1
+0001e9d0: 2e43 6861 7453 6572 7669 6365 436c 6965  .ChatServiceClie
+0001e9e0: 6e74 2829 0a0a 2020 2020 2020 2020 2020  nt()..          
+0001e9f0: 2020 2020 2020 2320 496e 6974 6961 6c69        # Initiali
+0001ea00: 7a65 2072 6571 7565 7374 2061 7267 756d  ze request argum
+0001ea10: 656e 7428 7329 0a20 2020 2020 2020 2020  ent(s).         
+0001ea20: 2020 2020 2020 2072 6571 7565 7374 203d         request =
+0001ea30: 2063 6861 745f 7631 2e55 7064 6174 654d   chat_v1.UpdateM
+0001ea40: 656d 6265 7273 6869 7052 6571 7565 7374  embershipRequest
+0001ea50: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0001ea60: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
+0001ea70: 2020 2020 2023 204d 616b 6520 7468 6520       # Make the 
+0001ea80: 7265 7175 6573 740a 2020 2020 2020 2020  request.        
+0001ea90: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+0001eaa0: 203d 2063 6c69 656e 742e 7570 6461 7465   = client.update
+0001eab0: 5f6d 656d 6265 7273 6869 7028 7265 7175  _membership(requ
+0001eac0: 6573 743d 7265 7175 6573 7429 0a0a 2020  est=request)..  
+0001ead0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0001eae0: 4861 6e64 6c65 2074 6865 2072 6573 706f  Handle the respo
+0001eaf0: 6e73 650a 2020 2020 2020 2020 2020 2020  nse.            
+0001eb00: 2020 2020 7072 696e 7428 7265 7370 6f6e      print(respon
+0001eb10: 7365 290a 0a20 2020 2020 2020 2041 7267  se)..        Arg
+0001eb20: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
+0001eb30: 6571 7565 7374 2028 556e 696f 6e5b 676f  equest (Union[go
+0001eb40: 6f67 6c65 2e61 7070 732e 6368 6174 5f76  ogle.apps.chat_v
+0001eb50: 312e 7479 7065 732e 5570 6461 7465 4d65  1.types.UpdateMe
+0001eb60: 6d62 6572 7368 6970 5265 7175 6573 742c  mbershipRequest,
+0001eb70: 2064 6963 745d 293a 0a20 2020 2020 2020   dict]):.       
+0001eb80: 2020 2020 2020 2020 2054 6865 2072 6571           The req
+0001eb90: 7565 7374 206f 626a 6563 742e 2052 6571  uest object. Req
+0001eba0: 7565 7374 206d 6573 7361 6765 2066 6f72  uest message for
+0001ebb0: 2075 7064 6174 696e 6720 610a 2020 2020   updating a.    
+0001ebc0: 2020 2020 2020 2020 2020 2020 6d65 6d62              memb
+0001ebd0: 6572 7368 6970 2e0a 2020 2020 2020 2020  ership..        
+0001ebe0: 2020 2020 6d65 6d62 6572 7368 6970 2028      membership (
+0001ebf0: 676f 6f67 6c65 2e61 7070 732e 6368 6174  google.apps.chat
+0001ec00: 5f76 312e 7479 7065 732e 4d65 6d62 6572  _v1.types.Member
+0001ec10: 7368 6970 293a 0a20 2020 2020 2020 2020  ship):.         
+0001ec20: 2020 2020 2020 2052 6571 7569 7265 642e         Required.
+0001ec30: 2054 6865 206d 656d 6265 7273 6869 7020   The membership 
+0001ec40: 746f 2075 7064 6174 652e 204f 6e6c 7920  to update. Only 
+0001ec50: 6669 656c 6473 0a20 2020 2020 2020 2020  fields.         
+0001ec60: 2020 2020 2020 2073 7065 6369 6669 6564         specified
+0001ec70: 2062 7920 6060 7570 6461 7465 5f6d 6173   by ``update_mas
+0001ec80: 6b60 6020 6172 6520 7570 6461 7465 642e  k`` are updated.
+0001ec90: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001eca0: 2020 5468 6973 2063 6f72 7265 7370 6f6e    This correspon
+0001ecb0: 6473 2074 6f20 7468 6520 6060 6d65 6d62  ds to the ``memb
+0001ecc0: 6572 7368 6970 6060 2066 6965 6c64 0a20  ership`` field. 
+0001ecd0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0001ece0: 6e20 7468 6520 6060 7265 7175 6573 7460  n the ``request`
+0001ecf0: 6020 696e 7374 616e 6365 3b20 6966 2060  ` instance; if `
+0001ed00: 6072 6571 7565 7374 6060 2069 7320 7072  `request`` is pr
+0001ed10: 6f76 6964 6564 2c20 7468 6973 0a20 2020  ovided, this.   
+0001ed20: 2020 2020 2020 2020 2020 2020 2073 686f               sho
+0001ed30: 756c 6420 6e6f 7420 6265 2073 6574 2e0a  uld not be set..
+0001ed40: 2020 2020 2020 2020 2020 2020 7570 6461              upda
+0001ed50: 7465 5f6d 6173 6b20 2867 6f6f 676c 652e  te_mask (google.
+0001ed60: 7072 6f74 6f62 7566 2e66 6965 6c64 5f6d  protobuf.field_m
+0001ed70: 6173 6b5f 7062 322e 4669 656c 644d 6173  ask_pb2.FieldMas
+0001ed80: 6b29 3a0a 2020 2020 2020 2020 2020 2020  k):.            
+0001ed90: 2020 2020 5265 7175 6972 6564 2e20 5468      Required. Th
+0001eda0: 6520 6669 656c 6420 7061 7468 7320 746f  e field paths to
+0001edb0: 2075 7064 6174 652e 2053 6570 6172 6174   update. Separat
+0001edc0: 6520 6d75 6c74 6970 6c65 0a20 2020 2020  e multiple.     
+0001edd0: 2020 2020 2020 2020 2020 2076 616c 7565             value
+0001ede0: 7320 7769 7468 2063 6f6d 6d61 7320 6f72  s with commas or
+0001edf0: 2075 7365 2060 602a 6060 2074 6f20 7570   use ``*`` to up
+0001ee00: 6461 7465 2061 6c6c 2066 6965 6c64 0a20  date all field. 
+0001ee10: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0001ee20: 6174 6873 2e0a 0a20 2020 2020 2020 2020  aths...         
+0001ee30: 2020 2020 2020 2043 7572 7265 6e74 6c79         Currently
+0001ee40: 2073 7570 706f 7274 6564 2066 6965 6c64   supported field
+0001ee50: 2070 6174 6873 3a0a 0a20 2020 2020 2020   paths:..       
+0001ee60: 2020 2020 2020 2020 202d 2020 6060 726f           -  ``ro
+0001ee70: 6c65 6060 0a0a 2020 2020 2020 2020 2020  le``..          
+0001ee80: 2020 2020 2020 5468 6973 2063 6f72 7265        This corre
+0001ee90: 7370 6f6e 6473 2074 6f20 7468 6520 6060  sponds to the ``
+0001eea0: 7570 6461 7465 5f6d 6173 6b60 6020 6669  update_mask`` fi
+0001eeb0: 656c 640a 2020 2020 2020 2020 2020 2020  eld.            
+0001eec0: 2020 2020 6f6e 2074 6865 2060 6072 6571      on the ``req
+0001eed0: 7565 7374 6060 2069 6e73 7461 6e63 653b  uest`` instance;
+0001eee0: 2069 6620 6060 7265 7175 6573 7460 6020   if ``request`` 
+0001eef0: 6973 2070 726f 7669 6465 642c 2074 6869  is provided, thi
+0001ef00: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+0001ef10: 2020 7368 6f75 6c64 206e 6f74 2062 6520    should not be 
+0001ef20: 7365 742e 0a20 2020 2020 2020 2020 2020  set..           
+0001ef30: 2072 6574 7279 2028 676f 6f67 6c65 2e61   retry (google.a
+0001ef40: 7069 5f63 6f72 652e 7265 7472 792e 5265  pi_core.retry.Re
+0001ef50: 7472 7929 3a20 4465 7369 676e 6174 696f  try): Designatio
+0001ef60: 6e20 6f66 2077 6861 7420 6572 726f 7273  n of what errors
+0001ef70: 2c20 6966 2061 6e79 2c0a 2020 2020 2020  , if any,.      
+0001ef80: 2020 2020 2020 2020 2020 7368 6f75 6c64            should
+0001ef90: 2062 6520 7265 7472 6965 642e 0a20 2020   be retried..   
+0001efa0: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
+0001efb0: 2028 666c 6f61 7429 3a20 5468 6520 7469   (float): The ti
+0001efc0: 6d65 6f75 7420 666f 7220 7468 6973 2072  meout for this r
+0001efd0: 6571 7565 7374 2e0a 2020 2020 2020 2020  equest..        
+0001efe0: 2020 2020 6d65 7461 6461 7461 2028 5365      metadata (Se
+0001eff0: 7175 656e 6365 5b54 7570 6c65 5b73 7472  quence[Tuple[str
+0001f000: 2c20 7374 725d 5d29 3a20 5374 7269 6e67  , str]]): String
+0001f010: 7320 7768 6963 6820 7368 6f75 6c64 2062  s which should b
+0001f020: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0001f030: 2020 7365 6e74 2061 6c6f 6e67 2077 6974    sent along wit
+0001f040: 6820 7468 6520 7265 7175 6573 7420 6173  h the request as
+0001f050: 206d 6574 6164 6174 612e 0a0a 2020 2020   metadata...    
+0001f060: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+0001f070: 2020 2020 2020 2020 2067 6f6f 676c 652e           google.
+0001f080: 6170 7073 2e63 6861 745f 7631 2e74 7970  apps.chat_v1.typ
+0001f090: 6573 2e4d 656d 6265 7273 6869 703a 0a20  es.Membership:. 
+0001f0a0: 2020 2020 2020 2020 2020 2020 2020 2052                 R
+0001f0b0: 6570 7265 7365 6e74 7320 6120 6d65 6d62  epresents a memb
+0001f0c0: 6572 7368 6970 2072 656c 6174 696f 6e20  ership relation 
+0001f0d0: 696e 0a20 2020 2020 2020 2020 2020 2020  in.             
+0001f0e0: 2020 2047 6f6f 676c 6520 4368 6174 2c20     Google Chat, 
+0001f0f0: 7375 6368 2061 7320 7768 6574 6865 7220  such as whether 
+0001f100: 6120 7573 6572 206f 720a 2020 2020 2020  a user or.      
+0001f110: 2020 2020 2020 2020 2020 4368 6174 2061            Chat a
+0001f120: 7070 2069 7320 696e 7669 7465 6420 746f  pp is invited to
+0001f130: 2c20 7061 7274 206f 662c 206f 720a 2020  , part of, or.  
+0001f140: 2020 2020 2020 2020 2020 2020 2020 6162                ab
+0001f150: 7365 6e74 2066 726f 6d20 6120 7370 6163  sent from a spac
+0001f160: 652e 0a0a 2020 2020 2020 2020 2222 220a  e...        """.
+0001f170: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
+0001f180: 206f 7220 636f 6572 6365 2061 2070 726f   or coerce a pro
+0001f190: 746f 6275 6620 7265 7175 6573 7420 6f62  tobuf request ob
+0001f1a0: 6a65 6374 2e0a 2020 2020 2020 2020 2320  ject..        # 
+0001f1b0: 5175 6963 6b20 6368 6563 6b3a 2049 6620  Quick check: If 
+0001f1c0: 7765 2067 6f74 2061 2072 6571 7565 7374  we got a request
+0001f1d0: 206f 626a 6563 742c 2077 6520 7368 6f75   object, we shou
+0001f1e0: 6c64 202a 6e6f 742a 2068 6176 650a 2020  ld *not* have.  
+0001f1f0: 2020 2020 2020 2320 676f 7474 656e 2061        # gotten a
+0001f200: 6e79 206b 6579 776f 7264 2061 7267 756d  ny keyword argum
+0001f210: 656e 7473 2074 6861 7420 6d61 7020 746f  ents that map to
+0001f220: 2074 6865 2072 6571 7565 7374 2e0a 2020   the request..  
+0001f230: 2020 2020 2020 6861 735f 666c 6174 7465        has_flatte
+0001f240: 6e65 645f 7061 7261 6d73 203d 2061 6e79  ned_params = any
+0001f250: 285b 6d65 6d62 6572 7368 6970 2c20 7570  ([membership, up
+0001f260: 6461 7465 5f6d 6173 6b5d 290a 2020 2020  date_mask]).    
+0001f270: 2020 2020 6966 2072 6571 7565 7374 2069      if request i
+0001f280: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2068  s not None and h
+0001f290: 6173 5f66 6c61 7474 656e 6564 5f70 6172  as_flattened_par
+0001f2a0: 616d 733a 0a20 2020 2020 2020 2020 2020  ams:.           
+0001f2b0: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+0001f2c0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+0001f2d0: 2020 2022 4966 2074 6865 2060 7265 7175     "If the `requ
+0001f2e0: 6573 7460 2061 7267 756d 656e 7420 6973  est` argument is
+0001f2f0: 2073 6574 2c20 7468 656e 206e 6f6e 6520   set, then none 
+0001f300: 6f66 2022 0a20 2020 2020 2020 2020 2020  of ".           
+0001f310: 2020 2020 2022 7468 6520 696e 6469 7669       "the indivi
+0001f320: 6475 616c 2066 6965 6c64 2061 7267 756d  dual field argum
+0001f330: 656e 7473 2073 686f 756c 6420 6265 2073  ents should be s
+0001f340: 6574 2e22 0a20 2020 2020 2020 2020 2020  et.".           
+0001f350: 2029 0a0a 2020 2020 2020 2020 2320 4d69   )..        # Mi
+0001f360: 6e6f 7220 6f70 7469 6d69 7a61 7469 6f6e  nor optimization
+0001f370: 2074 6f20 6176 6f69 6420 6d61 6b69 6e67   to avoid making
+0001f380: 2061 2063 6f70 7920 6966 2074 6865 2075   a copy if the u
+0001f390: 7365 7220 7061 7373 6573 0a20 2020 2020  ser passes.     
+0001f3a0: 2020 2023 2069 6e20 6120 6763 5f6d 656d     # in a gc_mem
+0001f3b0: 6265 7273 6869 702e 5570 6461 7465 4d65  bership.UpdateMe
+0001f3c0: 6d62 6572 7368 6970 5265 7175 6573 742e  mbershipRequest.
+0001f3d0: 0a20 2020 2020 2020 2023 2054 6865 7265  .        # There
+0001f3e0: 2773 206e 6f20 7269 736b 206f 6620 6d6f  's no risk of mo
+0001f3f0: 6469 6679 696e 6720 7468 6520 696e 7075  difying the inpu
+0001f400: 7420 6173 2077 6527 7665 2061 6c72 6561  t as we've alrea
+0001f410: 6479 2076 6572 6966 6965 640a 2020 2020  dy verified.    
+0001f420: 2020 2020 2320 7468 6572 6520 6172 6520      # there are 
+0001f430: 6e6f 2066 6c61 7474 656e 6564 2066 6965  no flattened fie
+0001f440: 6c64 732e 0a20 2020 2020 2020 2069 6620  lds..        if 
+0001f450: 6e6f 7420 6973 696e 7374 616e 6365 2872  not isinstance(r
+0001f460: 6571 7565 7374 2c20 6763 5f6d 656d 6265  equest, gc_membe
+0001f470: 7273 6869 702e 5570 6461 7465 4d65 6d62  rship.UpdateMemb
+0001f480: 6572 7368 6970 5265 7175 6573 7429 3a0a  ershipRequest):.
+0001f490: 2020 2020 2020 2020 2020 2020 7265 7175              requ
+0001f4a0: 6573 7420 3d20 6763 5f6d 656d 6265 7273  est = gc_members
+0001f4b0: 6869 702e 5570 6461 7465 4d65 6d62 6572  hip.UpdateMember
+0001f4c0: 7368 6970 5265 7175 6573 7428 7265 7175  shipRequest(requ
+0001f4d0: 6573 7429 0a20 2020 2020 2020 2020 2020  est).           
+0001f4e0: 2023 2049 6620 7765 2068 6176 6520 6b65   # If we have ke
+0001f4f0: 7977 6f72 6420 6172 6775 6d65 6e74 7320  yword arguments 
+0001f500: 636f 7272 6573 706f 6e64 696e 6720 746f  corresponding to
+0001f510: 2066 6965 6c64 7320 6f6e 2074 6865 0a20   fields on the. 
+0001f520: 2020 2020 2020 2020 2020 2023 2072 6571             # req
+0001f530: 7565 7374 2c20 6170 706c 7920 7468 6573  uest, apply thes
+0001f540: 652e 0a20 2020 2020 2020 2020 2020 2069  e..            i
+0001f550: 6620 6d65 6d62 6572 7368 6970 2069 7320  f membership is 
+0001f560: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0001f570: 2020 2020 2020 2020 2020 7265 7175 6573            reques
+0001f580: 742e 6d65 6d62 6572 7368 6970 203d 206d  t.membership = m
+0001f590: 656d 6265 7273 6869 700a 2020 2020 2020  embership.      
+0001f5a0: 2020 2020 2020 6966 2075 7064 6174 655f        if update_
+0001f5b0: 6d61 736b 2069 7320 6e6f 7420 4e6f 6e65  mask is not None
+0001f5c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001f5d0: 2020 7265 7175 6573 742e 7570 6461 7465    request.update
+0001f5e0: 5f6d 6173 6b20 3d20 7570 6461 7465 5f6d  _mask = update_m
+0001f5f0: 6173 6b0a 0a20 2020 2020 2020 2023 2057  ask..        # W
+0001f600: 7261 7020 7468 6520 5250 4320 6d65 7468  rap the RPC meth
+0001f610: 6f64 3b20 7468 6973 2061 6464 7320 7265  od; this adds re
+0001f620: 7472 7920 616e 6420 7469 6d65 6f75 7420  try and timeout 
+0001f630: 696e 666f 726d 6174 696f 6e2c 0a20 2020  information,.   
+0001f640: 2020 2020 2023 2061 6e64 2066 7269 656e       # and frien
+0001f650: 646c 7920 6572 726f 7220 6861 6e64 6c69  dly error handli
+0001f660: 6e67 2e0a 2020 2020 2020 2020 7270 6320  ng..        rpc 
+0001f670: 3d20 7365 6c66 2e5f 7472 616e 7370 6f72  = self._transpor
+0001f680: 742e 5f77 7261 7070 6564 5f6d 6574 686f  t._wrapped_metho
+0001f690: 6473 5b73 656c 662e 5f74 7261 6e73 706f  ds[self._transpo
+0001f6a0: 7274 2e75 7064 6174 655f 6d65 6d62 6572  rt.update_member
+0001f6b0: 7368 6970 5d0a 0a20 2020 2020 2020 2023  ship]..        #
+0001f6c0: 2043 6572 7461 696e 2066 6965 6c64 7320   Certain fields 
+0001f6d0: 7368 6f75 6c64 2062 6520 7072 6f76 6964  should be provid
+0001f6e0: 6564 2077 6974 6869 6e20 7468 6520 6d65  ed within the me
+0001f6f0: 7461 6461 7461 2068 6561 6465 723b 0a20  tadata header;. 
+0001f700: 2020 2020 2020 2023 2061 6464 2074 6865         # add the
+0001f710: 7365 2068 6572 652e 0a20 2020 2020 2020  se here..       
+0001f720: 206d 6574 6164 6174 6120 3d20 7475 706c   metadata = tupl
+0001f730: 6528 6d65 7461 6461 7461 2920 2b20 280a  e(metadata) + (.
+0001f740: 2020 2020 2020 2020 2020 2020 6761 7069              gapi
+0001f750: 635f 7631 2e72 6f75 7469 6e67 5f68 6561  c_v1.routing_hea
+0001f760: 6465 722e 746f 5f67 7270 635f 6d65 7461  der.to_grpc_meta
+0001f770: 6461 7461 280a 2020 2020 2020 2020 2020  data(.          
+0001f780: 2020 2020 2020 2828 226d 656d 6265 7273        (("members
+0001f790: 6869 702e 6e61 6d65 222c 2072 6571 7565  hip.name", reque
+0001f7a0: 7374 2e6d 656d 6265 7273 6869 702e 6e61  st.membership.na
+0001f7b0: 6d65 292c 290a 2020 2020 2020 2020 2020  me),).          
+0001f7c0: 2020 292c 0a20 2020 2020 2020 2029 0a0a    ),.        )..
+0001f7d0: 2020 2020 2020 2020 2320 5661 6c69 6461          # Valida
+0001f7e0: 7465 2074 6865 2075 6e69 7665 7273 6520  te the universe 
+0001f7f0: 646f 6d61 696e 2e0a 2020 2020 2020 2020  domain..        
+0001f800: 7365 6c66 2e5f 7661 6c69 6461 7465 5f75  self._validate_u
+0001f810: 6e69 7665 7273 655f 646f 6d61 696e 2829  niverse_domain()
+0001f820: 0a0a 2020 2020 2020 2020 2320 5365 6e64  ..        # Send
+0001f830: 2074 6865 2072 6571 7565 7374 2e0a 2020   the request..  
+0001f840: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
+0001f850: 2072 7063 280a 2020 2020 2020 2020 2020   rpc(.          
+0001f860: 2020 7265 7175 6573 742c 0a20 2020 2020    request,.     
+0001f870: 2020 2020 2020 2072 6574 7279 3d72 6574         retry=ret
+0001f880: 7279 2c0a 2020 2020 2020 2020 2020 2020  ry,.            
+0001f890: 7469 6d65 6f75 743d 7469 6d65 6f75 742c  timeout=timeout,
+0001f8a0: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
+0001f8b0: 6164 6174 613d 6d65 7461 6461 7461 2c0a  adata=metadata,.
+0001f8c0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0001f8d0: 2020 2023 2044 6f6e 653b 2072 6574 7572     # Done; retur
+0001f8e0: 6e20 7468 6520 7265 7370 6f6e 7365 2e0a  n the response..
+0001f8f0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0001f900: 6573 706f 6e73 650a 0a20 2020 2064 6566  esponse..    def
+0001f910: 2064 656c 6574 655f 6d65 6d62 6572 7368   delete_membersh
+0001f920: 6970 280a 2020 2020 2020 2020 7365 6c66  ip(.        self
+0001f930: 2c0a 2020 2020 2020 2020 7265 7175 6573  ,.        reques
+0001f940: 743a 204f 7074 696f 6e61 6c5b 556e 696f  t: Optional[Unio
+0001f950: 6e5b 6d65 6d62 6572 7368 6970 2e44 656c  n[membership.Del
+0001f960: 6574 654d 656d 6265 7273 6869 7052 6571  eteMembershipReq
+0001f970: 7565 7374 2c20 6469 6374 5d5d 203d 204e  uest, dict]] = N
+0001f980: 6f6e 652c 0a20 2020 2020 2020 202a 2c0a  one,.        *,.
+0001f990: 2020 2020 2020 2020 6e61 6d65 3a20 4f70          name: Op
+0001f9a0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+0001f9b0: 6e65 2c0a 2020 2020 2020 2020 7265 7472  ne,.        retr
+0001f9c0: 793a 204f 7074 696f 6e61 6c52 6574 7279  y: OptionalRetry
+0001f9d0: 203d 2067 6170 6963 5f76 312e 6d65 7468   = gapic_v1.meth
+0001f9e0: 6f64 2e44 4546 4155 4c54 2c0a 2020 2020  od.DEFAULT,.    
+0001f9f0: 2020 2020 7469 6d65 6f75 743a 2055 6e69      timeout: Uni
+0001fa00: 6f6e 5b66 6c6f 6174 2c20 6f62 6a65 6374  on[float, object
+0001fa10: 5d20 3d20 6761 7069 635f 7631 2e6d 6574  ] = gapic_v1.met
+0001fa20: 686f 642e 4445 4641 554c 542c 0a20 2020  hod.DEFAULT,.   
+0001fa30: 2020 2020 206d 6574 6164 6174 613a 2053       metadata: S
+0001fa40: 6571 7565 6e63 655b 5475 706c 655b 7374  equence[Tuple[st
+0001fa50: 722c 2073 7472 5d5d 203d 2028 292c 0a20  r, str]] = (),. 
+0001fa60: 2020 2029 202d 3e20 6d65 6d62 6572 7368     ) -> membersh
+0001fa70: 6970 2e4d 656d 6265 7273 6869 703a 0a20  ip.Membership:. 
+0001fa80: 2020 2020 2020 2072 2222 2244 656c 6574         r"""Delet
+0001fa90: 6573 2061 206d 656d 6265 7273 6869 702e  es a membership.
+0001faa0: 2046 6f72 2061 6e20 6578 616d 706c 652c   For an example,
+0001fab0: 2073 6565 2060 5265 6d6f 7665 2061 2075   see `Remove a u
+0001fac0: 7365 7220 6f72 2061 0a20 2020 2020 2020  ser or a.       
+0001fad0: 2047 6f6f 676c 6520 4368 6174 2061 7070   Google Chat app
+0001fae0: 2066 726f 6d20 610a 2020 2020 2020 2020   from a.        
+0001faf0: 7370 6163 6520 3c68 7474 7073 3a2f 2f64  space <https://d
+0001fb00: 6576 656c 6f70 6572 732e 676f 6f67 6c65  evelopers.google
+0001fb10: 2e63 6f6d 2f77 6f72 6b73 7061 6365 2f63  .com/workspace/c
+0001fb20: 6861 742f 6465 6c65 7465 2d6d 656d 6265  hat/delete-membe
+0001fb30: 7273 3e60 5f5f 2e0a 0a20 2020 2020 2020  rs>`__...       
+0001fb40: 2052 6571 7569 7265 7320 6075 7365 720a   Requires `user.
+0001fb50: 2020 2020 2020 2020 6175 7468 656e 7469          authenti
+0001fb60: 6361 7469 6f6e 203c 6874 7470 733a 2f2f  cation <https://
+0001fb70: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
+0001fb80: 652e 636f 6d2f 776f 726b 7370 6163 652f  e.com/workspace/
+0001fb90: 6368 6174 2f61 7574 6865 6e74 6963 6174  chat/authenticat
+0001fba0: 652d 6175 7468 6f72 697a 652d 6368 6174  e-authorize-chat
+0001fbb0: 2d75 7365 723e 605f 5f2e 0a0a 2020 2020  -user>`__...    
+0001fbc0: 2020 2020 2e2e 2063 6f64 652d 626c 6f63      .. code-bloc
+0001fbd0: 6b3a 3a20 7079 7468 6f6e 0a0a 2020 2020  k:: python..    
+0001fbe0: 2020 2020 2020 2020 2320 5468 6973 2073          # This s
+0001fbf0: 6e69 7070 6574 2068 6173 2062 6565 6e20  nippet has been 
+0001fc00: 6175 746f 6d61 7469 6361 6c6c 7920 6765  automatically ge
+0001fc10: 6e65 7261 7465 6420 616e 6420 7368 6f75  nerated and shou
+0001fc20: 6c64 2062 6520 7265 6761 7264 6564 2061  ld be regarded a
+0001fc30: 7320 610a 2020 2020 2020 2020 2020 2020  s a.            
+0001fc40: 2320 636f 6465 2074 656d 706c 6174 6520  # code template 
+0001fc50: 6f6e 6c79 2e0a 2020 2020 2020 2020 2020  only..          
+0001fc60: 2020 2320 4974 2077 696c 6c20 7265 7175    # It will requ
+0001fc70: 6972 6520 6d6f 6469 6669 6361 7469 6f6e  ire modification
+0001fc80: 7320 746f 2077 6f72 6b3a 0a20 2020 2020  s to work:.     
+0001fc90: 2020 2020 2020 2023 202d 2049 7420 6d61         # - It ma
+0001fca0: 7920 7265 7175 6972 6520 636f 7272 6563  y require correc
+0001fcb0: 742f 696e 2d72 616e 6765 2076 616c 7565  t/in-range value
+0001fcc0: 7320 666f 7220 7265 7175 6573 7420 696e  s for request in
+0001fcd0: 6974 6961 6c69 7a61 7469 6f6e 2e0a 2020  itialization..  
+0001fce0: 2020 2020 2020 2020 2020 2320 2d20 4974            # - It
+0001fcf0: 206d 6179 2072 6571 7569 7265 2073 7065   may require spe
+0001fd00: 6369 6679 696e 6720 7265 6769 6f6e 616c  cifying regional
+0001fd10: 2065 6e64 706f 696e 7473 2077 6865 6e20   endpoints when 
+0001fd20: 6372 6561 7469 6e67 2074 6865 2073 6572  creating the ser
+0001fd30: 7669 6365 0a20 2020 2020 2020 2020 2020  vice.           
+0001fd40: 2023 2020 2063 6c69 656e 7420 6173 2073   #   client as s
+0001fd50: 686f 776e 2069 6e3a 0a20 2020 2020 2020  hown in:.       
+0001fd60: 2020 2020 2023 2020 2068 7474 7073 3a2f       #   https:/
+0001fd70: 2f67 6f6f 676c 6561 7069 732e 6465 762f  /googleapis.dev/
+0001fd80: 7079 7468 6f6e 2f67 6f6f 676c 652d 6170  python/google-ap
+0001fd90: 692d 636f 7265 2f6c 6174 6573 742f 636c  i-core/latest/cl
+0001fda0: 6965 6e74 5f6f 7074 696f 6e73 2e68 746d  ient_options.htm
+0001fdb0: 6c0a 2020 2020 2020 2020 2020 2020 6672  l.            fr
+0001fdc0: 6f6d 2067 6f6f 676c 652e 6170 7073 2069  om google.apps i
+0001fdd0: 6d70 6f72 7420 6368 6174 5f76 310a 0a20  mport chat_v1.. 
+0001fde0: 2020 2020 2020 2020 2020 2064 6566 2073             def s
+0001fdf0: 616d 706c 655f 6465 6c65 7465 5f6d 656d  ample_delete_mem
+0001fe00: 6265 7273 6869 7028 293a 0a20 2020 2020  bership():.     
+0001fe10: 2020 2020 2020 2020 2020 2023 2043 7265             # Cre
+0001fe20: 6174 6520 6120 636c 6965 6e74 0a20 2020  ate a client.   
+0001fe30: 2020 2020 2020 2020 2020 2020 2063 6c69               cli
+0001fe40: 656e 7420 3d20 6368 6174 5f76 312e 4368  ent = chat_v1.Ch
+0001fe50: 6174 5365 7276 6963 6543 6c69 656e 7428  atServiceClient(
+0001fe60: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001fe70: 2020 2023 2049 6e69 7469 616c 697a 6520     # Initialize 
+0001fe80: 7265 7175 6573 7420 6172 6775 6d65 6e74  request argument
+0001fe90: 2873 290a 2020 2020 2020 2020 2020 2020  (s).            
+0001fea0: 2020 2020 7265 7175 6573 7420 3d20 6368      request = ch
+0001feb0: 6174 5f76 312e 4465 6c65 7465 4d65 6d62  at_v1.DeleteMemb
+0001fec0: 6572 7368 6970 5265 7175 6573 7428 0a20  ershipRequest(. 
+0001fed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fee0: 2020 206e 616d 653d 226e 616d 655f 7661     name="name_va
+0001fef0: 6c75 6522 2c0a 2020 2020 2020 2020 2020  lue",.          
+0001ff00: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0001ff10: 2020 2020 2020 2020 2023 204d 616b 6520           # Make 
+0001ff20: 7468 6520 7265 7175 6573 740a 2020 2020  the request.    
+0001ff30: 2020 2020 2020 2020 2020 2020 7265 7370              resp
+0001ff40: 6f6e 7365 203d 2063 6c69 656e 742e 6465  onse = client.de
+0001ff50: 6c65 7465 5f6d 656d 6265 7273 6869 7028  lete_membership(
+0001ff60: 7265 7175 6573 743d 7265 7175 6573 7429  request=request)
+0001ff70: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001ff80: 2020 2320 4861 6e64 6c65 2074 6865 2072    # Handle the r
+0001ff90: 6573 706f 6e73 650a 2020 2020 2020 2020  esponse.        
+0001ffa0: 2020 2020 2020 2020 7072 696e 7428 7265          print(re
+0001ffb0: 7370 6f6e 7365 290a 0a20 2020 2020 2020  sponse)..       
+0001ffc0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+0001ffd0: 2020 2072 6571 7565 7374 2028 556e 696f     request (Unio
+0001ffe0: 6e5b 676f 6f67 6c65 2e61 7070 732e 6368  n[google.apps.ch
+0001fff0: 6174 5f76 312e 7479 7065 732e 4465 6c65  at_v1.types.Dele
+00020000: 7465 4d65 6d62 6572 7368 6970 5265 7175  teMembershipRequ
+00020010: 6573 742c 2064 6963 745d 293a 0a20 2020  est, dict]):.   
+00020020: 2020 2020 2020 2020 2020 2020 2054 6865               The
+00020030: 2072 6571 7565 7374 206f 626a 6563 742e   request object.
+00020040: 2052 6571 7565 7374 2074 6f20 6465 6c65   Request to dele
+00020050: 7465 2061 206d 656d 6265 7273 6869 7020  te a membership 
+00020060: 696e 2061 0a20 2020 2020 2020 2020 2020  in a.           
+00020070: 2020 2020 2073 7061 6365 2e0a 2020 2020       space..    
+00020080: 2020 2020 2020 2020 6e61 6d65 2028 7374          name (st
+00020090: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+000200a0: 2020 2020 5265 7175 6972 6564 2e20 5265      Required. Re
+000200b0: 736f 7572 6365 206e 616d 6520 6f66 2074  source name of t
+000200c0: 6865 206d 656d 6265 7273 6869 7020 746f  he membership to
+000200d0: 2064 656c 6574 652e 0a20 2020 2020 2020   delete..       
+000200e0: 2020 2020 2020 2020 2043 6861 7420 6170           Chat ap
+000200f0: 7073 2063 616e 2064 656c 6574 6520 6875  ps can delete hu
+00020100: 6d61 6e20 7573 6572 7327 206f 7220 7468  man users' or th
+00020110: 6569 7220 6f77 6e0a 2020 2020 2020 2020  eir own.        
+00020120: 2020 2020 2020 2020 6d65 6d62 6572 7368          membersh
+00020130: 6970 732e 2043 6861 7420 6170 7073 2063  ips. Chat apps c
+00020140: 616e 2774 2064 656c 6574 6520 6f74 6865  an't delete othe
+00020150: 7220 6170 7073 270a 2020 2020 2020 2020  r apps'.        
+00020160: 2020 2020 2020 2020 6d65 6d62 6572 7368          membersh
+00020170: 6970 732e 0a0a 2020 2020 2020 2020 2020  ips...          
+00020180: 2020 2020 2020 5768 656e 2064 656c 6574        When delet
+00020190: 696e 6720 6120 6875 6d61 6e20 6d65 6d62  ing a human memb
+000201a0: 6572 7368 6970 2c20 7265 7175 6972 6573  ership, requires
+000201b0: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
+000201c0: 2020 2020 2060 6063 6861 742e 6d65 6d62       ``chat.memb
+000201d0: 6572 7368 6970 7360 6020 7363 6f70 6520  erships`` scope 
+000201e0: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
+000201f0: 2020 2020 6060 7370 6163 6573 2f7b 7370      ``spaces/{sp
+00020200: 6163 657d 2f6d 656d 6265 7273 2f7b 6d65  ace}/members/{me
+00020210: 6d62 6572 7d60 6020 666f 726d 6174 2e20  mber}`` format. 
+00020220: 596f 7520 6361 6e20 7573 650a 2020 2020  You can use.    
+00020230: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+00020240: 656d 6169 6c20 6173 2061 6e20 616c 6961  email as an alia
+00020250: 7320 666f 7220 6060 7b6d 656d 6265 727d  s for ``{member}
+00020260: 6060 2e20 466f 7220 6578 616d 706c 652c  ``. For example,
+00020270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020280: 2060 6073 7061 6365 732f 7b73 7061 6365   ``spaces/{space
+00020290: 7d2f 6d65 6d62 6572 732f 6578 616d 706c  }/members/exampl
+000202a0: 6540 676d 6169 6c2e 636f 6d60 6020 7768  e@gmail.com`` wh
+000202b0: 6572 650a 2020 2020 2020 2020 2020 2020  ere.            
+000202c0: 2020 2020 6060 6578 616d 706c 6540 676d      ``example@gm
+000202d0: 6169 6c2e 636f 6d60 6020 6973 2074 6865  ail.com`` is the
+000202e0: 2065 6d61 696c 206f 6620 7468 6520 476f   email of the Go
+000202f0: 6f67 6c65 2043 6861 740a 2020 2020 2020  ogle Chat.      
+00020300: 2020 2020 2020 2020 2020 7573 6572 2e0a            user..
+00020310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020320: 2057 6865 6e20 6465 6c65 7469 6e67 2061   When deleting a
+00020330: 6e20 6170 7020 6d65 6d62 6572 7368 6970  n app membership
+00020340: 2c20 7265 7175 6972 6573 2074 6865 0a20  , requires the. 
+00020350: 2020 2020 2020 2020 2020 2020 2020 2060                 `
+00020360: 6063 6861 742e 6d65 6d62 6572 7368 6970  `chat.membership
+00020370: 732e 6170 7060 6020 7363 6f70 6520 616e  s.app`` scope an
+00020380: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+00020390: 2020 6060 7370 6163 6573 2f7b 7370 6163    ``spaces/{spac
+000203a0: 657d 2f6d 656d 6265 7273 2f61 7070 6060  e}/members/app``
+000203b0: 2066 6f72 6d61 742e 0a0a 2020 2020 2020   format...      
+000203c0: 2020 2020 2020 2020 2020 466f 726d 6174            Format
+000203d0: 3a20 6060 7370 6163 6573 2f7b 7370 6163  : ``spaces/{spac
+000203e0: 657d 2f6d 656d 6265 7273 2f7b 6d65 6d62  e}/members/{memb
+000203f0: 6572 7d60 6020 6f72 0a20 2020 2020 2020  er}`` or.       
+00020400: 2020 2020 2020 2020 2060 6073 7061 6365           ``space
+00020410: 732f 7b73 7061 6365 7d2f 6d65 6d62 6572  s/{space}/member
+00020420: 732f 6170 7060 602e 0a0a 2020 2020 2020  s/app``...      
+00020430: 2020 2020 2020 2020 2020 5468 6973 2063            This c
+00020440: 6f72 7265 7370 6f6e 6473 2074 6f20 7468  orresponds to th
+00020450: 6520 6060 6e61 6d65 6060 2066 6965 6c64  e ``name`` field
+00020460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020470: 206f 6e20 7468 6520 6060 7265 7175 6573   on the ``reques
+00020480: 7460 6020 696e 7374 616e 6365 3b20 6966  t`` instance; if
+00020490: 2060 6072 6571 7565 7374 6060 2069 7320   ``request`` is 
+000204a0: 7072 6f76 6964 6564 2c20 7468 6973 0a20  provided, this. 
+000204b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000204c0: 686f 756c 6420 6e6f 7420 6265 2073 6574  hould not be set
+000204d0: 2e0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+000204e0: 7472 7920 2867 6f6f 676c 652e 6170 695f  try (google.api_
+000204f0: 636f 7265 2e72 6574 7279 2e52 6574 7279  core.retry.Retry
+00020500: 293a 2044 6573 6967 6e61 7469 6f6e 206f  ): Designation o
+00020510: 6620 7768 6174 2065 7272 6f72 732c 2069  f what errors, i
+00020520: 6620 616e 792c 0a20 2020 2020 2020 2020  f any,.         
+00020530: 2020 2020 2020 2073 686f 756c 6420 6265         should be
+00020540: 2072 6574 7269 6564 2e0a 2020 2020 2020   retried..      
+00020550: 2020 2020 2020 7469 6d65 6f75 7420 2866        timeout (f
+00020560: 6c6f 6174 293a 2054 6865 2074 696d 656f  loat): The timeo
+00020570: 7574 2066 6f72 2074 6869 7320 7265 7175  ut for this requ
+00020580: 6573 742e 0a20 2020 2020 2020 2020 2020  est..           
+00020590: 206d 6574 6164 6174 6120 2853 6571 7565   metadata (Seque
+000205a0: 6e63 655b 5475 706c 655b 7374 722c 2073  nce[Tuple[str, s
+000205b0: 7472 5d5d 293a 2053 7472 696e 6773 2077  tr]]): Strings w
+000205c0: 6869 6368 2073 686f 756c 6420 6265 0a20  hich should be. 
+000205d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000205e0: 656e 7420 616c 6f6e 6720 7769 7468 2074  ent along with t
+000205f0: 6865 2072 6571 7565 7374 2061 7320 6d65  he request as me
+00020600: 7461 6461 7461 2e0a 0a20 2020 2020 2020  tadata...       
+00020610: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00020620: 2020 2020 2020 676f 6f67 6c65 2e61 7070        google.app
+00020630: 732e 6368 6174 5f76 312e 7479 7065 732e  s.chat_v1.types.
+00020640: 4d65 6d62 6572 7368 6970 3a0a 2020 2020  Membership:.    
+00020650: 2020 2020 2020 2020 2020 2020 5265 7072              Repr
+00020660: 6573 656e 7473 2061 206d 656d 6265 7273  esents a members
+00020670: 6869 7020 7265 6c61 7469 6f6e 2069 6e0a  hip relation in.
+00020680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020690: 476f 6f67 6c65 2043 6861 742c 2073 7563  Google Chat, suc
+000206a0: 6820 6173 2077 6865 7468 6572 2061 2075  h as whether a u
+000206b0: 7365 7220 6f72 0a20 2020 2020 2020 2020  ser or.         
+000206c0: 2020 2020 2020 2043 6861 7420 6170 7020         Chat app 
+000206d0: 6973 2069 6e76 6974 6564 2074 6f2c 2070  is invited to, p
+000206e0: 6172 7420 6f66 2c20 6f72 0a20 2020 2020  art of, or.     
+000206f0: 2020 2020 2020 2020 2020 2061 6273 656e             absen
+00020700: 7420 6672 6f6d 2061 2073 7061 6365 2e0a  t from a space..
+00020710: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00020720: 2020 2020 2023 2043 7265 6174 6520 6f72       # Create or
+00020730: 2063 6f65 7263 6520 6120 7072 6f74 6f62   coerce a protob
+00020740: 7566 2072 6571 7565 7374 206f 626a 6563  uf request objec
+00020750: 742e 0a20 2020 2020 2020 2023 2051 7569  t..        # Qui
+00020760: 636b 2063 6865 636b 3a20 4966 2077 6520  ck check: If we 
+00020770: 676f 7420 6120 7265 7175 6573 7420 6f62  got a request ob
+00020780: 6a65 6374 2c20 7765 2073 686f 756c 6420  ject, we should 
+00020790: 2a6e 6f74 2a20 6861 7665 0a20 2020 2020  *not* have.     
+000207a0: 2020 2023 2067 6f74 7465 6e20 616e 7920     # gotten any 
+000207b0: 6b65 7977 6f72 6420 6172 6775 6d65 6e74  keyword argument
+000207c0: 7320 7468 6174 206d 6170 2074 6f20 7468  s that map to th
+000207d0: 6520 7265 7175 6573 742e 0a20 2020 2020  e request..     
+000207e0: 2020 2068 6173 5f66 6c61 7474 656e 6564     has_flattened
+000207f0: 5f70 6172 616d 7320 3d20 616e 7928 5b6e  _params = any([n
+00020800: 616d 655d 290a 2020 2020 2020 2020 6966  ame]).        if
+00020810: 2072 6571 7565 7374 2069 7320 6e6f 7420   request is not 
+00020820: 4e6f 6e65 2061 6e64 2068 6173 5f66 6c61  None and has_fla
+00020830: 7474 656e 6564 5f70 6172 616d 733a 0a20  ttened_params:. 
+00020840: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00020850: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
+00020860: 2020 2020 2020 2020 2020 2020 2022 4966               "If
+00020870: 2074 6865 2060 7265 7175 6573 7460 2061   the `request` a
+00020880: 7267 756d 656e 7420 6973 2073 6574 2c20  rgument is set, 
+00020890: 7468 656e 206e 6f6e 6520 6f66 2022 0a20  then none of ". 
+000208a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000208b0: 7468 6520 696e 6469 7669 6475 616c 2066  the individual f
+000208c0: 6965 6c64 2061 7267 756d 656e 7473 2073  ield arguments s
+000208d0: 686f 756c 6420 6265 2073 6574 2e22 0a20  hould be set.". 
+000208e0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+000208f0: 2020 2020 2020 2320 4d69 6e6f 7220 6f70        # Minor op
+00020900: 7469 6d69 7a61 7469 6f6e 2074 6f20 6176  timization to av
+00020910: 6f69 6420 6d61 6b69 6e67 2061 2063 6f70  oid making a cop
+00020920: 7920 6966 2074 6865 2075 7365 7220 7061  y if the user pa
+00020930: 7373 6573 0a20 2020 2020 2020 2023 2069  sses.        # i
+00020940: 6e20 6120 6d65 6d62 6572 7368 6970 2e44  n a membership.D
+00020950: 656c 6574 654d 656d 6265 7273 6869 7052  eleteMembershipR
+00020960: 6571 7565 7374 2e0a 2020 2020 2020 2020  equest..        
+00020970: 2320 5468 6572 6527 7320 6e6f 2072 6973  # There's no ris
+00020980: 6b20 6f66 206d 6f64 6966 7969 6e67 2074  k of modifying t
+00020990: 6865 2069 6e70 7574 2061 7320 7765 2776  he input as we'v
+000209a0: 6520 616c 7265 6164 7920 7665 7269 6669  e already verifi
+000209b0: 6564 0a20 2020 2020 2020 2023 2074 6865  ed.        # the
+000209c0: 7265 2061 7265 206e 6f20 666c 6174 7465  re are no flatte
+000209d0: 6e65 6420 6669 656c 6473 2e0a 2020 2020  ned fields..    
+000209e0: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
+000209f0: 7461 6e63 6528 7265 7175 6573 742c 206d  tance(request, m
+00020a00: 656d 6265 7273 6869 702e 4465 6c65 7465  embership.Delete
+00020a10: 4d65 6d62 6572 7368 6970 5265 7175 6573  MembershipReques
+00020a20: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00020a30: 7265 7175 6573 7420 3d20 6d65 6d62 6572  request = member
+00020a40: 7368 6970 2e44 656c 6574 654d 656d 6265  ship.DeleteMembe
+00020a50: 7273 6869 7052 6571 7565 7374 2872 6571  rshipRequest(req
+00020a60: 7565 7374 290a 2020 2020 2020 2020 2020  uest).          
+00020a70: 2020 2320 4966 2077 6520 6861 7665 206b    # If we have k
+00020a80: 6579 776f 7264 2061 7267 756d 656e 7473  eyword arguments
+00020a90: 2063 6f72 7265 7370 6f6e 6469 6e67 2074   corresponding t
+00020aa0: 6f20 6669 656c 6473 206f 6e20 7468 650a  o fields on the.
+00020ab0: 2020 2020 2020 2020 2020 2020 2320 7265              # re
+00020ac0: 7175 6573 742c 2061 7070 6c79 2074 6865  quest, apply the
+00020ad0: 7365 2e0a 2020 2020 2020 2020 2020 2020  se..            
+00020ae0: 6966 206e 616d 6520 6973 206e 6f74 204e  if name is not N
+00020af0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00020b00: 2020 2020 2072 6571 7565 7374 2e6e 616d       request.nam
+00020b10: 6520 3d20 6e61 6d65 0a0a 2020 2020 2020  e = name..      
+00020b20: 2020 2320 5772 6170 2074 6865 2052 5043    # Wrap the RPC
+00020b30: 206d 6574 686f 643b 2074 6869 7320 6164   method; this ad
+00020b40: 6473 2072 6574 7279 2061 6e64 2074 696d  ds retry and tim
+00020b50: 656f 7574 2069 6e66 6f72 6d61 7469 6f6e  eout information
+00020b60: 2c0a 2020 2020 2020 2020 2320 616e 6420  ,.        # and 
+00020b70: 6672 6965 6e64 6c79 2065 7272 6f72 2068  friendly error h
+00020b80: 616e 646c 696e 672e 0a20 2020 2020 2020  andling..       
+00020b90: 2072 7063 203d 2073 656c 662e 5f74 7261   rpc = self._tra
+00020ba0: 6e73 706f 7274 2e5f 7772 6170 7065 645f  nsport._wrapped_
+00020bb0: 6d65 7468 6f64 735b 7365 6c66 2e5f 7472  methods[self._tr
+00020bc0: 616e 7370 6f72 742e 6465 6c65 7465 5f6d  ansport.delete_m
+00020bd0: 656d 6265 7273 6869 705d 0a0a 2020 2020  embership]..    
+00020be0: 2020 2020 2320 4365 7274 6169 6e20 6669      # Certain fi
+00020bf0: 656c 6473 2073 686f 756c 6420 6265 2070  elds should be p
+00020c00: 726f 7669 6465 6420 7769 7468 696e 2074  rovided within t
+00020c10: 6865 206d 6574 6164 6174 6120 6865 6164  he metadata head
+00020c20: 6572 3b0a 2020 2020 2020 2020 2320 6164  er;.        # ad
+00020c30: 6420 7468 6573 6520 6865 7265 2e0a 2020  d these here..  
+00020c40: 2020 2020 2020 6d65 7461 6461 7461 203d        metadata =
+00020c50: 2074 7570 6c65 286d 6574 6164 6174 6129   tuple(metadata)
+00020c60: 202b 2028 0a20 2020 2020 2020 2020 2020   + (.           
+00020c70: 2067 6170 6963 5f76 312e 726f 7574 696e   gapic_v1.routin
+00020c80: 675f 6865 6164 6572 2e74 6f5f 6772 7063  g_header.to_grpc
+00020c90: 5f6d 6574 6164 6174 6128 2828 226e 616d  _metadata((("nam
+00020ca0: 6522 2c20 7265 7175 6573 742e 6e61 6d65  e", request.name
+00020cb0: 292c 2929 2c0a 2020 2020 2020 2020 290a  ),)),.        ).
+00020cc0: 0a20 2020 2020 2020 2023 2056 616c 6964  .        # Valid
+00020cd0: 6174 6520 7468 6520 756e 6976 6572 7365  ate the universe
+00020ce0: 2064 6f6d 6169 6e2e 0a20 2020 2020 2020   domain..       
+00020cf0: 2073 656c 662e 5f76 616c 6964 6174 655f   self._validate_
+00020d00: 756e 6976 6572 7365 5f64 6f6d 6169 6e28  universe_domain(
+00020d10: 290a 0a20 2020 2020 2020 2023 2053 656e  )..        # Sen
+00020d20: 6420 7468 6520 7265 7175 6573 742e 0a20  d the request.. 
+00020d30: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+00020d40: 3d20 7270 6328 0a20 2020 2020 2020 2020  = rpc(.         
+00020d50: 2020 2072 6571 7565 7374 2c0a 2020 2020     request,.    
+00020d60: 2020 2020 2020 2020 7265 7472 793d 7265          retry=re
+00020d70: 7472 792c 0a20 2020 2020 2020 2020 2020  try,.           
+00020d80: 2074 696d 656f 7574 3d74 696d 656f 7574   timeout=timeout
+00020d90: 2c0a 2020 2020 2020 2020 2020 2020 6d65  ,.            me
+00020da0: 7461 6461 7461 3d6d 6574 6164 6174 612c  tadata=metadata,
+00020db0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00020dc0: 2020 2020 2320 446f 6e65 3b20 7265 7475      # Done; retu
+00020dd0: 726e 2074 6865 2072 6573 706f 6e73 652e  rn the response.
+00020de0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00020df0: 7265 7370 6f6e 7365 0a0a 2020 2020 6465  response..    de
+00020e00: 6620 6372 6561 7465 5f72 6561 6374 696f  f create_reactio
+00020e10: 6e28 0a20 2020 2020 2020 2073 656c 662c  n(.        self,
+00020e20: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
+00020e30: 3a20 4f70 7469 6f6e 616c 5b55 6e69 6f6e  : Optional[Union
+00020e40: 5b67 635f 7265 6163 7469 6f6e 2e43 7265  [gc_reaction.Cre
+00020e50: 6174 6552 6561 6374 696f 6e52 6571 7565  ateReactionReque
+00020e60: 7374 2c20 6469 6374 5d5d 203d 204e 6f6e  st, dict]] = Non
+00020e70: 652c 0a20 2020 2020 2020 202a 2c0a 2020  e,.        *,.  
+00020e80: 2020 2020 2020 7061 7265 6e74 3a20 4f70        parent: Op
+00020e90: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00020ea0: 6e65 2c0a 2020 2020 2020 2020 7265 6163  ne,.        reac
+00020eb0: 7469 6f6e 3a20 4f70 7469 6f6e 616c 5b67  tion: Optional[g
+00020ec0: 635f 7265 6163 7469 6f6e 2e52 6561 6374  c_reaction.React
+00020ed0: 696f 6e5d 203d 204e 6f6e 652c 0a20 2020  ion] = None,.   
+00020ee0: 2020 2020 2072 6574 7279 3a20 4f70 7469       retry: Opti
+00020ef0: 6f6e 616c 5265 7472 7920 3d20 6761 7069  onalRetry = gapi
+00020f00: 635f 7631 2e6d 6574 686f 642e 4445 4641  c_v1.method.DEFA
+00020f10: 554c 542c 0a20 2020 2020 2020 2074 696d  ULT,.        tim
+00020f20: 656f 7574 3a20 556e 696f 6e5b 666c 6f61  eout: Union[floa
+00020f30: 742c 206f 626a 6563 745d 203d 2067 6170  t, object] = gap
+00020f40: 6963 5f76 312e 6d65 7468 6f64 2e44 4546  ic_v1.method.DEF
+00020f50: 4155 4c54 2c0a 2020 2020 2020 2020 6d65  AULT,.        me
+00020f60: 7461 6461 7461 3a20 5365 7175 656e 6365  tadata: Sequence
+00020f70: 5b54 7570 6c65 5b73 7472 2c20 7374 725d  [Tuple[str, str]
+00020f80: 5d20 3d20 2829 2c0a 2020 2020 2920 2d3e  ] = (),.    ) ->
+00020f90: 2067 635f 7265 6163 7469 6f6e 2e52 6561   gc_reaction.Rea
+00020fa0: 6374 696f 6e3a 0a20 2020 2020 2020 2072  ction:.        r
+00020fb0: 2222 2243 7265 6174 6573 2061 2072 6561  """Creates a rea
+00020fc0: 6374 696f 6e20 616e 6420 6164 6473 2069  ction and adds i
+00020fd0: 7420 746f 2061 206d 6573 7361 6765 2e20  t to a message. 
+00020fe0: 4f6e 6c79 2075 6e69 636f 6465 2065 6d6f  Only unicode emo
+00020ff0: 6a69 730a 2020 2020 2020 2020 6172 6520  jis.        are 
+00021000: 7375 7070 6f72 7465 642e 2046 6f72 2061  supported. For a
+00021010: 6e20 6578 616d 706c 652c 2073 6565 2060  n example, see `
+00021020: 4164 6420 6120 7265 6163 7469 6f6e 2074  Add a reaction t
+00021030: 6f20 610a 2020 2020 2020 2020 6d65 7373  o a.        mess
+00021040: 6167 6520 3c68 7474 7073 3a2f 2f64 6576  age <https://dev
+00021050: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
+00021060: 6f6d 2f77 6f72 6b73 7061 6365 2f63 6861  om/workspace/cha
+00021070: 742f 6372 6561 7465 2d72 6561 6374 696f  t/create-reactio
+00021080: 6e73 3e60 5f5f 2e0a 2020 2020 2020 2020  ns>`__..        
+00021090: 5265 7175 6972 6573 2060 7573 6572 0a20  Requires `user. 
+000210a0: 2020 2020 2020 2061 7574 6865 6e74 6963         authentic
+000210b0: 6174 696f 6e20 3c68 7474 7073 3a2f 2f64  ation <https://d
+000210c0: 6576 656c 6f70 6572 732e 676f 6f67 6c65  evelopers.google
+000210d0: 2e63 6f6d 2f77 6f72 6b73 7061 6365 2f63  .com/workspace/c
+000210e0: 6861 742f 6175 7468 656e 7469 6361 7465  hat/authenticate
+000210f0: 2d61 7574 686f 7269 7a65 2d63 6861 742d  -authorize-chat-
+00021100: 7573 6572 3e60 5f5f 2e0a 0a20 2020 2020  user>`__...     
+00021110: 2020 202e 2e20 636f 6465 2d62 6c6f 636b     .. code-block
+00021120: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
+00021130: 2020 2020 2020 2023 2054 6869 7320 736e         # This sn
+00021140: 6970 7065 7420 6861 7320 6265 656e 2061  ippet has been a
+00021150: 7574 6f6d 6174 6963 616c 6c79 2067 656e  utomatically gen
+00021160: 6572 6174 6564 2061 6e64 2073 686f 756c  erated and shoul
+00021170: 6420 6265 2072 6567 6172 6465 6420 6173  d be regarded as
+00021180: 2061 0a20 2020 2020 2020 2020 2020 2023   a.            #
+00021190: 2063 6f64 6520 7465 6d70 6c61 7465 206f   code template o
+000211a0: 6e6c 792e 0a20 2020 2020 2020 2020 2020  nly..           
+000211b0: 2023 2049 7420 7769 6c6c 2072 6571 7569   # It will requi
+000211c0: 7265 206d 6f64 6966 6963 6174 696f 6e73  re modifications
+000211d0: 2074 6f20 776f 726b 3a0a 2020 2020 2020   to work:.      
+000211e0: 2020 2020 2020 2320 2d20 4974 206d 6179        # - It may
+000211f0: 2072 6571 7569 7265 2063 6f72 7265 6374   require correct
+00021200: 2f69 6e2d 7261 6e67 6520 7661 6c75 6573  /in-range values
+00021210: 2066 6f72 2072 6571 7565 7374 2069 6e69   for request ini
+00021220: 7469 616c 697a 6174 696f 6e2e 0a20 2020  tialization..   
+00021230: 2020 2020 2020 2020 2023 202d 2049 7420           # - It 
+00021240: 6d61 7920 7265 7175 6972 6520 7370 6563  may require spec
+00021250: 6966 7969 6e67 2072 6567 696f 6e61 6c20  ifying regional 
+00021260: 656e 6470 6f69 6e74 7320 7768 656e 2063  endpoints when c
+00021270: 7265 6174 696e 6720 7468 6520 7365 7276  reating the serv
+00021280: 6963 650a 2020 2020 2020 2020 2020 2020  ice.            
+00021290: 2320 2020 636c 6965 6e74 2061 7320 7368  #   client as sh
+000212a0: 6f77 6e20 696e 3a0a 2020 2020 2020 2020  own in:.        
+000212b0: 2020 2020 2320 2020 6874 7470 733a 2f2f      #   https://
+000212c0: 676f 6f67 6c65 6170 6973 2e64 6576 2f70  googleapis.dev/p
+000212d0: 7974 686f 6e2f 676f 6f67 6c65 2d61 7069  ython/google-api
+000212e0: 2d63 6f72 652f 6c61 7465 7374 2f63 6c69  -core/latest/cli
+000212f0: 656e 745f 6f70 7469 6f6e 732e 6874 6d6c  ent_options.html
+00021300: 0a20 2020 2020 2020 2020 2020 2066 726f  .            fro
+00021310: 6d20 676f 6f67 6c65 2e61 7070 7320 696d  m google.apps im
+00021320: 706f 7274 2063 6861 745f 7631 0a0a 2020  port chat_v1..  
+00021330: 2020 2020 2020 2020 2020 6465 6620 7361            def sa
+00021340: 6d70 6c65 5f63 7265 6174 655f 7265 6163  mple_create_reac
+00021350: 7469 6f6e 2829 3a0a 2020 2020 2020 2020  tion():.        
+00021360: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
+00021370: 2061 2063 6c69 656e 740a 2020 2020 2020   a client.      
+00021380: 2020 2020 2020 2020 2020 636c 6965 6e74            client
+00021390: 203d 2063 6861 745f 7631 2e43 6861 7453   = chat_v1.ChatS
+000213a0: 6572 7669 6365 436c 6965 6e74 2829 0a0a  erviceClient()..
+000213b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000213c0: 2320 496e 6974 6961 6c69 7a65 2072 6571  # Initialize req
+000213d0: 7565 7374 2061 7267 756d 656e 7428 7329  uest argument(s)
+000213e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000213f0: 2072 6571 7565 7374 203d 2063 6861 745f   request = chat_
+00021400: 7631 2e43 7265 6174 6552 6561 6374 696f  v1.CreateReactio
+00021410: 6e52 6571 7565 7374 280a 2020 2020 2020  nRequest(.      
+00021420: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00021430: 7265 6e74 3d22 7061 7265 6e74 5f76 616c  rent="parent_val
+00021440: 7565 222c 0a20 2020 2020 2020 2020 2020  ue",.           
+00021450: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00021460: 2020 2020 2020 2020 2320 4d61 6b65 2074          # Make t
+00021470: 6865 2072 6571 7565 7374 0a20 2020 2020  he request.     
+00021480: 2020 2020 2020 2020 2020 2072 6573 706f             respo
+00021490: 6e73 6520 3d20 636c 6965 6e74 2e63 7265  nse = client.cre
+000214a0: 6174 655f 7265 6163 7469 6f6e 2872 6571  ate_reaction(req
+000214b0: 7565 7374 3d72 6571 7565 7374 290a 0a20  uest=request).. 
+000214c0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000214d0: 2048 616e 646c 6520 7468 6520 7265 7370   Handle the resp
+000214e0: 6f6e 7365 0a20 2020 2020 2020 2020 2020  onse.           
+000214f0: 2020 2020 2070 7269 6e74 2872 6573 706f       print(respo
+00021500: 6e73 6529 0a0a 2020 2020 2020 2020 4172  nse)..        Ar
+00021510: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00021520: 7265 7175 6573 7420 2855 6e69 6f6e 5b67  request (Union[g
+00021530: 6f6f 676c 652e 6170 7073 2e63 6861 745f  oogle.apps.chat_
+00021540: 7631 2e74 7970 6573 2e43 7265 6174 6552  v1.types.CreateR
+00021550: 6561 6374 696f 6e52 6571 7565 7374 2c20  eactionRequest, 
+00021560: 6469 6374 5d29 3a0a 2020 2020 2020 2020  dict]):.        
+00021570: 2020 2020 2020 2020 5468 6520 7265 7175          The requ
+00021580: 6573 7420 6f62 6a65 6374 2e20 4372 6561  est object. Crea
+00021590: 7465 7320 6120 7265 6163 7469 6f6e 2074  tes a reaction t
+000215a0: 6f20 6120 6d65 7373 6167 652e 0a20 2020  o a message..   
+000215b0: 2020 2020 2020 2020 2070 6172 656e 7420           parent 
+000215c0: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
+000215d0: 2020 2020 2020 2052 6571 7569 7265 642e         Required.
+000215e0: 2054 6865 206d 6573 7361 6765 2077 6865   The message whe
+000215f0: 7265 2074 6865 2072 6561 6374 696f 6e20  re the reaction 
+00021600: 6973 2063 7265 6174 6564 2e0a 0a20 2020  is created...   
+00021610: 2020 2020 2020 2020 2020 2020 2046 6f72               For
+00021620: 6d61 743a 2060 6073 7061 6365 732f 7b73  mat: ``spaces/{s
+00021630: 7061 6365 7d2f 6d65 7373 6167 6573 2f7b  pace}/messages/{
+00021640: 6d65 7373 6167 657d 6060 0a0a 2020 2020  message}``..    
+00021650: 2020 2020 2020 2020 2020 2020 5468 6973              This
+00021660: 2063 6f72 7265 7370 6f6e 6473 2074 6f20   corresponds to 
+00021670: 7468 6520 6060 7061 7265 6e74 6060 2066  the ``parent`` f
+00021680: 6965 6c64 0a20 2020 2020 2020 2020 2020  ield.           
+00021690: 2020 2020 206f 6e20 7468 6520 6060 7265       on the ``re
+000216a0: 7175 6573 7460 6020 696e 7374 616e 6365  quest`` instance
+000216b0: 3b20 6966 2060 6072 6571 7565 7374 6060  ; if ``request``
+000216c0: 2069 7320 7072 6f76 6964 6564 2c20 7468   is provided, th
+000216d0: 6973 0a20 2020 2020 2020 2020 2020 2020  is.             
+000216e0: 2020 2073 686f 756c 6420 6e6f 7420 6265     should not be
+000216f0: 2073 6574 2e0a 2020 2020 2020 2020 2020   set..          
+00021700: 2020 7265 6163 7469 6f6e 2028 676f 6f67    reaction (goog
+00021710: 6c65 2e61 7070 732e 6368 6174 5f76 312e  le.apps.chat_v1.
+00021720: 7479 7065 732e 5265 6163 7469 6f6e 293a  types.Reaction):
+00021730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021740: 2052 6571 7569 7265 642e 2054 6865 2072   Required. The r
+00021750: 6561 6374 696f 6e20 746f 2063 7265 6174  eaction to creat
+00021760: 652e 0a20 2020 2020 2020 2020 2020 2020  e..             
+00021770: 2020 2054 6869 7320 636f 7272 6573 706f     This correspo
+00021780: 6e64 7320 746f 2074 6865 2060 6072 6561  nds to the ``rea
+00021790: 6374 696f 6e60 6020 6669 656c 640a 2020  ction`` field.  
+000217a0: 2020 2020 2020 2020 2020 2020 2020 6f6e                on
+000217b0: 2074 6865 2060 6072 6571 7565 7374 6060   the ``request``
+000217c0: 2069 6e73 7461 6e63 653b 2069 6620 6060   instance; if ``
+000217d0: 7265 7175 6573 7460 6020 6973 2070 726f  request`` is pro
+000217e0: 7669 6465 642c 2074 6869 730a 2020 2020  vided, this.    
+000217f0: 2020 2020 2020 2020 2020 2020 7368 6f75              shou
+00021800: 6c64 206e 6f74 2062 6520 7365 742e 0a20  ld not be set.. 
+00021810: 2020 2020 2020 2020 2020 2072 6574 7279             retry
+00021820: 2028 676f 6f67 6c65 2e61 7069 5f63 6f72   (google.api_cor
+00021830: 652e 7265 7472 792e 5265 7472 7929 3a20  e.retry.Retry): 
+00021840: 4465 7369 676e 6174 696f 6e20 6f66 2077  Designation of w
+00021850: 6861 7420 6572 726f 7273 2c20 6966 2061  hat errors, if a
+00021860: 6e79 2c0a 2020 2020 2020 2020 2020 2020  ny,.            
+00021870: 2020 2020 7368 6f75 6c64 2062 6520 7265      should be re
+00021880: 7472 6965 642e 0a20 2020 2020 2020 2020  tried..         
+00021890: 2020 2074 696d 656f 7574 2028 666c 6f61     timeout (floa
+000218a0: 7429 3a20 5468 6520 7469 6d65 6f75 7420  t): The timeout 
+000218b0: 666f 7220 7468 6973 2072 6571 7565 7374  for this request
+000218c0: 2e0a 2020 2020 2020 2020 2020 2020 6d65  ..            me
+000218d0: 7461 6461 7461 2028 5365 7175 656e 6365  tadata (Sequence
+000218e0: 5b54 7570 6c65 5b73 7472 2c20 7374 725d  [Tuple[str, str]
+000218f0: 5d29 3a20 5374 7269 6e67 7320 7768 6963  ]): Strings whic
+00021900: 6820 7368 6f75 6c64 2062 650a 2020 2020  h should be.    
+00021910: 2020 2020 2020 2020 2020 2020 7365 6e74              sent
+00021920: 2061 6c6f 6e67 2077 6974 6820 7468 6520   along with the 
+00021930: 7265 7175 6573 7420 6173 206d 6574 6164  request as metad
+00021940: 6174 612e 0a0a 2020 2020 2020 2020 5265  ata...        Re
+00021950: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+00021960: 2020 2067 6f6f 676c 652e 6170 7073 2e63     google.apps.c
+00021970: 6861 745f 7631 2e74 7970 6573 2e52 6561  hat_v1.types.Rea
+00021980: 6374 696f 6e3a 0a20 2020 2020 2020 2020  ction:.         
+00021990: 2020 2020 2020 2041 2072 6561 6374 696f         A reactio
+000219a0: 6e20 746f 2061 206d 6573 7361 6765 2e0a  n to a message..
+000219b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000219c0: 2020 2020 2320 4372 6561 7465 206f 7220      # Create or 
+000219d0: 636f 6572 6365 2061 2070 726f 746f 6275  coerce a protobu
+000219e0: 6620 7265 7175 6573 7420 6f62 6a65 6374  f request object
+000219f0: 2e0a 2020 2020 2020 2020 2320 5175 6963  ..        # Quic
+00021a00: 6b20 6368 6563 6b3a 2049 6620 7765 2067  k check: If we g
+00021a10: 6f74 2061 2072 6571 7565 7374 206f 626a  ot a request obj
+00021a20: 6563 742c 2077 6520 7368 6f75 6c64 202a  ect, we should *
+00021a30: 6e6f 742a 2068 6176 650a 2020 2020 2020  not* have.      
+00021a40: 2020 2320 676f 7474 656e 2061 6e79 206b    # gotten any k
+00021a50: 6579 776f 7264 2061 7267 756d 656e 7473  eyword arguments
+00021a60: 2074 6861 7420 6d61 7020 746f 2074 6865   that map to the
+00021a70: 2072 6571 7565 7374 2e0a 2020 2020 2020   request..      
+00021a80: 2020 6861 735f 666c 6174 7465 6e65 645f    has_flattened_
+00021a90: 7061 7261 6d73 203d 2061 6e79 285b 7061  params = any([pa
+00021aa0: 7265 6e74 2c20 7265 6163 7469 6f6e 5d29  rent, reaction])
+00021ab0: 0a20 2020 2020 2020 2069 6620 7265 7175  .        if requ
+00021ac0: 6573 7420 6973 206e 6f74 204e 6f6e 6520  est is not None 
+00021ad0: 616e 6420 6861 735f 666c 6174 7465 6e65  and has_flattene
+00021ae0: 645f 7061 7261 6d73 3a0a 2020 2020 2020  d_params:.      
+00021af0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00021b00: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+00021b10: 2020 2020 2020 2020 2249 6620 7468 6520          "If the 
+00021b20: 6072 6571 7565 7374 6020 6172 6775 6d65  `request` argume
+00021b30: 6e74 2069 7320 7365 742c 2074 6865 6e20  nt is set, then 
+00021b40: 6e6f 6e65 206f 6620 220a 2020 2020 2020  none of ".      
+00021b50: 2020 2020 2020 2020 2020 2274 6865 2069            "the i
+00021b60: 6e64 6976 6964 7561 6c20 6669 656c 6420  ndividual field 
+00021b70: 6172 6775 6d65 6e74 7320 7368 6f75 6c64  arguments should
+00021b80: 2062 6520 7365 742e 220a 2020 2020 2020   be set.".      
+00021b90: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00021ba0: 2023 204d 696e 6f72 206f 7074 696d 697a   # Minor optimiz
+00021bb0: 6174 696f 6e20 746f 2061 766f 6964 206d  ation to avoid m
+00021bc0: 616b 696e 6720 6120 636f 7079 2069 6620  aking a copy if 
+00021bd0: 7468 6520 7573 6572 2070 6173 7365 730a  the user passes.
+00021be0: 2020 2020 2020 2020 2320 696e 2061 2067          # in a g
+00021bf0: 635f 7265 6163 7469 6f6e 2e43 7265 6174  c_reaction.Creat
+00021c00: 6552 6561 6374 696f 6e52 6571 7565 7374  eReactionRequest
+00021c10: 2e0a 2020 2020 2020 2020 2320 5468 6572  ..        # Ther
+00021c20: 6527 7320 6e6f 2072 6973 6b20 6f66 206d  e's no risk of m
+00021c30: 6f64 6966 7969 6e67 2074 6865 2069 6e70  odifying the inp
+00021c40: 7574 2061 7320 7765 2776 6520 616c 7265  ut as we've alre
+00021c50: 6164 7920 7665 7269 6669 6564 0a20 2020  ady verified.   
+00021c60: 2020 2020 2023 2074 6865 7265 2061 7265       # there are
+00021c70: 206e 6f20 666c 6174 7465 6e65 6420 6669   no flattened fi
+00021c80: 656c 6473 2e0a 2020 2020 2020 2020 6966  elds..        if
+00021c90: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
+00021ca0: 7265 7175 6573 742c 2067 635f 7265 6163  request, gc_reac
+00021cb0: 7469 6f6e 2e43 7265 6174 6552 6561 6374  tion.CreateReact
+00021cc0: 696f 6e52 6571 7565 7374 293a 0a20 2020  ionRequest):.   
+00021cd0: 2020 2020 2020 2020 2072 6571 7565 7374           request
+00021ce0: 203d 2067 635f 7265 6163 7469 6f6e 2e43   = gc_reaction.C
+00021cf0: 7265 6174 6552 6561 6374 696f 6e52 6571  reateReactionReq
+00021d00: 7565 7374 2872 6571 7565 7374 290a 2020  uest(request).  
+00021d10: 2020 2020 2020 2020 2020 2320 4966 2077            # If w
+00021d20: 6520 6861 7665 206b 6579 776f 7264 2061  e have keyword a
+00021d30: 7267 756d 656e 7473 2063 6f72 7265 7370  rguments corresp
+00021d40: 6f6e 6469 6e67 2074 6f20 6669 656c 6473  onding to fields
+00021d50: 206f 6e20 7468 650a 2020 2020 2020 2020   on the.        
+00021d60: 2020 2020 2320 7265 7175 6573 742c 2061      # request, a
+00021d70: 7070 6c79 2074 6865 7365 2e0a 2020 2020  pply these..    
+00021d80: 2020 2020 2020 2020 6966 2070 6172 656e          if paren
+00021d90: 7420 6973 206e 6f74 204e 6f6e 653a 0a20  t is not None:. 
+00021da0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00021db0: 6571 7565 7374 2e70 6172 656e 7420 3d20  equest.parent = 
+00021dc0: 7061 7265 6e74 0a20 2020 2020 2020 2020  parent.         
+00021dd0: 2020 2069 6620 7265 6163 7469 6f6e 2069     if reaction i
+00021de0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00021df0: 2020 2020 2020 2020 2020 2020 7265 7175              requ
+00021e00: 6573 742e 7265 6163 7469 6f6e 203d 2072  est.reaction = r
+00021e10: 6561 6374 696f 6e0a 0a20 2020 2020 2020  eaction..       
+00021e20: 2023 2057 7261 7020 7468 6520 5250 4320   # Wrap the RPC 
+00021e30: 6d65 7468 6f64 3b20 7468 6973 2061 6464  method; this add
+00021e40: 7320 7265 7472 7920 616e 6420 7469 6d65  s retry and time
+00021e50: 6f75 7420 696e 666f 726d 6174 696f 6e2c  out information,
+00021e60: 0a20 2020 2020 2020 2023 2061 6e64 2066  .        # and f
+00021e70: 7269 656e 646c 7920 6572 726f 7220 6861  riendly error ha
+00021e80: 6e64 6c69 6e67 2e0a 2020 2020 2020 2020  ndling..        
+00021e90: 7270 6320 3d20 7365 6c66 2e5f 7472 616e  rpc = self._tran
+00021ea0: 7370 6f72 742e 5f77 7261 7070 6564 5f6d  sport._wrapped_m
+00021eb0: 6574 686f 6473 5b73 656c 662e 5f74 7261  ethods[self._tra
+00021ec0: 6e73 706f 7274 2e63 7265 6174 655f 7265  nsport.create_re
+00021ed0: 6163 7469 6f6e 5d0a 0a20 2020 2020 2020  action]..       
+00021ee0: 2023 2043 6572 7461 696e 2066 6965 6c64   # Certain field
+00021ef0: 7320 7368 6f75 6c64 2062 6520 7072 6f76  s should be prov
+00021f00: 6964 6564 2077 6974 6869 6e20 7468 6520  ided within the 
+00021f10: 6d65 7461 6461 7461 2068 6561 6465 723b  metadata header;
+00021f20: 0a20 2020 2020 2020 2023 2061 6464 2074  .        # add t
+00021f30: 6865 7365 2068 6572 652e 0a20 2020 2020  hese here..     
+00021f40: 2020 206d 6574 6164 6174 6120 3d20 7475     metadata = tu
+00021f50: 706c 6528 6d65 7461 6461 7461 2920 2b20  ple(metadata) + 
+00021f60: 280a 2020 2020 2020 2020 2020 2020 6761  (.            ga
+00021f70: 7069 635f 7631 2e72 6f75 7469 6e67 5f68  pic_v1.routing_h
+00021f80: 6561 6465 722e 746f 5f67 7270 635f 6d65  eader.to_grpc_me
+00021f90: 7461 6461 7461 2828 2822 7061 7265 6e74  tadata((("parent
+00021fa0: 222c 2072 6571 7565 7374 2e70 6172 656e  ", request.paren
+00021fb0: 7429 2c29 292c 0a20 2020 2020 2020 2029  t),)),.        )
+00021fc0: 0a0a 2020 2020 2020 2020 2320 5661 6c69  ..        # Vali
+00021fd0: 6461 7465 2074 6865 2075 6e69 7665 7273  date the univers
+00021fe0: 6520 646f 6d61 696e 2e0a 2020 2020 2020  e domain..      
+00021ff0: 2020 7365 6c66 2e5f 7661 6c69 6461 7465    self._validate
+00022000: 5f75 6e69 7665 7273 655f 646f 6d61 696e  _universe_domain
+00022010: 2829 0a0a 2020 2020 2020 2020 2320 5365  ()..        # Se
+00022020: 6e64 2074 6865 2072 6571 7565 7374 2e0a  nd the request..
+00022030: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+00022040: 203d 2072 7063 280a 2020 2020 2020 2020   = rpc(.        
+00022050: 2020 2020 7265 7175 6573 742c 0a20 2020      request,.   
+00022060: 2020 2020 2020 2020 2072 6574 7279 3d72           retry=r
+00022070: 6574 7279 2c0a 2020 2020 2020 2020 2020  etry,.          
+00022080: 2020 7469 6d65 6f75 743d 7469 6d65 6f75    timeout=timeou
+00022090: 742c 0a20 2020 2020 2020 2020 2020 206d  t,.            m
+000220a0: 6574 6164 6174 613d 6d65 7461 6461 7461  etadata=metadata
+000220b0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+000220c0: 2020 2020 2023 2044 6f6e 653b 2072 6574       # Done; ret
+000220d0: 7572 6e20 7468 6520 7265 7370 6f6e 7365  urn the response
+000220e0: 2e0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000220f0: 2072 6573 706f 6e73 650a 0a20 2020 2064   response..    d
+00022100: 6566 206c 6973 745f 7265 6163 7469 6f6e  ef list_reaction
+00022110: 7328 0a20 2020 2020 2020 2073 656c 662c  s(.        self,
+00022120: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
+00022130: 3a20 4f70 7469 6f6e 616c 5b55 6e69 6f6e  : Optional[Union
+00022140: 5b72 6561 6374 696f 6e2e 4c69 7374 5265  [reaction.ListRe
+00022150: 6163 7469 6f6e 7352 6571 7565 7374 2c20  actionsRequest, 
+00022160: 6469 6374 5d5d 203d 204e 6f6e 652c 0a20  dict]] = None,. 
+00022170: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
+00022180: 2020 7061 7265 6e74 3a20 4f70 7469 6f6e    parent: Option
+00022190: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
+000221a0: 2020 2020 2020 2020 7265 7472 793a 204f          retry: O
+000221b0: 7074 696f 6e61 6c52 6574 7279 203d 2067  ptionalRetry = g
+000221c0: 6170 6963 5f76 312e 6d65 7468 6f64 2e44  apic_v1.method.D
+000221d0: 4546 4155 4c54 2c0a 2020 2020 2020 2020  EFAULT,.        
+000221e0: 7469 6d65 6f75 743a 2055 6e69 6f6e 5b66  timeout: Union[f
+000221f0: 6c6f 6174 2c20 6f62 6a65 6374 5d20 3d20  loat, object] = 
+00022200: 6761 7069 635f 7631 2e6d 6574 686f 642e  gapic_v1.method.
+00022210: 4445 4641 554c 542c 0a20 2020 2020 2020  DEFAULT,.       
+00022220: 206d 6574 6164 6174 613a 2053 6571 7565   metadata: Seque
+00022230: 6e63 655b 5475 706c 655b 7374 722c 2073  nce[Tuple[str, s
+00022240: 7472 5d5d 203d 2028 292c 0a20 2020 2029  tr]] = (),.    )
+00022250: 202d 3e20 7061 6765 7273 2e4c 6973 7452   -> pagers.ListR
+00022260: 6561 6374 696f 6e73 5061 6765 723a 0a20  eactionsPager:. 
+00022270: 2020 2020 2020 2072 2222 224c 6973 7473         r"""Lists
+00022280: 2072 6561 6374 696f 6e73 2074 6f20 6120   reactions to a 
+00022290: 6d65 7373 6167 652e 2046 6f72 2061 6e20  message. For an 
+000222a0: 6578 616d 706c 652c 2073 6565 2060 4c69  example, see `Li
+000222b0: 7374 0a20 2020 2020 2020 2072 6561 6374  st.        react
+000222c0: 696f 6e73 2066 6f72 2061 0a20 2020 2020  ions for a.     
+000222d0: 2020 206d 6573 7361 6765 203c 6874 7470     message <http
+000222e0: 733a 2f2f 6465 7665 6c6f 7065 7273 2e67  s://developers.g
+000222f0: 6f6f 676c 652e 636f 6d2f 776f 726b 7370  oogle.com/worksp
+00022300: 6163 652f 6368 6174 2f6c 6973 742d 7265  ace/chat/list-re
+00022310: 6163 7469 6f6e 733e 605f 5f2e 0a20 2020  actions>`__..   
+00022320: 2020 2020 2052 6571 7569 7265 7320 6075       Requires `u
+00022330: 7365 720a 2020 2020 2020 2020 6175 7468  ser.        auth
+00022340: 656e 7469 6361 7469 6f6e 203c 6874 7470  entication <http
+00022350: 733a 2f2f 6465 7665 6c6f 7065 7273 2e67  s://developers.g
+00022360: 6f6f 676c 652e 636f 6d2f 776f 726b 7370  oogle.com/worksp
+00022370: 6163 652f 6368 6174 2f61 7574 6865 6e74  ace/chat/authent
+00022380: 6963 6174 652d 6175 7468 6f72 697a 652d  icate-authorize-
+00022390: 6368 6174 2d75 7365 723e 605f 5f2e 0a0a  chat-user>`__...
+000223a0: 2020 2020 2020 2020 2e2e 2063 6f64 652d          .. code-
+000223b0: 626c 6f63 6b3a 3a20 7079 7468 6f6e 0a0a  block:: python..
+000223c0: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
+000223d0: 6973 2073 6e69 7070 6574 2068 6173 2062  is snippet has b
+000223e0: 6565 6e20 6175 746f 6d61 7469 6361 6c6c  een automaticall
+000223f0: 7920 6765 6e65 7261 7465 6420 616e 6420  y generated and 
+00022400: 7368 6f75 6c64 2062 6520 7265 6761 7264  should be regard
+00022410: 6564 2061 7320 610a 2020 2020 2020 2020  ed as a.        
+00022420: 2020 2020 2320 636f 6465 2074 656d 706c      # code templ
+00022430: 6174 6520 6f6e 6c79 2e0a 2020 2020 2020  ate only..      
+00022440: 2020 2020 2020 2320 4974 2077 696c 6c20        # It will 
+00022450: 7265 7175 6972 6520 6d6f 6469 6669 6361  require modifica
+00022460: 7469 6f6e 7320 746f 2077 6f72 6b3a 0a20  tions to work:. 
+00022470: 2020 2020 2020 2020 2020 2023 202d 2049             # - I
+00022480: 7420 6d61 7920 7265 7175 6972 6520 636f  t may require co
+00022490: 7272 6563 742f 696e 2d72 616e 6765 2076  rrect/in-range v
+000224a0: 616c 7565 7320 666f 7220 7265 7175 6573  alues for reques
+000224b0: 7420 696e 6974 6961 6c69 7a61 7469 6f6e  t initialization
+000224c0: 2e0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+000224d0: 2d20 4974 206d 6179 2072 6571 7569 7265  - It may require
+000224e0: 2073 7065 6369 6679 696e 6720 7265 6769   specifying regi
+000224f0: 6f6e 616c 2065 6e64 706f 696e 7473 2077  onal endpoints w
+00022500: 6865 6e20 6372 6561 7469 6e67 2074 6865  hen creating the
+00022510: 2073 6572 7669 6365 0a20 2020 2020 2020   service.       
+00022520: 2020 2020 2023 2020 2063 6c69 656e 7420       #   client 
+00022530: 6173 2073 686f 776e 2069 6e3a 0a20 2020  as shown in:.   
+00022540: 2020 2020 2020 2020 2023 2020 2068 7474           #   htt
+00022550: 7073 3a2f 2f67 6f6f 676c 6561 7069 732e  ps://googleapis.
+00022560: 6465 762f 7079 7468 6f6e 2f67 6f6f 676c  dev/python/googl
+00022570: 652d 6170 692d 636f 7265 2f6c 6174 6573  e-api-core/lates
+00022580: 742f 636c 6965 6e74 5f6f 7074 696f 6e73  t/client_options
+00022590: 2e68 746d 6c0a 2020 2020 2020 2020 2020  .html.          
+000225a0: 2020 6672 6f6d 2067 6f6f 676c 652e 6170    from google.ap
+000225b0: 7073 2069 6d70 6f72 7420 6368 6174 5f76  ps import chat_v
+000225c0: 310a 0a20 2020 2020 2020 2020 2020 2064  1..            d
+000225d0: 6566 2073 616d 706c 655f 6c69 7374 5f72  ef sample_list_r
+000225e0: 6561 6374 696f 6e73 2829 3a0a 2020 2020  eactions():.    
+000225f0: 2020 2020 2020 2020 2020 2020 2320 4372              # Cr
+00022600: 6561 7465 2061 2063 6c69 656e 740a 2020  eate a client.  
+00022610: 2020 2020 2020 2020 2020 2020 2020 636c                cl
+00022620: 6965 6e74 203d 2063 6861 745f 7631 2e43  ient = chat_v1.C
+00022630: 6861 7453 6572 7669 6365 436c 6965 6e74  hatServiceClient
+00022640: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
+00022650: 2020 2020 2320 496e 6974 6961 6c69 7a65      # Initialize
+00022660: 2072 6571 7565 7374 2061 7267 756d 656e   request argumen
+00022670: 7428 7329 0a20 2020 2020 2020 2020 2020  t(s).           
+00022680: 2020 2020 2072 6571 7565 7374 203d 2063       request = c
+00022690: 6861 745f 7631 2e4c 6973 7452 6561 6374  hat_v1.ListReact
+000226a0: 696f 6e73 5265 7175 6573 7428 0a20 2020  ionsRequest(.   
+000226b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000226c0: 2070 6172 656e 743d 2270 6172 656e 745f   parent="parent_
+000226d0: 7661 6c75 6522 2c0a 2020 2020 2020 2020  value",.        
+000226e0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+000226f0: 2020 2020 2020 2020 2020 2023 204d 616b             # Mak
+00022700: 6520 7468 6520 7265 7175 6573 740a 2020  e the request.  
+00022710: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00022720: 6765 5f72 6573 756c 7420 3d20 636c 6965  ge_result = clie
+00022730: 6e74 2e6c 6973 745f 7265 6163 7469 6f6e  nt.list_reaction
+00022740: 7328 7265 7175 6573 743d 7265 7175 6573  s(request=reques
+00022750: 7429 0a0a 2020 2020 2020 2020 2020 2020  t)..            
+00022760: 2020 2020 2320 4861 6e64 6c65 2074 6865      # Handle the
+00022770: 2072 6573 706f 6e73 650a 2020 2020 2020   response.      
+00022780: 2020 2020 2020 2020 2020 666f 7220 7265            for re
+00022790: 7370 6f6e 7365 2069 6e20 7061 6765 5f72  sponse in page_r
+000227a0: 6573 756c 743a 0a20 2020 2020 2020 2020  esult:.         
+000227b0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+000227c0: 2872 6573 706f 6e73 6529 0a0a 2020 2020  (response)..    
+000227d0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+000227e0: 2020 2020 2020 7265 7175 6573 7420 2855        request (U
+000227f0: 6e69 6f6e 5b67 6f6f 676c 652e 6170 7073  nion[google.apps
+00022800: 2e63 6861 745f 7631 2e74 7970 6573 2e4c  .chat_v1.types.L
+00022810: 6973 7452 6561 6374 696f 6e73 5265 7175  istReactionsRequ
+00022820: 6573 742c 2064 6963 745d 293a 0a20 2020  est, dict]):.   
+00022830: 2020 2020 2020 2020 2020 2020 2054 6865               The
+00022840: 2072 6571 7565 7374 206f 626a 6563 742e   request object.
+00022850: 204c 6973 7473 2072 6561 6374 696f 6e73   Lists reactions
+00022860: 2074 6f20 6120 6d65 7373 6167 652e 0a20   to a message.. 
+00022870: 2020 2020 2020 2020 2020 2070 6172 656e             paren
+00022880: 7420 2873 7472 293a 0a20 2020 2020 2020  t (str):.       
+00022890: 2020 2020 2020 2020 2052 6571 7569 7265           Require
+000228a0: 642e 2054 6865 206d 6573 7361 6765 2075  d. The message u
+000228b0: 7365 7273 2072 6561 6374 6564 2074 6f2e  sers reacted to.
+000228c0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000228d0: 2020 466f 726d 6174 3a20 6060 7370 6163    Format: ``spac
+000228e0: 6573 2f7b 7370 6163 657d 2f6d 6573 7361  es/{space}/messa
+000228f0: 6765 732f 7b6d 6573 7361 6765 7d60 600a  ges/{message}``.
+00022900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022910: 2054 6869 7320 636f 7272 6573 706f 6e64   This correspond
+00022920: 7320 746f 2074 6865 2060 6070 6172 656e  s to the ``paren
+00022930: 7460 6020 6669 656c 640a 2020 2020 2020  t`` field.      
+00022940: 2020 2020 2020 2020 2020 6f6e 2074 6865            on the
+00022950: 2060 6072 6571 7565 7374 6060 2069 6e73   ``request`` ins
+00022960: 7461 6e63 653b 2069 6620 6060 7265 7175  tance; if ``requ
+00022970: 6573 7460 6020 6973 2070 726f 7669 6465  est`` is provide
+00022980: 642c 2074 6869 730a 2020 2020 2020 2020  d, this.        
+00022990: 2020 2020 2020 2020 7368 6f75 6c64 206e          should n
+000229a0: 6f74 2062 6520 7365 742e 0a20 2020 2020  ot be set..     
+000229b0: 2020 2020 2020 2072 6574 7279 2028 676f         retry (go
+000229c0: 6f67 6c65 2e61 7069 5f63 6f72 652e 7265  ogle.api_core.re
+000229d0: 7472 792e 5265 7472 7929 3a20 4465 7369  try.Retry): Desi
+000229e0: 676e 6174 696f 6e20 6f66 2077 6861 7420  gnation of what 
+000229f0: 6572 726f 7273 2c20 6966 2061 6e79 2c0a  errors, if any,.
+00022a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022a10: 7368 6f75 6c64 2062 6520 7265 7472 6965  should be retrie
+00022a20: 642e 0a20 2020 2020 2020 2020 2020 2074  d..            t
+00022a30: 696d 656f 7574 2028 666c 6f61 7429 3a20  imeout (float): 
+00022a40: 5468 6520 7469 6d65 6f75 7420 666f 7220  The timeout for 
+00022a50: 7468 6973 2072 6571 7565 7374 2e0a 2020  this request..  
+00022a60: 2020 2020 2020 2020 2020 6d65 7461 6461            metada
+00022a70: 7461 2028 5365 7175 656e 6365 5b54 7570  ta (Sequence[Tup
+00022a80: 6c65 5b73 7472 2c20 7374 725d 5d29 3a20  le[str, str]]): 
+00022a90: 5374 7269 6e67 7320 7768 6963 6820 7368  Strings which sh
+00022aa0: 6f75 6c64 2062 650a 2020 2020 2020 2020  ould be.        
+00022ab0: 2020 2020 2020 2020 7365 6e74 2061 6c6f          sent alo
+00022ac0: 6e67 2077 6974 6820 7468 6520 7265 7175  ng with the requ
+00022ad0: 6573 7420 6173 206d 6574 6164 6174 612e  est as metadata.
+00022ae0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00022af0: 733a 0a20 2020 2020 2020 2020 2020 2067  s:.            g
+00022b00: 6f6f 676c 652e 6170 7073 2e63 6861 745f  oogle.apps.chat_
+00022b10: 7631 2e73 6572 7669 6365 732e 6368 6174  v1.services.chat
+00022b20: 5f73 6572 7669 6365 2e70 6167 6572 732e  _service.pagers.
+00022b30: 4c69 7374 5265 6163 7469 6f6e 7350 6167  ListReactionsPag
+00022b40: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
+00022b50: 2020 2020 5265 7370 6f6e 7365 2074 6f20      Response to 
+00022b60: 6120 6c69 7374 2072 6561 6374 696f 6e73  a list reactions
+00022b70: 2072 6571 7565 7374 2e0a 0a20 2020 2020   request...     
+00022b80: 2020 2020 2020 2020 2020 2049 7465 7261             Itera
+00022b90: 7469 6e67 206f 7665 7220 7468 6973 206f  ting over this o
+00022ba0: 626a 6563 7420 7769 6c6c 2079 6965 6c64  bject will yield
+00022bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022bc0: 2072 6573 756c 7473 2061 6e64 2072 6573   results and res
+00022bd0: 6f6c 7665 2061 6464 6974 696f 6e61 6c20  olve additional 
+00022be0: 7061 6765 730a 2020 2020 2020 2020 2020  pages.          
+00022bf0: 2020 2020 2020 6175 746f 6d61 7469 6361        automatica
+00022c00: 6c6c 792e 0a0a 2020 2020 2020 2020 2222  lly...        ""
+00022c10: 220a 2020 2020 2020 2020 2320 4372 6561  ".        # Crea
+00022c20: 7465 206f 7220 636f 6572 6365 2061 2070  te or coerce a p
+00022c30: 726f 746f 6275 6620 7265 7175 6573 7420  rotobuf request 
+00022c40: 6f62 6a65 6374 2e0a 2020 2020 2020 2020  object..        
+00022c50: 2320 5175 6963 6b20 6368 6563 6b3a 2049  # Quick check: I
+00022c60: 6620 7765 2067 6f74 2061 2072 6571 7565  f we got a reque
+00022c70: 7374 206f 626a 6563 742c 2077 6520 7368  st object, we sh
+00022c80: 6f75 6c64 202a 6e6f 742a 2068 6176 650a  ould *not* have.
+00022c90: 2020 2020 2020 2020 2320 676f 7474 656e          # gotten
+00022ca0: 2061 6e79 206b 6579 776f 7264 2061 7267   any keyword arg
+00022cb0: 756d 656e 7473 2074 6861 7420 6d61 7020  uments that map 
+00022cc0: 746f 2074 6865 2072 6571 7565 7374 2e0a  to the request..
+00022cd0: 2020 2020 2020 2020 6861 735f 666c 6174          has_flat
+00022ce0: 7465 6e65 645f 7061 7261 6d73 203d 2061  tened_params = a
+00022cf0: 6e79 285b 7061 7265 6e74 5d29 0a20 2020  ny([parent]).   
+00022d00: 2020 2020 2069 6620 7265 7175 6573 7420       if request 
+00022d10: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+00022d20: 6861 735f 666c 6174 7465 6e65 645f 7061  has_flattened_pa
+00022d30: 7261 6d73 3a0a 2020 2020 2020 2020 2020  rams:.          
+00022d40: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00022d50: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+00022d60: 2020 2020 2249 6620 7468 6520 6072 6571      "If the `req
+00022d70: 7565 7374 6020 6172 6775 6d65 6e74 2069  uest` argument i
+00022d80: 7320 7365 742c 2074 6865 6e20 6e6f 6e65  s set, then none
+00022d90: 206f 6620 220a 2020 2020 2020 2020 2020   of ".          
+00022da0: 2020 2020 2020 2274 6865 2069 6e64 6976        "the indiv
+00022db0: 6964 7561 6c20 6669 656c 6420 6172 6775  idual field argu
+00022dc0: 6d65 6e74 7320 7368 6f75 6c64 2062 6520  ments should be 
+00022dd0: 7365 742e 220a 2020 2020 2020 2020 2020  set.".          
+00022de0: 2020 290a 0a20 2020 2020 2020 2023 204d    )..        # M
+00022df0: 696e 6f72 206f 7074 696d 697a 6174 696f  inor optimizatio
+00022e00: 6e20 746f 2061 766f 6964 206d 616b 696e  n to avoid makin
+00022e10: 6720 6120 636f 7079 2069 6620 7468 6520  g a copy if the 
+00022e20: 7573 6572 2070 6173 7365 730a 2020 2020  user passes.    
+00022e30: 2020 2020 2320 696e 2061 2072 6561 6374      # in a react
+00022e40: 696f 6e2e 4c69 7374 5265 6163 7469 6f6e  ion.ListReaction
+00022e50: 7352 6571 7565 7374 2e0a 2020 2020 2020  sRequest..      
+00022e60: 2020 2320 5468 6572 6527 7320 6e6f 2072    # There's no r
+00022e70: 6973 6b20 6f66 206d 6f64 6966 7969 6e67  isk of modifying
+00022e80: 2074 6865 2069 6e70 7574 2061 7320 7765   the input as we
+00022e90: 2776 6520 616c 7265 6164 7920 7665 7269  've already veri
+00022ea0: 6669 6564 0a20 2020 2020 2020 2023 2074  fied.        # t
+00022eb0: 6865 7265 2061 7265 206e 6f20 666c 6174  here are no flat
+00022ec0: 7465 6e65 6420 6669 656c 6473 2e0a 2020  tened fields..  
+00022ed0: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
+00022ee0: 6e73 7461 6e63 6528 7265 7175 6573 742c  nstance(request,
+00022ef0: 2072 6561 6374 696f 6e2e 4c69 7374 5265   reaction.ListRe
+00022f00: 6163 7469 6f6e 7352 6571 7565 7374 293a  actionsRequest):
+00022f10: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
+00022f20: 7565 7374 203d 2072 6561 6374 696f 6e2e  uest = reaction.
+00022f30: 4c69 7374 5265 6163 7469 6f6e 7352 6571  ListReactionsReq
+00022f40: 7565 7374 2872 6571 7565 7374 290a 2020  uest(request).  
+00022f50: 2020 2020 2020 2020 2020 2320 4966 2077            # If w
+00022f60: 6520 6861 7665 206b 6579 776f 7264 2061  e have keyword a
+00022f70: 7267 756d 656e 7473 2063 6f72 7265 7370  rguments corresp
+00022f80: 6f6e 6469 6e67 2074 6f20 6669 656c 6473  onding to fields
+00022f90: 206f 6e20 7468 650a 2020 2020 2020 2020   on the.        
+00022fa0: 2020 2020 2320 7265 7175 6573 742c 2061      # request, a
+00022fb0: 7070 6c79 2074 6865 7365 2e0a 2020 2020  pply these..    
+00022fc0: 2020 2020 2020 2020 6966 2070 6172 656e          if paren
+00022fd0: 7420 6973 206e 6f74 204e 6f6e 653a 0a20  t is not None:. 
+00022fe0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00022ff0: 6571 7565 7374 2e70 6172 656e 7420 3d20  equest.parent = 
+00023000: 7061 7265 6e74 0a0a 2020 2020 2020 2020  parent..        
+00023010: 2320 5772 6170 2074 6865 2052 5043 206d  # Wrap the RPC m
+00023020: 6574 686f 643b 2074 6869 7320 6164 6473  ethod; this adds
+00023030: 2072 6574 7279 2061 6e64 2074 696d 656f   retry and timeo
+00023040: 7574 2069 6e66 6f72 6d61 7469 6f6e 2c0a  ut information,.
+00023050: 2020 2020 2020 2020 2320 616e 6420 6672          # and fr
+00023060: 6965 6e64 6c79 2065 7272 6f72 2068 616e  iendly error han
+00023070: 646c 696e 672e 0a20 2020 2020 2020 2072  dling..        r
+00023080: 7063 203d 2073 656c 662e 5f74 7261 6e73  pc = self._trans
+00023090: 706f 7274 2e5f 7772 6170 7065 645f 6d65  port._wrapped_me
+000230a0: 7468 6f64 735b 7365 6c66 2e5f 7472 616e  thods[self._tran
+000230b0: 7370 6f72 742e 6c69 7374 5f72 6561 6374  sport.list_react
+000230c0: 696f 6e73 5d0a 0a20 2020 2020 2020 2023  ions]..        #
+000230d0: 2043 6572 7461 696e 2066 6965 6c64 7320   Certain fields 
+000230e0: 7368 6f75 6c64 2062 6520 7072 6f76 6964  should be provid
+000230f0: 6564 2077 6974 6869 6e20 7468 6520 6d65  ed within the me
+00023100: 7461 6461 7461 2068 6561 6465 723b 0a20  tadata header;. 
+00023110: 2020 2020 2020 2023 2061 6464 2074 6865         # add the
+00023120: 7365 2068 6572 652e 0a20 2020 2020 2020  se here..       
+00023130: 206d 6574 6164 6174 6120 3d20 7475 706c   metadata = tupl
+00023140: 6528 6d65 7461 6461 7461 2920 2b20 280a  e(metadata) + (.
+00023150: 2020 2020 2020 2020 2020 2020 6761 7069              gapi
+00023160: 635f 7631 2e72 6f75 7469 6e67 5f68 6561  c_v1.routing_hea
+00023170: 6465 722e 746f 5f67 7270 635f 6d65 7461  der.to_grpc_meta
+00023180: 6461 7461 2828 2822 7061 7265 6e74 222c  data((("parent",
+00023190: 2072 6571 7565 7374 2e70 6172 656e 7429   request.parent)
+000231a0: 2c29 292c 0a20 2020 2020 2020 2029 0a0a  ,)),.        )..
+000231b0: 2020 2020 2020 2020 2320 5661 6c69 6461          # Valida
+000231c0: 7465 2074 6865 2075 6e69 7665 7273 6520  te the universe 
+000231d0: 646f 6d61 696e 2e0a 2020 2020 2020 2020  domain..        
+000231e0: 7365 6c66 2e5f 7661 6c69 6461 7465 5f75  self._validate_u
+000231f0: 6e69 7665 7273 655f 646f 6d61 696e 2829  niverse_domain()
+00023200: 0a0a 2020 2020 2020 2020 2320 5365 6e64  ..        # Send
+00023210: 2074 6865 2072 6571 7565 7374 2e0a 2020   the request..  
+00023220: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
+00023230: 2072 7063 280a 2020 2020 2020 2020 2020   rpc(.          
+00023240: 2020 7265 7175 6573 742c 0a20 2020 2020    request,.     
+00023250: 2020 2020 2020 2072 6574 7279 3d72 6574         retry=ret
+00023260: 7279 2c0a 2020 2020 2020 2020 2020 2020  ry,.            
+00023270: 7469 6d65 6f75 743d 7469 6d65 6f75 742c  timeout=timeout,
+00023280: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
+00023290: 6164 6174 613d 6d65 7461 6461 7461 2c0a  adata=metadata,.
+000232a0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+000232b0: 2020 2023 2054 6869 7320 6d65 7468 6f64     # This method
+000232c0: 2069 7320 7061 6765 643b 2077 7261 7020   is paged; wrap 
+000232d0: 7468 6520 7265 7370 6f6e 7365 2069 6e20  the response in 
+000232e0: 6120 7061 6765 722c 2077 6869 6368 2070  a pager, which p
+000232f0: 726f 7669 6465 730a 2020 2020 2020 2020  rovides.        
+00023300: 2320 616e 2060 5f5f 6974 6572 5f5f 6020  # an `__iter__` 
+00023310: 636f 6e76 656e 6965 6e63 6520 6d65 7468  convenience meth
+00023320: 6f64 2e0a 2020 2020 2020 2020 7265 7370  od..        resp
+00023330: 6f6e 7365 203d 2070 6167 6572 732e 4c69  onse = pagers.Li
+00023340: 7374 5265 6163 7469 6f6e 7350 6167 6572  stReactionsPager
+00023350: 280a 2020 2020 2020 2020 2020 2020 6d65  (.            me
+00023360: 7468 6f64 3d72 7063 2c0a 2020 2020 2020  thod=rpc,.      
+00023370: 2020 2020 2020 7265 7175 6573 743d 7265        request=re
+00023380: 7175 6573 742c 0a20 2020 2020 2020 2020  quest,.         
+00023390: 2020 2072 6573 706f 6e73 653d 7265 7370     response=resp
+000233a0: 6f6e 7365 2c0a 2020 2020 2020 2020 2020  onse,.          
+000233b0: 2020 6d65 7461 6461 7461 3d6d 6574 6164    metadata=metad
+000233c0: 6174 612c 0a20 2020 2020 2020 2029 0a0a  ata,.        )..
+000233d0: 2020 2020 2020 2020 2320 446f 6e65 3b20          # Done; 
+000233e0: 7265 7475 726e 2074 6865 2072 6573 706f  return the respo
+000233f0: 6e73 652e 0a20 2020 2020 2020 2072 6574  nse..        ret
+00023400: 7572 6e20 7265 7370 6f6e 7365 0a0a 2020  urn response..  
+00023410: 2020 6465 6620 6465 6c65 7465 5f72 6561    def delete_rea
+00023420: 6374 696f 6e28 0a20 2020 2020 2020 2073  ction(.        s
+00023430: 656c 662c 0a20 2020 2020 2020 2072 6571  elf,.        req
+00023440: 7565 7374 3a20 4f70 7469 6f6e 616c 5b55  uest: Optional[U
+00023450: 6e69 6f6e 5b72 6561 6374 696f 6e2e 4465  nion[reaction.De
+00023460: 6c65 7465 5265 6163 7469 6f6e 5265 7175  leteReactionRequ
+00023470: 6573 742c 2064 6963 745d 5d20 3d20 4e6f  est, dict]] = No
+00023480: 6e65 2c0a 2020 2020 2020 2020 2a2c 0a20  ne,.        *,. 
+00023490: 2020 2020 2020 206e 616d 653a 204f 7074         name: Opt
+000234a0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+000234b0: 652c 0a20 2020 2020 2020 2072 6574 7279  e,.        retry
+000234c0: 3a20 4f70 7469 6f6e 616c 5265 7472 7920  : OptionalRetry 
+000234d0: 3d20 6761 7069 635f 7631 2e6d 6574 686f  = gapic_v1.metho
+000234e0: 642e 4445 4641 554c 542c 0a20 2020 2020  d.DEFAULT,.     
+000234f0: 2020 2074 696d 656f 7574 3a20 556e 696f     timeout: Unio
+00023500: 6e5b 666c 6f61 742c 206f 626a 6563 745d  n[float, object]
+00023510: 203d 2067 6170 6963 5f76 312e 6d65 7468   = gapic_v1.meth
+00023520: 6f64 2e44 4546 4155 4c54 2c0a 2020 2020  od.DEFAULT,.    
+00023530: 2020 2020 6d65 7461 6461 7461 3a20 5365      metadata: Se
+00023540: 7175 656e 6365 5b54 7570 6c65 5b73 7472  quence[Tuple[str
+00023550: 2c20 7374 725d 5d20 3d20 2829 2c0a 2020  , str]] = (),.  
+00023560: 2020 2920 2d3e 204e 6f6e 653a 0a20 2020    ) -> None:.   
+00023570: 2020 2020 2072 2222 2244 656c 6574 6573       r"""Deletes
+00023580: 2061 2072 6561 6374 696f 6e20 746f 2061   a reaction to a
+00023590: 206d 6573 7361 6765 2e20 4f6e 6c79 2075   message. Only u
+000235a0: 6e69 636f 6465 2065 6d6f 6a69 7320 6172  nicode emojis ar
+000235b0: 650a 2020 2020 2020 2020 7375 7070 6f72  e.        suppor
+000235c0: 7465 642e 2046 6f72 2061 6e20 6578 616d  ted. For an exam
+000235d0: 706c 652c 2073 6565 2060 4465 6c65 7465  ple, see `Delete
+000235e0: 2061 0a20 2020 2020 2020 2072 6561 6374   a.        react
+000235f0: 696f 6e20 3c68 7474 7073 3a2f 2f64 6576  ion <https://dev
+00023600: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
+00023610: 6f6d 2f77 6f72 6b73 7061 6365 2f63 6861  om/workspace/cha
+00023620: 742f 6465 6c65 7465 2d72 6561 6374 696f  t/delete-reactio
+00023630: 6e73 3e60 5f5f 2e0a 2020 2020 2020 2020  ns>`__..        
+00023640: 5265 7175 6972 6573 2060 7573 6572 0a20  Requires `user. 
+00023650: 2020 2020 2020 2061 7574 6865 6e74 6963         authentic
+00023660: 6174 696f 6e20 3c68 7474 7073 3a2f 2f64  ation <https://d
+00023670: 6576 656c 6f70 6572 732e 676f 6f67 6c65  evelopers.google
+00023680: 2e63 6f6d 2f77 6f72 6b73 7061 6365 2f63  .com/workspace/c
+00023690: 6861 742f 6175 7468 656e 7469 6361 7465  hat/authenticate
+000236a0: 2d61 7574 686f 7269 7a65 2d63 6861 742d  -authorize-chat-
+000236b0: 7573 6572 3e60 5f5f 2e0a 0a20 2020 2020  user>`__...     
+000236c0: 2020 202e 2e20 636f 6465 2d62 6c6f 636b     .. code-block
+000236d0: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
+000236e0: 2020 2020 2020 2023 2054 6869 7320 736e         # This sn
+000236f0: 6970 7065 7420 6861 7320 6265 656e 2061  ippet has been a
+00023700: 7574 6f6d 6174 6963 616c 6c79 2067 656e  utomatically gen
+00023710: 6572 6174 6564 2061 6e64 2073 686f 756c  erated and shoul
+00023720: 6420 6265 2072 6567 6172 6465 6420 6173  d be regarded as
+00023730: 2061 0a20 2020 2020 2020 2020 2020 2023   a.            #
+00023740: 2063 6f64 6520 7465 6d70 6c61 7465 206f   code template o
+00023750: 6e6c 792e 0a20 2020 2020 2020 2020 2020  nly..           
+00023760: 2023 2049 7420 7769 6c6c 2072 6571 7569   # It will requi
+00023770: 7265 206d 6f64 6966 6963 6174 696f 6e73  re modifications
+00023780: 2074 6f20 776f 726b 3a0a 2020 2020 2020   to work:.      
+00023790: 2020 2020 2020 2320 2d20 4974 206d 6179        # - It may
+000237a0: 2072 6571 7569 7265 2063 6f72 7265 6374   require correct
+000237b0: 2f69 6e2d 7261 6e67 6520 7661 6c75 6573  /in-range values
+000237c0: 2066 6f72 2072 6571 7565 7374 2069 6e69   for request ini
+000237d0: 7469 616c 697a 6174 696f 6e2e 0a20 2020  tialization..   
+000237e0: 2020 2020 2020 2020 2023 202d 2049 7420           # - It 
+000237f0: 6d61 7920 7265 7175 6972 6520 7370 6563  may require spec
+00023800: 6966 7969 6e67 2072 6567 696f 6e61 6c20  ifying regional 
+00023810: 656e 6470 6f69 6e74 7320 7768 656e 2063  endpoints when c
+00023820: 7265 6174 696e 6720 7468 6520 7365 7276  reating the serv
+00023830: 6963 650a 2020 2020 2020 2020 2020 2020  ice.            
+00023840: 2320 2020 636c 6965 6e74 2061 7320 7368  #   client as sh
+00023850: 6f77 6e20 696e 3a0a 2020 2020 2020 2020  own in:.        
+00023860: 2020 2020 2320 2020 6874 7470 733a 2f2f      #   https://
+00023870: 676f 6f67 6c65 6170 6973 2e64 6576 2f70  googleapis.dev/p
+00023880: 7974 686f 6e2f 676f 6f67 6c65 2d61 7069  ython/google-api
+00023890: 2d63 6f72 652f 6c61 7465 7374 2f63 6c69  -core/latest/cli
+000238a0: 656e 745f 6f70 7469 6f6e 732e 6874 6d6c  ent_options.html
+000238b0: 0a20 2020 2020 2020 2020 2020 2066 726f  .            fro
+000238c0: 6d20 676f 6f67 6c65 2e61 7070 7320 696d  m google.apps im
+000238d0: 706f 7274 2063 6861 745f 7631 0a0a 2020  port chat_v1..  
+000238e0: 2020 2020 2020 2020 2020 6465 6620 7361            def sa
+000238f0: 6d70 6c65 5f64 656c 6574 655f 7265 6163  mple_delete_reac
+00023900: 7469 6f6e 2829 3a0a 2020 2020 2020 2020  tion():.        
+00023910: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
+00023920: 2061 2063 6c69 656e 740a 2020 2020 2020   a client.      
+00023930: 2020 2020 2020 2020 2020 636c 6965 6e74            client
+00023940: 203d 2063 6861 745f 7631 2e43 6861 7453   = chat_v1.ChatS
+00023950: 6572 7669 6365 436c 6965 6e74 2829 0a0a  erviceClient()..
+00023960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023970: 2320 496e 6974 6961 6c69 7a65 2072 6571  # Initialize req
+00023980: 7565 7374 2061 7267 756d 656e 7428 7329  uest argument(s)
+00023990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000239a0: 2072 6571 7565 7374 203d 2063 6861 745f   request = chat_
+000239b0: 7631 2e44 656c 6574 6552 6561 6374 696f  v1.DeleteReactio
+000239c0: 6e52 6571 7565 7374 280a 2020 2020 2020  nRequest(.      
+000239d0: 2020 2020 2020 2020 2020 2020 2020 6e61                na
+000239e0: 6d65 3d22 6e61 6d65 5f76 616c 7565 222c  me="name_value",
+000239f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00023a00: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
+00023a10: 2020 2020 2320 4d61 6b65 2074 6865 2072      # Make the r
+00023a20: 6571 7565 7374 0a20 2020 2020 2020 2020  equest.         
+00023a30: 2020 2020 2020 2063 6c69 656e 742e 6465         client.de
+00023a40: 6c65 7465 5f72 6561 6374 696f 6e28 7265  lete_reaction(re
+00023a50: 7175 6573 743d 7265 7175 6573 7429 0a0a  quest=request)..
+00023a60: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00023a70: 2020 2020 2020 2020 2020 7265 7175 6573            reques
+00023a80: 7420 2855 6e69 6f6e 5b67 6f6f 676c 652e  t (Union[google.
+00023a90: 6170 7073 2e63 6861 745f 7631 2e74 7970  apps.chat_v1.typ
+00023aa0: 6573 2e44 656c 6574 6552 6561 6374 696f  es.DeleteReactio
+00023ab0: 6e52 6571 7565 7374 2c20 6469 6374 5d29  nRequest, dict])
+00023ac0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00023ad0: 2020 5468 6520 7265 7175 6573 7420 6f62    The request ob
+00023ae0: 6a65 6374 2e20 4465 6c65 7465 7320 6120  ject. Deletes a 
+00023af0: 7265 6163 7469 6f6e 2074 6f20 6120 6d65  reaction to a me
+00023b00: 7373 6167 652e 0a20 2020 2020 2020 2020  ssage..         
+00023b10: 2020 206e 616d 6520 2873 7472 293a 0a20     name (str):. 
+00023b20: 2020 2020 2020 2020 2020 2020 2020 2052                 R
+00023b30: 6571 7569 7265 642e 204e 616d 6520 6f66  equired. Name of
+00023b40: 2074 6865 2072 6561 6374 696f 6e20 746f   the reaction to
+00023b50: 2064 656c 6574 652e 0a0a 2020 2020 2020   delete...      
+00023b60: 2020 2020 2020 2020 2020 466f 726d 6174            Format
+00023b70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00023b80: 2020 6060 7370 6163 6573 2f7b 7370 6163    ``spaces/{spac
+00023b90: 657d 2f6d 6573 7361 6765 732f 7b6d 6573  e}/messages/{mes
+00023ba0: 7361 6765 7d2f 7265 6163 7469 6f6e 732f  sage}/reactions/
+00023bb0: 7b72 6561 6374 696f 6e7d 6060 0a0a 2020  {reaction}``..  
+00023bc0: 2020 2020 2020 2020 2020 2020 2020 5468                Th
+00023bd0: 6973 2063 6f72 7265 7370 6f6e 6473 2074  is corresponds t
+00023be0: 6f20 7468 6520 6060 6e61 6d65 6060 2066  o the ``name`` f
+00023bf0: 6965 6c64 0a20 2020 2020 2020 2020 2020  ield.           
+00023c00: 2020 2020 206f 6e20 7468 6520 6060 7265       on the ``re
+00023c10: 7175 6573 7460 6020 696e 7374 616e 6365  quest`` instance
+00023c20: 3b20 6966 2060 6072 6571 7565 7374 6060  ; if ``request``
+00023c30: 2069 7320 7072 6f76 6964 6564 2c20 7468   is provided, th
+00023c40: 6973 0a20 2020 2020 2020 2020 2020 2020  is.             
+00023c50: 2020 2073 686f 756c 6420 6e6f 7420 6265     should not be
+00023c60: 2073 6574 2e0a 2020 2020 2020 2020 2020   set..          
+00023c70: 2020 7265 7472 7920 2867 6f6f 676c 652e    retry (google.
+00023c80: 6170 695f 636f 7265 2e72 6574 7279 2e52  api_core.retry.R
+00023c90: 6574 7279 293a 2044 6573 6967 6e61 7469  etry): Designati
+00023ca0: 6f6e 206f 6620 7768 6174 2065 7272 6f72  on of what error
+00023cb0: 732c 2069 6620 616e 792c 0a20 2020 2020  s, if any,.     
+00023cc0: 2020 2020 2020 2020 2020 2073 686f 756c             shoul
+00023cd0: 6420 6265 2072 6574 7269 6564 2e0a 2020  d be retried..  
+00023ce0: 2020 2020 2020 2020 2020 7469 6d65 6f75            timeou
+00023cf0: 7420 2866 6c6f 6174 293a 2054 6865 2074  t (float): The t
+00023d00: 696d 656f 7574 2066 6f72 2074 6869 7320  imeout for this 
+00023d10: 7265 7175 6573 742e 0a20 2020 2020 2020  request..       
+00023d20: 2020 2020 206d 6574 6164 6174 6120 2853       metadata (S
+00023d30: 6571 7565 6e63 655b 5475 706c 655b 7374  equence[Tuple[st
+00023d40: 722c 2073 7472 5d5d 293a 2053 7472 696e  r, str]]): Strin
+00023d50: 6773 2077 6869 6368 2073 686f 756c 6420  gs which should 
+00023d60: 6265 0a20 2020 2020 2020 2020 2020 2020  be.             
+00023d70: 2020 2073 656e 7420 616c 6f6e 6720 7769     sent along wi
+00023d80: 7468 2074 6865 2072 6571 7565 7374 2061  th the request a
+00023d90: 7320 6d65 7461 6461 7461 2e0a 2020 2020  s metadata..    
+00023da0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00023db0: 2320 4372 6561 7465 206f 7220 636f 6572  # Create or coer
+00023dc0: 6365 2061 2070 726f 746f 6275 6620 7265  ce a protobuf re
+00023dd0: 7175 6573 7420 6f62 6a65 6374 2e0a 2020  quest object..  
+00023de0: 2020 2020 2020 2320 5175 6963 6b20 6368        # Quick ch
+00023df0: 6563 6b3a 2049 6620 7765 2067 6f74 2061  eck: If we got a
+00023e00: 2072 6571 7565 7374 206f 626a 6563 742c   request object,
+00023e10: 2077 6520 7368 6f75 6c64 202a 6e6f 742a   we should *not*
+00023e20: 2068 6176 650a 2020 2020 2020 2020 2320   have.        # 
+00023e30: 676f 7474 656e 2061 6e79 206b 6579 776f  gotten any keywo
+00023e40: 7264 2061 7267 756d 656e 7473 2074 6861  rd arguments tha
+00023e50: 7420 6d61 7020 746f 2074 6865 2072 6571  t map to the req
+00023e60: 7565 7374 2e0a 2020 2020 2020 2020 6861  uest..        ha
+00023e70: 735f 666c 6174 7465 6e65 645f 7061 7261  s_flattened_para
+00023e80: 6d73 203d 2061 6e79 285b 6e61 6d65 5d29  ms = any([name])
+00023e90: 0a20 2020 2020 2020 2069 6620 7265 7175  .        if requ
+00023ea0: 6573 7420 6973 206e 6f74 204e 6f6e 6520  est is not None 
+00023eb0: 616e 6420 6861 735f 666c 6174 7465 6e65  and has_flattene
+00023ec0: 645f 7061 7261 6d73 3a0a 2020 2020 2020  d_params:.      
+00023ed0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00023ee0: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+00023ef0: 2020 2020 2020 2020 2249 6620 7468 6520          "If the 
+00023f00: 6072 6571 7565 7374 6020 6172 6775 6d65  `request` argume
+00023f10: 6e74 2069 7320 7365 742c 2074 6865 6e20  nt is set, then 
+00023f20: 6e6f 6e65 206f 6620 220a 2020 2020 2020  none of ".      
+00023f30: 2020 2020 2020 2020 2020 2274 6865 2069            "the i
+00023f40: 6e64 6976 6964 7561 6c20 6669 656c 6420  ndividual field 
+00023f50: 6172 6775 6d65 6e74 7320 7368 6f75 6c64  arguments should
+00023f60: 2062 6520 7365 742e 220a 2020 2020 2020   be set.".      
+00023f70: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00023f80: 2023 204d 696e 6f72 206f 7074 696d 697a   # Minor optimiz
+00023f90: 6174 696f 6e20 746f 2061 766f 6964 206d  ation to avoid m
+00023fa0: 616b 696e 6720 6120 636f 7079 2069 6620  aking a copy if 
+00023fb0: 7468 6520 7573 6572 2070 6173 7365 730a  the user passes.
+00023fc0: 2020 2020 2020 2020 2320 696e 2061 2072          # in a r
+00023fd0: 6561 6374 696f 6e2e 4465 6c65 7465 5265  eaction.DeleteRe
+00023fe0: 6163 7469 6f6e 5265 7175 6573 742e 0a20  actionRequest.. 
+00023ff0: 2020 2020 2020 2023 2054 6865 7265 2773         # There's
+00024000: 206e 6f20 7269 736b 206f 6620 6d6f 6469   no risk of modi
+00024010: 6679 696e 6720 7468 6520 696e 7075 7420  fying the input 
+00024020: 6173 2077 6527 7665 2061 6c72 6561 6479  as we've already
+00024030: 2076 6572 6966 6965 640a 2020 2020 2020   verified.      
+00024040: 2020 2320 7468 6572 6520 6172 6520 6e6f    # there are no
+00024050: 2066 6c61 7474 656e 6564 2066 6965 6c64   flattened field
+00024060: 732e 0a20 2020 2020 2020 2069 6620 6e6f  s..        if no
+00024070: 7420 6973 696e 7374 616e 6365 2872 6571  t isinstance(req
+00024080: 7565 7374 2c20 7265 6163 7469 6f6e 2e44  uest, reaction.D
+00024090: 656c 6574 6552 6561 6374 696f 6e52 6571  eleteReactionReq
+000240a0: 7565 7374 293a 0a20 2020 2020 2020 2020  uest):.         
+000240b0: 2020 2072 6571 7565 7374 203d 2072 6561     request = rea
+000240c0: 6374 696f 6e2e 4465 6c65 7465 5265 6163  ction.DeleteReac
+000240d0: 7469 6f6e 5265 7175 6573 7428 7265 7175  tionRequest(requ
+000240e0: 6573 7429 0a20 2020 2020 2020 2020 2020  est).           
+000240f0: 2023 2049 6620 7765 2068 6176 6520 6b65   # If we have ke
+00024100: 7977 6f72 6420 6172 6775 6d65 6e74 7320  yword arguments 
+00024110: 636f 7272 6573 706f 6e64 696e 6720 746f  corresponding to
+00024120: 2066 6965 6c64 7320 6f6e 2074 6865 0a20   fields on the. 
+00024130: 2020 2020 2020 2020 2020 2023 2072 6571             # req
+00024140: 7565 7374 2c20 6170 706c 7920 7468 6573  uest, apply thes
+00024150: 652e 0a20 2020 2020 2020 2020 2020 2069  e..            i
+00024160: 6620 6e61 6d65 2069 7320 6e6f 7420 4e6f  f name is not No
+00024170: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00024180: 2020 2020 7265 7175 6573 742e 6e61 6d65      request.name
+00024190: 203d 206e 616d 650a 0a20 2020 2020 2020   = name..       
+000241a0: 2023 2057 7261 7020 7468 6520 5250 4320   # Wrap the RPC 
+000241b0: 6d65 7468 6f64 3b20 7468 6973 2061 6464  method; this add
+000241c0: 7320 7265 7472 7920 616e 6420 7469 6d65  s retry and time
+000241d0: 6f75 7420 696e 666f 726d 6174 696f 6e2c  out information,
+000241e0: 0a20 2020 2020 2020 2023 2061 6e64 2066  .        # and f
+000241f0: 7269 656e 646c 7920 6572 726f 7220 6861  riendly error ha
+00024200: 6e64 6c69 6e67 2e0a 2020 2020 2020 2020  ndling..        
+00024210: 7270 6320 3d20 7365 6c66 2e5f 7472 616e  rpc = self._tran
+00024220: 7370 6f72 742e 5f77 7261 7070 6564 5f6d  sport._wrapped_m
+00024230: 6574 686f 6473 5b73 656c 662e 5f74 7261  ethods[self._tra
+00024240: 6e73 706f 7274 2e64 656c 6574 655f 7265  nsport.delete_re
+00024250: 6163 7469 6f6e 5d0a 0a20 2020 2020 2020  action]..       
+00024260: 2023 2043 6572 7461 696e 2066 6965 6c64   # Certain field
+00024270: 7320 7368 6f75 6c64 2062 6520 7072 6f76  s should be prov
+00024280: 6964 6564 2077 6974 6869 6e20 7468 6520  ided within the 
+00024290: 6d65 7461 6461 7461 2068 6561 6465 723b  metadata header;
+000242a0: 0a20 2020 2020 2020 2023 2061 6464 2074  .        # add t
+000242b0: 6865 7365 2068 6572 652e 0a20 2020 2020  hese here..     
+000242c0: 2020 206d 6574 6164 6174 6120 3d20 7475     metadata = tu
+000242d0: 706c 6528 6d65 7461 6461 7461 2920 2b20  ple(metadata) + 
+000242e0: 280a 2020 2020 2020 2020 2020 2020 6761  (.            ga
+000242f0: 7069 635f 7631 2e72 6f75 7469 6e67 5f68  pic_v1.routing_h
+00024300: 6561 6465 722e 746f 5f67 7270 635f 6d65  eader.to_grpc_me
+00024310: 7461 6461 7461 2828 2822 6e61 6d65 222c  tadata((("name",
+00024320: 2072 6571 7565 7374 2e6e 616d 6529 2c29   request.name),)
+00024330: 292c 0a20 2020 2020 2020 2029 0a0a 2020  ),.        )..  
+00024340: 2020 2020 2020 2320 5661 6c69 6461 7465        # Validate
+00024350: 2074 6865 2075 6e69 7665 7273 6520 646f   the universe do
+00024360: 6d61 696e 2e0a 2020 2020 2020 2020 7365  main..        se
+00024370: 6c66 2e5f 7661 6c69 6461 7465 5f75 6e69  lf._validate_uni
+00024380: 7665 7273 655f 646f 6d61 696e 2829 0a0a  verse_domain()..
+00024390: 2020 2020 2020 2020 2320 5365 6e64 2074          # Send t
+000243a0: 6865 2072 6571 7565 7374 2e0a 2020 2020  he request..    
+000243b0: 2020 2020 7270 6328 0a20 2020 2020 2020      rpc(.       
+000243c0: 2020 2020 2072 6571 7565 7374 2c0a 2020       request,.  
+000243d0: 2020 2020 2020 2020 2020 7265 7472 793d            retry=
+000243e0: 7265 7472 792c 0a20 2020 2020 2020 2020  retry,.         
+000243f0: 2020 2074 696d 656f 7574 3d74 696d 656f     timeout=timeo
+00024400: 7574 2c0a 2020 2020 2020 2020 2020 2020  ut,.            
+00024410: 6d65 7461 6461 7461 3d6d 6574 6164 6174  metadata=metadat
+00024420: 612c 0a20 2020 2020 2020 2029 0a0a 2020  a,.        )..  
+00024430: 2020 6465 6620 5f5f 656e 7465 725f 5f28    def __enter__(
+00024440: 7365 6c66 2920 2d3e 2022 4368 6174 5365  self) -> "ChatSe
+00024450: 7276 6963 6543 6c69 656e 7422 3a0a 2020  rviceClient":.  
+00024460: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00024470: 660a 0a20 2020 2064 6566 205f 5f65 7869  f..    def __exi
+00024480: 745f 5f28 7365 6c66 2c20 7479 7065 2c20  t__(self, type, 
+00024490: 7661 6c75 652c 2074 7261 6365 6261 636b  value, traceback
+000244a0: 293a 0a20 2020 2020 2020 2022 2222 5265  ):.        """Re
+000244b0: 6c65 6173 6573 2075 6e64 6572 6c79 696e  leases underlyin
+000244c0: 6720 7472 616e 7370 6f72 7427 7320 7265  g transport's re
+000244d0: 736f 7572 6365 732e 0a0a 2020 2020 2020  sources...      
+000244e0: 2020 2e2e 2077 6172 6e69 6e67 3a3a 0a20    .. warning::. 
+000244f0: 2020 2020 2020 2020 2020 204f 4e4c 5920             ONLY 
+00024500: 7573 6520 6173 2061 2063 6f6e 7465 7874  use as a context
+00024510: 206d 616e 6167 6572 2069 6620 7468 6520   manager if the 
+00024520: 7472 616e 7370 6f72 7420 6973 204e 4f54  transport is NOT
+00024530: 2073 6861 7265 640a 2020 2020 2020 2020   shared.        
+00024540: 2020 2020 7769 7468 206f 7468 6572 2063      with other c
+00024550: 6c69 656e 7473 2120 4578 6974 696e 6720  lients! Exiting 
+00024560: 7468 6520 7769 7468 2062 6c6f 636b 2077  the with block w
+00024570: 696c 6c20 434c 4f53 4520 7468 6520 7472  ill CLOSE the tr
+00024580: 616e 7370 6f72 740a 2020 2020 2020 2020  ansport.        
+00024590: 2020 2020 616e 6420 6d61 7920 6361 7573      and may caus
+000245a0: 6520 6572 726f 7273 2069 6e20 6f74 6865  e errors in othe
+000245b0: 7220 636c 6965 6e74 7321 0a20 2020 2020  r clients!.     
+000245c0: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
+000245d0: 656c 662e 7472 616e 7370 6f72 742e 636c  elf.transport.cl
+000245e0: 6f73 6528 290a 0a0a 4445 4641 554c 545f  ose()...DEFAULT_
+000245f0: 434c 4945 4e54 5f49 4e46 4f20 3d20 6761  CLIENT_INFO = ga
+00024600: 7069 635f 7631 2e63 6c69 656e 745f 696e  pic_v1.client_in
+00024610: 666f 2e43 6c69 656e 7449 6e66 6f28 0a20  fo.ClientInfo(. 
+00024620: 2020 2067 6170 6963 5f76 6572 7369 6f6e     gapic_version
+00024630: 3d70 6163 6b61 6765 5f76 6572 7369 6f6e  =package_version
+00024640: 2e5f 5f76 6572 7369 6f6e 5f5f 0a29 0a0a  .__version__.)..
+00024650: 0a5f 5f61 6c6c 5f5f 203d 2028 2243 6861  .__all__ = ("Cha
+00024660: 7453 6572 7669 6365 436c 6965 6e74 222c  tServiceClient",
+00024670: 290a                                     ).
```

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/services/chat_service/pagers.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/services/chat_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/services/chat_service/transports/__init__.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/services/chat_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/services/chat_service/transports/base.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/services/chat_service/transports/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -400,14 +400,28 @@
                         core_exceptions.ServiceUnavailable,
                     ),
                     deadline=30.0,
                 ),
                 default_timeout=30.0,
                 client_info=client_info,
             ),
+            self.update_membership: gapic_v1.method.wrap_method(
+                self.update_membership,
+                default_retry=retries.Retry(
+                    initial=1.0,
+                    maximum=10.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=30.0,
+                ),
+                default_timeout=30.0,
+                client_info=client_info,
+            ),
             self.delete_membership: gapic_v1.method.wrap_method(
                 self.delete_membership,
                 default_retry=retries.Retry(
                     initial=1.0,
                     maximum=10.0,
                     multiplier=1.3,
                     predicate=retries.if_exception_type(
@@ -630,14 +644,23 @@
     ) -> Callable[
         [gc_membership.CreateMembershipRequest],
         Union[gc_membership.Membership, Awaitable[gc_membership.Membership]],
     ]:
         raise NotImplementedError()
 
     @property
+    def update_membership(
+        self,
+    ) -> Callable[
+        [gc_membership.UpdateMembershipRequest],
+        Union[gc_membership.Membership, Awaitable[gc_membership.Membership]],
+    ]:
+        raise NotImplementedError()
+
+    @property
     def delete_membership(
         self,
     ) -> Callable[
         [membership.DeleteMembershipRequest],
         Union[membership.Membership, Awaitable[membership.Membership]],
     ]:
         raise NotImplementedError()
```

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/services/chat_service/transports/grpc.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/services/chat_service/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -930,14 +930,41 @@
                 "/google.chat.v1.ChatService/CreateMembership",
                 request_serializer=gc_membership.CreateMembershipRequest.serialize,
                 response_deserializer=gc_membership.Membership.deserialize,
             )
         return self._stubs["create_membership"]
 
     @property
+    def update_membership(
+        self,
+    ) -> Callable[[gc_membership.UpdateMembershipRequest], gc_membership.Membership]:
+        r"""Return a callable for the update membership method over gRPC.
+
+        Updates a membership. Requires `user
+        authentication <https://developers.google.com/chat/api/guides/auth/users>`__.
+
+        Returns:
+            Callable[[~.UpdateMembershipRequest],
+                    ~.Membership]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "update_membership" not in self._stubs:
+            self._stubs["update_membership"] = self.grpc_channel.unary_unary(
+                "/google.chat.v1.ChatService/UpdateMembership",
+                request_serializer=gc_membership.UpdateMembershipRequest.serialize,
+                response_deserializer=gc_membership.Membership.deserialize,
+            )
+        return self._stubs["update_membership"]
+
+    @property
     def delete_membership(
         self,
     ) -> Callable[[membership.DeleteMembershipRequest], membership.Membership]:
         r"""Return a callable for the delete membership method over gRPC.
 
         Deletes a membership. For an example, see `Remove a user or a
         Google Chat app from a
```

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/services/chat_service/transports/grpc_asyncio.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/services/chat_service/transports/grpc_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -949,14 +949,43 @@
                 "/google.chat.v1.ChatService/CreateMembership",
                 request_serializer=gc_membership.CreateMembershipRequest.serialize,
                 response_deserializer=gc_membership.Membership.deserialize,
             )
         return self._stubs["create_membership"]
 
     @property
+    def update_membership(
+        self,
+    ) -> Callable[
+        [gc_membership.UpdateMembershipRequest], Awaitable[gc_membership.Membership]
+    ]:
+        r"""Return a callable for the update membership method over gRPC.
+
+        Updates a membership. Requires `user
+        authentication <https://developers.google.com/chat/api/guides/auth/users>`__.
+
+        Returns:
+            Callable[[~.UpdateMembershipRequest],
+                    Awaitable[~.Membership]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "update_membership" not in self._stubs:
+            self._stubs["update_membership"] = self.grpc_channel.unary_unary(
+                "/google.chat.v1.ChatService/UpdateMembership",
+                request_serializer=gc_membership.UpdateMembershipRequest.serialize,
+                response_deserializer=gc_membership.Membership.deserialize,
+            )
+        return self._stubs["update_membership"]
+
+    @property
     def delete_membership(
         self,
     ) -> Callable[
         [membership.DeleteMembershipRequest], Awaitable[membership.Membership]
     ]:
         r"""Return a callable for the delete membership method over gRPC.
```

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/services/chat_service/transports/rest.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/services/chat_service/transports/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,14 +210,22 @@
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_set_up_space(self, response):
                 logging.log(f"Received response: {response}")
                 return response
 
+            def pre_update_membership(self, request, metadata):
+                logging.log(f"Received request: {request}")
+                return request, metadata
+
+            def post_update_membership(self, response):
+                logging.log(f"Received response: {response}")
+                return response
+
             def pre_update_message(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_update_message(self, response):
                 logging.log(f"Received response: {response}")
                 return response
@@ -618,14 +626,37 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the ChatService server but before
         it is returned to user code.
         """
         return response
 
+    def pre_update_membership(
+        self,
+        request: gc_membership.UpdateMembershipRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[gc_membership.UpdateMembershipRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for update_membership
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the ChatService server.
+        """
+        return request, metadata
+
+    def post_update_membership(
+        self, response: gc_membership.Membership
+    ) -> gc_membership.Membership:
+        """Post-rpc interceptor for update_membership
+
+        Override in a subclass to manipulate the response
+        after it is returned by the ChatService server but before
+        it is returned to user code.
+        """
+        return response
+
     def pre_update_message(
         self,
         request: gc_message.UpdateMessageRequest,
         metadata: Sequence[Tuple[str, str]],
     ) -> Tuple[gc_message.UpdateMessageRequest, Sequence[Tuple[str, str]]]:
         """Pre-rpc interceptor for update_message
 
@@ -2446,14 +2477,115 @@
             resp = space.Space()
             pb_resp = space.Space.pb(resp)
 
             json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
             resp = self._interceptor.post_set_up_space(resp)
             return resp
 
+    class _UpdateMembership(ChatServiceRestStub):
+        def __hash__(self):
+            return hash("UpdateMembership")
+
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {
+            "updateMask": {},
+        }
+
+        @classmethod
+        def _get_unset_required_fields(cls, message_dict):
+            return {
+                k: v
+                for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
+                if k not in message_dict
+            }
+
+        def __call__(
+            self,
+            request: gc_membership.UpdateMembershipRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> gc_membership.Membership:
+            r"""Call the update membership method over HTTP.
+
+            Args:
+                request (~.gc_membership.UpdateMembershipRequest):
+                    The request object. Request message for updating a
+                membership.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                ~.gc_membership.Membership:
+                    Represents a membership relation in
+                Google Chat, such as whether a user or
+                Chat app is invited to, part of, or
+                absent from a space.
+
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "patch",
+                    "uri": "/v1/{membership.name=spaces/*/members/*}",
+                    "body": "membership",
+                },
+            ]
+            request, metadata = self._interceptor.pre_update_membership(
+                request, metadata
+            )
+            pb_request = gc_membership.UpdateMembershipRequest.pb(request)
+            transcoded_request = path_template.transcode(http_options, pb_request)
+
+            # Jsonify the request body
+
+            body = json_format.MessageToJson(
+                transcoded_request["body"], use_integers_for_enums=True
+            )
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(
+                json_format.MessageToJson(
+                    transcoded_request["query_params"],
+                    use_integers_for_enums=True,
+                )
+            )
+            query_params.update(self._get_unset_required_fields(query_params))
+
+            query_params["$alt"] = "json;enum-encoding=int"
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params, strict=True),
+                data=body,
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            # Return the response
+            resp = gc_membership.Membership()
+            pb_resp = gc_membership.Membership.pb(resp)
+
+            json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
+            resp = self._interceptor.post_update_membership(resp)
+            return resp
+
     class _UpdateMessage(ChatServiceRestStub):
         def __hash__(self):
             return hash("UpdateMessage")
 
         __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
@@ -2880,14 +3012,22 @@
     @property
     def set_up_space(self) -> Callable[[space_setup.SetUpSpaceRequest], space.Space]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._SetUpSpace(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
+    def update_membership(
+        self,
+    ) -> Callable[[gc_membership.UpdateMembershipRequest], gc_membership.Membership]:
+        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
+        # In C++ this would require a dynamic_cast
+        return self._UpdateMembership(self._session, self._host, self._interceptor)  # type: ignore
+
+    @property
     def update_message(
         self,
     ) -> Callable[[gc_message.UpdateMessageRequest], gc_message.Message]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._UpdateMessage(self._session, self._host, self._interceptor)  # type: ignore
```

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/types/__init__.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 from .membership import (
     CreateMembershipRequest,
     DeleteMembershipRequest,
     GetMembershipRequest,
     ListMembershipsRequest,
     ListMembershipsResponse,
     Membership,
+    UpdateMembershipRequest,
 )
 from .message import (
     AccessoryWidget,
     ActionResponse,
     AttachedGif,
     CardWithId,
     CreateMessageRequest,
@@ -108,14 +109,15 @@
     "MatchedUrl",
     "CreateMembershipRequest",
     "DeleteMembershipRequest",
     "GetMembershipRequest",
     "ListMembershipsRequest",
     "ListMembershipsResponse",
     "Membership",
+    "UpdateMembershipRequest",
     "AccessoryWidget",
     "ActionResponse",
     "AttachedGif",
     "CardWithId",
     "CreateMessageRequest",
     "DeleteMessageRequest",
     "Dialog",
```

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/types/action_status.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/types/action_status.py`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/types/annotation.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/types/annotation.py`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/types/attachment.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/types/attachment.py`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/types/chat_service.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/types/chat_service.py`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/types/contextual_addon.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/types/contextual_addon.py`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/types/deletion_metadata.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/types/deletion_metadata.py`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/types/group.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/types/group.py`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/types/history_state.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/types/history_state.py`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/types/matched_url.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/types/matched_url.py`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/types/membership.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/types/membership.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,24 +13,26 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from __future__ import annotations
 
 from typing import MutableMapping, MutableSequence
 
+from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 from google.apps.chat_v1.types import group, user
 
 __protobuf__ = proto.module(
     package="google.chat.v1",
     manifest={
         "Membership",
         "CreateMembershipRequest",
+        "UpdateMembershipRequest",
         "ListMembershipsRequest",
         "ListMembershipsResponse",
         "GetMembershipRequest",
         "DeleteMembershipRequest",
     },
 )
 
@@ -54,16 +56,14 @@
             Format: ``spaces/{space}/members/{member}``
         state (google.apps.chat_v1.types.Membership.MembershipState):
             Output only. State of the membership.
         role (google.apps.chat_v1.types.Membership.MembershipRole):
             Optional. User's role within a Chat space, which determines
             their permitted actions in the space.
 
-            `Developer
-            Preview <https://developers.google.com/workspace/preview>`__:
             This field can only be used as input in
             ``UpdateMembership``.
         member (google.apps.chat_v1.types.User):
             The Google Chat user or app the membership corresponds to.
             If your Chat app `authenticates as a
             user <https://developers.google.com/workspace/chat/authenticate-authorize-chat-user>`__,
             the output populates the
@@ -219,14 +219,42 @@
     membership: "Membership" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="Membership",
     )
 
 
+class UpdateMembershipRequest(proto.Message):
+    r"""Request message for updating a membership.
+
+    Attributes:
+        membership (google.apps.chat_v1.types.Membership):
+            Required. The membership to update. Only fields specified by
+            ``update_mask`` are updated.
+        update_mask (google.protobuf.field_mask_pb2.FieldMask):
+            Required. The field paths to update. Separate multiple
+            values with commas or use ``*`` to update all field paths.
+
+            Currently supported field paths:
+
+            -  ``role``
+    """
+
+    membership: "Membership" = proto.Field(
+        proto.MESSAGE,
+        number=1,
+        message="Membership",
+    )
+    update_mask: field_mask_pb2.FieldMask = proto.Field(
+        proto.MESSAGE,
+        number=2,
+        message=field_mask_pb2.FieldMask,
+    )
+
+
 class ListMembershipsRequest(proto.Message):
     r"""Request message for listing memberships.
 
     Attributes:
         parent (str):
             Required. The resource name of the space for
             which to fetch a membership list.
```

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/types/message.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/types/message.py`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/types/reaction.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/types/reaction.py`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/types/slash_command.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/types/slash_command.py`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/types/space.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/types/space.py`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/types/space_setup.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/types/space_setup.py`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/types/user.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/types/user.py`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/google/apps/chat_v1/types/widgets.py` & `google-apps-chat-0.1.4/google/apps/chat_v1/types/widgets.py`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/google_apps_chat.egg-info/PKG-INFO` & `google-apps-chat-0.1.4/google_apps_chat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-apps-chat
-Version: 0.1.3
+Version: 0.1.4
 Summary: Google Apps Chat API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-apps-chat
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-apps-chat-0.1.3/google_apps_chat.egg-info/SOURCES.txt` & `google-apps-chat-0.1.4/google_apps_chat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/setup.py` & `google-apps-chat-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/tests/__init__.py` & `google-apps-chat-0.1.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/tests/unit/__init__.py` & `google-apps-chat-0.1.4/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/tests/unit/gapic/__init__.py` & `google-apps-chat-0.1.4/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/tests/unit/gapic/chat_v1/__init__.py` & `google-apps-chat-0.1.4/tests/unit/gapic/chat_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-chat-0.1.3/tests/unit/gapic/chat_v1/test_chat_service.py` & `google-apps-chat-0.1.4/tests/unit/gapic/chat_v1/test_chat_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -6571,14 +6571,330 @@
             membership=gc_membership.Membership(name="name_value"),
         )
 
 
 @pytest.mark.parametrize(
     "request_type",
     [
+        gc_membership.UpdateMembershipRequest,
+        dict,
+    ],
+)
+def test_update_membership(request_type, transport: str = "grpc"):
+    client = ChatServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_membership), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = gc_membership.Membership(
+            name="name_value",
+            state=gc_membership.Membership.MembershipState.JOINED,
+            role=gc_membership.Membership.MembershipRole.ROLE_MEMBER,
+        )
+        response = client.update_membership(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        request = gc_membership.UpdateMembershipRequest()
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, gc_membership.Membership)
+    assert response.name == "name_value"
+    assert response.state == gc_membership.Membership.MembershipState.JOINED
+    assert response.role == gc_membership.Membership.MembershipRole.ROLE_MEMBER
+
+
+def test_update_membership_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ChatServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_membership), "__call__"
+    ) as call:
+        client.update_membership()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == gc_membership.UpdateMembershipRequest()
+
+
+def test_update_membership_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ChatServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = gc_membership.UpdateMembershipRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_membership), "__call__"
+    ) as call:
+        client.update_membership(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == gc_membership.UpdateMembershipRequest()
+
+
+@pytest.mark.asyncio
+async def test_update_membership_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ChatServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_membership), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            gc_membership.Membership(
+                name="name_value",
+                state=gc_membership.Membership.MembershipState.JOINED,
+                role=gc_membership.Membership.MembershipRole.ROLE_MEMBER,
+            )
+        )
+        response = await client.update_membership()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == gc_membership.UpdateMembershipRequest()
+
+
+@pytest.mark.asyncio
+async def test_update_membership_async(
+    transport: str = "grpc_asyncio", request_type=gc_membership.UpdateMembershipRequest
+):
+    client = ChatServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_membership), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            gc_membership.Membership(
+                name="name_value",
+                state=gc_membership.Membership.MembershipState.JOINED,
+                role=gc_membership.Membership.MembershipRole.ROLE_MEMBER,
+            )
+        )
+        response = await client.update_membership(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        request = gc_membership.UpdateMembershipRequest()
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, gc_membership.Membership)
+    assert response.name == "name_value"
+    assert response.state == gc_membership.Membership.MembershipState.JOINED
+    assert response.role == gc_membership.Membership.MembershipRole.ROLE_MEMBER
+
+
+@pytest.mark.asyncio
+async def test_update_membership_async_from_dict():
+    await test_update_membership_async(request_type=dict)
+
+
+def test_update_membership_field_headers():
+    client = ChatServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = gc_membership.UpdateMembershipRequest()
+
+    request.membership.name = "name_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_membership), "__call__"
+    ) as call:
+        call.return_value = gc_membership.Membership()
+        client.update_membership(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "membership.name=name_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_update_membership_field_headers_async():
+    client = ChatServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = gc_membership.UpdateMembershipRequest()
+
+    request.membership.name = "name_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_membership), "__call__"
+    ) as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            gc_membership.Membership()
+        )
+        await client.update_membership(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "membership.name=name_value",
+    ) in kw["metadata"]
+
+
+def test_update_membership_flattened():
+    client = ChatServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_membership), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = gc_membership.Membership()
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        client.update_membership(
+            membership=gc_membership.Membership(name="name_value"),
+            update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].membership
+        mock_val = gc_membership.Membership(name="name_value")
+        assert arg == mock_val
+        arg = args[0].update_mask
+        mock_val = field_mask_pb2.FieldMask(paths=["paths_value"])
+        assert arg == mock_val
+
+
+def test_update_membership_flattened_error():
+    client = ChatServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.update_membership(
+            gc_membership.UpdateMembershipRequest(),
+            membership=gc_membership.Membership(name="name_value"),
+            update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
+        )
+
+
+@pytest.mark.asyncio
+async def test_update_membership_flattened_async():
+    client = ChatServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_membership), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = gc_membership.Membership()
+
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            gc_membership.Membership()
+        )
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        response = await client.update_membership(
+            membership=gc_membership.Membership(name="name_value"),
+            update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].membership
+        mock_val = gc_membership.Membership(name="name_value")
+        assert arg == mock_val
+        arg = args[0].update_mask
+        mock_val = field_mask_pb2.FieldMask(paths=["paths_value"])
+        assert arg == mock_val
+
+
+@pytest.mark.asyncio
+async def test_update_membership_flattened_error_async():
+    client = ChatServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        await client.update_membership(
+            gc_membership.UpdateMembershipRequest(),
+            membership=gc_membership.Membership(name="name_value"),
+            update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
+        )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
         membership.DeleteMembershipRequest,
         dict,
     ],
 )
 def test_delete_membership(request_type, transport: str = "grpc"):
     client = ChatServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -13786,14 +14102,374 @@
         credentials=ga_credentials.AnonymousCredentials(), transport="rest"
     )
 
 
 @pytest.mark.parametrize(
     "request_type",
     [
+        gc_membership.UpdateMembershipRequest,
+        dict,
+    ],
+)
+def test_update_membership_rest(request_type):
+    client = ChatServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {"membership": {"name": "spaces/sample1/members/sample2"}}
+    request_init["membership"] = {
+        "name": "spaces/sample1/members/sample2",
+        "state": 1,
+        "role": 1,
+        "member": {
+            "name": "name_value",
+            "display_name": "display_name_value",
+            "domain_id": "domain_id_value",
+            "type_": 1,
+            "is_anonymous": True,
+        },
+        "group_member": {"name": "name_value"},
+        "create_time": {"seconds": 751, "nanos": 543},
+        "delete_time": {},
+    }
+    # The version of a generated dependency at test runtime may differ from the version used during generation.
+    # Delete any fields which are not present in the current runtime dependency
+    # See https://github.com/googleapis/gapic-generator-python/issues/1748
+
+    # Determine if the message type is proto-plus or protobuf
+    test_field = gc_membership.UpdateMembershipRequest.meta.fields["membership"]
+
+    def get_message_fields(field):
+        # Given a field which is a message (composite type), return a list with
+        # all the fields of the message.
+        # If the field is not a composite type, return an empty list.
+        message_fields = []
+
+        if hasattr(field, "message") and field.message:
+            is_field_type_proto_plus_type = not hasattr(field.message, "DESCRIPTOR")
+
+            if is_field_type_proto_plus_type:
+                message_fields = field.message.meta.fields.values()
+            # Add `# pragma: NO COVER` because there may not be any `*_pb2` field types
+            else:  # pragma: NO COVER
+                message_fields = field.message.DESCRIPTOR.fields
+        return message_fields
+
+    runtime_nested_fields = [
+        (field.name, nested_field.name)
+        for field in get_message_fields(test_field)
+        for nested_field in get_message_fields(field)
+    ]
+
+    subfields_not_in_runtime = []
+
+    # For each item in the sample request, create a list of sub fields which are not present at runtime
+    # Add `# pragma: NO COVER` because this test code will not run if all subfields are present at runtime
+    for field, value in request_init["membership"].items():  # pragma: NO COVER
+        result = None
+        is_repeated = False
+        # For repeated fields
+        if isinstance(value, list) and len(value):
+            is_repeated = True
+            result = value[0]
+        # For fields where the type is another message
+        if isinstance(value, dict):
+            result = value
+
+        if result and hasattr(result, "keys"):
+            for subfield in result.keys():
+                if (field, subfield) not in runtime_nested_fields:
+                    subfields_not_in_runtime.append(
+                        {
+                            "field": field,
+                            "subfield": subfield,
+                            "is_repeated": is_repeated,
+                        }
+                    )
+
+    # Remove fields from the sample request which are not present in the runtime version of the dependency
+    # Add `# pragma: NO COVER` because this test code will not run if all subfields are present at runtime
+    for subfield_to_delete in subfields_not_in_runtime:  # pragma: NO COVER
+        field = subfield_to_delete.get("field")
+        field_repeated = subfield_to_delete.get("is_repeated")
+        subfield = subfield_to_delete.get("subfield")
+        if subfield:
+            if field_repeated:
+                for i in range(0, len(request_init["membership"][field])):
+                    del request_init["membership"][field][i][subfield]
+            else:
+                del request_init["membership"][field][subfield]
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = gc_membership.Membership(
+            name="name_value",
+            state=gc_membership.Membership.MembershipState.JOINED,
+            role=gc_membership.Membership.MembershipRole.ROLE_MEMBER,
+        )
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        # Convert return value to protobuf type
+        return_value = gc_membership.Membership.pb(return_value)
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.update_membership(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, gc_membership.Membership)
+    assert response.name == "name_value"
+    assert response.state == gc_membership.Membership.MembershipState.JOINED
+    assert response.role == gc_membership.Membership.MembershipRole.ROLE_MEMBER
+
+
+def test_update_membership_rest_required_fields(
+    request_type=gc_membership.UpdateMembershipRequest,
+):
+    transport_class = transports.ChatServiceRestTransport
+
+    request_init = {}
+    request = request_type(**request_init)
+    pb_request = request_type.pb(request)
+    jsonified_request = json.loads(
+        json_format.MessageToJson(pb_request, use_integers_for_enums=False)
+    )
+
+    # verify fields with default values are dropped
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).update_membership._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with default values are now present
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).update_membership._get_unset_required_fields(jsonified_request)
+    # Check that path parameters and body parameters are not mixing in.
+    assert not set(unset_fields) - set(("update_mask",))
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with non-default values are left alone
+
+    client = ChatServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request = request_type(**request_init)
+
+    # Designate an appropriate value for the returned response.
+    return_value = gc_membership.Membership()
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(Session, "request") as req:
+        # We need to mock transcode() because providing default values
+        # for required fields will fail the real version if the http_options
+        # expect actual values for those fields.
+        with mock.patch.object(path_template, "transcode") as transcode:
+            # A uri without fields and an empty body will force all the
+            # request fields to show up in the query_params.
+            pb_request = request_type.pb(request)
+            transcode_result = {
+                "uri": "v1/sample_method",
+                "method": "patch",
+                "query_params": pb_request,
+            }
+            transcode_result["body"] = pb_request
+            transcode.return_value = transcode_result
+
+            response_value = Response()
+            response_value.status_code = 200
+
+            # Convert return value to protobuf type
+            return_value = gc_membership.Membership.pb(return_value)
+            json_return_value = json_format.MessageToJson(return_value)
+
+            response_value._content = json_return_value.encode("UTF-8")
+            req.return_value = response_value
+
+            response = client.update_membership(request)
+
+            expected_params = [("$alt", "json;enum-encoding=int")]
+            actual_params = req.call_args.kwargs["params"]
+            assert expected_params == actual_params
+
+
+def test_update_membership_rest_unset_required_fields():
+    transport = transports.ChatServiceRestTransport(
+        credentials=ga_credentials.AnonymousCredentials
+    )
+
+    unset_fields = transport.update_membership._get_unset_required_fields({})
+    assert set(unset_fields) == (
+        set(("updateMask",))
+        & set(
+            (
+                "membership",
+                "updateMask",
+            )
+        )
+    )
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_update_membership_rest_interceptors(null_interceptor):
+    transport = transports.ChatServiceRestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.ChatServiceRestInterceptor(),
+    )
+    client = ChatServiceClient(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        transports.ChatServiceRestInterceptor, "post_update_membership"
+    ) as post, mock.patch.object(
+        transports.ChatServiceRestInterceptor, "pre_update_membership"
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = gc_membership.UpdateMembershipRequest.pb(
+            gc_membership.UpdateMembershipRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = gc_membership.Membership.to_json(
+            gc_membership.Membership()
+        )
+
+        request = gc_membership.UpdateMembershipRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = gc_membership.Membership()
+
+        client.update_membership(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_update_membership_rest_bad_request(
+    transport: str = "rest", request_type=gc_membership.UpdateMembershipRequest
+):
+    client = ChatServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {"membership": {"name": "spaces/sample1/members/sample2"}}
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.update_membership(request)
+
+
+def test_update_membership_rest_flattened():
+    client = ChatServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = gc_membership.Membership()
+
+        # get arguments that satisfy an http rule for this method
+        sample_request = {"membership": {"name": "spaces/sample1/members/sample2"}}
+
+        # get truthy value for each flattened field
+        mock_args = dict(
+            membership=gc_membership.Membership(name="name_value"),
+            update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
+        )
+        mock_args.update(sample_request)
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        # Convert return value to protobuf type
+        return_value = gc_membership.Membership.pb(return_value)
+        json_return_value = json_format.MessageToJson(return_value)
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        client.update_membership(**mock_args)
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(req.mock_calls) == 1
+        _, args, _ = req.mock_calls[0]
+        assert path_template.validate(
+            "%s/v1/{membership.name=spaces/*/members/*}" % client.transport._host,
+            args[1],
+        )
+
+
+def test_update_membership_rest_flattened_error(transport: str = "rest"):
+    client = ChatServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.update_membership(
+            gc_membership.UpdateMembershipRequest(),
+            membership=gc_membership.Membership(name="name_value"),
+            update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
+        )
+
+
+def test_update_membership_rest_error():
+    client = ChatServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(), transport="rest"
+    )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
         membership.DeleteMembershipRequest,
         dict,
     ],
 )
 def test_delete_membership_rest(request_type):
     client = ChatServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -15144,14 +15820,15 @@
         "create_space",
         "set_up_space",
         "update_space",
         "delete_space",
         "complete_import_space",
         "find_direct_message",
         "create_membership",
+        "update_membership",
         "delete_membership",
         "create_reaction",
         "list_reactions",
         "delete_reaction",
     )
     for method in methods:
         with pytest.raises(NotImplementedError):
@@ -15519,14 +16196,17 @@
     assert session1 != session2
     session1 = client1.transport.find_direct_message._session
     session2 = client2.transport.find_direct_message._session
     assert session1 != session2
     session1 = client1.transport.create_membership._session
     session2 = client2.transport.create_membership._session
     assert session1 != session2
+    session1 = client1.transport.update_membership._session
+    session2 = client2.transport.update_membership._session
+    assert session1 != session2
     session1 = client1.transport.delete_membership._session
     session2 = client2.transport.delete_membership._session
     assert session1 != session2
     session1 = client1.transport.create_reaction._session
     session2 = client2.transport.create_reaction._session
     assert session1 != session2
     session1 = client1.transport.list_reactions._session
```

