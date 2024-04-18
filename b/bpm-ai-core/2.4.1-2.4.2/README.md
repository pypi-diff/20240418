# Comparing `tmp/bpm_ai_core-2.4.1.tar.gz` & `tmp/bpm_ai_core-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpm_ai_core-2.4.1.tar", max compression
+gzip compressed data, was "bpm_ai_core-2.4.2.tar", max compression
```

## Comparing `bpm_ai_core-2.4.1.tar` & `bpm_ai_core-2.4.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0       13 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/README.md
--rw-r--r--   0        0        0        0 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/classification/__init__.py
--rw-r--r--   0        0        0     1420 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/classification/zero_shot_classifier.py
--rw-r--r--   0        0        0        0 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/llm/__init__.py
--rw-r--r--   0        0        0      862 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/llm/anthropic_chat/__init__.py
--rw-r--r--   0        0        0      306 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/llm/anthropic_chat/_constants.py
--rw-r--r--   0        0        0     6645 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py
--rw-r--r--   0        0        0      226 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/llm/anthropic_chat/output_schema.prompt
--rw-r--r--   0        0        0     4872 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/llm/anthropic_chat/util.py
--rw-r--r--   0        0        0        0 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/llm/common/__init__.py
--rw-r--r--   0        0        0     6141 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/llm/common/blob.py
--rw-r--r--   0        0        0     2445 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/llm/common/llm.py
--rw-r--r--   0        0        0     2710 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/llm/common/message.py
--rw-r--r--   0        0        0     2781 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/llm/common/tool.py
--rw-r--r--   0        0        0     1455 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/llm/openai_chat/__init__.py
--rw-r--r--   0        0        0      430 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/llm/openai_chat/_constants.py
--rw-r--r--   0        0        0     7777 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/llm/openai_chat/openai_chat.py
--rw-r--r--   0        0        0     3340 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/llm/openai_chat/util.py
--rw-r--r--   0        0        0        0 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/ocr/__init__.py
--rw-r--r--   0        0        0     5611 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/ocr/amazon_textract.py
--rw-r--r--   0        0        0     2698 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/ocr/azure_doc_intelligence.py
--rw-r--r--   0        0        0     1220 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/ocr/ocr.py
--rw-r--r--   0        0        0        0 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/pos/__init__.py
--rw-r--r--   0        0        0      590 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/pos/pos_tagger.py
--rw-r--r--   0        0        0        0 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/prompt/__init__.py
--rw-r--r--   0        0        0      372 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/prompt/filters.py
--rw-r--r--   0        0        0     6259 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/prompt/prompt.py
--rw-r--r--   0        0        0        0 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/question_answering/__init__.py
--rw-r--r--   0        0        0     2085 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/question_answering/amazon_textract_docvqa.py
--rw-r--r--   0        0        0     3018 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py
--rw-r--r--   0        0        0     1096 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/question_answering/question_answering.py
--rw-r--r--   0        0        0        0 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/speech_recognition/__init__.py
--rw-r--r--   0        0        0      827 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/speech_recognition/asr.py
--rw-r--r--   0        0        0     1428 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/speech_recognition/openai_whisper.py
--rw-r--r--   0        0        0        0 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/testing/__init__.py
--rw-r--r--   0        0        0     2889 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/testing/fake_llm.py
--rw-r--r--   0        0        0        0 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/token_classification/__init__.py
--rw-r--r--   0        0        0      909 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/token_classification/zero_shot_token_classifier.py
--rw-r--r--   0        0        0        0 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/tracing/__init__.py
--rw-r--r--   0        0        0     2434 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/tracing/decorators.py
--rw-r--r--   0        0        0     1597 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/tracing/delegate.py
--rw-r--r--   0        0        0     4381 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/tracing/langfuse.py
--rw-r--r--   0        0        0     2347 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/tracing/logging.py
--rw-r--r--   0        0        0     1097 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/tracing/tracer.py
--rw-r--r--   0        0        0      876 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/tracing/tracing.py
--rw-r--r--   0        0        0        0 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/translation/__init__.py
--rw-r--r--   0        0        0     1302 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/translation/amazon_translate.py
--rw-r--r--   0        0        0     1572 2024-04-16 15:03:46.641817 bpm_ai_core-2.4.1/bpm_ai_core/translation/azure_translation.py
--rw-r--r--   0        0        0      475 2024-04-16 15:03:46.645817 bpm_ai_core-2.4.1/bpm_ai_core/translation/nmt.py
--rw-r--r--   0        0        0        0 2024-04-16 15:03:46.645817 bpm_ai_core-2.4.1/bpm_ai_core/util/__init__.py
--rw-r--r--   0        0        0     1154 2024-04-16 15:03:46.645817 bpm_ai_core-2.4.1/bpm_ai_core/util/audio.py
--rw-r--r--   0        0        0     2290 2024-04-16 15:03:46.645817 bpm_ai_core-2.4.1/bpm_ai_core/util/file.py
--rw-r--r--   0        0        0     5945 2024-04-16 15:03:46.645817 bpm_ai_core-2.4.1/bpm_ai_core/util/image.py
--rw-r--r--   0        0        0     3135 2024-04-16 15:03:46.645817 bpm_ai_core-2.4.1/bpm_ai_core/util/json_schema.py
--rw-r--r--   0        0        0    22412 2024-04-16 15:03:46.645817 bpm_ai_core-2.4.1/bpm_ai_core/util/linguistics.py
--rw-r--r--   0        0        0     1130 2024-04-16 15:03:46.645817 bpm_ai_core-2.4.1/bpm_ai_core/util/markdown.py
--rw-r--r--   0        0        0     5280 2024-04-16 15:03:46.645817 bpm_ai_core-2.4.1/bpm_ai_core/util/remote_object.py
--rw-r--r--   0        0        0     2596 2024-04-16 15:03:46.645817 bpm_ai_core-2.4.1/bpm_ai_core/util/storage.py
--rw-r--r--   0        0        0      670 2024-04-16 15:03:46.645817 bpm_ai_core-2.4.1/bpm_ai_core/util/text.py
--rw-r--r--   0        0        0      675 2024-04-16 15:03:46.645817 bpm_ai_core-2.4.1/bpm_ai_core/util/xml_convert.py
--rw-r--r--   0        0        0     1014 2024-04-16 15:03:46.645817 bpm_ai_core-2.4.1/pyproject.toml
--rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 bpm_ai_core-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0       13 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/classification/__init__.py
+-rw-r--r--   0        0        0     1420 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/classification/zero_shot_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/__init__.py
+-rw-r--r--   0        0        0      862 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/anthropic_chat/__init__.py
+-rw-r--r--   0        0        0      306 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/anthropic_chat/_constants.py
+-rw-r--r--   0        0        0     6645 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py
+-rw-r--r--   0        0        0      226 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/anthropic_chat/output_schema.prompt
+-rw-r--r--   0        0        0     4872 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/anthropic_chat/util.py
+-rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/common/__init__.py
+-rw-r--r--   0        0        0     6141 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/common/blob.py
+-rw-r--r--   0        0        0     2445 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/common/llm.py
+-rw-r--r--   0        0        0     2710 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/common/message.py
+-rw-r--r--   0        0        0     2781 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/common/tool.py
+-rw-r--r--   0        0        0     1455 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/openai_chat/__init__.py
+-rw-r--r--   0        0        0      430 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/openai_chat/_constants.py
+-rw-r--r--   0        0        0     7777 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/openai_chat/openai_chat.py
+-rw-r--r--   0        0        0     3340 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/openai_chat/util.py
+-rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/ocr/__init__.py
+-rw-r--r--   0        0        0     5611 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/ocr/amazon_textract.py
+-rw-r--r--   0        0        0     2698 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/ocr/azure_doc_intelligence.py
+-rw-r--r--   0        0        0     1220 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/ocr/ocr.py
+-rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/pos/__init__.py
+-rw-r--r--   0        0        0      590 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/pos/pos_tagger.py
+-rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/prompt/__init__.py
+-rw-r--r--   0        0        0      372 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/prompt/filters.py
+-rw-r--r--   0        0        0     6259 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/prompt/prompt.py
+-rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/question_answering/__init__.py
+-rw-r--r--   0        0        0     1989 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/question_answering/amazon_textract_docvqa.py
+-rw-r--r--   0        0        0     3028 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py
+-rw-r--r--   0        0        0     1096 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/question_answering/question_answering.py
+-rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/speech_recognition/__init__.py
+-rw-r--r--   0        0        0      827 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/speech_recognition/asr.py
+-rw-r--r--   0        0        0     1428 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/speech_recognition/openai_whisper.py
+-rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/testing/__init__.py
+-rw-r--r--   0        0        0     2894 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/testing/fake_llm.py
+-rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/token_classification/__init__.py
+-rw-r--r--   0        0        0      909 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/token_classification/zero_shot_token_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/tracing/__init__.py
+-rw-r--r--   0        0        0     2434 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/tracing/decorators.py
+-rw-r--r--   0        0        0     1597 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/tracing/delegate.py
+-rw-r--r--   0        0        0     4381 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/tracing/langfuse.py
+-rw-r--r--   0        0        0     2347 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/tracing/logging.py
+-rw-r--r--   0        0        0     1097 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/tracing/tracer.py
+-rw-r--r--   0        0        0      876 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/tracing/tracing.py
+-rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/translation/__init__.py
+-rw-r--r--   0        0        0     1302 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/translation/amazon_translate.py
+-rw-r--r--   0        0        0     1572 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/translation/azure_translation.py
+-rw-r--r--   0        0        0      475 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/translation/nmt.py
+-rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/util/__init__.py
+-rw-r--r--   0        0        0     1154 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/util/audio.py
+-rw-r--r--   0        0        0     2290 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/util/file.py
+-rw-r--r--   0        0        0     6130 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/util/image.py
+-rw-r--r--   0        0        0     3135 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/util/json_schema.py
+-rw-r--r--   0        0        0    22412 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/util/linguistics.py
+-rw-r--r--   0        0        0     1130 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/util/markdown.py
+-rw-r--r--   0        0        0     5280 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/util/remote_object.py
+-rw-r--r--   0        0        0     2596 2024-04-18 11:33:11.404127 bpm_ai_core-2.4.2/bpm_ai_core/util/storage.py
+-rw-r--r--   0        0        0      670 2024-04-18 11:33:11.404127 bpm_ai_core-2.4.2/bpm_ai_core/util/text.py
+-rw-r--r--   0        0        0      675 2024-04-18 11:33:11.404127 bpm_ai_core-2.4.2/bpm_ai_core/util/xml_convert.py
+-rw-r--r--   0        0        0     1036 2024-04-18 11:33:11.404127 bpm_ai_core-2.4.2/pyproject.toml
+-rw-r--r--   0        0        0      953 1970-01-01 00:00:00.000000 bpm_ai_core-2.4.2/PKG-INFO
```

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/classification/zero_shot_classifier.py` & `bpm_ai_core-2.4.2/bpm_ai_core/classification/zero_shot_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/llm/anthropic_chat/__init__.py` & `bpm_ai_core-2.4.2/bpm_ai_core/llm/anthropic_chat/__init__.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py` & `bpm_ai_core-2.4.2/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/llm/anthropic_chat/util.py` & `bpm_ai_core-2.4.2/bpm_ai_core/llm/anthropic_chat/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/llm/common/blob.py` & `bpm_ai_core-2.4.2/bpm_ai_core/llm/common/blob.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/llm/common/llm.py` & `bpm_ai_core-2.4.2/bpm_ai_core/llm/common/llm.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/llm/common/message.py` & `bpm_ai_core-2.4.2/bpm_ai_core/llm/common/message.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/llm/common/tool.py` & `bpm_ai_core-2.4.2/bpm_ai_core/llm/common/tool.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/llm/openai_chat/__init__.py` & `bpm_ai_core-2.4.2/bpm_ai_core/llm/openai_chat/__init__.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/llm/openai_chat/openai_chat.py` & `bpm_ai_core-2.4.2/bpm_ai_core/llm/openai_chat/openai_chat.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/llm/openai_chat/util.py` & `bpm_ai_core-2.4.2/bpm_ai_core/llm/openai_chat/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/ocr/amazon_textract.py` & `bpm_ai_core-2.4.2/bpm_ai_core/ocr/amazon_textract.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/ocr/azure_doc_intelligence.py` & `bpm_ai_core-2.4.2/bpm_ai_core/ocr/azure_doc_intelligence.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/ocr/ocr.py` & `bpm_ai_core-2.4.2/bpm_ai_core/ocr/ocr.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/pos/pos_tagger.py` & `bpm_ai_core-2.4.2/bpm_ai_core/pos/pos_tagger.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/prompt/prompt.py` & `bpm_ai_core-2.4.2/bpm_ai_core/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/question_answering/amazon_textract_docvqa.py` & `bpm_ai_core-2.4.2/bpm_ai_core/question_answering/amazon_textract_docvqa.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,19 +49,16 @@
                 ]}
             )
 
         prediction = next((b for b in response['Blocks'] if b["BlockType"] == "QUERY_RESULT"), {})
 
         logger.debug(f"prediction: {prediction}")
 
-        if prediction is None:
-            raise Exception('AmazonTextractDocVQA failed to extract information.')
-
         return QAResult(
-            answer=prediction['Text'],
-            score=prediction['Confidence'] / 100.0,
+            answer=prediction.get('Text', None),
+            score=prediction.get('Confidence', 0.0) / 100.0,
             start_index=None,
             end_index=None,
         )
```

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py` & `bpm_ai_core-2.4.2/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             )
 
             # Wait for the extraction to complete asynchronously
             result = await document.result()
             prediction = result['documents'][0]['fields'][question]
 
         return QAResult(
-            answer=prediction['content'],
+            answer=prediction.get('content', None),
             score=prediction['confidence'],
             start_index=None,
             end_index=None,
         )
 
     @staticmethod
     def to_camel_case(text: str) -> str:
```

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/question_answering/question_answering.py` & `bpm_ai_core-2.4.2/bpm_ai_core/question_answering/question_answering.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/speech_recognition/asr.py` & `bpm_ai_core-2.4.2/bpm_ai_core/speech_recognition/asr.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/speech_recognition/openai_whisper.py` & `bpm_ai_core-2.4.2/bpm_ai_core/speech_recognition/openai_whisper.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/testing/fake_llm.py` & `bpm_ai_core-2.4.2/bpm_ai_core/testing/fake_llm.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from bpm_ai_core.llm.common.llm import LLM
 from bpm_ai_core.llm.common.message import ChatMessage, ToolCallMessage, AssistantMessage
 from bpm_ai_core.llm.common.tool import Tool
 from bpm_ai_core.tracing.tracing import Tracing
 
 
 def messages_to_str(messages: List[ChatMessage]) -> str:
-    return "\n\n".join([m.content for m in messages])
+    return "\n\n".join([str(m.content) for m in messages])
 
 
 def tool_response(name, payload):
     return AssistantMessage(tool_calls=[ToolCallMessage(id="fake", name=name, payload=payload)])
 
 
 class FakeLLM(LLM):
```

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/token_classification/zero_shot_token_classifier.py` & `bpm_ai_core-2.4.2/bpm_ai_core/token_classification/zero_shot_token_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/tracing/decorators.py` & `bpm_ai_core-2.4.2/bpm_ai_core/tracing/decorators.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/tracing/delegate.py` & `bpm_ai_core-2.4.2/bpm_ai_core/tracing/delegate.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/tracing/langfuse.py` & `bpm_ai_core-2.4.2/bpm_ai_core/tracing/langfuse.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/tracing/logging.py` & `bpm_ai_core-2.4.2/bpm_ai_core/tracing/logging.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/tracing/tracer.py` & `bpm_ai_core-2.4.2/bpm_ai_core/tracing/tracer.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/tracing/tracing.py` & `bpm_ai_core-2.4.2/bpm_ai_core/tracing/tracing.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/translation/amazon_translate.py` & `bpm_ai_core-2.4.2/bpm_ai_core/translation/amazon_translate.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/translation/azure_translation.py` & `bpm_ai_core-2.4.2/bpm_ai_core/translation/azure_translation.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/util/audio.py` & `bpm_ai_core-2.4.2/bpm_ai_core/util/audio.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/util/file.py` & `bpm_ai_core-2.4.2/bpm_ai_core/util/file.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/util/image.py` & `bpm_ai_core-2.4.2/bpm_ai_core/util/image.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import re
 import tempfile
 from io import BytesIO
 from typing import Union, Tuple
 
 from PIL import Image, ImageDraw
 from pdf2image import convert_from_path, convert_from_bytes
+from pypdfium2 import PdfDocument
 
 logger = logging.getLogger(__name__)
 
 
 image_ext_map = {
     'bmp': 'image/bmp',
     'gif': 'image/gif',
@@ -47,64 +48,73 @@
 
     Returns:
         A list of PIL Image objects or a list of bytes representing the converted images.
     """
     if blob.is_pdf():
         # Convert PDF to a list of images
         logger.info("Converting PDF to a list of images...")
-        images = pdf_to_images(await blob.as_bytes())
+        try:
+            images = pdf_to_images(await blob.as_bytes())
+        except Exception:
+            logger.warning("Could not convert to PDF using pypdfium2, trying pdf2image...")
+            images = pdf_to_images_poppler(await blob.as_bytes())
     elif blob.is_image():
         # Load the image from the blob
         images = [Image.open(await blob.as_bytes_io())]
     else:
         raise ValueError(f"Unsupported blob type: {blob.mimetype}")
 
     accept_formats = [f.lower() for f in accept_formats]
 
     # Convert images to the accepted formats if necessary
     converted_images = []
     for image in images:
-        if image.format.lower() not in accept_formats:
+        if (not image.format) or (image.format.lower() not in accept_formats):
             # Convert the image to the first accepted format
             output_format = accept_formats[0]
-            logger.info(f"Converting images from {image.format.lower()} to accepted format: {output_format}")
-            if return_bytes:
-                # Convert the image to bytes
-                with io.BytesIO() as output_bytes:
-                    if not image.mode == "RGB":
-                        image = image.convert("RGB")
-                    image.save(output_bytes, format=output_format)
-                    converted_images.append(output_bytes.getvalue())
-            else:
-                # Convert the image to PIL Image object
-                converted_image = io.BytesIO()
-                if not image.mode == "RGB":
-                    image = image.convert("RGB")
-                image.save(converted_image, format=output_format)
-                converted_image.seek(0)
-                converted_images.append(Image.open(converted_image))
+            logger.info(f"Converting images from {image.format.lower() if image.format else 'bitmap'} to accepted format: {output_format}")
+            converted_images.append(
+                convert_image(image, format=output_format, return_bytes=return_bytes)
+            )
         else:
             if return_bytes:
                 # Convert the image to bytes
                 with io.BytesIO() as output_bytes:
                     image.save(output_bytes, format=image.format)
                     converted_images.append(output_bytes.getvalue())
             else:
                 converted_images.append(image)
 
     return converted_images
 
 
 def pdf_to_images(pdf: bytes | str) -> list[Image]:
+    pdf = PdfDocument(pdf)
+    return [page.render(scale=2).to_pil() for page in pdf]
+
+
+def pdf_to_images_poppler(pdf: bytes | str) -> list[Image]:
     with tempfile.TemporaryDirectory() as path:
         if isinstance(pdf, bytes):
             func = convert_from_bytes
         else:
             func = convert_from_path
-        return func(pdf, output_folder=path, dpi=100, use_pdftocairo=True)
+        return func(pdf, output_folder=path, dpi=150, use_pdftocairo=True)
+
+
+def convert_image(image: Image, format="PNG", return_bytes=False):
+    image_buffer = io.BytesIO()
+    if not image.mode == "RGB":
+        image = image.convert("RGB")
+    image.save(image_buffer, format=format, quality=100)
+    image_buffer.seek(0)
+    if return_bytes:
+        return image_buffer.getvalue()
+    else:
+        return Image.open(image_buffer)
 
 
 def base64_encode_image(image: Image):
     """
     Get a base64 encoded string from a Pillow Image object.
 
     Parameters:
```

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/util/json_schema.py` & `bpm_ai_core-2.4.2/bpm_ai_core/util/json_schema.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/util/linguistics.py` & `bpm_ai_core-2.4.2/bpm_ai_core/util/linguistics.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/util/markdown.py` & `bpm_ai_core-2.4.2/bpm_ai_core/util/markdown.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/util/remote_object.py` & `bpm_ai_core-2.4.2/bpm_ai_core/util/remote_object.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/util/storage.py` & `bpm_ai_core-2.4.2/bpm_ai_core/util/storage.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/util/text.py` & `bpm_ai_core-2.4.2/bpm_ai_core/util/text.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/bpm_ai_core/util/xml_convert.py` & `bpm_ai_core-2.4.2/bpm_ai_core/util/xml_convert.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.1/pyproject.toml` & `bpm_ai_core-2.4.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpm-ai-core"
-version = "2.4.1"
+version = "2.4.2"
 description = "Core AI abstractions and helpers."
 authors = ["Bennet Krause <bennet.krause@holisticon.de>"]
 repository = "https://github.com/holunda-io/bpm-ai"
 homepage = "https://www.holisticon.de/"
 license = "Apache-2.0"
 readme = "README.md"
 
@@ -14,14 +14,15 @@
 tenacity = "^8.2.3"
 pydantic = "^2.6.4"
 pillow = "^10.1.0"
 pdf2image = "^1.17.0"
 requests = "^2.31.0"
 xmltodict = "^0.13.0"
 aiohttp = "^3.9.3"
+pypdfium2 = "^4.29.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.2"
 pytest-asyncio = "^0.23.5"
 pytest-dotenv = "^0.5.2"
```

