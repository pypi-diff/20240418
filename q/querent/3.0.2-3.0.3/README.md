# Comparing `tmp/querent-3.0.2.tar.gz` & `tmp/querent-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "querent-3.0.2.tar", last modified: Sat Apr 13 07:50:58 2024, max compression
+gzip compressed data, was "querent-3.0.3.tar", last modified: Thu Apr 18 21:26:32 2024, max compression
```

## Comparing `querent-3.0.2.tar` & `querent-3.0.3.tar`

### file list

```diff
@@ -1,267 +1,262 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.845642 querent-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-13 07:45:05.000000 querent-3.0.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)    17092 2024-04-13 07:50:58.845642 querent-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-04-13 07:45:05.000000 querent-3.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.773641 querent-3.0.2/querent/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-13 07:45:05.000000 querent-3.0.2/querent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.773641 querent-3.0.2/querent/callback/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-13 07:45:05.000000 querent-3.0.2/querent/callback/event_callback_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-13 07:45:05.000000 querent-3.0.2/querent/callback/event_callback_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.777641 querent-3.0.2/querent/channel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-13 07:45:05.000000 querent-3.0.2/querent/channel/channel_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.777641 querent-3.0.2/querent/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.777641 querent-3.0.2/querent/collectors/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.777641 querent-3.0.2/querent/collectors/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/aws/aws_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.777641 querent-3.0.2/querent/collectors/azure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/azure/azure_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/collector_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/collector_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/collector_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/collector_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.781641 querent-3.0.2/querent/collectors/drive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/drive/google_drive_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.781641 querent-3.0.2/querent/collectors/dropbox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/dropbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/dropbox/dropbox_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.781641 querent-3.0.2/querent/collectors/email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/email/email_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/email/imap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.781641 querent-3.0.2/querent/collectors/fs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/fs/fs_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.781641 querent-3.0.2/querent/collectors/gcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/gcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/gcs/gcs_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.781641 querent-3.0.2/querent/collectors/github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/github/github_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.785641 querent-3.0.2/querent/collectors/jira/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/jira/jira_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.785641 querent-3.0.2/querent/collectors/news/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/news/news_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.785641 querent-3.0.2/querent/collectors/slack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/slack/slack_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.785641 querent-3.0.2/querent/collectors/webscaper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/webscaper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/webscaper/web_scraper_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.789641 querent-3.0.2/querent/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/common_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.789641 querent-3.0.2/querent/common/errors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/errors/metric_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.793641 querent-3.0.2/querent/common/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/collected_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/collector_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/engine_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/file_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/ingested_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/ingested_images.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/ingested_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/ingested_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/querent_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/querent_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/resource_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/workflow_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/uri.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.793641 querent-3.0.2/querent/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.797641 querent-3.0.2/querent/config/collector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/collector/collector_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.797641 querent-3.0.2/querent/config/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/core/gpt_llm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/core/llm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/core/opensource_llm_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.797641 querent-3.0.2/querent/config/engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/engine/engine_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/graph_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.797641 querent-3.0.2/querent/config/ingestor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/ingestor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/ingestor/ingestor_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.801641 querent-3.0.2/querent/config/logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/logger/logger_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.801641 querent-3.0.2/querent/config/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/metric/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.801641 querent-3.0.2/querent/config/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/resource/resource_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.801641 querent-3.0.2/querent/config/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/workflow/workflow_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.801641 querent-3.0.2/querent/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/controllers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.801641 querent-3.0.2/querent/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11430 2024-04-13 07:45:05.000000 querent-3.0.2/querent/core/base_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.805641 querent-3.0.2/querent/core/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/core/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13746 2024-04-13 07:45:05.000000 querent-3.0.2/querent/core/transformers/bert_ner_opensourcellm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10369 2024-04-13 07:45:05.000000 querent-3.0.2/querent/core/transformers/fixed_entities_set_opensourcellm.py
--rw-r--r--   0 runner    (1001) docker     (127)    16808 2024-04-13 07:45:05.000000 querent-3.0.2/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py
--rw-r--r--   0 runner    (1001) docker     (127)    21403 2024-04-13 07:45:05.000000 querent-3.0.2/querent/core/transformers/gpt_llm_gpt_ner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12910 2024-04-13 07:45:05.000000 querent-3.0.2/querent/core/transformers/relationship_extraction_llm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.805641 querent-3.0.2/querent/dal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/dal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.805641 querent-3.0.2/querent/gnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/gnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.809641 querent-3.0.2/querent/graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-13 07:45:05.000000 querent-3.0.2/querent/graph/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-04-13 07:45:05.000000 querent-3.0.2/querent/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-13 07:45:05.000000 querent-3.0.2/querent/graph/graph_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-13 07:45:05.000000 querent-3.0.2/querent/graph/ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-13 07:45:05.000000 querent-3.0.2/querent/graph/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-04-13 07:45:05.000000 querent-3.0.2/querent/graph/shacl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-13 07:45:05.000000 querent-3.0.2/querent/graph/subject.py
--rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-04-13 07:45:05.000000 querent-3.0.2/querent/graph/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.813641 querent-3.0.2/querent/ingestors/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.813641 querent-3.0.2/querent/ingestors/audio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/audio/audio_ingestors.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/base_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.813641 querent-3.0.2/querent/ingestors/code/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/code/code_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.813641 querent-3.0.2/querent/ingestors/csv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/csv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/csv/csv_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.813641 querent-3.0.2/querent/ingestors/doc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/doc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/doc/doc_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.817641 querent-3.0.2/querent/ingestors/email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/email/email_ingestor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/email/email_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.817641 querent-3.0.2/querent/ingestors/github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/github/github_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.817641 querent-3.0.2/querent/ingestors/html/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/html/html_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.817641 querent-3.0.2/querent/ingestors/images/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/images/image_ingestor.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/ingestor_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/ingestor_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.817641 querent-3.0.2/querent/ingestors/json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/json/json_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.817641 querent-3.0.2/querent/ingestors/pdfs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/pdfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/pdfs/pdf_ingestor_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.821642 querent-3.0.2/querent/ingestors/ppt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/ppt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/ppt/ppt_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.821642 querent-3.0.2/querent/ingestors/texts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/texts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/texts/text_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.821642 querent-3.0.2/querent/ingestors/video/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/video/video_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.821642 querent-3.0.2/querent/ingestors/xlsx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/xlsx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/xlsx/xlsx_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.821642 querent-3.0.2/querent/ingestors/xml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/xml/xml_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.821642 querent-3.0.2/querent/insights/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/insights/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.821642 querent-3.0.2/querent/kg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.825641 querent-3.0.2/querent/kg/ner_helperfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/ner_helperfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/ner_helperfunctions/attn_scores.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/ner_helperfunctions/contextual_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/ner_helperfunctions/dependency_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/ner_helperfunctions/filter_triples.py
--rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/ner_helperfunctions/fixed_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/ner_helperfunctions/fixed_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/ner_helperfunctions/ner_llm_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/querent_kg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.829642 querent-3.0.2/querent/kg/rel_helperfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/rel_helperfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/rel_helperfunctions/contextual_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/rel_helperfunctions/embedding_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/rel_helperfunctions/filter_semantic_triples.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/rel_helperfunctions/fixed_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/rel_helperfunctions/opeai_ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/rel_helperfunctions/openai_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/rel_helperfunctions/openllm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/rel_helperfunctions/questionanswer_llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/rel_helperfunctions/rag_retriever.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/rel_helperfunctions/rel_normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/rel_helperfunctions/triple_to_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.833642 querent-3.0.2/querent/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-13 07:45:05.000000 querent-3.0.2/querent/logging/custom_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-13 07:45:05.000000 querent-3.0.2/querent/logging/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-13 07:45:05.000000 querent-3.0.2/querent/logging/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-13 07:45:05.000000 querent-3.0.2/querent/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.833642 querent-3.0.2/querent/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.837642 querent-3.0.2/querent/metric/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/metric/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-13 07:45:05.000000 querent-3.0.2/querent/metric/adapters/promethus_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-13 07:45:05.000000 querent-3.0.2/querent/metric/base_metric_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-13 07:45:05.000000 querent-3.0.2/querent/metric/metric_logging_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-13 07:45:05.000000 querent-3.0.2/querent/metric/metric_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.837642 querent-3.0.2/querent/processors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-13 07:45:05.000000 querent-3.0.2/querent/processors/async_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-13 07:45:05.000000 querent-3.0.2/querent/processors/text_cleanup_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-13 07:45:05.000000 querent-3.0.2/querent/processors/text_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.837642 querent-3.0.2/querent/querent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/querent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-13 07:45:05.000000 querent-3.0.2/querent/querent/auto_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-13 07:45:05.000000 querent-3.0.2/querent/querent/querent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-13 07:45:05.000000 querent-3.0.2/querent/querent/resource_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/querent/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.837642 querent-3.0.2/querent/search/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/search/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.841642 querent-3.0.2/querent/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-13 07:45:05.000000 querent-3.0.2/querent/storage/gcs_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-13 07:45:05.000000 querent-3.0.2/querent/storage/milvus_vectorevent_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-13 07:45:05.000000 querent-3.0.2/querent/storage/neo4j_graphevent_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-13 07:45:05.000000 querent-3.0.2/querent/storage/postgres_graphevent_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-13 07:45:05.000000 querent-3.0.2/querent/storage/s3-data-management.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.841642 querent-3.0.2/querent/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10882 2024-04-13 07:45:05.000000 querent-3.0.2/querent/tools/web_page_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.841642 querent-3.0.2/querent/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-13 07:45:05.000000 querent-3.0.2/querent/utils/webpage_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.845642 querent-3.0.2/querent/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-13 07:45:05.000000 querent-3.0.2/querent/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-04-13 07:45:05.000000 querent-3.0.2/querent/workflow/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-04-13 07:45:05.000000 querent-3.0.2/querent/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.845642 querent-3.0.2/querent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17092 2024-04-13 07:50:58.000000 querent-3.0.2/querent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-04-13 07:50:58.000000 querent-3.0.2/querent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 07:50:58.000000 querent-3.0.2/querent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-13 07:50:58.000000 querent-3.0.2/querent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-13 07:50:58.000000 querent-3.0.2/querent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 07:50:58.845642 querent-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-04-13 07:45:05.000000 querent-3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.857486 querent-3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-18 21:20:47.000000 querent-3.0.3/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)    17092 2024-04-18 21:26:32.857486 querent-3.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-04-18 21:20:47.000000 querent-3.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.797486 querent-3.0.3/querent/
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-18 21:20:47.000000 querent-3.0.3/querent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.797486 querent-3.0.3/querent/callback/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-18 21:20:47.000000 querent-3.0.3/querent/callback/event_callback_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-18 21:20:47.000000 querent-3.0.3/querent/callback/event_callback_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.797486 querent-3.0.3/querent/channel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-18 21:20:47.000000 querent-3.0.3/querent/channel/channel_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.797486 querent-3.0.3/querent/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.801486 querent-3.0.3/querent/collectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.801486 querent-3.0.3/querent/collectors/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/aws/aws_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.801486 querent-3.0.3/querent/collectors/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/azure/azure_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/collector_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/collector_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/collector_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/collector_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.801486 querent-3.0.3/querent/collectors/drive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/drive/google_drive_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.801486 querent-3.0.3/querent/collectors/dropbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/dropbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/dropbox/dropbox_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.805486 querent-3.0.3/querent/collectors/email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/email/email_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/email/imap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.805486 querent-3.0.3/querent/collectors/fs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/fs/fs_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.805486 querent-3.0.3/querent/collectors/gcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/gcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/gcs/gcs_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.805486 querent-3.0.3/querent/collectors/github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/github/github_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.805486 querent-3.0.3/querent/collectors/jira/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/jira/jira_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.805486 querent-3.0.3/querent/collectors/news/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/news/news_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.805486 querent-3.0.3/querent/collectors/slack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/slack/slack_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.809486 querent-3.0.3/querent/collectors/webscaper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/webscaper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-18 21:20:47.000000 querent-3.0.3/querent/collectors/webscaper/web_scraper_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.809486 querent-3.0.3/querent/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/common_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.809486 querent-3.0.3/querent/common/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/errors/metric_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.813486 querent-3.0.3/querent/common/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/collected_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/collector_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/engine_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/file_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/ingested_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/ingested_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/ingested_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/ingested_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/querent_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/querent_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/resource_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/types/workflow_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-18 21:20:47.000000 querent-3.0.3/querent/common/uri.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.817486 querent-3.0.3/querent/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.817486 querent-3.0.3/querent/config/collector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/collector/collector_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.817486 querent-3.0.3/querent/config/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/core/gpt_llm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/core/llm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/core/opensource_llm_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.817486 querent-3.0.3/querent/config/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/engine/engine_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/graph_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.817486 querent-3.0.3/querent/config/ingestor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/ingestor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/ingestor/ingestor_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.817486 querent-3.0.3/querent/config/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/logger/logger_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.821486 querent-3.0.3/querent/config/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/metric/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.821486 querent-3.0.3/querent/config/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/resource/resource_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.821486 querent-3.0.3/querent/config/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-18 21:20:47.000000 querent-3.0.3/querent/config/workflow/workflow_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.821486 querent-3.0.3/querent/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/controllers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.821486 querent-3.0.3/querent/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-18 21:20:47.000000 querent-3.0.3/querent/core/base_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.825486 querent-3.0.3/querent/core/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/core/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13817 2024-04-18 21:20:47.000000 querent-3.0.3/querent/core/transformers/bert_ner_opensourcellm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-04-18 21:20:47.000000 querent-3.0.3/querent/core/transformers/fixed_entities_set_opensourcellm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16897 2024-04-18 21:20:47.000000 querent-3.0.3/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21490 2024-04-18 21:20:47.000000 querent-3.0.3/querent/core/transformers/gpt_llm_gpt_ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12910 2024-04-18 21:20:47.000000 querent-3.0.3/querent/core/transformers/relationship_extraction_llm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.825486 querent-3.0.3/querent/dal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/dal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.825486 querent-3.0.3/querent/gnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/gnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.825486 querent-3.0.3/querent/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-18 21:20:47.000000 querent-3.0.3/querent/graph/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-04-18 21:20:47.000000 querent-3.0.3/querent/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-18 21:20:47.000000 querent-3.0.3/querent/graph/graph_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-18 21:20:47.000000 querent-3.0.3/querent/graph/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-18 21:20:47.000000 querent-3.0.3/querent/graph/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-04-18 21:20:47.000000 querent-3.0.3/querent/graph/shacl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-18 21:20:47.000000 querent-3.0.3/querent/graph/subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-04-18 21:20:47.000000 querent-3.0.3/querent/graph/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.829486 querent-3.0.3/querent/ingestors/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.829486 querent-3.0.3/querent/ingestors/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/audio/audio_ingestors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/base_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.829486 querent-3.0.3/querent/ingestors/code/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/code/code_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.829486 querent-3.0.3/querent/ingestors/csv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/csv/csv_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.829486 querent-3.0.3/querent/ingestors/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/doc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/doc/doc_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.833486 querent-3.0.3/querent/ingestors/email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/email/email_ingestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/email/email_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.833486 querent-3.0.3/querent/ingestors/github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/github/github_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.833486 querent-3.0.3/querent/ingestors/html/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/html/html_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.833486 querent-3.0.3/querent/ingestors/images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/images/image_ingestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/ingestor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/ingestor_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.833486 querent-3.0.3/querent/ingestors/json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/json/json_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.833486 querent-3.0.3/querent/ingestors/pdfs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/pdfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/pdfs/pdf_ingestor_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.833486 querent-3.0.3/querent/ingestors/ppt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/ppt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/ppt/ppt_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.837486 querent-3.0.3/querent/ingestors/texts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/texts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/texts/text_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.837486 querent-3.0.3/querent/ingestors/video/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/video/video_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.837486 querent-3.0.3/querent/ingestors/xlsx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/xlsx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/xlsx/xlsx_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.837486 querent-3.0.3/querent/ingestors/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-18 21:20:47.000000 querent-3.0.3/querent/ingestors/xml/xml_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.837486 querent-3.0.3/querent/kg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.841486 querent-3.0.3/querent/kg/ner_helperfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/ner_helperfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/ner_helperfunctions/attn_scores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/ner_helperfunctions/contextual_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/ner_helperfunctions/dependency_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/ner_helperfunctions/filter_triples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/ner_helperfunctions/fixed_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/ner_helperfunctions/fixed_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/ner_helperfunctions/ner_llm_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/querent_kg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.845486 querent-3.0.3/querent/kg/rel_helperfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/rel_helperfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/rel_helperfunctions/contextual_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/rel_helperfunctions/embedding_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/rel_helperfunctions/filter_semantic_triples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/rel_helperfunctions/fixed_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/rel_helperfunctions/opeai_ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/rel_helperfunctions/openai_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/rel_helperfunctions/openllm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/rel_helperfunctions/questionanswer_llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/rel_helperfunctions/rag_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/rel_helperfunctions/rel_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-18 21:20:47.000000 querent-3.0.3/querent/kg/rel_helperfunctions/triple_to_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.845486 querent-3.0.3/querent/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-18 21:20:47.000000 querent-3.0.3/querent/logging/custom_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-18 21:20:47.000000 querent-3.0.3/querent/logging/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-18 21:20:47.000000 querent-3.0.3/querent/logging/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-18 21:20:47.000000 querent-3.0.3/querent/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.849486 querent-3.0.3/querent/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.849486 querent-3.0.3/querent/metric/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/metric/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-18 21:20:47.000000 querent-3.0.3/querent/metric/adapters/promethus_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-18 21:20:47.000000 querent-3.0.3/querent/metric/base_metric_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-18 21:20:47.000000 querent-3.0.3/querent/metric/metric_logging_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-18 21:20:47.000000 querent-3.0.3/querent/metric/metric_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.849486 querent-3.0.3/querent/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-18 21:20:47.000000 querent-3.0.3/querent/processors/async_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-18 21:20:47.000000 querent-3.0.3/querent/processors/text_cleanup_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-18 21:20:47.000000 querent-3.0.3/querent/processors/text_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.853486 querent-3.0.3/querent/querent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/querent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-18 21:20:47.000000 querent-3.0.3/querent/querent/auto_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-18 21:20:47.000000 querent-3.0.3/querent/querent/querent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-18 21:20:47.000000 querent-3.0.3/querent/querent/resource_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/querent/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.853486 querent-3.0.3/querent/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-18 21:20:47.000000 querent-3.0.3/querent/storage/gcs_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-18 21:20:47.000000 querent-3.0.3/querent/storage/milvus_vectorevent_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-18 21:20:47.000000 querent-3.0.3/querent/storage/neo4j_graphevent_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-18 21:20:47.000000 querent-3.0.3/querent/storage/postgres_graphevent_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.853486 querent-3.0.3/querent/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10882 2024-04-18 21:20:47.000000 querent-3.0.3/querent/tools/web_page_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.853486 querent-3.0.3/querent/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:20:47.000000 querent-3.0.3/querent/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-18 21:20:47.000000 querent-3.0.3/querent/utils/webpage_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.853486 querent-3.0.3/querent/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 21:20:47.000000 querent-3.0.3/querent/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-04-18 21:20:47.000000 querent-3.0.3/querent/workflow/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-18 21:20:47.000000 querent-3.0.3/querent/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:26:32.857486 querent-3.0.3/querent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17092 2024-04-18 21:26:32.000000 querent-3.0.3/querent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-18 21:26:32.000000 querent-3.0.3/querent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 21:26:32.000000 querent-3.0.3/querent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-18 21:26:32.000000 querent-3.0.3/querent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 21:26:32.000000 querent-3.0.3/querent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 21:26:32.857486 querent-3.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-04-18 21:20:47.000000 querent-3.0.3/setup.py
```

### Comparing `querent-3.0.2/LICENCE` & `querent-3.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/PKG-INFO` & `querent-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querent
-Version: 3.0.2
+Version: 3.0.3
 Summary: The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 Home-page: https://github.com/Querent-ai/querent-ai
 Author: Querent AI
 License: Business Source License 1.1
 Project-URL: Documentation, https://github.com/Querent-ai/querent-ai/docs
 Project-URL: Issue Tracker, https://github.com/Querent-ai/querent-ai/issues
 Keywords: Graph Neural Network,Scalability,Data-Driven Insights,GNN,Async,Knowledge Graphs,KG,Large Language Models,asyncio,Insights,aysnchronous,LLM,transformers,pytorch,Llama-index,AI,Artificial Intelligence,Neo4j,Queues,QuiAssisstant,Collectors,Data,Data Science,Data Engineering,Data Analysis,Data Analytics,News,NLP,Natural Language Processing,Text,Text Analysis,Deep Learning,Graphs,Graph Theory,Graph Algorithms,Graph Analytics,Graph Databases,Graph Processing,Graph Mining,Graph Neural Networks,GNN,GNNs,Graph Neural Network
```

### Comparing `querent-3.0.2/README.md` & `querent-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/__init__.py` & `querent-3.0.3/querent/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,12 @@
 from .querent.querent import Querent
 from .processors import *
 
 # System Data Storage
 # System Callbacks
 from .callback import *
 
-# System Insights
-from .insights import *
-
 # System Logging and Utilities
 from .core import *
 from .utils import *
 from .logging import *
 from .workflow import *
```

### Comparing `querent-3.0.2/querent/callback/event_callback_dispatcher.py` & `querent-3.0.3/querent/callback/event_callback_dispatcher.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/callback/event_callback_interface.py` & `querent-3.0.3/querent/callback/event_callback_interface.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/channel/channel_interface.py` & `querent-3.0.3/querent/channel/channel_interface.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/collectors/aws/aws_collector.py` & `querent-3.0.3/querent/collectors/aws/aws_collector.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,16 +48,16 @@
 
         try:
             response = self.s3_client.list_objects_v2(Bucket=self.bucket_name)
 
             for obj in response.get("Contents", []):
                 file = self.download_object_as_byte_stream(obj["Key"])
                 async for chunk in self.read_chunks(file):
-                    yield CollectedBytes(file=obj["Key"], data=chunk, error=None)
-                yield CollectedBytes(file=obj["Key"], data=None, error=None, eof=True)
+                    yield CollectedBytes(file=obj["Key"], data=chunk, error=None, doc_source=f"s3://{self.bucket_name}/{self.region}")
+                yield CollectedBytes(file=obj["Key"], data=None, error=None, eof=True, doc_source=f"s3://{self.bucket_name}/{self.region}")
 
         except PermissionError as exc:
             self.logger.error(f"Getting Permission Error on file {file}, as {exc}")
         except OSError as exc:
             self.logger.error(f"Getting OS Error on file {file}, as {exc}")
         finally:
             await self.disconnect()  # Disconnect when done
```

### Comparing `querent-3.0.2/querent/collectors/azure/azure_collector.py` & `querent-3.0.3/querent/collectors/azure/azure_collector.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,16 +53,16 @@
 
             blob_list = self.container_client.list_blobs(name_starts_with=self.prefix)
             for blob in blob_list:
                 file = self.download_blob_as_byte_stream(
                     self.container_client, blob.name
                 )
                 async for chunk in self.read_chunks(file):
-                    yield CollectedBytes(file=blob.name, data=chunk, error=None)
-                yield CollectedBytes(file=blob.name, data=None, error=None, eof=True)
+                    yield CollectedBytes(file=blob.name, data=chunk, error=None, doc_source=f"azure://{self.container_name}/{self.account_url}")
+                yield CollectedBytes(file=blob.name, data=None, error=None, eof=True, doc_source=f"azure://{self.container_name}/{self.account_url}")
         except Exception as e:
             # Handle exceptions gracefully, e.g., log the error
             self.logger.error(f"Error polling Azure Blob Storage: {e}")
             raise e
         finally:
             # Disconnect the client when done
             await self.disconnect()
```

### Comparing `querent-3.0.2/querent/collectors/collector_errors.py` & `querent-3.0.3/querent/collectors/collector_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/collectors/collector_factory.py` & `querent-3.0.3/querent/collectors/collector_factory.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/collectors/collector_resolver.py` & `querent-3.0.3/querent/collectors/collector_resolver.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/collectors/drive/google_drive_collector.py` & `querent-3.0.3/querent/collectors/drive/google_drive_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,16 +84,16 @@
                 query = f"'{self.folder_to_crawl}' in parents"
             results = self.drive_service.files().list(q=query).execute()
             files = results.get("files", [])
             if not files:
                 self.logger.info("No files found in Google Drive")
             for file in files:
                 async for chunk in self.read_chunks(file["id"]):
-                    yield CollectedBytes(data=chunk, file=file["name"])
-                yield CollectedBytes(data=None, file=file["name"], eof=True)
+                    yield CollectedBytes(data=chunk, file=file["name"], doc_source=f"drive://{self.folder_to_crawl}")
+                yield CollectedBytes(data=None, file=file["name"], eof=True, doc_source=f"drive://{self.folder_to_crawl}")
         except Exception as e:
             raise common_errors.PollingError(
                 f"Failed to poll Google Drive: {str(e)}"
             ) from e
         finally:
             await self.disconnect()
```

### Comparing `querent-3.0.2/querent/collectors/dropbox/dropbox_collector.py` & `querent-3.0.3/querent/collectors/dropbox/dropbox_collector.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,16 +65,16 @@
                         f"Token expired. Refreshing access token and retrying."
                     )
                     self.connect()  # Attempt to refresh access token
                     file_metadata, response = self.dbx.files_download(name)
 
                 file_content_bytes = response.content
                 async for chunk in self.stream_blob(file_content_bytes):
-                    yield CollectedBytes(file=entry.name, data=chunk)
-                yield CollectedBytes(file=entry.name, data=None, eof=True)
+                    yield CollectedBytes(file=entry.name, data=chunk, doc_source=f"dropbox://{self.folder_path}")
+                yield CollectedBytes(file=entry.name, data=None, eof=True, doc_source=f"dropbox://{self.folder_path}")
         except dropbox.exceptions.ApiError as e:
             self.logger.error(f"Error polling Dropbox: {e}")
             raise common_errors.PollingError(
                 "Failed to poll Dropbox: {}".format(str(e))
             ) from e
         finally:
             await self.disconnect()
```

### Comparing `querent-3.0.2/querent/collectors/email/email_collector.py` & `querent-3.0.3/querent/collectors/email/email_collector.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,19 +53,21 @@
                 _, data = self.imap_connection.fetch(str(i), "(RFC822)")
                 for response_part in data:
                     if isinstance(response_part, tuple):
                         message = response_part[1]
                         yield CollectedBytes(
                             data=message,
                             file=f"{self.config.imap_username}:{self.config.imap_folder}/{i}.email",
+                            doc_source=f"email://{self.config.imap_server}/{self.config.imap_folder}"
                         )
                 yield CollectedBytes(
                     data=None,
                     file=f"{self.config.imap_username}:{self.config.imap_folder}/{i}.email",
                     eof=True,
+                    doc_source=f"email://{self.config.imap_server}/{self.config.imap_folder}"
                 )
         except imaplib.IMAP4.error as e:
             self.logger.error(f"Error fetching emails from IMAP server: {e}")
             raise common_errors.ConnectionError(
                 "Failed to fetch emails from the IMAP server: {}".format(str(e))
             ) from e
         finally:
```

### Comparing `querent-3.0.2/querent/collectors/email/imap.py` & `querent-3.0.3/querent/collectors/email/imap.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/collectors/fs/fs_collector.py` & `querent-3.0.3/querent/collectors/fs/fs_collector.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 
     async def poll(self) -> AsyncGenerator[CollectedBytes, None]:
         async for file_path in self.walk_files(self.root_dir):
             try:
                 async with aiofiles.open(file_path, "rb") as file:
                     file_path_str = str(file_path)
                     async for chunk in self.read_chunks(file):
-                        yield CollectedBytes(file=file_path_str, data=chunk, error=None)
+                        yield CollectedBytes(file=file_path_str, data=chunk, error=None, doc_source=f"file://{self.root_dir}")
                     yield CollectedBytes(
-                        file=file_path_str, data=None, error=None, eof=True
+                        file=file_path_str, data=None, error=None, eof=True, doc_source=f"file://{self.root_dir}"
                     )
             except PermissionError as exc:
                 raise common_errors.PermissionError(
                     f"Unable to open this file {file_path}, getting error as {exc}"
                 ) from exc
             except OSError as exc:
                 raise common_errors.OSError(
```

### Comparing `querent-3.0.2/querent/collectors/gcs/gcs_collector.py` & `querent-3.0.3/querent/collectors/gcs/gcs_collector.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,16 +51,16 @@
             await self.connect()
 
         try:
             bucket = self.client.get_bucket(self.bucket_name)
             blobs = list(bucket.list_blobs())  # Convert to a list
             for blob in blobs:
                 async for chunk in self.stream_blob(blob):
-                    yield CollectedBytes(file=blob.name, data=chunk, error=None)
-                yield CollectedBytes(file=blob.name, data=None, error=None, eof=True)
+                    yield CollectedBytes(file=blob.name, data=chunk, error=None, doc_source=f"gcs://{self.bucket_name}")
+                yield CollectedBytes(file=blob.name, data=None, error=None, eof=True, doc_source=f"gcs://{self.bucket_name}")
         except Exception as e:
             # Handle exceptions gracefully, e.g., log the error
             self.logger.error(f"Error connecting to GCS: {e}")
         finally:
             # Disconnect the client when done
             await self.disconnect()
```

### Comparing `querent-3.0.2/querent/collectors/github/github_collector.py` & `querent-3.0.3/querent/collectors/github/github_collector.py`

 * *Files 21% similar despite different names*

```diff
@@ -44,17 +44,17 @@
                     for item in contents:
                         if item["type"] == "file":
                             file_url = item["download_url"]
                             async with session.get(file_url, headers=headers) as file_response:
                                 file_response.raise_for_status()
                                 file_contents = await file_response.read()
                                 # Assume process_data() is correctly implemented for your file type
-                                yield CollectedBytes(file=item["name"], data=file_contents)
+                                yield CollectedBytes(file=item["name"], data=file_contents, doc_source=f"github://{self.repository}")
 
-                            yield CollectedBytes(file = item["name"], data = None, eof = True)
+                            yield CollectedBytes(file = item["name"], data = None, eof = True, doc_source=f"github://{self.repository}")
                         elif item["type"] == "dir":
                             # Recursively fetch files in subfolders
                             async for sub_item in self.fetch_files_in_folder(item["url"]):
                                 yield sub_item
 
         except requests.exceptions.RequestException as e:
             self.logger.error(f"Error connecting to Github: {e}")
```

### Comparing `querent-3.0.2/querent/collectors/jira/jira_collector.py` & `querent-3.0.3/querent/collectors/jira/jira_collector.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,18 +78,18 @@
                 expand=self.config.jira_expand,
                 json_result=False,
             )
 
             for issue in issues:
                 json_issue = json.dumps(issue.raw).encode("utf-8")
                 yield CollectedBytes(
-                    data=json_issue, file=f"jira_issue_{issue.key}.json.jira"
+                    data=json_issue, file=f"jira_issue_{issue.key}.json.jira", doc_source=f"jira://{self.config.jira_server}/{self.config.jira_project}"
                 )
                 yield CollectedBytes(
-                    data=None, file=f"jira_issue_{issue.key}.json.jira", eof=True
+                    data=None, file=f"jira_issue_{issue.key}.json.jira", eof=True, doc_source=f"jira://{self.config.jira_server}/{self.config.jira_project}"
                 )
 
         except common_errors.ConnectionError as e:
             self.logger.error(f"Error polling Jira issues: {e}")
             raise  # Re-raise ConnectionError without adding additional information
         except Exception as e:
             raise common_errors.ConnectionError(
```

### Comparing `querent-3.0.2/querent/collectors/news/news_collector.py` & `querent-3.0.3/querent/collectors/news/news_collector.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,30 +74,30 @@
                                 "urlToImage": article.get('urlToImage'),
                                 "publishedAt": article.get('publishedAt'),
                                 "content": article.get('content')
                                 }
                                 publish_date = article.get('publishedAt').split('T')[0]
 
                                 title = article['title']
-                                yield CollectedBytes(file=f"{self.config.query}_{publish_date}.news", data=str(article_data).encode("utf-8"))
-                                yield CollectedBytes(file=f"{self.config.query}_{publish_date}.news", data=None, error=None, eof=True)
+                                yield CollectedBytes(file=f"{self.config.query}_{publish_date}.news", data=str(article_data).encode("utf-8"), doc_source=f"news://{self.config.query}")
+                                yield CollectedBytes(file=f"{self.config.query}_{publish_date}.news", data=None, error=None, eof=True, doc_source=f"news://{self.config.query}")
 
                             total_results = response.get("totalResults", 0)
                             total_pages = (
                                 total_results + self.config.page_size - 1
                             ) // self.config.page_size
                             current_page += 1
                         else:
                             self.logger.error(
                                 f"News API request failed: {response.get('message')}"
                             )
                             break
                     except Exception as e:
                         self.logger.error(f"Error fetching news articles: {e}")
-                        yield CollectedBytes(file="Error", data=None, error=e)
+                        yield CollectedBytes(file="Error", data=None, error=e, doc_source=f"news://{self.config.query}")
                         break
 
                 # After exhausting the current batch, reset for next polling cycle
                 current_page = 1
                 total_pages = float("inf")
                 if not should_keep_going:
                     break
@@ -133,16 +133,16 @@
                         "urlToImage": article.get('urlToImage'),
                         "publishedAt": article.get('publishedAt'),
                         "content": article.get('content')
                         }
 
                         publish_date = article.get('publishedAt').split('T')[0]
                         title = article['title']
-                        yield CollectedBytes(file=f"{self.config.query}_{publish_date}.news", data=str(article_data).encode("utf-8"))
-                    yield CollectedBytes(file=f"{self.config.query}_{publish_date}.news", data=None, error=None, eof=True)
+                        yield CollectedBytes(file=f"{self.config.query}_{publish_date}.news", data=str(article_data).encode("utf-8"), doc_source=f"news://{self.config.query}")
+                    yield CollectedBytes(file=f"{self.config.query}_{publish_date}.news", data=None, error=None, eof=True, doc_source=f"news://{self.config.query}")
             except Exception as e:
                 self.logger.error(f"Error fetching news articles: {e}")
 
 
 
 
 class NewsCollectorFactory(CollectorFactory):
```

### Comparing `querent-3.0.2/querent/collectors/slack/slack_collector.py` & `querent-3.0.3/querent/collectors/slack/slack_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,22 +59,24 @@
                 )
                 if response["ok"]:
                     messages = response["messages"]
                     for message in messages:
                         yield CollectedBytes(
                             file=f"slack://{self.channel}.slack",
                             data=bytes(message["text"] + "\n\n", "utf-8"),
+                            doc_source = f"slack://{self.channel}"
                         )
 
                     if not response["has_more"]:
                         yield CollectedBytes(
                             file=f"slack://{self.channel}.slack",
                             data=None,
                             error=None,
                             eof=True,
+                            doc_source = f"slack://{self.channel}"
                         )
                         break
                 else:
                     raise common_errors.SlackApiError(
                         f"Slack API Error: {response['error']}"
                     )
```

### Comparing `querent-3.0.2/querent/collectors/webscaper/web_scraper_collector.py` & `querent-3.0.3/querent/collectors/webscaper/web_scraper_collector.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     async def poll(self):
         async with self.poll_lock:
             urls_to_scrape = [self.website_url]
             while urls_to_scrape:
                 url = urls_to_scrape.pop()
                 content = await self.scrape_website(url)
-                yield CollectedBytes(file=None, data=content.data, error=None)
+                yield CollectedBytes(file=None, data=content.data, error=None, doc_source=self.website_url)
                 # Find and add links from this page to the list of URLs to scrape
                 new_urls = self.extract_links(url)
                 urls_to_scrape.extend(new_urls)
 
     async def scrape_website(self, website_url: str):
         async with self.semaphore:
             async with ClientSession(connector=TCPConnector(ssl=False)) as session:
```

### Comparing `querent-3.0.2/querent/common/common_errors.py` & `querent-3.0.3/querent/common/common_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/common/errors/metric_errors.py` & `querent-3.0.3/querent/common/errors/metric_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/common/types/collected_bytes.py` & `querent-3.0.3/querent/common/types/collected_bytes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Union
 
 
 class CollectedBytes:
-    def __init__(self, file: str, data: bytes, error: str = None, eof: bool = False):
+    def __init__(self, file: str, data: bytes, error: str = None, eof: bool = False, doc_source = str):
         self.data = data
         self.error = error
         self.file = file
         self.eof = eof
+        self.doc_source = doc_source
         if self.file:
             file = str(file)
             self.extension = file.split(".")[-1]
             self.file_id = file.split("/")[-1].split(".")[0]
 
     def __str__(self):
         if self.error:
```

### Comparing `querent-3.0.2/querent/common/types/file_buffer.py` & `querent-3.0.3/querent/common/types/file_buffer.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,43 +27,40 @@
 
     def __init__(self):
         self.logger = setup_logger(__name__, "FileBuffer")
         self.file_chunks = {} 
 
     def add_chunk(self, filename, chunk):
         try:
-            if chunk is None:
-                return self.end_file(filename)
-
             if filename not in self.file_chunks:
                 self.file_chunks[filename] = {}
-
-            # Automatically assign a chunk ID
+                
+            if chunk is None:
+                return self.end_file(filename)
+            
             chunk_id = len(self.file_chunks[filename])
             self.file_chunks[filename][chunk_id] = chunk
 
             return filename, None
                 
         except Exception as e:
-            self.logger.error(f"Error adding a chunk: {e}")
-            raise Exception(f"An error occurred while adding a chunk: {e}")   
+            return filename, None   
 
     def end_file(self, filename):
         try:
             # Assemble file content from chunks
             if filename in self.file_chunks:
                 chunks = self.file_chunks[filename]
                 full_content = ''.join([chunks[i] for i in sorted(chunks.keys())])
                 del self.file_chunks[filename]  # Clear the file entry
                 return filename, full_content
             else:
-                raise Exception(f"No chunks found for file: {filename}")
+                return filename, None
         except Exception as e:
-            self.logger.error(f"Error ending the file: {e}")
-            raise Exception(f"An error occurred while ending the file: {e}")
+            return filename, None
 
     def get_content(self, filename):
         try:
             if filename in self.file_chunks:
                 chunks = self.file_chunks[filename]
                 return ''.join([chunks[i] for i in sorted(chunks.keys())])
             else:
```

### Comparing `querent-3.0.2/querent/common/types/ingested_code.py` & `querent-3.0.3/querent/common/types/ingested_code.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 class IngestedCode:
     """Class for ingested code type of data"""
 
-    def __init__(self, file: str, data: [str], error: str = None) -> None:
+    def __init__(self, file: str, data: [str], doc_source: str, error: str = None) -> None:
         self.data = data
         self.error = error
         self.file = file
+        self.doc_source = doc_source
         file = str(file)
         self.extension = file.rsplit(".", maxsplit=1)[-1]
 
     def __str__(self):
         if self.error:
             return f"Error: {self.error}"
         return f"Data: {self.data}"
```

### Comparing `querent-3.0.2/querent/common/types/ingested_messages.py` & `querent-3.0.3/querent/common/types/ingested_messages.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/common/types/ingested_tokens.py` & `querent-3.0.3/querent/common/types/ingested_tokens.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from typing import Union
+from typing import Union, List
 
 
 class IngestedTokens:
     def __init__(
-        self, file: str, data: [str], error: str = None, is_token_stream=False
+        self, file: str, data: List[str], error: str = None, is_token_stream=False, doc_source=str
     ) -> None:
         self.data = data
         self.error = error
         self.is_token_stream = is_token_stream
+        self.doc_source = doc_source
         if file:
             self.file = file
             file = str(file)
             self.extension = file.split(".")[-1]
             self.file_id = file.split("/")[-1].split(".")[0]
 
     def __str__(self):
```

### Comparing `querent-3.0.2/querent/common/types/querent_queue.py` & `querent-3.0.3/querent/common/types/querent_queue.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,14 +110,18 @@
         Check if the queue is empty.
 
         Returns:
             bool: True if the queue is empty, False otherwise.
 
         """
         return self.queue.empty()
+    
+    def qsize(self):
+
+        return self.queue.qsize()
 
     def __aiter__(self):
         return self
 
     async def __anext__(self):
         item = await self.get()
         if item is None:
```

### Comparing `querent-3.0.2/querent/common/uri.py` & `querent-3.0.3/querent/common/uri.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/config/collector/collector_config.py` & `querent-3.0.3/querent/config/collector/collector_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/config/config.py` & `querent-3.0.3/querent/config/config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/config/core/gpt_llm_config.py` & `querent-3.0.3/querent/config/core/gpt_llm_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/config/core/llm_config.py` & `querent-3.0.3/querent/config/core/llm_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/config/core/opensource_llm_config.py` & `querent-3.0.3/querent/config/core/opensource_llm_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/config/engine/engine_config.py` & `querent-3.0.3/querent/config/engine/engine_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/config/graph_config.py` & `querent-3.0.3/querent/config/graph_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/config/ingestor/ingestor_config.py` & `querent-3.0.3/querent/config/ingestor/ingestor_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/config/metric/prometheus.py` & `querent-3.0.3/querent/config/metric/prometheus.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/config/resource/resource_config.py` & `querent-3.0.3/querent/config/resource/resource_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/config/workflow/workflow_config.py` & `querent-3.0.3/querent/config/workflow/workflow_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/core/base_engine.py` & `querent-3.0.3/querent/core/base_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,18 +176,19 @@
     async def _listen_for_state_changes(self):
         while not self.state_queue.empty() or not self.termination_event.is_set():
             new_state = await self.state_queue.get()
             if isinstance(new_state, EventState):
                 if new_state.payload == "Terminate":
                     break
                 new_state = {
-                    "event_type": new_state.event_type,
+                    "event_type": str(new_state.event_type),
                     "timestamp": new_state.timestamp,
                     "payload": new_state.payload,
-                    "file": new_state.file
+                    "file": new_state.file,
+                    "doc_source": new_state.doc_source,
                 }
                 await self._notify_subscribers(new_state["event_type"], new_state)
             else:
                 raise Exception(
                     f"Bad state type {type(new_state)} for {self.__class__.__name__}. Supported type: {EventState}"
                 )
             await self.state_queue.task_done()
```

### Comparing `querent-3.0.2/querent/core/transformers/bert_ner_opensourcellm.py` & `querent-3.0.3/querent/core/transformers/bert_ner_opensourcellm.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,15 @@
             self.triple_filter = TripleFilter(**kwargs)
     
     
     async def process_tokens(self, data: IngestedTokens):
         doc_entity_pairs = []
         number_sentences = 0
         try:
+            doc_source = data.doc_source
             if not BERTLLM.validate_ingested_tokens(data):
                     self.set_termination_event()                                      
                     return
             if data.data:
                 single_string = ' '.join(data.data)
                 # clean_text = unidecode(single_string)
                 clean_text = single_string
@@ -195,34 +196,35 @@
                     else:
                         # filtered_triples, _ = self.triple_filter.filter_triples(clustered_triples)
                         self.logger.debug(f"Filtering in {self.__class__.__name__} producing 0 entity pairs. Filtering Disabled. ")
                         filtered_triples = pairs_with_predicates
                 else:
                     filtered_triples = pairs_with_predicates
                 if not filtered_triples:
-                    self.logger.debug("No entity pairs")
                     return
                 elif not self.skip_inferences:
                     relationships = self.semantic_extractor.process_tokens(filtered_triples)
                     relationships = self.semantictriplefilter.filter_triples(relationships)
                     if len(relationships) > 0:
                         embedding_triples = self.create_emb.generate_embeddings(relationships)
                         if self.sample_relationships:
                             embedding_triples = self.predicate_context_extractor.process_predicate_types(embedding_triples)
                         for triple in embedding_triples:
                             if not self.termination_event.is_set():
                                 graph_json = json.dumps(TripleToJsonConverter.convert_graphjson(triple))
                                 if graph_json:
-                                    current_state = EventState(EventType.Graph,1.0, graph_json, file)
+                                    current_state = EventState(EventType.Graph,1.0, graph_json, file, doc_source=doc_source)
                                     await self.set_state(new_state=current_state)
                                 vector_json = json.dumps(TripleToJsonConverter.convert_vectorjson(triple))
                                 if vector_json:
-                                    current_state = EventState(EventType.Vector,1.0, vector_json, file)
+                                    current_state = EventState(EventType.Vector,1.0, vector_json, file, doc_source=doc_source)
                                     await self.set_state(new_state=current_state)
                             else:
                                 return
                     else:
                         return
                 else:
                     return filtered_triples, file
+            else:
+                return
         except Exception as e:
             self.logger.debug(f"Invalid {self.__class__.__name__} configuration. Unable to process tokens. {e}")
```

### Comparing `querent-3.0.2/querent/core/transformers/fixed_entities_set_opensourcellm.py` & `querent-3.0.3/querent/core/transformers/fixed_entities_set_opensourcellm.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,14 +123,15 @@
             self.triple_filter = TripleFilter(**kwargs)
     
     
     async def process_tokens(self, data: IngestedTokens):
         doc_entity_pairs = []
         number_sentences = 0
         try:
+            doc_source = data.doc_source
             if not Fixed_Entities_LLM.validate_ingested_tokens(data):
                     self.set_termination_event()                                      
                     return
             if data.data:
                 single_string = ' '.join(data.data)
                 clean_text = single_string
                 # clean_text = unidecode(single_string)
@@ -151,15 +152,14 @@
                 for tokenized_sentence, original_sentence, sentence_idx in tokens:
                     (entities, entity_pairs,) = self.ner_llm_instance.extract_entities_from_sentence(original_sentence, sentence_idx, [s[1] for s in tokens],self.isConfinedSearch, self.fixed_entities, self.sample_entities)
                     if entity_pairs:
                         doc_entity_pairs.append(self.ner_llm_instance.transform_entity_pairs(entity_pairs))
                     number_sentences = number_sentences + 1
             else:
                 return
-
             if self.sample_entities:
                 doc_entity_pairs = self.entity_context_extractor.process_entity_types(doc_entities=doc_entity_pairs)
             if doc_entity_pairs and any(doc_entity_pairs):
                 doc_entity_pairs = self.ner_llm_instance.remove_duplicates(doc_entity_pairs)
                 filtered_triples = process_data(doc_entity_pairs, file)
                 if not filtered_triples:
                     self.logger.debug("No entity pairs")
@@ -172,19 +172,19 @@
                         embedding_triples = self.create_emb.generate_embeddings(relationships)
                         if self.sample_relationships:
                             embedding_triples = self.predicate_context_extractor.process_predicate_types(embedding_triples)
                         for triple in embedding_triples:
                             if not self.termination_event.is_set():
                                 graph_json = json.dumps(TripleToJsonConverter.convert_graphjson(triple))
                                 if graph_json:
-                                    current_state = EventState(EventType.Graph,1.0, graph_json, file)
+                                    current_state = EventState(EventType.Graph,1.0, graph_json, file, doc_source=doc_source)
                                     await self.set_state(new_state=current_state)
                                 vector_json = json.dumps(TripleToJsonConverter.convert_vectorjson(triple))
                                 if vector_json:
-                                    current_state = EventState(EventType.Vector,1.0, vector_json, file)
+                                    current_state = EventState(EventType.Vector,1.0, vector_json, file, doc_source=doc_source)
                                     await self.set_state(new_state=current_state)
                             else:
                                 return
                     else:
                         return
                 else:
                     return filtered_triples, file
```

### Comparing `querent-3.0.2/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py` & `querent-3.0.3/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,16 +251,18 @@
         return output_tuple
       
     async def process_tokens(self, data: IngestedTokens):
         try:
             if not GPTLLM.validate_ingested_tokens(data):
                     self.set_termination_event()                    
                     return 
+            
+            doc_source = data.doc_source
             relationships = []
-            result = await self.llm_instance.process_tokens(data)           
+            result = await self.llm_instance.process_tokens(data)
             if not result: return 
             else:
                 filtered_triples, file = result
                 modified_data = GPTLLM.remove_items_from_tuples(filtered_triples)
                 for entity1, context_json, entity2 in modified_data:
                     context_data = json.loads(context_json)
                     context = context_data.get("context", "")
@@ -276,19 +278,19 @@
                     embedding_triples = self.create_emb.generate_embeddings(relationships)
                     if self.sample_relationships:
                             embedding_triples = self.predicate_context_extractor.process_predicate_types(embedding_triples)
                     for triple in embedding_triples:
                         if not self.termination_event.is_set():
                             graph_json = json.dumps(TripleToJsonConverter.convert_graphjson(triple))
                             if graph_json:
-                                    current_state = EventState(EventType.Graph,1.0, graph_json, file)
+                                    current_state = EventState(EventType.Graph,1.0, graph_json, file, doc_source=doc_source)
                                     await self.set_state(new_state=current_state)
                             vector_json = json.dumps(TripleToJsonConverter.convert_vectorjson(triple))
                             if vector_json:
-                                    current_state = EventState(EventType.Vector,1.0, vector_json, file)
+                                    current_state = EventState(EventType.Vector,1.0, vector_json, file, doc_source=doc_source)
                                     await self.set_state(new_state=current_state)
                         else:
                             return
         except Exception as e:
             self.logger.error(f"Invalid {self.__class__.__name__} configuration. Unable to extract predicates using GPT. {e}")
             raise Exception(f"An error occurred while extracting predicates using GPT: {e}")
```

### Comparing `querent-3.0.2/querent/core/transformers/gpt_llm_gpt_ner.py` & `querent-3.0.3/querent/core/transformers/gpt_llm_gpt_ner.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,14 +180,15 @@
       
     async def process_tokens(self, data: IngestedTokens):
         try:
             if not GPTNERLLM.validate_ingested_tokens(data):
                     self.set_termination_event()                    
                     return 
 
+            doc_source = data.doc_source
             if data.data:
                 clean_text = ' '.join(data.data)
                 #clean_text = unidecode(single_string)
             else:
                 clean_text = data.data
             if not data.is_token_stream : 
                 file, content = self.file_buffer.add_chunk(
@@ -242,22 +243,22 @@
                 #final_triples = [{'subject': 'paleocene–eocene thermal maximum (petm) record', 'predicate': 'is present in', 'object': '543-m-thick (1780 ft) deep-marine section in the gulf of mexico (gom)', 'subject_type': 'event', 'object_type': 'location', 'predicate_type': 'occurrence', 'sentence': 'ABSTRACT In this study, we present evidence of a Paleocene–Eocene Thermal Maximum (PETM) record within a 543-m-thick (1780 ft) deep-marine section in the Gulf of Mexico (GoM) using organic carbon stable isotopes and biostratigraphic constraints. We suggest that climate and tectonic perturbations in the upstream North American catchments can induce a substantial response in the downstream sectors of the Gulf Coastal Plain and ultimately in the GoM.'}, {'subject': 'climate and tectonic perturbations', 'predicate': 'can induce', 'object': 'a substantial response', 'subject_type': 'process', 'object_type': 'event', 'predicate_type': 'causative', 'sentence': 'ABSTRACT In this study, we present evidence of a Paleocene–Eocene Thermal Maximum (PETM) record within a 543-m-thick (1780 ft) deep-marine section in the Gulf of Mexico (GoM) using organic carbon stable isotopes and biostratigraphic constraints. We suggest that climate and tectonic perturbations in the upstream North American catchments can induce a substantial response in the downstream sectors of the Gulf Coastal Plain and ultimately in the GoM.'}, {'subject': 'gulf coastal plain', 'predicate': 'is', 'object': 'ultimately in the gom', 'subject_type': 'location', 'object_type': 'location', 'predicate_type': 'ownership', 'sentence': 'ABSTRACT In this study, we present evidence of a Paleocene–Eocene Thermal Maximum (PETM) record within a 543-m-thick (1780 ft) deep-marine section in the Gulf of Mexico (GoM) using organic carbon stable isotopes and biostratigraphic constraints. We suggest that climate and tectonic perturbations in the upstream North American catchments can induce a substantial response in the downstream sectors of the Gulf Coastal Plain and ultimately in the GoM.'}, {'subject': 'paleocene–eocene thermal maximum (petm) record', 'predicate': 'is present in', 'object': '543-m-thick (1780 ft) deep-marine section in the gulf of mexico (gom)', 'subject_type': 'event', 'object_type': 'location', 'predicate_type': 'occurrence', 'sentence': 'ABSTRACT In this study, we present evidence of a Paleocene–Eocene Thermal Maximum (PETM) record within a 543-m-thick (1780 ft) deep-marine section in the Gulf of Mexico (GoM) using organic carbon stable isotopes and biostratigraphic constraints. We suggest that climate and tectonic perturbations in the upstream North American catchments can induce a substantial response in the downstream sectors of the Gulf Coastal Plain and ultimately in the GoM. This relationship is illustrated in the deep-water basin by (1) a high accom- modation and deposition of a shale interval when coarse-grained terrigenous material was trapped upstream at the onset of the PETM, and (2) a considerable increase in sedi- ment supply during the PETM, which is archived as a particularly thick sedimentary section in the deep-sea fans of the GoM basin.'}, {'subject': 'climate and tectonic perturbations', 'predicate': 'can induce', 'object': 'a substantial response', 'subject_type': 'process', 'object_type': 'event', 'predicate_type': 'causative', 'sentence': 'ABSTRACT In this study, we present evidence of a Paleocene–Eocene Thermal Maximum (PETM) record within a 543-m-thick (1780 ft) deep-marine section in the Gulf of Mexico (GoM) using organic carbon stable isotopes and biostratigraphic constraints. We suggest that climate and tectonic perturbations in the upstream North American catchments can induce a substantial response in the downstream sectors of the Gulf Coastal Plain and ultimately in the GoM. This relationship is illustrated in the deep-water basin by (1) a high accom- modation and deposition of a shale interval when coarse-grained terrigenous material was trapped upstream at the onset of the PETM, and (2) a considerable increase in sedi- ment supply during the PETM, which is archived as a particularly thick sedimentary section in the deep-sea fans of the GoM basin.'}, {'subject': 'upstream north american catchments', 'predicate': 'can induce', 'object': 'a substantial response', 'subject_type': 'location', 'object_type': 'event', 'predicate_type': 'causative', 'sentence': 'ABSTRACT In this study, we present evidence of a Paleocene–Eocene Thermal Maximum (PETM) record within a 543-m-thick (1780 ft) deep-marine section in the Gulf of Mexico (GoM) using organic carbon stable isotopes and biostratigraphic constraints. We suggest that climate and tectonic perturbations in the upstream North American catchments can induce a substantial response in the downstream sectors of the Gulf Coastal Plain and ultimately in the GoM. This relationship is illustrated in the deep-water basin by (1) a high accom- modation and deposition of a shale interval when coarse-grained terrigenous material was trapped upstream at the onset of the PETM, and (2) a considerable increase in sedi- ment supply during the PETM, which is archived as a particularly thick sedimentary section in the deep-sea fans of the GoM basin.'}, {'subject': 'downstream sectors of the gulf coastal plain', 'predicate': 'can be impacted by', 'object': 'upstream north american catchments', 'subject_type': 'location', 'object_type': 'location', 'predicate_type': 'causative', 'sentence': 'ABSTRACT In this study, we present evidence of a Paleocene–Eocene Thermal Maximum (PETM) record within a 543-m-thick (1780 ft) deep-marine section in the Gulf of Mexico (GoM) using organic carbon stable isotopes and biostratigraphic constraints. We suggest that climate and tectonic perturbations in the upstream North American catchments can induce a substantial response in the downstream sectors of the Gulf Coastal Plain and ultimately in the GoM. This relationship is illustrated in the deep-water basin by (1) a high accom- modation and deposition of a shale interval when coarse-grained terrigenous material was trapped upstream at the onset of the PETM, and (2) a considerable increase in sedi- ment supply during the PETM, which is archived as a particularly thick sedimentary section in the deep-sea fans of the GoM basin.'}, {'subject': 'climate and tectonic perturbations', 'predicate': 'can induce', 'object': 'a substantial response', 'subject_type': 'process', 'object_type': 'event', 'predicate_type': 'causative', 'sentence': 'We suggest that climate and tectonic perturbations in the upstream North American catchments can induce a substantial response in the downstream sectors of the Gulf Coastal Plain and ultimately in the GoM. This relationship is illustrated in the deep-water basin by (1) a high accom- modation and deposition of a shale interval when coarse-grained terrigenous material was trapped upstream at the onset of the PETM, and (2) a considerable increase in sedi- ment supply during the PETM, which is archived as a particularly thick sedimentary section in the deep-sea fans of the GoM basin. Despite other thick PETM sections being observed elsewhere in the world, the one described in this study links with a continental- scale paleo-drainage, which makes it of particular interest for paleoclimate and source- to-sink reconstructions.'}, {'subject': 'upstream north american catchments', 'predicate': 'can induce', 'object': 'a substantial response', 'subject_type': 'location', 'object_type': 'event', 'predicate_type': 'causative', 'sentence': 'We suggest that climate and tectonic perturbations in the upstream North American catchments can induce a substantial response in the downstream sectors of the Gulf Coastal Plain and ultimately in the GoM. This relationship is illustrated in the deep-water basin by (1) a high accom- modation and deposition of a shale interval when coarse-grained terrigenous material was trapped upstream at the onset of the PETM, and (2) a considerable increase in sedi- ment supply during the PETM, which is archived as a particularly thick sedimentary section in the deep-sea fans of the GoM basin. Despite other thick PETM sections being observed elsewhere in the world, the one described in this study links with a continental- scale paleo-drainage, which makes it of particular interest for paleoclimate and source- to-sink reconstructions.'}]
                 final_triples = self.remove_duplicate_triplets(final_triples)
                 if len(final_triples) > 0:
                     for triple in final_triples:
                         if not self.termination_event.is_set():
                             graph_json = json.dumps(triple)
                             if graph_json:
-                                current_state = EventState(EventType.Graph,1.0, graph_json, file)
+                                current_state = EventState(EventType.Graph,1.0, graph_json, file, doc_source=doc_source)
                                 await self.set_state(new_state=current_state)
                             context_embeddings = self.create_emb.get_embeddings([triple['sentence']])[0]
                             triple['context_embeddings'] = context_embeddings
                             triple['context'] = triple['sentence']
                             vector_json = json.dumps(TripleToJsonConverter.convert_vectorjson((triple['subject'],json.dumps(triple), triple['object'])))
                             if vector_json:
-                                    current_state = EventState(EventType.Vector,1.0, vector_json, file)
+                                    current_state = EventState(EventType.Vector,1.0, vector_json, file, doc_source=doc_source)
                                     await self.set_state(new_state=current_state)
                         else:
                             return
 
         except Exception as e:
             self.logger.debug(f"Invalid {self.__class__.__name__} configuration. Unable to extract predicates using GPT NER LLM class. {e}")
```

### Comparing `querent-3.0.2/querent/core/transformers/relationship_extraction_llm.py` & `querent-3.0.3/querent/core/transformers/relationship_extraction_llm.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/graph/errors.py` & `querent-3.0.3/querent/graph/errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/graph/graph.py` & `querent-3.0.3/querent/graph/graph.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/graph/graph_namespace.py` & `querent-3.0.3/querent/graph/graph_namespace.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/graph/ontology.py` & `querent-3.0.3/querent/graph/ontology.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/graph/schema.py` & `querent-3.0.3/querent/graph/schema.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/graph/shacl.py` & `querent-3.0.3/querent/graph/shacl.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/graph/subject.py` & `querent-3.0.3/querent/graph/subject.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/graph/utils.py` & `querent-3.0.3/querent/graph/utils.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/ingestors/audio/audio_ingestors.py` & `querent-3.0.3/querent/ingestors/audio/audio_ingestors.py`

 * *Files 9% similar despite different names*

```diff
@@ -77,33 +77,34 @@
                 if current_file is None:
                     current_file = chunk_bytes.file
                 elif current_file != chunk_bytes.file:
                     # we have a new file, process the old one
                     async for text in self.extract_and_process_audio(
                         CollectedBytes(file=current_file, data=collected_bytes)
                     ):
-                        yield IngestedTokens(file=current_file, data=[text], error=None)
+                        yield IngestedTokens(file=current_file, data=[text], error=None, doc_source= chunk_bytes.doc_source)
                     yield IngestedTokens(
                         file=current_file,
                         data=None,
                         error=None,
+                        doc_source= chunk_bytes.doc_source
                     )
                     collected_bytes = b""
                     current_file = chunk_bytes.file
                 collected_bytes += chunk_bytes.data
         except Exception as e:
-            yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}")
+            yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}", doc_source=chunk_bytes.doc_source)
         finally:
             # process the last file
             async for text in self.extract_and_process_audio(
                 CollectedBytes(file=current_file, data=collected_bytes)
             ):
-                yield IngestedTokens(file=current_file, data=[text], error=None)
+                yield IngestedTokens(file=current_file, data=[text], error=None, doc_source=chunk_bytes.doc_source)
 
-            yield IngestedTokens(file=current_file, data=None, error=None)
+            yield IngestedTokens(file=current_file, data=None, error=None, doc_source=chunk_bytes.doc_source)
 
     async def extract_and_process_audio(
         self, collected_bytes: CollectedBytes
     ) -> AsyncGenerator[IngestedTokens, None]:
         # Recognize the text using the recognizer
         try:
             audio_segment = AudioSegment.from_file(
```

### Comparing `querent-3.0.2/querent/ingestors/base_ingestor.py` & `querent-3.0.3/querent/ingestors/base_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/ingestors/code/code_ingestor.py` & `querent-3.0.3/querent/ingestors/code/code_ingestor.py`

 * *Files 21% similar despite different names*

```diff
@@ -73,36 +73,39 @@
                     async for line in self.extract_code_from_bytes(
                         CollectedBytes(file=current_file, data=collected_bytes)
                     ):
                         yield IngestedTokens(
                             file=current_file,
                             data=[line],
                             error=None,
+                            doc_source=chunk_bytes.doc_source,
                         )
                     yield IngestedTokens(
                         file=current_file,
                         data=None,
                         error=None,
+                        doc_source=chunk_bytes.doc_source
                     )
                     collected_bytes = b""
                     current_file = chunk_bytes.file
                 collected_bytes += chunk_bytes.data
             if current_file:
                 async for line in self.extract_code_from_bytes(
                     CollectedBytes(file=current_file, data=collected_bytes)
                 ):
                     yield IngestedTokens(
                         file=current_file,
                         data=[line],
                         error=None,
+                        doc_source=chunk_bytes.doc_source
                     )
-                yield IngestedTokens(file=current_file, data=None, error=None)
+                yield IngestedTokens(file=current_file, data=None, error=None, doc_source=chunk_bytes.doc_source)
         except Exception as exc:
             yield IngestedTokens(
-                file=current_file, data=None, error=f"Exception: {exc}"
+                file=current_file, data=None, error=f"Exception: {exc}", doc_source=chunk_bytes.doc_source,
             )
             raise Exception from exc
 
     async def extract_code_from_bytes(
         self, chunk_bytes: CollectedBytes
     ) -> AsyncGenerator[IngestedTokens, None]:
         try:
```

### Comparing `querent-3.0.2/querent/ingestors/csv/csv_ingestor.py` & `querent-3.0.3/querent/ingestors/csv/csv_ingestor.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,33 +45,34 @@
                 if current_file is None:
                     current_file = chunk_bytes.file
                 elif current_file != chunk_bytes.file:
                     # we have a new file, process the old one
                     async for row in self.extract_and_process_csv(
                         CollectedBytes(file=current_file, data=collected_bytes)
                     ):
-                        yield IngestedTokens(file=current_file, data=[row], error=None)
+                        yield IngestedTokens(file=current_file, data=[row], error=None, doc_source=chunk_bytes.doc_source)
                     yield IngestedTokens(
                         file=current_file,
                         data=None,
                         error=None,
+                        doc_source=chunk_bytes.doc_source,
                     )
                     collected_bytes = b""
                     current_file = chunk_bytes.file
                 collected_bytes += chunk_bytes.data
         except Exception as e:
-            yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}")
+            yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}", doc_source=chunk_bytes.doc_source)
         finally:
             # process the last file
             async for row in self.extract_and_process_csv(
                 CollectedBytes(file=current_file, data=collected_bytes)
             ):
-                yield IngestedTokens(file=current_file, data=[row], error=None)
+                yield IngestedTokens(file=current_file, data=[row], error=None,doc_source=chunk_bytes.doc_source)
 
-            yield IngestedTokens(file=current_file, data=None, error=None)
+            yield IngestedTokens(file=current_file, data=None, error=None, doc_source=chunk_bytes.doc_source)
 
     async def extract_and_process_csv(
         self, collected_bytes: CollectedBytes
     ) -> AsyncGenerator[str, None]:
         text = await self.extract_text_from_csv(collected_bytes)
         rows = text.splitlines()
         for row in rows:
```

### Comparing `querent-3.0.2/querent/ingestors/doc/doc_ingestor.py` & `querent-3.0.3/querent/ingestors/doc/doc_ingestor.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,68 +50,70 @@
                     # TODO handle error
                     continue
                 if current_file is None:
                     current_file = chunk_bytes.file
                 elif current_file != chunk_bytes.file:
                     # we have a new file, process the old one
                     async for ingested_data in self.extract_and_process_doc(
-                        CollectedBytes(file=current_file, data=collected_bytes)
+                        CollectedBytes(file=current_file, data=collected_bytes), doc_source=chunk_bytes.doc_source
                     ):
+                        ingested_data.doc_source = chunk_bytes.doc_source
                         yield ingested_data
                     yield IngestedTokens(
                         file=current_file,
                         data=None,
                         error=None,
+                        doc_source=chunk_bytes.doc_source
                     )
                     collected_bytes = b""
                     current_file = chunk_bytes.file
                 collected_bytes += chunk_bytes.data
         except Exception as e:
             yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}")
         finally:
             # process the last file
             async for ingested_data in self.extract_and_process_doc(
-                CollectedBytes(file=current_file, data=collected_bytes)
+                CollectedBytes(file=current_file, data=collected_bytes), doc_source=chunk_bytes.doc_source
             ):
                 yield ingested_data
-            yield IngestedTokens(file=current_file, data=None, error=None)
+            yield IngestedTokens(file=current_file, data=None, doc_source = chunk_bytes.doc_source, error=None)
 
     async def extract_and_process_doc(
-        self, collected_bytes: CollectedBytes
+        self, collected_bytes: CollectedBytes, doc_source: str
     ) -> AsyncGenerator[str, None]:
-        async for paragraph in self.extract_text_from_doc(collected_bytes):            
+        async for paragraph in self.extract_text_from_doc(collected_bytes, doc_source):            
             yield paragraph
 
-    async def extract_text_from_doc(self, collected_bytes: CollectedBytes):
+    async def extract_text_from_doc(self, collected_bytes: CollectedBytes, doc_source: str):
         # Determine file extension
         file_extension = collected_bytes.extension.lower()
         if file_extension == "docx":
             doc = Document(io.BytesIO(collected_bytes.data))
             text = ""
             for paragraph in doc.paragraphs:
                 text += paragraph.text + "\n"
 
             text = await self.process_data(text)
             yield IngestedTokens(
-                file=collected_bytes.file, data=text, error=None
+                file=collected_bytes.file, data=text, error=None, doc_source=doc_source
             )
 
             # i = 1
             # for rel in doc.part.rels.values():
             #     if "image" in rel.reltype:
             #         image = rel.target_part.blob 
             #         ocr_text = await self.process_image(image)
             #         encoded_image = base64.b64encode(image)
             #         yield IngestedImages(file = collected_bytes.file, image = encoded_image.decode('utf-8'), image_name=str(uuid.uuid4()), page_num=i, text=text, ocr_text=ocr_text, error=None, coordinates=None)
             #         i += 1
 
         elif file_extension == "doc":
             current_doc_text = await self.temp_extract_from(collected_bytes)
             yield IngestedTokens(
-                file=collected_bytes.file, data=current_doc_text, error=None
+                file=collected_bytes.file, data=current_doc_text, error=None, doc_source=doc_source
             )
         else:
             raise common_errors.UnknownError(
                 f"Not a doc or docx file {collected_bytes.file}"
             )
 
     async def temp_extract_from(self, collected_bytes: CollectedBytes) -> str:
```

### Comparing `querent-3.0.2/querent/ingestors/email/email_ingestor.py` & `querent-3.0.3/querent/ingestors/email/email_ingestor.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,39 +54,43 @@
                     email = await self.extract_and_process_email(
                         CollectedBytes(file=current_file, data=collected_bytes)
                     )
                     yield IngestedTokens(
                         file=current_file,
                         data=[email],
                         error=None,
+                        doc_source=chunk_bytes.doc_source,
                     )
                     yield IngestedTokens(
                         file=current_file,
                         data=None,
                         error=None,
+                        doc_source=chunk_bytes.doc_source
                     )
                     collected_bytes = b""
                     current_file = chunk_bytes.file
                 collected_bytes += chunk_bytes.data
         except Exception as e:
-            yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}")
+            yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}", doc_source=chunk_bytes.doc_source)
         finally:
             if current_file is not None:
                 email = await self.extract_and_process_email(
                     CollectedBytes(file=current_file, data=collected_bytes)
                 )
                 yield IngestedTokens(
                     file=current_file,
                     data=[email],
                     error=None,
+                    doc_source=chunk_bytes.doc_source
                 )
                 yield IngestedTokens(
                     file=current_file,
                     data=None,
                     error=None,
+                    doc_source=chunk_bytes.doc_source,
                 )
 
     async def extract_and_process_email(
         self, collected_bytes: CollectedBytes
     ) -> List[str]:
         text = await self.extract_text_from_email(collected_bytes)
         processed_text = await self.process_data(text)
```

### Comparing `querent-3.0.2/querent/ingestors/email/email_reader.py` & `querent-3.0.3/querent/ingestors/email/email_reader.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/ingestors/github/github_ingestor.py` & `querent-3.0.3/querent/ingestors/github/github_ingestor.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,39 +29,42 @@
                     current_file = chunk_bytes.file
                 elif current_file != chunk_bytes.file:
                     async for line in self.extract_and_process_code(
                         CollectedBytes(file=current_file, data=collected_bytes)
                     ):
                         yield IngestedCode(
                             file=current_file,
-                            data=[line],  # Wrap line in a list
+                            data=[line],
                             error=None,
+                            doc_source=chunk_bytes.doc_source,
                         )
                     yield IngestedCode(
                         file=current_file,
                         data=None,
                         error=None,
+                        doc_source=chunk_bytes.doc_source,
                     )
                     collected_bytes = b""
                     current_file = chunk_bytes.file
 
                 collected_bytes += chunk_bytes.data
 
             if current_file:
                 async for line in self.extract_and_process_code(
                     CollectedBytes(file=current_file, data=collected_bytes)
                 ):
                     yield IngestedCode(
                         file=current_file,
-                        data=[line],  # Wrap line in a list
+                        data=[line],
                         error=None,
+                        doc_source=chunk_bytes.doc_source,
                     )
-                yield IngestedCode(file=current_file, data=None, error=None)
+                yield IngestedCode(file=current_file, data=None, error=None, doc_source=chunk_bytes.doc_source)
         except Exception as e:
-            yield IngestedCode(file=current_file, data=None, error=f"Exception: {e}")
+            yield IngestedCode(file=current_file, data=None, error=f"Exception: {e}", doc_source=chunk_bytes.doc_source)
 
     async def extract_and_process_code(
         self, chunk_bytes: CollectedBytes
     ) -> AsyncGenerator[IngestedCode, None]:
         message_bytes = chunk_bytes.data.decode("UTF-8")
         yield message_bytes
```

### Comparing `querent-3.0.2/querent/ingestors/html/html_ingestor.py` & `querent-3.0.3/querent/ingestors/html/html_ingestor.py`

 * *Files 11% similar despite different names*

```diff
@@ -47,44 +47,45 @@
                 if chunk_bytes.is_error() or chunk_bytes.is_eof():
                     continue
                 if current_file is None:
                     current_file = chunk_bytes.file
                 elif current_file != chunk_bytes.file:
                     # we have a new file, process the old one
                     async for ingested_data in self.extract_and_process_html(
-                        CollectedBytes(file=current_file, data=collected_bytes)
+                        CollectedBytes(file=current_file, data=collected_bytes), chunk_bytes.doc_source
                     ):
                         yield ingested_data
                     yield IngestedTokens(
                         file=current_file,
                         data=None,
                         error=None,
+                        doc_source=chunk_bytes.doc_source,
                     )
                     collected_bytes = b""
                     current_file = chunk_bytes.file
                 collected_bytes += chunk_bytes.data
         except Exception as e:
-            yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}")
+            yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}", doc_source=chunk_bytes.doc_source)
         finally:
             # process the last file
             async for ingested_data in self.extract_and_process_html(
-                CollectedBytes(file=current_file, data=collected_bytes)
+                CollectedBytes(file=current_file, data=collected_bytes), chunk_bytes.doc_source
             ):
                 yield ingested_data
-            yield IngestedTokens(file=current_file, data=None, error=None)
+            yield IngestedTokens(file=current_file, data=None, error=None, doc_source=chunk_bytes.doc_source)
 
     async def extract_and_process_html(
-        self, collected_bytes: CollectedBytes
+        self, collected_bytes: CollectedBytes, doc_source: str
     ) -> AsyncGenerator[str, None]:
         """Function to extract and process xml files"""
-        async for elements in self.extract_text_from_html(collected_bytes):
+        async for elements in self.extract_text_from_html(collected_bytes, doc_source):
             yield elements
 
     async def extract_text_from_html(
-        self, collected_bytes: CollectedBytes
+        self, collected_bytes: CollectedBytes, doc_source: str
     ):
         """Function to extract text from xml"""
         try:
             html_content = collected_bytes.data.decode("UTF-8")
             soup = BeautifulSoup(html_content, "html.parser")
             elements = []
             tags = ["p", "h1", "h2", "h3", "h4", "h5", "a", "footer", "article"]
@@ -93,39 +94,39 @@
                     link_text = element.get_text().strip()
                     link_href = element.get("href")
                     elements.append(f"Link: {link_text}, URL: {link_href}")
                 else:
                     element_text = element.get_text().strip()
                     elements.append(element_text)
 
-            # i = 1
-            # for img_tag in soup.find_all('img'):
-            #     img_src = img_tag.get('src')
-            #     if img_src and img_src.startswith('data:image'):
-            #         base64_data = img_src.split(';base64,')[-1]
-            #         image_data = base64.b64decode(base64_data)
-            #         image_ocr = await self.process_image(io.BytesIO(image_data))
+            i = 1
+            for img_tag in soup.find_all('img'):
+                img_src = img_tag.get('src')
+                if img_src and img_src.startswith('data:image'):
+                    base64_data = img_src.split(';base64,')[-1]
+                    image_data = base64.b64decode(base64_data)
+                    image_ocr = await self.process_image(io.BytesIO(image_data))
 
-            #         yield IngestedImages(file = collected_bytes.file, image = base64_data, image_name = str(uuid.uuid4()), page_num=i, text = soup, ocr_text = image_ocr, coordinates= None, error= None)
-            #         i += 1
+                    yield IngestedImages(file = collected_bytes.file, image = base64_data, image_name = str(uuid.uuid4()), page_num=i, text = soup, ocr_text = image_ocr, coordinates= None, error= None, doc_source=doc_source)
+                    i += 1
         except UnicodeDecodeError as exc:
             raise common_errors.UnicodeDecodeError(
                 f"Getting UnicodeDecodeError on this file {collected_bytes.file} as {exc}"
             ) from exc
         except LookupError as exc:
             raise common_errors.LookupError(
                 f"Getting LookupError on this file {collected_bytes.file} as {exc}"
             ) from exc
         except TypeError as exc:
             raise common_errors.TypeError(
                 f"Getting TypeError on this file {collected_bytes.file} as {exc}"
             ) from exc
         for element in elements:
             processed_element = await self.process_data(element)
-            yield IngestedTokens(file=collected_bytes.file, data=[processed_element], error=None)
+            yield IngestedTokens(file=collected_bytes.file, data=[processed_element], error=None, doc_source=doc_source)
 
     async def process_data(self, text: str) -> str:
         if self.processors is None or len(self.processors) == 0:
             return text
         try:
             processed_data = text
             for processor in self.processors:
```

### Comparing `querent-3.0.2/querent/ingestors/images/image_ingestor.py` & `querent-3.0.3/querent/ingestors/images/image_ingestor.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,31 +48,31 @@
                     continue
 
                 if chunk_bytes.file != current_file:
                     if current_file:
                         text = await self.extract_and_process_image(
                             CollectedBytes(file=current_file, data=collected_bytes)
                         )
-                        yield IngestedTokens(file=current_file, data=[text], error=None)
-                        yield IngestedTokens(file=current_file, data=None, error=None)
+                        yield IngestedTokens(file=current_file, data=[text], error=None, doc_source=chunk_bytes.doc_source)
+                        yield IngestedTokens(file=current_file, data=None, error=None, doc_source=chunk_bytes.doc_source)
 
                     current_file = chunk_bytes.file
                     collected_bytes = b""
 
                 collected_bytes += chunk_bytes.data
 
             if current_file:
                 text = await self.extract_and_process_image(
                     CollectedBytes(file=current_file, data=collected_bytes)
                 )
-                yield IngestedTokens(file=current_file, data=[text], error=None)
-                yield IngestedTokens(file=current_file, data=None, error=None)
+                yield IngestedTokens(file=current_file, data=[text], error=None, doc_source=chunk_bytes.doc_source)
+                yield IngestedTokens(file=current_file, data=None, error=None, doc_source=chunk_bytes.doc_source)
 
         except Exception as e:
-            yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}")
+            yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}", doc_source=chunk_bytes.doc_source)
 
     async def extract_and_process_image(self, collected_bytes: CollectedBytes) -> str:
         text = await self.extract_text_from_image(collected_bytes)
         return await self.process_data(text)
 
     async def extract_text_from_image(self, collected_bytes: CollectedBytes) -> str:
         try:
```

### Comparing `querent-3.0.2/querent/ingestors/ingestor_factory.py` & `querent-3.0.3/querent/ingestors/ingestor_factory.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/ingestors/ingestor_manager.py` & `querent-3.0.3/querent/ingestors/ingestor_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -105,15 +105,15 @@
             IngestorBackend.XML.value: XmlIngestorFactory(),
             IngestorBackend.HTML.value: HtmlIngestorFactory(),
             IngestorBackend.MP4.value: VideoIngestorFactory(),
             IngestorBackend.GITHUB.value: GithubIngestorFactory(),
             IngestorBackend.Slack.value: TextIngestorFactory(is_token_stream=True),
             IngestorBackend.Email.value: EmailIngestorFactory(),
             IngestorBackend.Jira.value: JsonIngestorFactory(),
-            IngestorBackend.News.value: TextIngestorFactory(is_token_stream=True)
+            IngestorBackend.News.value: TextIngestorFactory(is_token_stream=True),
             # Add more mappings as needed
         }
         self.file_caches = LRUCache(maxsize=cache_size)
         self.result_queue = result_queue
         self.tokens_feader = tokens_feader
         self.logger = setup_logger(__name__, "IngestorFactoryManager")
 
@@ -137,16 +137,14 @@
         factory = await self.get_factory(file_extension)
         return factory.supports(file_extension)
 
     @cachedmethod(cache=lambda self: self.file_caches)
     async def ingest_file_async(
         self,
         file_id: str,
-        result_queue: Optional[Queue] = None,
-        tokens_feader: Optional[ChannelCommandInterface] = None,
     ):
         collected_bytes_list = None
         try:
             collected_bytes_list = self.file_caches.pop(file_id)
             file_extension = collected_bytes_list[0].extension
             ingestor = await self.get_ingestor(file_extension)
             if ingestor is not None:
@@ -154,43 +152,28 @@
                 async def chunk_generator() -> AsyncGenerator[CollectedBytes, None]:
                     for chunk in collected_bytes_list:
                         if chunk.eof or chunk.error is not None:
                             break
                         yield chunk
 
                 async for chunk_tokens in ingestor.ingest(chunk_generator()):
-                    if result_queue is not None:
-                        result_queue.put_nowait(chunk_tokens)
-                    if tokens_feader is not None:
-                        tokens_feader.send_tokens_in_rust(
-                            {
-                                "data": (
-                                    chunk_tokens.data
-                                    if type(chunk_tokens) == IngestedTokens
-                                    else chunk_tokens.ocr_text
-                                ),
-                                "file": chunk_tokens.file,
-                                "is_token_stream": True,
-                            }
-                        )
-                        await asyncio.sleep(0.1)
+                    if self.result_queue is not None:
+                        await self.result_queue.put(chunk_tokens)
             else:
                 self.logger.warning(
                     f"Unsupported file extension {file_extension} for file {collected_bytes_list[0].file}"
                 )
         except Exception as e:
             self.logger.error(
                 f"Error ingesting file {collected_bytes_list[0].file}: {str(e)}"
             )
 
     async def ingest_collector_async(
         self,
         collector: Collector,
-        result_queue: Optional[Queue] = None,
-        token_feader: Optional[ChannelCommandInterface] = None,
     ):
         """Asynchronously ingest data from a single collector."""
         async for collected_bytes in collector.poll():
             current_file = collected_bytes.file
 
             if current_file not in self.file_caches:
                 if not collected_bytes.eof:
@@ -199,28 +182,23 @@
                 if not collected_bytes.eof:
                     self.file_caches[current_file].append(collected_bytes)
 
             # Check if this is the end of the file
             if collected_bytes.eof:
                 # Try to ingest the ongoing file even if the cache is full
                 try:
-                    await self.ingest_file_async(
-                        current_file, result_queue, token_feader
-                    )
+                    await self.ingest_file_async(current_file)
                 except Exception as e:
                     self.logger.error(f"Error ingesting file {current_file}: {str(e)}")
 
                 # Wait for ongoing file processing to complete before checking for the next file
                 while current_file in self.file_caches:
                     await asyncio.sleep(0.1)
 
     async def ingest_all_async(self):
         """Asynchronously ingest data from all collectors concurrently."""
         ingestion_tasks = [
-            self.ingest_collector_async(
-                collector, self.result_queue, self.tokens_feader
-            )
-            for collector in self.collectors
+            self.ingest_collector_async(collector) for collector in self.collectors
         ]
         await asyncio.gather(*ingestion_tasks)
         if self.result_queue is not None:
             await self.result_queue.put(None)
```

### Comparing `querent-3.0.2/querent/ingestors/json/json_ingestor.py` & `querent-3.0.3/querent/ingestors/json/json_ingestor.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,44 +43,45 @@
 
                     if chunk_bytes.file != current_file:
                         if current_file:
                             async for json_objects in self.extract_and_process_json(
                                 CollectedBytes(file=current_file, data=collected_bytes)
                             ):
                                 yield IngestedTokens(
-                                    file=current_file, data=[json_objects], error=None
+                                    file=current_file, data=[json_objects], error=None, doc_source=chunk_bytes.doc_source
                                 )
                         if current_file:
                             yield IngestedTokens(
                                 file=current_file,
                                 data=None,
                                 error=None,
+                                doc_source=chunk_bytes.doc_source
                             )
                         collected_bytes = b""
                         current_file = chunk_bytes.file
 
                     collected_bytes += chunk_bytes.data
 
             except json.JSONDecodeError:
                 yield IngestedTokens(
-                    file=current_file, data=None, error="JSON Decode Error"
+                    file=current_file, data=None, error="JSON Decode Error", doc_source=chunk_bytes.doc_source
                 )
             finally:
                 async for json_objects in self.extract_and_process_json(
                     CollectedBytes(file=current_file, data=collected_bytes)
                 ):
                     yield IngestedTokens(
-                        file=current_file, data=[json_objects], error=None
+                        file=current_file, data=[json_objects], error=None, doc_source=chunk_bytes.doc_source
                     )
-                yield IngestedTokens(file=current_file, data=None, error=None)
+                yield IngestedTokens(file=current_file, data=None, error=None, doc_source=chunk_bytes.doc_source)
 
         except Exception as e:
-            yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}")
+            yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}", doc_source=chunk_bytes.doc_source)
 
-    async def extract_and_process_json(self, collected_bytes: CollectedBytes) -> str:
+    async def extract_and_process_json(self, collected_bytes: CollectedBytes):
         try:
             json_data = collected_bytes.data.decode("utf-8")
             processed_text = await self.process_data(json_data)
             yield processed_text
         except json.JSONDecodeError as exc:
             raise common_errors.JsonDecodeError(
                 f"Getting UnicodeDecodeError on this file {collected_bytes.file}"
```

### Comparing `querent-3.0.2/querent/ingestors/pdfs/pdf_ingestor_v1.py` & `querent-3.0.3/querent/ingestors/pdfs/pdf_ingestor_v1.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,45 +51,47 @@
                     continue
 
                 if current_file is None:
                     current_file = chunk_bytes.file
                 elif current_file != chunk_bytes.file:
                     # we have a new file, process the old one
                     async for page_text in self.extract_and_process_pdf(
-                        CollectedBytes(file=current_file, data=collected_bytes)
+                        CollectedBytes(file=current_file, data=collected_bytes), chunk_bytes.doc_source
                     ):
                         yield page_text
                     collected_bytes = b""
                     current_file = chunk_bytes.file
                     yield IngestedTokens(
                         file=current_file,
                         data=None,
                         error=None,
+                        doc_source=chunk_bytes.doc_source,
                     )
                 collected_bytes += chunk_bytes.data
         except Exception as e:
             # at the queue level, we can sample out the error
-            yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}")
+            yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}", doc_source=chunk_bytes.doc_source)
         finally:
             # process the last file
             try:
                 async for page_text in self.extract_and_process_pdf(
-                    CollectedBytes(file=current_file, data=collected_bytes)
+                    CollectedBytes(file=current_file, data=collected_bytes), chunk_bytes.doc_source
                 ):
                     yield page_text
-                yield IngestedTokens(file=current_file, data=None, error=None)
+                yield IngestedTokens(file=current_file, data=None, error=None, doc_source=chunk_bytes.doc_source)
             except Exception as exc:
                 yield IngestedTokens(
                     file=current_file,
                     data=None,
                     error=f"Exception: {exc}",
+                    doc_source=chunk_bytes.doc_source,
                 )
 
     async def extract_and_process_pdf(
-        self, collected_bytes: CollectedBytes
+        self, collected_bytes: CollectedBytes, doc_source: str
     ) -> AsyncGenerator[IngestedTokens, None]:
         try:
             path = BytesIO(collected_bytes.data)
             loader = fitz.open(stream=path.read(), filetype="pdf")
 
 
             for page in loader:
@@ -101,14 +103,15 @@
 
                 processed_text = await self.process_data(text)
                 # Yield processed text as IngestedTokens
                 yield IngestedTokens(
                     file=collected_bytes.file,
                     data=processed_text,
                     error=collected_bytes.error,
+                    doc_source=doc_source,
                 )
                 # async for image_result in self.extract_images_and_ocr(
                 #     page,
                 #     page_num,
                 #     processed_text,
                 #     collected_bytes.data,
                 #     collected_bytes.file,
```

### Comparing `querent-3.0.2/querent/ingestors/ppt/ppt_ingestor.py` & `querent-3.0.3/querent/ingestors/ppt/ppt_ingestor.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,36 +52,37 @@
                 if chunk_bytes.is_error() or chunk_bytes.is_eof():
                     continue
 
                 if current_file is None:
                     current_file = chunk_bytes.file
                 elif current_file != chunk_bytes.file:
                     async for ingested_data in self.extract_and_process_ppt(
-                        CollectedBytes(file=current_file, data=collected_bytes)
+                        CollectedBytes(file=current_file, data=collected_bytes), chunk_bytes.doc_source
                     ):
                         yield ingested_data
                     yield IngestedTokens(
                         file=current_file,
                         data=None,
                         error=None,
+                        doc_source=chunk_bytes.doc_source,
                     )
                     collected_bytes = b""
                     current_file = chunk_bytes.file
                 collected_bytes += chunk_bytes.data
         except Exception as e:
-            yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}")
+            yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}", doc_source=chunk_bytes.doc_source)
         finally:
             async for ingested_data in self.extract_and_process_ppt(
-                CollectedBytes(file=current_file, data=collected_bytes)
+                CollectedBytes(file=current_file, data=collected_bytes), chunk_bytes.doc_source
             ):
                 yield ingested_data
-            yield IngestedTokens(file=current_file, data=None, error=None)
+            yield IngestedTokens(file=current_file, data=None, error=None, doc_source=chunk_bytes.doc_source)
 
     async def extract_and_process_ppt(
-        self, collected_bytes: CollectedBytes
+        self, collected_bytes: CollectedBytes, doc_source: str
     ) -> AsyncGenerator[str, None]:
         try:
             if collected_bytes.extension == "pptx":
                 ppt_file = BytesIO(collected_bytes.data)
                 presentation = Presentation(ppt_file)
                 i=1
                 for slide in presentation.slides:
@@ -91,23 +92,23 @@
                             text.append(shape.text)
                         # if shape.shape_type == MSO_SHAPE_TYPE.PICTURE or (shape.shape_type in [MSO_SHAPE_TYPE.PLACEHOLDER, MSO_SHAPE_TYPE.AUTO_SHAPE] and hasattr(shape, "image")):
                         #     ocr_text = await self.process_image(shape)
                         #     yield IngestedImages(file=collected_bytes.file, image=pybase64.b64encode(shape.image.blob), image_name=str(uuid.uuid4()), page_num=i, text = text, ocr_text=[ocr_text], coordinates=None)
                     slide_text = "\n".join(text)
                     processed_slide_text = await self.process_data(slide_text)
                     yield IngestedTokens(
-                        file=collected_bytes.file, data=processed_slide_text, error=None
+                        file=collected_bytes.file, data=processed_slide_text, error=None, doc_source=doc_source
                     )
                     i+=1
             elif collected_bytes.extension == "ppt":
                 parsed = parser.from_buffer(collected_bytes.data)
                 extracted_text = parsed["content"]
                 processed_text = await self.process_data(extracted_text)
                 yield IngestedTokens(
-                    file=collected_bytes.file, data=processed_text, error=None
+                    file=collected_bytes.file, data=processed_text, error=None, doc_source=doc_source
                 )
             else:
                 raise common_errors.WrongPptFileError(
                     f"Given file is not ppt {collected_bytes.file}"
                 )
         except InvalidXmlError as exc:
             raise common_errors.InvalidXmlError(
```

### Comparing `querent-3.0.2/querent/ingestors/texts/text_ingestor.py` & `querent-3.0.3/querent/ingestors/texts/text_ingestor.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,48 +46,52 @@
                     async for line in self.ingest_token_stream(chunk_bytes=chunk_bytes):
                         process_text = await self.process_data(line)
                         yield IngestedTokens(
                             file=chunk_bytes.file,
                             data=[process_text],
                             error=None,
                             is_token_stream=True,
+                            doc_source=chunk_bytes.doc_source
                         )
                 else:
                     if current_file is None:
                         current_file = chunk_bytes.file
                     elif current_file != chunk_bytes.file:
                         async for line in self.extract_and_process_text(
                             CollectedBytes(file=current_file, data=collected_bytes)
                         ):
                             yield IngestedTokens(
                                 file=current_file,
-                                data=[line],  # Wrap line in a list
+                                data=[line],
                                 error=None,
+                                doc_source=chunk_bytes.doc_source
                             )
                         yield IngestedTokens(
                             file=current_file,
                             data=None,
                             error=None,
+                            doc_source=chunk_bytes.doc_source
                         )
                         collected_bytes = b""
                         current_file = chunk_bytes.file
                     collected_bytes += chunk_bytes.data
 
             if current_file:
                 async for line in self.extract_and_process_text(
                     CollectedBytes(file=current_file, data=collected_bytes)
                 ):
                     yield IngestedTokens(
                         file=current_file,
-                        data=[line],  # Wrap line in a list
+                        data=[line],
                         error=None,
+                        doc_source=chunk_bytes.doc_source,
                     )
-                yield IngestedTokens(file=current_file, data=None, error=None)
+                yield IngestedTokens(file=current_file, data=None, error=None, doc_source=chunk_bytes.doc_source)
         except Exception as e:
-            yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}")
+            yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}", doc_source=chunk_bytes.doc_source)
 
     async def ingest_token_stream(
         self, chunk_bytes: CollectedBytes
     ) -> AsyncGenerator[IngestedTokens, None]:
         message_bytes = chunk_bytes.data.decode("UTF-8")
         lines = message_bytes.split("\n")
         for line in lines:
```

### Comparing `querent-3.0.2/querent/ingestors/video/video_ingestor.py` & `querent-3.0.3/querent/ingestors/video/video_ingestor.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,34 +43,35 @@
                 if current_file is None:
                     current_file = chunk_bytes.file
                 elif current_file != chunk_bytes.file:
                     # We have a new file, process the old one
                     async for text in self.extract_and_process_video(
                         CollectedBytes(file=current_file, data=collected_bytes)
                     ):
-                        yield IngestedTokens(file=current_file, data=[text], error=None)
+                        yield IngestedTokens(file=current_file, data=[text], error=None, doc_source=chunk_bytes.doc_source)
                     # Ensure a final yield for the last processed text
                     yield IngestedTokens(
                         file=current_file,
                         data=None,
                         error=None,
+                        doc_source=chunk_bytes.doc_source
                     )
                     collected_bytes = b""
                     current_file = chunk_bytes.file
                 collected_bytes += chunk_bytes.data
         except Exception as e:
-            yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}")
+            yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}", doc_source=chunk_bytes.doc_source)
         finally:
             if collected_bytes:  # Check if there's data left to process for the last file
                 async for text in self.extract_and_process_video(
                     CollectedBytes(file=current_file, data=collected_bytes)
                 ):
-                    yield IngestedTokens(file=current_file, data=[text], error=None)
+                    yield IngestedTokens(file=current_file, data=[text], error=None, doc_source=chunk_bytes.doc_source)
                 # Ensure a final yield for the last processed text
-                yield IngestedTokens(file=current_file, data=None, error=None)
+                yield IngestedTokens(file=current_file, data=None, error=None, doc_source=chunk_bytes.doc_source)
 
     async def extract_and_process_video(self, collected_bytes: CollectedBytes) -> AsyncGenerator[str, None]:
         text = ""
         async for video_text in self.extract_text_from_video(collected_bytes):
             text += video_text
         processed_text = await self.process_data(text)
         yield processed_text
```

### Comparing `querent-3.0.2/querent/ingestors/xlsx/xlsx_ingestor.py` & `querent-3.0.3/querent/ingestors/xlsx/xlsx_ingestor.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,35 +48,38 @@
                     async for data in self.extract_and_process_xlsx(
                         CollectedBytes(file=current_file, data=collected_bytes)
                     ):
                         yield IngestedTokens(
                             file=current_file,
                             data=[data],
                             error=None,
+                            doc_source=chunk_bytes.doc_source
                         )
                     yield IngestedTokens(
                         file=current_file,
                         data=None,
                         error=None,
+                        doc_source=chunk_bytes.doc_source
                     )
                     collected_bytes = b""
                     current_file = chunk_bytes.file
                 collected_bytes += chunk_bytes.data
         except Exception as e:
-            yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}")
+            yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}", doc_source=chunk_bytes.doc_source)
         finally:
             async for data in self.extract_and_process_xlsx(
                 CollectedBytes(file=current_file, data=collected_bytes)
             ):
                 yield IngestedTokens(
                     file=current_file,
                     data=[data],
                     error=None,
+                    doc_source=chunk_bytes.doc_source
                 )
-            yield IngestedTokens(file=current_file, data=None, error=None)
+            yield IngestedTokens(file=current_file, data=None, error=None, doc_source=chunk_bytes.doc_source)
 
     async def extract_and_process_xlsx(
         self, collected_bytes: CollectedBytes
     ) -> AsyncGenerator[pd.DataFrame, None]:
         df = await self.extract_text_from_xlsx(collected_bytes)
         processed_text = await self.process_data(df.to_string())
         yield processed_text
```

### Comparing `querent-3.0.2/querent/ingestors/xml/xml_ingestor.py` & `querent-3.0.3/querent/ingestors/xml/xml_ingestor.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,32 +49,33 @@
                     continue
                 if current_file is None:
                     current_file = chunk_bytes.file
                 elif current_file != chunk_bytes.file:
                     async for text in self.extract_and_process_xml(
                         CollectedBytes(file=current_file, data=collected_bytes)
                     ):
-                        yield IngestedTokens(file=current_file, data=[text], error=None)
+                        yield IngestedTokens(file=current_file, data=[text], error=None, doc_source=chunk_bytes.doc_source)
                     yield IngestedTokens(
                         file=current_file,
                         data=None,
                         error=None,
+                        doc_source=chunk_bytes.doc_source
                     )
                     collected_bytes = b""
                     current_file = chunk_bytes.file
                 collected_bytes += chunk_bytes.data
         except Exception as e:
-            yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}")
+            yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}", doc_source=chunk_bytes.doc_source)
         finally:
             async for text in self.extract_and_process_xml(
                 CollectedBytes(file=current_file, data=collected_bytes)
             ):
-                yield IngestedTokens(file=current_file, data=[text], error=None)
+                yield IngestedTokens(file=current_file, data=[text], error=None, doc_source=chunk_bytes.doc_source)
 
-            yield IngestedTokens(file=current_file, data=None, error=None)
+            yield IngestedTokens(file=current_file, data=None, error=None, doc_source=chunk_bytes.doc_source)
 
     async def extract_and_process_xml(
         self, collected_bytes: CollectedBytes
     ) -> AsyncGenerator[str, None]:
         """Function to extract and process xml files"""
         text = await self.extract_text_from_xml(collected_bytes)
         processed_text = await self.process_data(text)
```

### Comparing `querent-3.0.2/querent/kg/ner_helperfunctions/attn_scores.py` & `querent-3.0.3/querent/kg/ner_helperfunctions/attn_scores.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/kg/ner_helperfunctions/contextual_embeddings.py` & `querent-3.0.3/querent/kg/ner_helperfunctions/contextual_embeddings.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/kg/ner_helperfunctions/dependency_parsing.py` & `querent-3.0.3/querent/kg/ner_helperfunctions/dependency_parsing.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/kg/ner_helperfunctions/filter_triples.py` & `querent-3.0.3/querent/kg/ner_helperfunctions/filter_triples.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/kg/ner_helperfunctions/fixed_entities.py` & `querent-3.0.3/querent/kg/ner_helperfunctions/fixed_entities.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/kg/ner_helperfunctions/fixed_predicate.py` & `querent-3.0.3/querent/kg/ner_helperfunctions/fixed_predicate.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/kg/ner_helperfunctions/ner_llm_transformer.py` & `querent-3.0.3/querent/kg/ner_helperfunctions/ner_llm_transformer.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/kg/querent_kg.py` & `querent-3.0.3/querent/kg/querent_kg.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/kg/rel_helperfunctions/contextual_predicate.py` & `querent-3.0.3/querent/kg/rel_helperfunctions/contextual_predicate.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/kg/rel_helperfunctions/embedding_store.py` & `querent-3.0.3/querent/kg/rel_helperfunctions/embedding_store.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/kg/rel_helperfunctions/filter_semantic_triples.py` & `querent-3.0.3/querent/kg/rel_helperfunctions/filter_semantic_triples.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/kg/rel_helperfunctions/fixed_relationships.py` & `querent-3.0.3/querent/kg/rel_helperfunctions/fixed_relationships.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py` & `querent-3.0.3/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/kg/rel_helperfunctions/openai_functions.py` & `querent-3.0.3/querent/kg/rel_helperfunctions/openai_functions.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/kg/rel_helperfunctions/questionanswer_llama2.py` & `querent-3.0.3/querent/kg/rel_helperfunctions/questionanswer_llama2.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/kg/rel_helperfunctions/rag_retriever.py` & `querent-3.0.3/querent/kg/rel_helperfunctions/rag_retriever.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/kg/rel_helperfunctions/rel_normalize.py` & `querent-3.0.3/querent/kg/rel_helperfunctions/rel_normalize.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/kg/rel_helperfunctions/triple_to_json.py` & `querent-3.0.3/querent/kg/rel_helperfunctions/triple_to_json.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/logging/filters.py` & `querent-3.0.3/querent/logging/filters.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/logging/handlers.py` & `querent-3.0.3/querent/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/logging/logger.py` & `querent-3.0.3/querent/logging/logger.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/metric/adapters/promethus_adapter.py` & `querent-3.0.3/querent/metric/adapters/promethus_adapter.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/metric/metric_logging_handler.py` & `querent-3.0.3/querent/metric/metric_logging_handler.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/metric/metric_registry.py` & `querent-3.0.3/querent/metric/metric_registry.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/processors/text_cleanup_processor.py` & `querent-3.0.3/querent/processors/text_cleanup_processor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/processors/text_processor.py` & `querent-3.0.3/querent/processors/text_processor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/querent/auto_scaler.py` & `querent-3.0.3/querent/querent/auto_scaler.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/querent/querent.py` & `querent-3.0.3/querent/querent/querent.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/querent/resource_manager.py` & `querent-3.0.3/querent/querent/resource_manager.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/storage/gcs_query.py` & `querent-3.0.3/querent/storage/gcs_query.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/storage/milvus_vectorevent_storage.py` & `querent-3.0.3/querent/storage/milvus_vectorevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/storage/neo4j_graphevent_storage.py` & `querent-3.0.3/querent/storage/neo4j_graphevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/storage/postgres_graphevent_storage.py` & `querent-3.0.3/querent/storage/postgres_graphevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/tools/web_page_extractor.py` & `querent-3.0.3/querent/tools/web_page_extractor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/utils/webpage_extractor.py` & `querent-3.0.3/querent/utils/webpage_extractor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/querent/workflow/_helpers.py` & `querent-3.0.3/querent/workflow/_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,30 +33,30 @@
     # nltk.data.path.append(config.engines[0].nltk_path)
     
     # Set spaCy model path
     spacy_model_path = os.path.join(search_directory, 'en_core_web_lg-3.7.1/en_core_web_lg/en_core_web_lg-3.7.1')
     config.engines[0].spacy_model_path = spacy_model_path
 
     
-async def start_collectors(config: Config):
+async def start_collectors(config: Config, result_queue: QuerentQueue):
     collectors = []
     for collector_config in config.collectors:
         uri = Uri(collector_config.uri)
         collectors.append(CollectorResolver().resolve(uri=uri, config=collector_config))
 
     for collector in collectors:
         await collector.connect()
 
     text_cleanup_processor = TextCleanupProcessor()
     text_processor = TextProcessor()
 
     ingestor_factory_manager = IngestorFactoryManager(
         collectors=collectors,
-        result_queue=None,
-        tokens_feader=config.workflow.tokens_feader,
+        result_queue=result_queue,
+        tokens_feader=None,
         processors=[text_cleanup_processor, text_processor]
     )
 
     ingest_task = asyncio.create_task(ingestor_factory_manager.ingest_all_async())
 
     await ingest_task
 
@@ -142,15 +142,15 @@
 async def receive_token_feeder(
     resource_manager: ResourceManager, config: Config, result_queue: QuerentQueue
 ):
     while not resource_manager.querent_termination_event.is_set():
         tokens = config.workflow.tokens_feader.receive_tokens_in_python()
         if tokens is not None:
             ingested_tokens = IngestedTokens(
-                file=tokens.get("file", None), data=tokens.get("data", None), is_token_stream= tokens.get("is_token_stream"), 
+                file=tokens.get("file", None), data=tokens.get("data", None), is_token_stream= tokens.get("is_token_stream"), doc_source=tokens.get("doc_source", "")
             )
             await result_queue.put(ingested_tokens)
         else:
             await asyncio.sleep(10)
     await result_queue.put(None)
```

### Comparing `querent-3.0.2/querent/workflow/workflow.py` & `querent-3.0.3/querent/workflow/workflow.py`

 * *Files 26% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         if engine_params is not None:
             engine_params_json = {}
             
             if engine_params.get("fixed_entities") is not None:
                 engine_params_json["fixed_entities"] = [x for x in engine_params.get("fixed_entities").split(",")]
             
             if engine_params.get("sample_entities") is not None:
-                engine_params_json["sample_entities"] = [x for x in engine_params.get("fixed_entities").split(",")]
+                engine_params_json["sample_entities"] = [x for x in engine_params.get("sample_entities").split(",")]
             
             if engine_params.get("ner_model_name") is not None:
                 engine_params_json["ner_model_name"] = engine_params.get("ner_model_name")
             
             if engine_params.get("enable_filtering") is not None:
                 engine_params_json["enable_filtering"] = engine_params.get("enable_filtering")
             
@@ -79,75 +79,14 @@
     workflows = {
         "knowledge_graph_using_openai": start_gpt_workflow,
         "knowledge_graph_using_llama2_v1": start_llama_workflow,
     }
 
     workflow = workflows.get(config.workflow.name)
     result_queue = QuerentQueue()
-    collector_tasks = asyncio.create_task(start_collectors(config))
+    collector_tasks = asyncio.create_task(start_collectors(config, result_queue))
     engine_tasks = asyncio.create_task(
         workflow(ResourceManager(), config, result_queue)
     )
     await asyncio.gather(collector_tasks, engine_tasks)
     logger.info("Workflow is finished. All events have been released.")
 
-
-async def start_ingestion(config_dict: dict):
-    if not config_dict:
-        return
-    collectors = []
-    collector_configs = config_dict.get("collectors", [])
-    for collector_config in collector_configs:
-        collectors.append(CollectorConfig(config_source=collector_config).resolve())
-    workflow_config = config_dict.get("workflow")
-    workflow = WorkflowConfig(config_source=workflow_config)
-    config_dict["collectors"] = collectors
-    config_dict["workflow"] = workflow
-    config = Config(config_source=config_dict)
-    collectors = []
-    for collector_config in config.collectors:
-        uri = Uri(collector_config.uri)
-        collectors.append(CollectorResolver().resolve(uri=uri, config=collector_config))
-
-    for collector in collectors:
-        await collector.connect()
-
-    ingestor_factory_manager = IngestorFactoryManager(
-        collectors=collectors,
-        result_queue=None,
-        tokens_feader=config.workflow.tokens_feader,
-    )
-
-    resource_manager = ResourceManager()
-    
-    ingest_task = asyncio.create_task(ingestor_factory_manager.ingest_all_async())
-    check_message_states_task = asyncio.create_task(
-        check_message_states(config, resource_manager, [ingest_task])
-    )
-    await asyncio.gather(ingest_task, check_message_states_task)
-
-async def start_workflow_engine(config_dict: Config):
-    if not config_dict:
-        return
-    workflow_config = config_dict.get("workflow")
-    workflow = WorkflowConfig(config_source=workflow_config)
-    engine_configs = config_dict.get("engines", [])
-    engines = []
-    for engine_config in engine_configs:
-        engine_config_source = engine_config.get("config", {})
-        if engine_config["name"] == "knowledge_graph_using_openai":
-            engines.append(GPTConfig(config_source=engine_config_source))
-        elif engine_config["name"] == "knowledge_graph_using_llama2_v1":
-            engines.append(LLM_Config(config_source=engine_config_source))
-    config_dict["engines"] = engines
-    config_dict["collectors"] = None
-    config_dict["workflow"] = workflow
-    config = Config(config_source=config_dict)
-    workflows = {
-        "knowledge_graph_using_openai": start_gpt_workflow,
-        "knowledge_graph_using_llama2_v1": start_llama_workflow,
-    }
-    workflow = workflows.get(config.workflow.name)
-    result_queue = QuerentQueue()
-    resource_manager = ResourceManager()
-
-    await workflow(resource_manager, config, result_queue)
```

### Comparing `querent-3.0.2/querent.egg-info/PKG-INFO` & `querent-3.0.3/querent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querent
-Version: 3.0.2
+Version: 3.0.3
 Summary: The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 Home-page: https://github.com/Querent-ai/querent-ai
 Author: Querent AI
 License: Business Source License 1.1
 Project-URL: Documentation, https://github.com/Querent-ai/querent-ai/docs
 Project-URL: Issue Tracker, https://github.com/Querent-ai/querent-ai/issues
 Keywords: Graph Neural Network,Scalability,Data-Driven Insights,GNN,Async,Knowledge Graphs,KG,Large Language Models,asyncio,Insights,aysnchronous,LLM,transformers,pytorch,Llama-index,AI,Artificial Intelligence,Neo4j,Queues,QuiAssisstant,Collectors,Data,Data Science,Data Engineering,Data Analysis,Data Analytics,News,NLP,Natural Language Processing,Text,Text Analysis,Deep Learning,Graphs,Graph Theory,Graph Algorithms,Graph Analytics,Graph Databases,Graph Processing,Graph Mining,Graph Neural Networks,GNN,GNNs,Graph Neural Network
```

### Comparing `querent-3.0.2/querent.egg-info/SOURCES.txt` & `querent-3.0.3/querent.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,14 @@
 querent/ingestors/texts/text_ingestor.py
 querent/ingestors/video/__init__.py
 querent/ingestors/video/video_ingestor.py
 querent/ingestors/xlsx/__init__.py
 querent/ingestors/xlsx/xlsx_ingestor.py
 querent/ingestors/xml/__init__.py
 querent/ingestors/xml/xml_ingestor.py
-querent/insights/__init__.py
 querent/kg/__init__.py
 querent/kg/querent_kg.py
 querent/kg/ner_helperfunctions/__init__.py
 querent/kg/ner_helperfunctions/attn_scores.py
 querent/kg/ner_helperfunctions/contextual_embeddings.py
 querent/kg/ner_helperfunctions/dependency_parsing.py
 querent/kg/ner_helperfunctions/filter_triples.py
@@ -178,21 +177,19 @@
 querent/processors/text_cleanup_processor.py
 querent/processors/text_processor.py
 querent/querent/__init__.py
 querent/querent/auto_scaler.py
 querent/querent/querent.py
 querent/querent/resource_manager.py
 querent/querent/worker.py
-querent/search/__init__.py
 querent/storage/__init__.py
 querent/storage/gcs_query.py
 querent/storage/milvus_vectorevent_storage.py
 querent/storage/neo4j_graphevent_storage.py
 querent/storage/postgres_graphevent_storage.py
-querent/storage/s3-data-management.py
 querent/tools/__init__.py
 querent/tools/web_page_extractor.py
 querent/utils/__init__.py
 querent/utils/webpage_extractor.py
 querent/workflow/__init__.py
 querent/workflow/_helpers.py
 querent/workflow/workflow.py
```

### Comparing `querent-3.0.2/querent.egg-info/requires.txt` & `querent-3.0.3/querent.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `querent-3.0.2/setup.py` & `querent-3.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 ]
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="querent",
-    version="3.0.2",
+    version="3.0.3",
     author="Querent AI",
     description="The Asynchronous Data Dynamo and Graph Neural Network Catalyst",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Querent-ai/querent-ai",
     project_urls={
         "Documentation": "https://github.com/Querent-ai/querent-ai/docs",
```

