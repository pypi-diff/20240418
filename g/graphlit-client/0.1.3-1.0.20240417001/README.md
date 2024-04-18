# Comparing `tmp/graphlit_client-0.1.3.tar.gz` & `tmp/graphlit_client-1.0.20240417001.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphlit_client-0.1.3.tar", last modified: Tue Mar 19 01:29:36 2024, max compression
+gzip compressed data, was "graphlit_client-1.0.20240417001.tar", last modified: Thu Apr 18 01:42:02 2024, max compression
```

## Comparing `graphlit_client-0.1.3.tar` & `graphlit_client-1.0.20240417001.tar`

### file list

```diff
@@ -1,15 +1,97 @@
-drwxr-xr-x   0 vaibhavprakashchhajed   (501) staff       (20)        0 2024-03-19 01:29:36.593897 graphlit_client-0.1.3/
--rw-r--r--   0 vaibhavprakashchhajed   (501) staff       (20)     1065 2024-03-19 01:00:26.000000 graphlit_client-0.1.3/LICENSE
--rw-r--r--   0 vaibhavprakashchhajed   (501) staff       (20)     2784 2024-03-19 01:29:36.593690 graphlit_client-0.1.3/PKG-INFO
--rw-r--r--   0 vaibhavprakashchhajed   (501) staff       (20)     2464 2024-03-19 01:26:47.000000 graphlit_client-0.1.3/README.md
-drwxr-xr-x   0 vaibhavprakashchhajed   (501) staff       (20)        0 2024-03-19 01:29:36.592649 graphlit_client-0.1.3/graphlit_client/
--rw-r--r--   0 vaibhavprakashchhajed   (501) staff       (20)       29 2024-03-19 01:00:26.000000 graphlit_client-0.1.3/graphlit_client/__init__.py
--rw-r--r--   0 vaibhavprakashchhajed   (501) staff       (20)     1891 2024-03-19 01:00:26.000000 graphlit_client-0.1.3/graphlit_client/client.py
-drwxr-xr-x   0 vaibhavprakashchhajed   (501) staff       (20)        0 2024-03-19 01:29:36.593429 graphlit_client-0.1.3/graphlit_client.egg-info/
--rw-r--r--   0 vaibhavprakashchhajed   (501) staff       (20)     2784 2024-03-19 01:29:36.000000 graphlit_client-0.1.3/graphlit_client.egg-info/PKG-INFO
--rw-r--r--   0 vaibhavprakashchhajed   (501) staff       (20)      274 2024-03-19 01:29:36.000000 graphlit_client-0.1.3/graphlit_client.egg-info/SOURCES.txt
--rw-r--r--   0 vaibhavprakashchhajed   (501) staff       (20)        1 2024-03-19 01:29:36.000000 graphlit_client-0.1.3/graphlit_client.egg-info/dependency_links.txt
--rw-r--r--   0 vaibhavprakashchhajed   (501) staff       (20)        6 2024-03-19 01:29:36.000000 graphlit_client-0.1.3/graphlit_client.egg-info/requires.txt
--rw-r--r--   0 vaibhavprakashchhajed   (501) staff       (20)       16 2024-03-19 01:29:36.000000 graphlit_client-0.1.3/graphlit_client.egg-info/top_level.txt
--rw-r--r--   0 vaibhavprakashchhajed   (501) staff       (20)       38 2024-03-19 01:29:36.593957 graphlit_client-0.1.3/setup.cfg
--rw-r--r--   0 vaibhavprakashchhajed   (501) staff       (20)      595 2024-03-19 01:29:26.000000 graphlit_client-0.1.3/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 01:42:02.555794 graphlit_client-1.0.20240417001/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1074 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-18 01:42:02.555794 graphlit_client-1.0.20240417001/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2253 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 01:42:02.535793 graphlit_client-1.0.20240417001/graphlit/
+-rw-r--r--   0 vsts      (1001) docker     (127)       31 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1757 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit/graphlit.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 01:42:02.551794 graphlit_client-1.0.20240417001/graphlit_api/
+-rw-r--r--   0 vsts      (1001) docker     (127)    58887 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/add_contents_to_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12578 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/async_base_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/base_model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/clear_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41993 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/close_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/create_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/create_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/create_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/create_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/create_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/create_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      984 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/credits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/delete_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/delete_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/delete_all_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/delete_all_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/delete_all_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/delete_all_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/delete_all_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      452 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/delete_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      482 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/delete_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/delete_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/delete_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/delete_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/delete_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/delete_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/delete_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/delete_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/delete_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/delete_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/disable_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/disable_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/enable_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/enable_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16585 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2411 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/extract_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3609 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/get_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/get_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7230 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/get_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4014 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/get_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7138 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/get_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4451 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/get_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7887 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/get_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      677 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/ingest_encoded_file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      606 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/ingest_text.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      598 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/ingest_uri.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    67968 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/input_types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/is_content_done.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/is_feed_done.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/lookup_credits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1568 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/lookup_usage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39264 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/operations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1236 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/project.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3242 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/prompt_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2055 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/prompt_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      796 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/publish_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/publish_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/query_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/query_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1112 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/query_content_facets.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7934 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/query_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4623 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/query_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7942 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/query_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4902 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/query_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8865 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/query_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/remove_contents_from_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/suggest_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/summarize_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/update_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/update_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      644 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/update_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/update_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/update_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/update_project.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/update_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/update_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1482 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/graphlit_api/usage.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 01:42:02.551794 graphlit_client-1.0.20240417001/graphlit_client.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-18 01:42:02.000000 graphlit_client-1.0.20240417001/graphlit_client.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2827 2024-04-18 01:42:02.000000 graphlit_client-1.0.20240417001/graphlit_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-18 01:42:02.000000 graphlit_client-1.0.20240417001/graphlit_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-04-18 01:42:02.000000 graphlit_client-1.0.20240417001/graphlit_client.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-04-18 01:42:02.000000 graphlit_client-1.0.20240417001/graphlit_client.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      292 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-18 01:42:02.555794 graphlit_client-1.0.20240417001/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      739 2024-04-18 01:41:46.000000 graphlit_client-1.0.20240417001/setup.py
```

### Comparing `graphlit_client-0.1.3/LICENSE` & `graphlit_client-1.0.20240417001/LICENSE`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 Graphlit
+Copyright (c) 2024 Unstruk Data Inc.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `graphlit_client-0.1.3/PKG-INFO` & `graphlit_client-1.0.20240417001/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,111 +1,83 @@
 Metadata-Version: 2.1
-Name: graphlit_client
-Version: 0.1.3
-Summary: A package for creating tokens for Graphlit services
+Name: graphlit-client
+Version: 1.0.20240417001
+Summary: Graphlit API Python Client
 Home-page: https://github.com/graphlit/graphlit-client-python
-Author: Graphlit
+Author: Unstruk Data Inc.
 Author-email: questions@graphlit.com
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: httpx
+Requires-Dist: pydantic<3.0.0,>=2.0.0
 Requires-Dist: PyJWT
+Requires-Dist: websockets
 
-# graphlit-client-python
+# Python Client for Graphlit Platform
 
 ## Overview
 
 The Graphlit Client for Python enables easy interaction with the Graphlit API, allowing developers to execute queries and mutations against the Graphlit service. This document outlines the setup process and provides a basic example of using the client.
 
 ## Prerequisites
 
 Before you begin, ensure you have the following:
 
 - Python 3.x installed on your system.
-- An active account on [graphlit.com](https://portal.graphlit.dev) with access to the API settings dashboard.
+- An active account on the [Graphlit Platform](https://portal.graphlit.dev) with access to the API settings dashboard.
 
 ## Installation
 
 To install the Graphlit Client, use pip:
 
 ```bash
 pip install graphlit-client
 ```
 
 ## Configuration
 
-The Graphlit Client requires three environment variables to be set for authentication and configuration:
+The Graphlit Client supports environment variables to be set for authentication and configuration:
 
-- `ENVIRONMENT_ID`: Your environment ID.
-- `ORGANIZATION_ID`: Your organization ID.
-- `SECRET_KEY`: Your secret key for API access.
+- `GRAPHLIT_ENVIRONMENT_ID`: Your environment ID.
+- `GRAPHLIT_ORGANIZATION_ID`: Your organization ID.
+- `GRAPHLIT_JWT_SECRET`: Your JWT secret for signing the JWT token.
 
-You can find these values in the API settings dashboard on [graphlit.com](https://portal.graphlit.dev).
+Alternately, you can pass these values with the constructor of the Graphlit client.
+
+You can find these values in the API settings dashboard on the [Graphlit Platform](https://portal.graphlit.dev).
 
 ### Setting Environment Variables
 
 To set these environment variables on your system, use the following commands, replacing `your_value` with the actual values from your account.
 
 For Unix/Linux/macOS:
 
 ```bash
-export ENVIRONMENT_ID=your_environment_id_value
-export ORGANIZATION_ID=your_organization_id_value
-export SECRET_KEY=your_secret_key_value
+export GRAPHLIT_ENVIRONMENT_ID=your_environment_id_value
+export GRAPHLIT_ORGANIZATION_ID=your_organization_id_value
+export GRAPHLIT_JWT_SECRET=your_secret_key_value
 ```
 
 For Windows Command Prompt (CMD):
 
 ```cmd
-set ENVIRONMENT_ID=your_environment_id_value
-set ORGANIZATION_ID=your_organization_id_value
-set SECRET_KEY=your_secret_key_value
+set GRAPHLIT_ENVIRONMENT_ID=your_environment_id_value
+set GRAPHLIT_ORGANIZATION_ID=your_organization_id_value
+set GRAPHLIT_JWT_SECRET=your_secret_key_value
 ```
 
 For Windows PowerShell:
 
 ```powershell
-$env:ENVIRONMENT_ID="your_environment_id_value"
-$env:ORGANIZATION_ID="your_organization_id_value"
-$env:SECRET_KEY="your_secret_key_value"
+$env:GRAPHLIT_ENVIRONMENT_ID="your_environment_id_value"
+$env:GRAPHLIT_ORGANIZATION_ID="your_organization_id_value"
+$env:GRAPHLIT_JWT_SECRET="your_secret_key_value"
 ```
 
-## Usage Example
-
-Here's a simple example of how to use the Graphlit Client to create a Feed.
-
-```python
-from graphlit_client import Graphlit
-
-# Initialize the client
-client = Graphlit()
-
-# Print the client token
-print(client.token)
-
-# Execute a query
-response = client.request(query="""
-mutation CreateFeed($feed: FeedInput!) {
-  createFeed(feed: $feed) {
-    id
-    name
-    state
-    type
-  }
-}""", variables={
-  "feed": {
-    "type": "WEB",
-    "web": {
-      "uri": "https://openai.com/blog"
-    },
-    "name": "OpenAI Blog"
-  }
-})
+## Support
 
-# Print the response
-print(response)
-```
+Please refer to the [Graphlit API Documentation](https://docs.graphlit.dev/).
 
-## Support
+For support with the Graphlit Client, please submit a [GitHub Issue](https://github.com/graphlit/graphlit-client-python/issues).  
 
-For issues and support with the Graphlit Client or API,  
-Please refer to the [documentation](https://docs.graphlit.dev/) and
-join our [Discord](https://discord.gg/ygFmfjy3Qx) community.
+For further support with the Graphlit Platform, please join our [Discord](https://discord.gg/ygFmfjy3Qx) community.
```

### Comparing `graphlit_client-0.1.3/README.md` & `graphlit_client-1.0.20240417001/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,100 +1,68 @@
-# graphlit-client-python
+# Python Client for Graphlit Platform
 
 ## Overview
 
 The Graphlit Client for Python enables easy interaction with the Graphlit API, allowing developers to execute queries and mutations against the Graphlit service. This document outlines the setup process and provides a basic example of using the client.
 
 ## Prerequisites
 
 Before you begin, ensure you have the following:
 
 - Python 3.x installed on your system.
-- An active account on [graphlit.com](https://portal.graphlit.dev) with access to the API settings dashboard.
+- An active account on the [Graphlit Platform](https://portal.graphlit.dev) with access to the API settings dashboard.
 
 ## Installation
 
 To install the Graphlit Client, use pip:
 
 ```bash
 pip install graphlit-client
 ```
 
 ## Configuration
 
-The Graphlit Client requires three environment variables to be set for authentication and configuration:
+The Graphlit Client supports environment variables to be set for authentication and configuration:
 
-- `ENVIRONMENT_ID`: Your environment ID.
-- `ORGANIZATION_ID`: Your organization ID.
-- `SECRET_KEY`: Your secret key for API access.
+- `GRAPHLIT_ENVIRONMENT_ID`: Your environment ID.
+- `GRAPHLIT_ORGANIZATION_ID`: Your organization ID.
+- `GRAPHLIT_JWT_SECRET`: Your JWT secret for signing the JWT token.
 
-You can find these values in the API settings dashboard on [graphlit.com](https://portal.graphlit.dev).
+Alternately, you can pass these values with the constructor of the Graphlit client.
+
+You can find these values in the API settings dashboard on the [Graphlit Platform](https://portal.graphlit.dev).
 
 ### Setting Environment Variables
 
 To set these environment variables on your system, use the following commands, replacing `your_value` with the actual values from your account.
 
 For Unix/Linux/macOS:
 
 ```bash
-export ENVIRONMENT_ID=your_environment_id_value
-export ORGANIZATION_ID=your_organization_id_value
-export SECRET_KEY=your_secret_key_value
+export GRAPHLIT_ENVIRONMENT_ID=your_environment_id_value
+export GRAPHLIT_ORGANIZATION_ID=your_organization_id_value
+export GRAPHLIT_JWT_SECRET=your_secret_key_value
 ```
 
 For Windows Command Prompt (CMD):
 
 ```cmd
-set ENVIRONMENT_ID=your_environment_id_value
-set ORGANIZATION_ID=your_organization_id_value
-set SECRET_KEY=your_secret_key_value
+set GRAPHLIT_ENVIRONMENT_ID=your_environment_id_value
+set GRAPHLIT_ORGANIZATION_ID=your_organization_id_value
+set GRAPHLIT_JWT_SECRET=your_secret_key_value
 ```
 
 For Windows PowerShell:
 
 ```powershell
-$env:ENVIRONMENT_ID="your_environment_id_value"
-$env:ORGANIZATION_ID="your_organization_id_value"
-$env:SECRET_KEY="your_secret_key_value"
+$env:GRAPHLIT_ENVIRONMENT_ID="your_environment_id_value"
+$env:GRAPHLIT_ORGANIZATION_ID="your_organization_id_value"
+$env:GRAPHLIT_JWT_SECRET="your_secret_key_value"
 ```
 
-## Usage Example
-
-Here's a simple example of how to use the Graphlit Client to create a Feed.
-
-```python
-from graphlit_client import Graphlit
-
-# Initialize the client
-client = Graphlit()
-
-# Print the client token
-print(client.token)
-
-# Execute a query
-response = client.request(query="""
-mutation CreateFeed($feed: FeedInput!) {
-  createFeed(feed: $feed) {
-    id
-    name
-    state
-    type
-  }
-}""", variables={
-  "feed": {
-    "type": "WEB",
-    "web": {
-      "uri": "https://openai.com/blog"
-    },
-    "name": "OpenAI Blog"
-  }
-})
+## Support
 
-# Print the response
-print(response)
-```
+Please refer to the [Graphlit API Documentation](https://docs.graphlit.dev/).
 
-## Support
+For support with the Graphlit Client, please submit a [GitHub Issue](https://github.com/graphlit/graphlit-client-python/issues).  
 
-For issues and support with the Graphlit Client or API,  
-Please refer to the [documentation](https://docs.graphlit.dev/) and
-join our [Discord](https://discord.gg/ygFmfjy3Qx) community.
+For further support with the Graphlit Platform, please join our [Discord](https://discord.gg/ygFmfjy3Qx) community.
```

### Comparing `graphlit_client-0.1.3/graphlit_client.egg-info/PKG-INFO` & `graphlit_client-1.0.20240417001/graphlit_client.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,111 +1,83 @@
 Metadata-Version: 2.1
 Name: graphlit-client
-Version: 0.1.3
-Summary: A package for creating tokens for Graphlit services
+Version: 1.0.20240417001
+Summary: Graphlit API Python Client
 Home-page: https://github.com/graphlit/graphlit-client-python
-Author: Graphlit
+Author: Unstruk Data Inc.
 Author-email: questions@graphlit.com
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: httpx
+Requires-Dist: pydantic<3.0.0,>=2.0.0
 Requires-Dist: PyJWT
+Requires-Dist: websockets
 
-# graphlit-client-python
+# Python Client for Graphlit Platform
 
 ## Overview
 
 The Graphlit Client for Python enables easy interaction with the Graphlit API, allowing developers to execute queries and mutations against the Graphlit service. This document outlines the setup process and provides a basic example of using the client.
 
 ## Prerequisites
 
 Before you begin, ensure you have the following:
 
 - Python 3.x installed on your system.
-- An active account on [graphlit.com](https://portal.graphlit.dev) with access to the API settings dashboard.
+- An active account on the [Graphlit Platform](https://portal.graphlit.dev) with access to the API settings dashboard.
 
 ## Installation
 
 To install the Graphlit Client, use pip:
 
 ```bash
 pip install graphlit-client
 ```
 
 ## Configuration
 
-The Graphlit Client requires three environment variables to be set for authentication and configuration:
+The Graphlit Client supports environment variables to be set for authentication and configuration:
 
-- `ENVIRONMENT_ID`: Your environment ID.
-- `ORGANIZATION_ID`: Your organization ID.
-- `SECRET_KEY`: Your secret key for API access.
+- `GRAPHLIT_ENVIRONMENT_ID`: Your environment ID.
+- `GRAPHLIT_ORGANIZATION_ID`: Your organization ID.
+- `GRAPHLIT_JWT_SECRET`: Your JWT secret for signing the JWT token.
 
-You can find these values in the API settings dashboard on [graphlit.com](https://portal.graphlit.dev).
+Alternately, you can pass these values with the constructor of the Graphlit client.
+
+You can find these values in the API settings dashboard on the [Graphlit Platform](https://portal.graphlit.dev).
 
 ### Setting Environment Variables
 
 To set these environment variables on your system, use the following commands, replacing `your_value` with the actual values from your account.
 
 For Unix/Linux/macOS:
 
 ```bash
-export ENVIRONMENT_ID=your_environment_id_value
-export ORGANIZATION_ID=your_organization_id_value
-export SECRET_KEY=your_secret_key_value
+export GRAPHLIT_ENVIRONMENT_ID=your_environment_id_value
+export GRAPHLIT_ORGANIZATION_ID=your_organization_id_value
+export GRAPHLIT_JWT_SECRET=your_secret_key_value
 ```
 
 For Windows Command Prompt (CMD):
 
 ```cmd
-set ENVIRONMENT_ID=your_environment_id_value
-set ORGANIZATION_ID=your_organization_id_value
-set SECRET_KEY=your_secret_key_value
+set GRAPHLIT_ENVIRONMENT_ID=your_environment_id_value
+set GRAPHLIT_ORGANIZATION_ID=your_organization_id_value
+set GRAPHLIT_JWT_SECRET=your_secret_key_value
 ```
 
 For Windows PowerShell:
 
 ```powershell
-$env:ENVIRONMENT_ID="your_environment_id_value"
-$env:ORGANIZATION_ID="your_organization_id_value"
-$env:SECRET_KEY="your_secret_key_value"
+$env:GRAPHLIT_ENVIRONMENT_ID="your_environment_id_value"
+$env:GRAPHLIT_ORGANIZATION_ID="your_organization_id_value"
+$env:GRAPHLIT_JWT_SECRET="your_secret_key_value"
 ```
 
-## Usage Example
-
-Here's a simple example of how to use the Graphlit Client to create a Feed.
-
-```python
-from graphlit_client import Graphlit
-
-# Initialize the client
-client = Graphlit()
-
-# Print the client token
-print(client.token)
-
-# Execute a query
-response = client.request(query="""
-mutation CreateFeed($feed: FeedInput!) {
-  createFeed(feed: $feed) {
-    id
-    name
-    state
-    type
-  }
-}""", variables={
-  "feed": {
-    "type": "WEB",
-    "web": {
-      "uri": "https://openai.com/blog"
-    },
-    "name": "OpenAI Blog"
-  }
-})
+## Support
 
-# Print the response
-print(response)
-```
+Please refer to the [Graphlit API Documentation](https://docs.graphlit.dev/).
 
-## Support
+For support with the Graphlit Client, please submit a [GitHub Issue](https://github.com/graphlit/graphlit-client-python/issues).  
 
-For issues and support with the Graphlit Client or API,  
-Please refer to the [documentation](https://docs.graphlit.dev/) and
-join our [Discord](https://discord.gg/ygFmfjy3Qx) community.
+For further support with the Graphlit Platform, please join our [Discord](https://discord.gg/ygFmfjy3Qx) community.
```

### Comparing `graphlit_client-0.1.3/setup.py` & `graphlit_client-1.0.20240417001/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 from setuptools import setup, find_packages
+import os
 
 # Read the content of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
+version = os.getenv('PACKAGE_VERSION', '1.0.0')
+
 setup(
-    name='graphlit_client',
-    version='0.1.3',
+    name='graphlit-client',
+    version=version,
     packages=find_packages(),
     install_requires=[
+        'httpx',
+        'pydantic>=2.0.0,<3.0.0',
         'PyJWT',
+        'websockets'
     ],
-    author='Graphlit',
+    python_requires='>=3.6',
+    author='Unstruk Data Inc.',
     author_email='questions@graphlit.com',
-    description='A package for creating tokens for Graphlit services',
+    description='Graphlit API Python Client',
     url='https://github.com/graphlit/graphlit-client-python',
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

