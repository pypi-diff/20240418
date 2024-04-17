# Comparing `tmp/eidolon_ai_sdk-0.1.27.tar.gz` & `tmp/eidolon_ai_sdk-0.1.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eidolon_ai_sdk-0.1.27.tar", max compression
+gzip compressed data, was "eidolon_ai_sdk-0.1.28.tar", max compression
```

## Comparing `eidolon_ai_sdk-0.1.27.tar` & `eidolon_ai_sdk-0.1.28.tar`

### file list

```diff
@@ -1,143 +1,143 @@
--rw-r--r--   0        0        0     2569 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/README.md
--rw-r--r--   0        0        0        0 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/__init__.py
--rw-r--r--   0        0        0     2400 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/agent.py
--rw-r--r--   0        0        0        0 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/__init__.py
--rw-r--r--   0        0        0     3025 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/document_manager.py
--rw-r--r--   0        0        0     2710 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/document_processor.py
--rw-r--r--   0        0        0        0 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/loaders/__init__.py
--rw-r--r--   0        0        0      971 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py
--rw-r--r--   0        0        0     3405 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py
--rw-r--r--   0        0        0     4173 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py
--rw-r--r--   0        0        0        0 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/__init__.py
--rw-r--r--   0        0        0     2805 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py
--rw-r--r--   0        0        0     4519 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py
--rw-r--r--   0        0        0        0 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/__init__.py
--rw-r--r--   0        0        0      448 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/base_ast_generator.py
--rw-r--r--   0        0        0     3699 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py
--rw-r--r--   0        0        0     2053 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py
--rw-r--r--   0        0        0     3212 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py
--rw-r--r--   0        0        0     1647 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py
--rw-r--r--   0        0        0     1328 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py
--rw-r--r--   0        0        0     3356 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py
--rw-r--r--   0        0        0     1400 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py
--rw-r--r--   0        0        0        0 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/transformer/__init__.py
--rw-r--r--   0        0        0     1398 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py
--rw-r--r--   0        0        0     4786 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py
--rw-r--r--   0        0        0    43465 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py
--rw-r--r--   0        0        0     4825 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/generic_agent.py
--rw-r--r--   0        0        0     1924 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/openai_whisper_agent.py
--rw-r--r--   0        0        0        0 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/retriever_agent/__init__.py
--rw-r--r--   0        0        0     2078 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py
--rw-r--r--   0        0        0     1434 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py
--rw-r--r--   0        0        0     2329 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py
--rw-r--r--   0        0        0      559 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py
--rw-r--r--   0        0        0     2904 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/retriever_agent/retriever.py
--rw-r--r--   0        0        0     3721 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py
--rw-r--r--   0        0        0    12896 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/simple_agent.py
--rw-r--r--   0        0        0        0 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/__init__.py
--rw-r--r--   0        0        0     1815 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/checker.py
--rw-r--r--   0        0        0     2468 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/controller.py
--rw-r--r--   0        0        0     1503 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/memory.py
--rw-r--r--   0        0        0     1423 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/prompts.py
--rw-r--r--   0        0        0      364 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/thought.py
--rw-r--r--   0        0        0     4951 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/thought_generators.py
--rw-r--r--   0        0        0     7614 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/tot_agent.py
--rw-r--r--   0        0        0     4563 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent_os.py
--rw-r--r--   0        0        0    12721 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent_os_interfaces.py
--rw-r--r--   0        0        0        0 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/bin/__init__.py
--rwxr-xr-x   0        0        0     9444 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/bin/agent_creator.py
--rw-r--r--   0        0        0     7743 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/bin/agent_http_server.py
--rwxr-xr-x   0        0        0     3789 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/bin/replay.py
--rw-r--r--   0        0        0        0 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/__init__.py
--rw-r--r--   0        0        0     8852 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/code_builtins.py
--rw-r--r--   0        0        0        0 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/components/__init__.py
--rw-r--r--   0        0        0     2223 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/components/opentelemetry.py
--rw-r--r--   0        0        0     4256 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/components/usage.py
--rw-r--r--   0        0        0        0 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/logic_units/__init__.py
--rw-r--r--   0        0        0     5662 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/logic_units/web_search.py
--rw-r--r--   0        0        0      550 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml
--rw-r--r--   0        0        0      544 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/resources/claude_opus.yaml
--rw-r--r--   0        0        0      557 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml
--rw-r--r--   0        0        0      181 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/resources/machine.yaml
--rw-r--r--   0        0        0      540 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/resources/mistral_large.yaml
--rw-r--r--   0        0        0      547 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml
--rw-r--r--   0        0        0      540 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/resources/mistral_small.yaml
--rw-r--r--   0        0        0      534 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/resources/openai_35.yaml
--rw-r--r--   0        0        0      557 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/resources/openai_4.yaml
--rw-r--r--   0        0        0        0 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/__init__.py
--rw-r--r--   0        0        0     1843 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/agent_call_history.py
--rw-r--r--   0        0        0     4638 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/agent_cpu.py
--rw-r--r--   0        0        0     2474 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/agent_io.py
--rw-r--r--   0        0        0     7916 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/agents_logic_unit.py
--rw-r--r--   0        0        0     1641 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/audio_unit.py
--rw-r--r--   0        0        0      292 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/call_context.py
--rw-r--r--   0        0        0     2833 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/conversation_memory_unit.py
--rw-r--r--   0        0        0    14068 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/conversational_apu.py
--rw-r--r--   0        0        0     1856 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/image_unit.py
--rw-r--r--   0        0        0        0 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm/__init__.py
--rw-r--r--   0        0        0    10023 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py
--rw-r--r--   0        0        0    11932 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py
--rw-r--r--   0        0        0     5396 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py
--rw-r--r--   0        0        0     5631 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py
--rw-r--r--   0        0        0     9485 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py
--rw-r--r--   0        0        0     3375 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm/open_ai_speech.py
--rw-r--r--   0        0        0     3930 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm_message.py
--rw-r--r--   0        0        0     2421 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm_unit.py
--rw-r--r--   0        0        0     4199 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/logic_unit.py
--rw-r--r--   0        0        0     3541 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/memory_unit.py
--rw-r--r--   0        0        0      825 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/processing_unit.py
--rw-r--r--   0        0        0        0 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/io/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/__init__.py
--rw-r--r--   0        0        0     1193 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/agent_memory.py
--rw-r--r--   0        0        0     5309 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/chroma_vector_store.py
--rw-r--r--   0        0        0      641 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/document.py
--rw-r--r--   0        0        0     2766 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/embeddings.py
--rw-r--r--   0        0        0      907 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/file_memory.py
--rw-r--r--   0        0        0     4203 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/file_system_vector_store.py
--rw-r--r--   0        0        0     3974 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/in_memory_file_memory.py
--rw-r--r--   0        0        0     5788 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/local_file_memory.py
--rw-r--r--   0        0        0     4845 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/local_symbolic_memory.py
--rw-r--r--   0        0        0     3770 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/mongo_symbolic_memory.py
--rw-r--r--   0        0        0      996 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/noop_memory.py
--rw-r--r--   0        0        0     1984 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/s3_file_memory.py
--rw-r--r--   0        0        0      975 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/semantic_memory.py
--rw-r--r--   0        0        0     2809 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/similarity_memory.py
--rw-r--r--   0        0        0     1516 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/vector_store.py
--rw-r--r--   0        0        0        0 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/__init__.py
--rw-r--r--   0        0        0      771 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/authentication_processor.py
--rw-r--r--   0        0        0     2091 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/azure_authorizer.py
--rw-r--r--   0        0        0     1277 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/functional_authorizer.py
--rw-r--r--   0        0        0     2001 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/google_auth.py
--rw-r--r--   0        0        0     1867 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/jwt_processor.py
--rw-r--r--   0        0        0      484 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/okta_authorizor.py
--rw-r--r--   0        0        0     1017 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/permissions.py
--rw-r--r--   0        0        0     2508 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/process_authorizer.py
--rw-r--r--   0        0        0     2977 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/security_manager.py
--rw-r--r--   0        0        0     1035 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/security_middleware.py
--rw-r--r--   0        0        0      428 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/user.py
--rw-r--r--   0        0        0        0 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/__init__.py
--rw-r--r--   0        0        0     1377 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/agent_contract.py
--rw-r--r--   0        0        0    21672 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/agent_controller.py
--rw-r--r--   0        0        0    14143 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/agent_machine.py
--rw-r--r--   0        0        0     1149 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/dynamic_middleware.py
--rw-r--r--   0        0        0     3432 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/fn_handler.py
--rw-r--r--   0        0        0     4880 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/process_file_system.py
--rw-r--r--   0        0        0     4275 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/processes.py
--rw-r--r--   0        0        0     6895 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/reference_model.py
--rw-r--r--   0        0        0        0 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/resources/__init__.py
--rw-r--r--   0        0        0      314 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/resources/agent_resource.py
--rw-r--r--   0        0        0      414 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/resources/machine_resource.py
--rw-r--r--   0        0        0      684 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/resources/reference_resource.py
--rw-r--r--   0        0        0     1663 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/resources/resources_base.py
--rw-r--r--   0        0        0        0 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/__init__.py
--rw-r--r--   0        0        0      509 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/async_wrapper.py
--rw-r--r--   0        0        0     2806 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/class_utils.py
--rw-r--r--   0        0        0     1604 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/image_utils.py
--rw-r--r--   0        0        0     3812 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/replay.py
--rw-r--r--   0        0        0     6483 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/schema_to_model.py
--rw-r--r--   0        0        0      900 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/str_utils.py
--rw-r--r--   0        0        0     3445 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/stream_collector.py
--rw-r--r--   0        0        0      565 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/logging.conf
--rw-r--r--   0        0        0     2030 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/pyproject.toml
--rw-r--r--   0        0        0     4807 1970-01-01 00:00:00.000000 eidolon_ai_sdk-0.1.27/PKG-INFO
+-rw-r--r--   0        0        0     2569 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/__init__.py
+-rw-r--r--   0        0        0     2400 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/agent.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/__init__.py
+-rw-r--r--   0        0        0     3025 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/document_manager.py
+-rw-r--r--   0        0        0     2710 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/document_processor.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/loaders/__init__.py
+-rw-r--r--   0        0        0      971 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py
+-rw-r--r--   0        0        0     3405 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py
+-rw-r--r--   0        0        0     4173 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/__init__.py
+-rw-r--r--   0        0        0     2817 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py
+-rw-r--r--   0        0        0     4519 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/__init__.py
+-rw-r--r--   0        0        0      448 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/base_ast_generator.py
+-rw-r--r--   0        0        0     3699 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py
+-rw-r--r--   0        0        0     2053 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py
+-rw-r--r--   0        0        0     3212 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py
+-rw-r--r--   0        0        0     1647 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py
+-rw-r--r--   0        0        0     1328 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py
+-rw-r--r--   0        0        0     3356 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py
+-rw-r--r--   0        0        0     1400 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/transformer/__init__.py
+-rw-r--r--   0        0        0     1398 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py
+-rw-r--r--   0        0        0     4786 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py
+-rw-r--r--   0        0        0    43465 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py
+-rw-r--r--   0        0        0     4825 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/generic_agent.py
+-rw-r--r--   0        0        0     1950 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/openai_whisper_agent.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/retriever_agent/__init__.py
+-rw-r--r--   0        0        0     2078 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py
+-rw-r--r--   0        0        0     1434 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py
+-rw-r--r--   0        0        0     2329 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py
+-rw-r--r--   0        0        0      559 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py
+-rw-r--r--   0        0        0     2864 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/retriever_agent/retriever.py
+-rw-r--r--   0        0        0     3717 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py
+-rw-r--r--   0        0        0    12914 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/simple_agent.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/__init__.py
+-rw-r--r--   0        0        0     1815 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/checker.py
+-rw-r--r--   0        0        0     2468 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/controller.py
+-rw-r--r--   0        0        0     1503 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/memory.py
+-rw-r--r--   0        0        0     1423 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/prompts.py
+-rw-r--r--   0        0        0      364 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/thought.py
+-rw-r--r--   0        0        0     4951 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/thought_generators.py
+-rw-r--r--   0        0        0     7614 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/tot_agent.py
+-rw-r--r--   0        0        0     4572 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent_os.py
+-rw-r--r--   0        0        0    12735 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent_os_interfaces.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/bin/__init__.py
+-rwxr-xr-x   0        0        0     9444 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/bin/agent_creator.py
+-rw-r--r--   0        0        0     7743 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/bin/agent_http_server.py
+-rwxr-xr-x   0        0        0     3789 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/bin/replay.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/__init__.py
+-rw-r--r--   0        0        0     8906 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/code_builtins.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/components/__init__.py
+-rw-r--r--   0        0        0     2223 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/components/opentelemetry.py
+-rw-r--r--   0        0        0     4256 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/components/usage.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/logic_units/__init__.py
+-rw-r--r--   0        0        0     5662 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/logic_units/web_search.py
+-rw-r--r--   0        0        0      550 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml
+-rw-r--r--   0        0        0      544 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/claude_opus.yaml
+-rw-r--r--   0        0        0      557 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml
+-rw-r--r--   0        0        0      181 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/machine.yaml
+-rw-r--r--   0        0        0      540 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/mistral_large.yaml
+-rw-r--r--   0        0        0      547 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml
+-rw-r--r--   0        0        0      540 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/mistral_small.yaml
+-rw-r--r--   0        0        0      534 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/openai_35.yaml
+-rw-r--r--   0        0        0      557 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/openai_4.yaml
+-rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/__init__.py
+-rw-r--r--   0        0        0     1843 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/agent_call_history.py
+-rw-r--r--   0        0        0     4638 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/agent_cpu.py
+-rw-r--r--   0        0        0     2562 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/agent_io.py
+-rw-r--r--   0        0        0     7916 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/agents_logic_unit.py
+-rw-r--r--   0        0        0     1641 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/audio_unit.py
+-rw-r--r--   0        0        0      292 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/call_context.py
+-rw-r--r--   0        0        0     2833 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/conversation_memory_unit.py
+-rw-r--r--   0        0        0    14320 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/conversational_apu.py
+-rw-r--r--   0        0        0     1891 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/image_unit.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm/__init__.py
+-rw-r--r--   0        0        0     9936 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py
+-rw-r--r--   0        0        0    11967 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py
+-rw-r--r--   0        0        0     4518 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py
+-rw-r--r--   0        0        0     5760 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py
+-rw-r--r--   0        0        0     9430 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py
+-rw-r--r--   0        0        0     3375 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm/open_ai_speech.py
+-rw-r--r--   0        0        0     3930 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm_message.py
+-rw-r--r--   0        0        0     2421 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm_unit.py
+-rw-r--r--   0        0        0     4199 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/logic_unit.py
+-rw-r--r--   0        0        0     3541 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/memory_unit.py
+-rw-r--r--   0        0        0      825 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/processing_unit.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/io/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/__init__.py
+-rw-r--r--   0        0        0     1193 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/agent_memory.py
+-rw-r--r--   0        0        0     5309 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/chroma_vector_store.py
+-rw-r--r--   0        0        0      641 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/document.py
+-rw-r--r--   0        0        0     2766 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/embeddings.py
+-rw-r--r--   0        0        0      907 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/file_memory.py
+-rw-r--r--   0        0        0     4203 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/file_system_vector_store.py
+-rw-r--r--   0        0        0     3974 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/in_memory_file_memory.py
+-rw-r--r--   0        0        0     5788 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/local_file_memory.py
+-rw-r--r--   0        0        0     4845 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/local_symbolic_memory.py
+-rw-r--r--   0        0        0     3793 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/mongo_symbolic_memory.py
+-rw-r--r--   0        0        0      996 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/noop_memory.py
+-rw-r--r--   0        0        0     1984 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/s3_file_memory.py
+-rw-r--r--   0        0        0      974 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/semantic_memory.py
+-rw-r--r--   0        0        0     2809 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/similarity_memory.py
+-rw-r--r--   0        0        0     1516 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/vector_store.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/__init__.py
+-rw-r--r--   0        0        0      771 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/authentication_processor.py
+-rw-r--r--   0        0        0     2159 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/azure_authorizer.py
+-rw-r--r--   0        0        0     1277 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/functional_authorizer.py
+-rw-r--r--   0        0        0     2001 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/google_auth.py
+-rw-r--r--   0        0        0     1867 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/jwt_processor.py
+-rw-r--r--   0        0        0      484 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/okta_authorizor.py
+-rw-r--r--   0        0        0     1017 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/permissions.py
+-rw-r--r--   0        0        0     2508 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/process_authorizer.py
+-rw-r--r--   0        0        0     2977 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/security_manager.py
+-rw-r--r--   0        0        0     1035 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/security_middleware.py
+-rw-r--r--   0        0        0      428 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/user.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/__init__.py
+-rw-r--r--   0        0        0     1377 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/agent_contract.py
+-rw-r--r--   0        0        0    21705 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/agent_controller.py
+-rw-r--r--   0        0        0    14099 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/agent_machine.py
+-rw-r--r--   0        0        0     1149 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/dynamic_middleware.py
+-rw-r--r--   0        0        0     3432 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/fn_handler.py
+-rw-r--r--   0        0        0     4904 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/process_file_system.py
+-rw-r--r--   0        0        0     4275 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/processes.py
+-rw-r--r--   0        0        0     6895 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/reference_model.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/resources/__init__.py
+-rw-r--r--   0        0        0      314 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/resources/agent_resource.py
+-rw-r--r--   0        0        0      414 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/resources/machine_resource.py
+-rw-r--r--   0        0        0      684 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/resources/reference_resource.py
+-rw-r--r--   0        0        0     1663 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/resources/resources_base.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/__init__.py
+-rw-r--r--   0        0        0      509 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/async_wrapper.py
+-rw-r--r--   0        0        0     2806 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/class_utils.py
+-rw-r--r--   0        0        0     1604 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/image_utils.py
+-rw-r--r--   0        0        0     3808 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/replay.py
+-rw-r--r--   0        0        0     6521 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/schema_to_model.py
+-rw-r--r--   0        0        0      898 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/str_utils.py
+-rw-r--r--   0        0        0     3445 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/stream_collector.py
+-rw-r--r--   0        0        0      565 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/logging.conf
+-rw-r--r--   0        0        0     2030 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/pyproject.toml
+-rw-r--r--   0        0        0     4807 1970-01-01 00:00:00.000000 eidolon_ai_sdk-0.1.28/PKG-INFO
```

### Comparing `eidolon_ai_sdk-0.1.27/README.md` & `eidolon_ai_sdk-0.1.28/README.md`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/agent.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/document_manager.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/document_manager.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/document_processor.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/document_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,16 @@
         elif blob.mimetype == "text/x-cobol":
             from eidolon_ai_sdk.agent.doc_manager.parsers.code_ast_parsers.programing_language_parser import (
                 LanguageParser,
             )
 
             yield from LanguageParser(LanguageParserSpec(language="cobol")).parse(blob)
         elif (
-            blob.mimetype and blob.mimetype.startswith("text/")
+            blob.mimetype
+            and blob.mimetype.startswith("text/")
             or blob.mimetype == "application/json"
             or blob.mimetype == "application/xml"
             or blob.mimetype == "application/yaml"
             or blob.mimetype == "application/x-yaml"
             or blob.mimetype == "application/x-yml"
         ):
             from eidolon_ai_sdk.agent.doc_manager.parsers.text_parsers import TextParser
```

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/generic_agent.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/generic_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/openai_whisper_agent.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/openai_whisper_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,16 +20,17 @@
     def __init__(self, spec: AutonomousSpeechAgentSpec):
         super().__init__(spec=spec)
         self.speech_llm = self.spec.speech_llm.instantiate(processing_unit_locator=None)
         self.cpu = self.spec.cpu.instantiate()
 
     @register_program()
     async def speech_to_text(
-        self, process_id, audio: Annotated[FileHandle, Body(description="The audio file", embed=True)]
+        self, audio: Annotated[FileHandle, Body(description="The audio file", embed=True)]
     ):
+        process_id = audio.process_id
         await ProcessDoc.set_delete_on_terminate(process_id, True)
         file, metadata = await AgentOS.process_file_system.read_file(process_id, audio.file_id)
         mimetype = "audio/wav"
         if metadata and "mimetype" in metadata:
             mimetype = metadata["mimetype"]
         # audio = AudioSegment.from_file(file)
         # # Convert to mp3
```

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/retriever_agent/retriever.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/retriever_agent/retriever.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,17 +28,15 @@
         Specable.__init__(self, **kwargs)
 
         self.question_transformer = (
             self.spec.question_transformer.instantiate() if self.spec.question_transformer else None
         )
         self.document_reranker = self.spec.document_reranker.instantiate()
 
-    async def search(
-            self, vector_collection_name: str, question: str
-    ) -> List[DocSummary]:
+    async def search(self, vector_collection_name: str, question: str) -> List[DocSummary]:
         """
         Process the question by searching the document store.
         :param vector_collection_name:
         :param question: The question to process
         :return: The response from the cpu
         """
         if self.question_transformer:
@@ -52,17 +50,15 @@
             rerank_questions[question] = {doc.id: doc.score for doc in docs}
 
         reranked_docs = await self.document_reranker.rerank(rerank_questions)
 
         # now limit reranked_docs to max_num_results
         reranked_docs = reranked_docs[: self.spec.max_num_results]
 
-        docs = AgentOS.similarity_memory.get_docs(
-            vector_collection_name, [doc[0] for doc in reranked_docs]
-        )
+        docs = AgentOS.similarity_memory.get_docs(vector_collection_name, [doc[0] for doc in reranked_docs])
         summaries = []
         async for doc in docs:
             file_path = doc.metadata["source"]
             summaries.append(
                 DocSummary(id=doc.id, file_name=file_path.split("/")[-1], file_path=file_path, text=doc.page_content)
             )
```

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         :return: The response from the cpu
         """
         files = [item async for item in await self.document_manager.list_files()]
         return AgentState(name="idle", data=files)
 
     @register_program(description=make_description)
     async def search(
-            self, question: Annotated[str, Body(description="The question to search for", embed=True)]
+        self, question: Annotated[str, Body(description="The question to search for", embed=True)]
     ) -> List[DocSummary]:
         """
         Process the question by searching the document store.
         :param question: The question to process
         :return: The response from the cpu
         """
         await self.document_manager.sync_docs()
```

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/simple_agent.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/simple_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,29 +37,37 @@
     @field_validator("input_schema")
     def validate_prompt_properties(cls, input_dict):
         if not isinstance(input_dict, dict):
             raise ValueError("prompt_properties must be a dict")
         for k, v in input_dict.items():
             if isinstance(v, dict):
                 if v.get("format") == "binary":
-                    raise ValueError(
-                        "prompt_properties cannot contain format = 'binary' fields."
-                    )
+                    raise ValueError("prompt_properties cannot contain format = 'binary' fields.")
         return input_dict
 
     @field_validator("supported_mime_types")
     def validate_supported_mime_types(cls, supported_mime_types):
         if not isinstance(supported_mime_types, list):
             raise ValueError("supported_mime_types must be a List[str]")
         if not supported_mime_types:
             return supported_mime_types
 
-        all_mime_types = {"application/json", "text/plain", "image/*", "audio/*", "application/pdf", "application/msword",
-                          "application/vnd.openxmlformats-officedocument.wordprocessingml.document", "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet",
-                          "application/vnd.ms-excel", "application/vnd.ms-powerpoint", "application/vnd.openxmlformats-officedocument.presentationml.presentation"}
+        all_mime_types = {
+            "application/json",
+            "text/plain",
+            "image/*",
+            "audio/*",
+            "application/pdf",
+            "application/msword",
+            "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
+            "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet",
+            "application/vnd.ms-excel",
+            "application/vnd.ms-powerpoint",
+            "application/vnd.openxmlformats-officedocument.presentationml.presentation",
+        }
         bad_types = []
         for mime_type in supported_mime_types:
             if mime_type not in all_mime_types:
                 bad_types.append(mime_type)
         if bad_types:
             raise ValueError(f"supported_mime_types contains unsupported entries: {bad_types}")
 
@@ -134,18 +142,20 @@
     def validate_cpus(self):
         if self.apus:
             self.apu = None
         return self
 
 
 class SimpleAgent(Specable[SimpleAgentSpec]):
-    generate_title_prompt = ("You are generating a title for a conversation. Consider the context and content of the discussion or text. "
-                             "Create a concise, relevant, and accurate representation of the main topic or theme in the content."
-                             "Create a title that draws insiration from key phrases or ideas in the content. "
-                             "The title should be no longer than 5 words. Do not wrap the title in quotes. Answer only with the title. The prompt for the conversation is:\n")
+    generate_title_prompt = (
+        "You are generating a title for a conversation. Consider the context and content of the discussion or text. "
+        "Create a concise, relevant, and accurate representation of the main topic or theme in the content."
+        "Create a title that draws insiration from key phrases or ideas in the content. "
+        "The title should be no longer than 5 words. Do not wrap the title in quotes. Answer only with the title. The prompt for the conversation is:\n"
+    )
 
     def __init__(self, spec):
         super().__init__(spec=spec)
         if self.spec.apu:
             self.cpu = self.spec.apu.instantiate()
             self.cpu.title = self.cpu.__class__.__name__
             self._register_refs_logic_unit(self.cpu, self.spec.agent_refs)
@@ -246,15 +256,17 @@
                     cpu = named_cpu
                     break
         else:
             cpu = self.cpu
 
         yield UserInputEvent(input=request_body, files=attached_files)
         thread = await cpu.main_thread(process_id)
-        response = thread.stream_request(output_format=action.output_schema, prompts=[*attached_files_messages, text_message])
+        response = thread.stream_request(
+            output_format=action.output_schema, prompts=[*attached_files_messages, text_message]
+        )
 
         async for event in response:
             yield event
         yield AgentStateEvent(state=action.output_state)
 
     async def _gen_title(self, action: ActionDefinition, process_id, **kwargs) -> AsyncIterable[StreamEvent]:
         last_state = RequestContext.get("__last_state__")
```

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/checker.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/checker.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/controller.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/controller.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/memory.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/prompts.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/prompts.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/thought_generators.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/thought_generators.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/tot_agent.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/tot_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent_os.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent_os.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from __future__ import annotations
 
 import os
 import pathlib
 from typing import Dict, Tuple, TypeVar, Type
 
 from eidolon_ai_client.util.logger import logger
-from eidolon_ai_sdk.agent_os_interfaces import ProcessFileSystem, FileMemory, SymbolicMemory, SecurityManager, SimilarityMemory
+from eidolon_ai_sdk.agent_os_interfaces import (
+    ProcessFileSystem,
+    FileMemory,
+    SymbolicMemory,
+    SecurityManager,
+    SimilarityMemory,
+)
 from eidolon_ai_sdk.system.resources.resources_base import load_resources, Resource
 
 T = TypeVar("T", bound="Resource")  # noqa: F821
 S = TypeVar("S", bound="BaseModel")  # noqa: F821
 
 
 class AgentOS:
@@ -50,21 +56,20 @@
         resources = cls._get_or_load_resources()
         if resource.kind not in resources:
             resources[resource.kind] = {}
         bucket = resources[resource.kind]
         if resource.metadata.name in bucket:
             if bucket[resource.metadata.name][1] == "builtin":
                 logger.info(f"Overriding builtin resource '{resource.kind}.{resource.metadata.name}'")
-
-                old_impl = getattr(bucket[resource.metadata.name][0], "spec", {}).get("implementation")
-                if old_impl:
-                    new_spec = getattr(resource, "spec")
-                    new_impl = new_spec.get("implementation") if isinstance(new_spec, dict) else new_spec
-                    if not new_impl or resource.metadata.name == new_impl:
-                        new_spec["implementation"] = old_impl
+                old_spec = getattr(bucket[resource.metadata.name][0], "spec", {})
+                old_spec = dict(implementation=old_spec) if isinstance(old_spec, str) else old_spec
+                new_spec = getattr(resource, "spec")
+                new_spec = dict(implementation=new_spec) if isinstance(new_spec, str) else new_spec
+                old_spec.update(new_spec)
+                resource.spec = old_spec
             else:
                 raise ValueError(
                     f"Resource {resource.metadata.name} already registered by {bucket[resource.metadata.name][1]}"
                 )
         logger.debug(f"Registering resource {resource.kind}.{resource.metadata.name}")
         bucket[resource.metadata.name] = (resource, source)
```

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent_os_interfaces.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent_os_interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,17 @@
         :param process_id:
         :param file_id:
         :return:
         """
         raise NotImplementedError("not implemented")
 
     @abstractmethod
-    async def write_file(self, process_id: str, file_contents: bytes, file_md: Optional[Dict[str, any]] = None) -> FileHandle:
+    async def write_file(
+        self, process_id: str, file_contents: bytes, file_md: Optional[Dict[str, any]] = None
+    ) -> FileHandle:
         """
         Writes the given `file_contents` to a new file within the context of the process_id.
         :param file_md:
         :param process_id:
         :param file_contents:
         :return:
         """
```

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/bin/agent_creator.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/bin/agent_creator.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/bin/agent_http_server.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/bin/agent_http_server.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/bin/replay.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/bin/replay.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/code_builtins.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/code_builtins.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Tuple
 
-from azure.identity import DefaultAzureCredential
+from azure.identity import DefaultAzureCredential, EnvironmentCredential
 from openai import AsyncOpenAI
 from openai.lib.azure import AsyncAzureOpenAI
 from opentelemetry.exporter.otlp.proto.grpc.trace_exporter import OTLPSpanExporter
 from opentelemetry.sdk.trace import SpanProcessor
 from opentelemetry.sdk.trace.export import BatchSpanProcessor, SpanExporter
 from opentelemetry.sdk.trace.sampling import Sampler
 
@@ -192,11 +192,12 @@
         OpenAiSpeech,
         AsyncOpenAI,
         AsyncAzureOpenAI,
         UsageClient,
         OpenAIConnectionHandler,
         AzureOpenAIConnectionHandler,
         DefaultAzureCredential,
+        EnvironmentCredential,
         # config objects
         ReplayConfig,
     ]
     return [_to_resource(maybe_tuple) for maybe_tuple in builtin_list if maybe_tuple]
```

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/components/opentelemetry.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/components/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/components/usage.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/components/usage.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/logic_units/web_search.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/logic_units/web_search.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/resources/claude_opus.yaml` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/claude_opus.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/resources/mistral_large.yaml` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/mistral_large.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/resources/mistral_small.yaml` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/mistral_small.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/resources/openai_35.yaml` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/openai_35.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/resources/openai_4.yaml` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/openai_4.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/agent_call_history.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/agent_call_history.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/agent_cpu.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/agent_cpu.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/agent_io.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/agent_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from eidolon_ai_client.events import FileHandle
 from eidolon_ai_sdk.agent_os import AgentOS
 from eidolon_ai_sdk.cpu.call_context import CallContext
 from eidolon_ai_sdk.cpu.llm_message import (
     UserMessageText,
     SystemMessage,
     UserMessage,
-    LLMMessage, UserMessageFileHandle,
+    LLMMessage,
+    UserMessageFileHandle,
 )
 from eidolon_ai_sdk.cpu.processing_unit import ProcessingUnit
 
 
 class ResponseHandler(ABC):
     @abstractmethod
     async def handle(self, process_id: str, response: Dict[str, Any]):
@@ -56,15 +57,19 @@
         user_message_parts = []
         for prompt in prompts:
             if prompt.type == "user":
                 user_message_parts.append(UserMessageText(text=prompt.prompt))
             elif prompt.type == "system":
                 conv_messages.append(SystemMessage(content=prompt.prompt))
             elif prompt.type == "file":
-                user_message_parts.append(await UserMessageFileHandle.create(file=prompt.file, process_id=call_context.process_id, include_directly=prompt.include_directly))
+                user_message_parts.append(
+                    await UserMessageFileHandle.create(
+                        file=prompt.file, process_id=call_context.process_id, include_directly=prompt.include_directly
+                    )
+                )
             else:
                 raise ValueError(f"Unknown prompt type {prompt.type}")
 
         if len(user_message_parts) > 0:
             conv_messages.append(UserMessage(content=user_message_parts))
 
         return conv_messages
```

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/agents_logic_unit.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/agents_logic_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/audio_unit.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/audio_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/conversation_memory_unit.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/conversation_memory_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/conversational_apu.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/conversational_apu.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,24 @@
 from eidolon_ai_sdk.agent.doc_manager.parsers.base_parser import DataBlob
 from eidolon_ai_sdk.agent_os import AgentOS
 from eidolon_ai_sdk.cpu.agent_cpu import APU, APUSpec, Thread, CPUException, APUCapabilities
 from eidolon_ai_sdk.cpu.agent_io import IOUnit, CPUMessageTypes
 from eidolon_ai_sdk.cpu.audio_unit import AudioUnit
 from eidolon_ai_sdk.cpu.call_context import CallContext
 from eidolon_ai_sdk.cpu.image_unit import ImageUnit
-from eidolon_ai_sdk.cpu.llm_message import AssistantMessage, ToolResponseMessage, LLMMessage, UserMessageFile, UserMessageAudio, UserMessageImage, \
-    UserMessageText, UserMessage
+from eidolon_ai_sdk.cpu.llm_message import (
+    AssistantMessage,
+    ToolResponseMessage,
+    LLMMessage,
+    UserMessageFile,
+    UserMessageAudio,
+    UserMessageImage,
+    UserMessageText,
+    UserMessage,
+)
 from eidolon_ai_sdk.cpu.llm_unit import LLMUnit
 from eidolon_ai_sdk.cpu.logic_unit import LogicUnit, LLMToolWrapper
 from eidolon_ai_sdk.cpu.memory_unit import MemoryUnit
 from eidolon_ai_sdk.cpu.processing_unit import ProcessingUnitLocator, PU_T
 from eidolon_ai_sdk.system.reference_model import Reference, AnnotatedReference, Specable
 from eidolon_ai_sdk.util.stream_collector import StreamCollector, stream_manager, ManagedContextError
 
@@ -151,15 +159,17 @@
         num_iterations = 0
         while num_iterations < self.spec.max_num_function_calls:
             with tracer.start_as_current_span("building tools"):
                 tool_defs = await LLMToolWrapper.from_logic_units(call_context, self.logic_units)
                 tool_call_events = []
                 llm_facing_tools = [w.llm_message for w in tool_defs.values()]
             with tracer.start_as_current_span("llm execution"):
-                execute_llm_ = self.llm_unit.execute_llm(call_context, converted_conversation, llm_facing_tools, output_format)
+                execute_llm_ = self.llm_unit.execute_llm(
+                    call_context, converted_conversation, llm_facing_tools, output_format
+                )
                 # yield the events but capture the output, so it can be rolled into one event for memory.
                 stream_collector = StreamCollector(execute_llm_)
                 async for event in stream_collector:
                     if event.is_root_and_type(LLMToolCallRequestEvent):
                         tool_call_events.append(event)
                     yield event
             if stream_collector.get_content():
@@ -172,15 +182,17 @@
             )
             if self.record_memory:
                 await self.memory_unit.storeMessages(call_context, [assistant_message])
             converted_conversation.append(assistant_message)
 
             if tool_call_events:
                 with tracer.start_as_current_span("tool calls"):
-                    streams = [self._call_tool(call_context, tce, tool_defs, converted_conversation) for tce in tool_call_events]
+                    streams = [
+                        self._call_tool(call_context, tce, tool_defs, converted_conversation) for tce in tool_call_events
+                    ]
                     async for e in merge_streams(streams):
                         yield e
             else:
                 return
 
         raise CPUException(f"exceeded maximum number of function calls ({self.spec.max_num_function_calls})")
 
@@ -241,18 +253,25 @@
         text = await self.audio_unit.speech_to_text(audio=audio_data, mime_type=mimetype)
         return [UserMessageText(text=f"The following text as converted from the audio file {path}:\n{text}\n\n")]
 
     async def process_image_message(self, call_context: CallContext, message: UserMessageImage):
         if self.get_capabilities().supports_image_input:
             return [message]
         elif self.image_unit is not None:
-            image_data, metadata = await AgentOS.process_file_system.read_file(call_context.process_id, message.file.file_id)
+            image_data, metadata = await AgentOS.process_file_system.read_file(
+                call_context.process_id, message.file.file_id
+            )
             path = metadata.get("path") or metadata.get("filename") or ""
-            text = await self.image_unit.image_to_text(prompt="Create a detailed text description of the following image. Be sure to include as much information as needed to describe the image.  Be very verbose.", image=image_data)
-            return [UserMessageText(text=f"The following text is a detailed description of an image {path}:\n{text}\n\n")]
+            text = await self.image_unit.image_to_text(
+                prompt="Create a detailed text description of the following image. Be sure to include as much information as needed to describe the image.  Be very verbose.",
+                image=image_data,
+            )
+            return [
+                UserMessageText(text=f"The following text is a detailed description of an image {path}:\n{text}\n\n")
+            ]
         else:
             raise ValueError("Image processing not supported")
 
     async def process_file_message(self, process_id: str, message: UserMessageFile):
         parts = []
         if message.include_directly:
             data, metadata = await AgentOS.process_file_system.read_file(process_id, message.file.file_id)
@@ -264,15 +283,17 @@
 
             parts.append(UserMessageText(text=message))
         else:
             data, metadata = await AgentOS.process_file_system.read_file(process_id, message.file.file_id)
             path = metadata.get("path") or metadata.get("filename") or None
             mimetype = metadata.get("mimetype")
             blob = DataBlob.from_bytes(data=data, mimetype=mimetype, path=path)
-            await self.document_processor.addFile(f"pf_pid_{process_id}", FileInfo(data=blob, path="", metadata=metadata))
+            await self.document_processor.addFile(
+                f"pf_pid_{process_id}", FileInfo(data=blob, path="", metadata=metadata)
+            )
             message = f"The file {path} is available to search. Use the provided search tool to find information contained in the file\n"
             parts.append(UserMessageText(text=message))
 
         return parts
 
     async def clone_thread(self, call_context: CallContext) -> Thread:
         new_context = call_context.derive_call_context()
```

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/image_unit.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/image_unit.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,16 +37,23 @@
         Returns:
             str: The text.
             :param image:
             :param prompt:
         """
         raise NotImplementedError("image_to_text not implemented")
 
-    async def text_to_image(self, call_context: CallContext, text: str, quality: Optional[str] = None, size: Tuple[int, int] = (1024, 1024), style: Optional[str] = None,
-                            image_format: Literal["jpeg", "png", "tiff", "bmp", "webp"] = "webp") -> List[FileHandle]:
+    async def text_to_image(
+        self,
+        call_context: CallContext,
+        text: str,
+        quality: Optional[str] = None,
+        size: Tuple[int, int] = (1024, 1024),
+        style: Optional[str] = None,
+        image_format: Literal["jpeg", "png", "tiff", "bmp", "webp"] = "webp",
+    ) -> List[FileHandle]:
         """
         Converts text to an image.
 
         Args:
             text (str): The text.
 
         Returns:
```

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,46 +141,42 @@
         super().__init__(**kwargs)
         LLMUnit.__init__(self, **kwargs)
         Specable.__init__(self, **kwargs)
 
         self.temperature = self.spec.temperature
 
     async def execute_llm(
-            self,
-            call_context: CallContext,
-            messages: List[LLMMessage],
-            tools: List[LLMCallFunction],
-            output_format: Union[Literal["str"], Dict[str, Any]],
+        self,
+        call_context: CallContext,
+        messages: List[LLMMessage],
+        tools: List[LLMCallFunction],
+        output_format: Union[Literal["str"], Dict[str, Any]],
     ) -> AsyncIterator[AssistantMessage]:
         if len(tools) > 0:
             logger.warn("Anthropic does not support tool calls, ignoring")
         can_stream_message, request = await self._build_request(messages, tools, output_format)
 
         logger.info("executing open ai llm request", extra=request)
         if logger.isEnabledFor(logging.DEBUG):
             logger.debug("request content:\n" + yaml.dump(request))
-        llm_request = replayable(
-            fn=_llm_request(), name_override="anthropic_completion", parser=_raw_parser
-        )
+        llm_request = replayable(fn=_llm_request(), name_override="anthropic_completion", parser=_raw_parser)
         complete_message = ""
         try:
             async for message in llm_request(client_args=self.spec.client_args, **request):
                 # todo -- handle tool calls in some weird way...
                 if can_stream_message:
-                    logger.debug(
-                        f"anthropic llm stream response: {message}", extra=dict(content=message)
-                    )
+                    logger.debug(f"anthropic llm stream response: {message}", extra=dict(content=message))
                     yield StringOutputEvent(content=message)
                 else:
                     complete_message += message
 
             if not can_stream_message:
                 logger.debug(f"anthropic llm object response: {complete_message}", extra=dict(content=complete_message))
                 # message format looks like json```{...}```, parse content and pull out the json
-                complete_message = complete_message[complete_message.find("{"): complete_message.rfind("}") + 1]
+                complete_message = complete_message[complete_message.find("{") : complete_message.rfind("}") + 1]
 
                 content = json.loads(complete_message) if complete_message else {}
                 yield ObjectOutputEvent(content=content)
         except APIConnectionError as e:
             raise HTTPException(502, f"Anthropic Error: {e.message}") from e
         except RateLimitError as e:
             raise HTTPException(429, "Anthropic Rate Limit Exceeded") from e
```

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,28 +129,26 @@
 class MistralGPT(LLMUnit, Specable[MistralGPTSpec]):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         LLMUnit.__init__(self, **kwargs)
         Specable.__init__(self, **kwargs)
 
     async def execute_llm(
-            self,
-            call_context: CallContext,
-            messages: List[LLMMessage],
-            tools: List[LLMCallFunction],
-            output_format: Union[Literal["str"], Dict[str, Any]],
+        self,
+        call_context: CallContext,
+        messages: List[LLMMessage],
+        tools: List[LLMCallFunction],
+        output_format: Union[Literal["str"], Dict[str, Any]],
     ) -> AsyncIterator[AssistantMessage]:
         can_stream_message, request = await self._build_request(messages, tools, output_format)
 
         logger.info("executing mistral llm request", extra=request)
         if logger.isEnabledFor(logging.DEBUG):
             logger.debug("request content:\n" + yaml.dump(request))
-        llm_request = replayable(
-            fn=_mistral_client(), name_override="mistral_completion", parser=_raw_parser
-        )
+        llm_request = replayable(fn=_mistral_client(), name_override="mistral_completion", parser=_raw_parser)
         complete_message = ""
         tools_to_call = []
         try:
             async for m_chunk in llm_request(client_args=self.spec.client_args, **request):
                 chunk = cast(ChatCompletionStreamResponse, m_chunk)
                 if not chunk.choices:
                     logger.info("open ai llm chunk has no choices, skipping")
@@ -188,15 +186,15 @@
                 for tool in tools_to_call:
                     tool_call = _convert_tool_call(tool)
                     yield LLMToolCallRequestEvent(tool_call=tool_call)
             if not can_stream_message:
                 logger.debug(f"open ai llm object response: {complete_message}", extra=dict(content=complete_message))
                 if not self.spec.force_json:
                     # message format looks like json```{...}```, parse content and pull out the json
-                    complete_message = complete_message[complete_message.find("{"): complete_message.rfind("}") + 1]
+                    complete_message = complete_message[complete_message.find("{") : complete_message.rfind("}") + 1]
 
                 content = json.loads(complete_message) if complete_message else {}
                 yield ObjectOutputEvent(content=content)
         except MistralConnectionException as e:
             raise HTTPException(429, f"Mistral Connection Error: {e.message}") from e
         except MistralAPIStatusException as e:
             raise HTTPException(502, f"Mistral Status Error: {e.message}") from e
@@ -237,20 +235,23 @@
 
     async def _build_tools(self, inTools):
         tools = []
         for tool in inTools:
             tools.append(
                 {
                     "type": "function",
-                    "function": Function(**{
-                        "name": tool.name,
-                        "description": tool.description,
-                        "parameters": tool.parameters,
-                    }).model_dump()
-                })
+                    "function": Function(
+                        **{
+                            "name": tool.name,
+                            "description": tool.description,
+                            "parameters": tool.parameters,
+                        }
+                    ).model_dump(),
+                }
+            )
         return tools
 
 
 def _convert_tool_call(tool: Dict[str, any]) -> ToolCall:
     name = tool["name"]
     try:
         loads = json.loads(tool["arguments"])
```

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,130 +1,108 @@
+import os
 from typing import Optional, cast, List
 
-from azure.identity import DefaultAzureCredential, get_bearer_token_provider
-from fastapi import HTTPException
-from openai import AsyncOpenAI, AsyncStream, APIConnectionError, RateLimitError, APIStatusError
+from azure.identity import get_bearer_token_provider, EnvironmentCredential
+from openai import AsyncOpenAI, AsyncStream
 from openai.lib.azure import AsyncAzureOpenAI
 from openai.types import ImagesResponse
 from openai.types.chat import ChatCompletionChunk, ChatCompletion
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 
 from eidolon_ai_sdk.system.reference_model import Specable, Reference
 from eidolon_ai_sdk.util.replay import replayable
 
 
-class OpenAIConnectionHandlerSpec(BaseModel, extra='allow'):
+class OpenAIConnectionHandlerSpec(BaseModel, extra="allow"):
     pass
 
 
 class OpenAIConnectionHandler(Specable[OpenAIConnectionHandlerSpec]):
     def makeClient(self) -> AsyncOpenAI:
         return AsyncOpenAI(**self.spec.model_extra)
 
-    async def completion(self, kwargs: dict) -> ChatCompletion | AsyncStream[ChatCompletionChunk]:
-        return await self._do_request(self.makeClient().chat.completions.create, kwargs)
-
-    async def generate_image(self, kwargs: dict) -> ImagesResponse:
-        return await self._do_request(self.makeClient().images.generate, kwargs)
-
-    async def _do_request(self, open_ai_fn, kwargs: dict):
-        async def _send_request():
-            try:
-                async for e in await self.makeClient().chat.completions.create(**kwargs):
-                    yield e
-            except APIConnectionError as e:
-                raise HTTPException(502, f"OpenAI Error: {e.message}") from e
-            except RateLimitError as e:
-                raise HTTPException(429, "OpenAI Rate Limit Exceeded") from e
-            except APIStatusError as e:
-                raise HTTPException(502, f"OpenAI Status Error: {e.message}") from e
-
-        async def _send_request_no_gen() -> ChatCompletion:
-            return await open_ai_fn(**kwargs)
-
-        if kwargs.get("stream"):
-            print("here")
-            llm_request = replayable(
-                fn=_send_request, name_override="openai_completion", parser=_open_ai_replay_parser
-            )
-
-            return llm_request()
-        else:
-            llm_request = replayable(
-                fn=_send_request_no_gen, name_override="openai_completion", parser=_open_ai_replay_parser_no_stream
-            )
-            return await llm_request()
+    async def completion(self, **kwargs) -> ChatCompletion | AsyncStream[ChatCompletionChunk]:
+        return await replayable(
+            fn=lambda **_kwargs: self.makeClient().chat.completions.create(**_kwargs),
+            parser=_replay_parser,
+            name_override="openai_completion",
+        )(**kwargs)
+
+    async def generate_image(self, **kwargs) -> ImagesResponse:
+        # todo, image generation should be repayable, but needs custom parser
+        return await self.makeClient().images.generate(**kwargs)
+
+
+def get_default_token_provider():
+    if os.environ.get("AZURE_CLIENT_ID") and os.environ.get("AZURE_CLIENT_SECRET") and os.environ.get("AZURE_TENANT_ID"):
+        return Reference[EnvironmentCredential]()
+    return None
 
 
 class AzureOpenAIConnectionHandlerSpec(OpenAIConnectionHandlerSpec):
     """
     Automatically infers the values from environment variables for:
         - `api_key` from `AZURE_OPENAI_API_KEY` (IFF `api_key` AND 'azure_ad_token_provider' is not provided)
         - `organization` from `OPENAI_ORG_ID`
         - `azure_ad_token` from `AZURE_OPENAI_AD_TOKEN`
         - `api_version` from `OPENAI_API_VERSION`
         - `azure_endpoint` from `AZURE_OPENAI_ENDPOINT`
-        """
-    token_provider: Optional[Reference[DefaultAzureCredential]] = None
+    """
+
+    azure_ad_token_provider: Optional[Reference] = Field(default_factory=get_default_token_provider)
     token_provider_scopes: List[str] = ["https://cognitiveservices.azure.com/.default"]
+    api_version: str = os.environ.get("OPENAI_API_VERSION") or "2024-02-01"
 
 
 class AzureOpenAIConnectionHandler(OpenAIConnectionHandler, Specable[AzureOpenAIConnectionHandlerSpec]):
     def makeClient(self):
         params = self.spec.model_extra
-        if self.spec.token_provider:
-            provider = self.spec.token_provider.instantiate()
+        if self.spec.azure_ad_token_provider:
+            provider = self.spec.azure_ad_token_provider.instantiate()
             token_provider = get_bearer_token_provider(provider, *self.spec.token_provider_scopes)
-            params["token_provider"] = token_provider
+            params["azure_ad_token_provider"] = token_provider
+        params["api_version"] = self.spec.api_version
         return AsyncAzureOpenAI(**params)
 
 
-async def _open_ai_replay_parser(resp):
+async def _replay_parser(resp):
     """
     Parses responses from openai and yield strings to accumulate to a human-readable message.
 
     Makes assumptions around tool calls. These are currently true, but may change as openai mutates their API
     1. Tool call functions names are always in a complete message
     2. Tool calls are ordered (No chunk for tool #2 until #1 is complete)
     """
     calling_tools = False
     prefix = ""
-    async for m_chunk in resp:
-        chunk = cast(ChatCompletionChunk, m_chunk)
-        if not chunk.choices:
-            continue
-        message = chunk.choices[0].delta
-
+    await_resp = await resp
+    if hasattr(await_resp, "__aiter__"):
+        async for m_chunk in await_resp:
+            chunk = cast(ChatCompletionChunk, m_chunk)
+            if not chunk.choices:
+                continue
+            message = chunk.choices[0].delta
+
+            if message.tool_calls:
+                calling_tools = True
+                for i, tool_call in enumerate(message.tool_calls):
+                    if tool_call.function.name:
+                        yield prefix + f"Tool Call: {tool_call.function.name}\nArguments: "
+                        prefix = "\n"
+                    if tool_call.function.arguments:
+                        yield tool_call.function.arguments
+            elif calling_tools:
+                yield "\n"
+            if message.content:
+                yield message.content
+                prefix = "\n"
+    else:
+        message = await_resp.choices[0].message
         if message.tool_calls:
-            calling_tools = True
             for i, tool_call in enumerate(message.tool_calls):
                 if tool_call.function.name:
-                    yield prefix + f"Tool Call: {tool_call.function.name}\nArguments: "
-                    prefix = "\n"
+                    yield f"Tool Call: {tool_call.function.name}\nArguments: "
                 if tool_call.function.arguments:
                     yield tool_call.function.arguments
-        elif calling_tools:
-            yield "\n"
+                yield "\n"
         if message.content:
             yield message.content
-            prefix = "\n"
-
-
-async def _open_ai_replay_parser_no_stream(resp: ChatCompletion):
-    """
-    Parses responses from openai and yield strings to accumulate to a human-readable message.
-
-    Makes assumptions around tool calls. These are currently true, but may change as openai mutates their API
-    1. Tool call functions names are always in a complete message
-    2. Tool calls are ordered (No chunk for tool #2 until #1 is complete)
-    """
-    message = resp.choices[0].message
-
-    if message.tool_calls:
-        for i, tool_call in enumerate(message.tool_calls):
-            if tool_call.function.name:
-                yield f"Tool Call: {tool_call.function.name}\nArguments: "
-            if tool_call.function.arguments:
-                yield tool_call.function.arguments
-            yield "\n"
-    if message.content:
-        yield message.content
```

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,33 +19,38 @@
 
 
 class OpenAIImageUnitSpec(ImageUnitSpec):
     connection_handler: AnnotatedReference[OpenAIConnectionHandler]
     image_to_text_model: str = Field(default="gpt-4-vision-preview", description="The model to use for the vision LLM.")
     text_to_image_model: str = Field(default="dall-e-3", description="The model to use for the vision LLM.")
     temperature: float = 0.3
-    image_to_text_system_prompt: str = Field("You are an expert at answering questions about images. "
-                                             "You are presented with an image and a question and must answer the question based on the information in the image.",
-                                             description="The system prompt to use for text to image.")
+    image_to_text_system_prompt: str = Field(
+        "You are an expert at answering questions about images. "
+        "You are presented with an image and a question and must answer the question based on the information in the image.",
+        description="The system prompt to use for text to image.",
+    )
 
 
 class OpenAIImageUnit(ImageUnit, Specable[OpenAIImageUnitSpec]):
     connection_handler: OpenAIConnectionHandler
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         Specable.__init__(self, **kwargs)
         self.connection_handler = self.spec.connection_handler.instantiate()
 
     def get_capabilities(self) -> ImageCreationCapabilities:
         return ImageCreationCapabilities(
             qualities=["standard", "hd"],
             sizes=[(1024, 1024), (1792, 1024), (1024, 1792)],
-            styles=["vivid", "natural", ],
-            max_prompt_size=4000
+            styles=[
+                "vivid",
+                "natural",
+            ],
+            max_prompt_size=4000,
         )
 
     async def image_to_text(self, prompt: str, image: bytes) -> str:
         """
         Converts an image to text.
 
         Args:
@@ -58,34 +63,44 @@
         """
         # scale the image such that the max size of the shortest size is at most 768px
         data = scale_image(image)
         # base64 encode the data
         base64_image = base64.b64encode(data).decode("utf-8")
         messages = [
             {"role": "system", "content": self.spec.image_to_text_system_prompt},
-            {"role": "user", "content": [
-                {"type": "text", "text": prompt},
-                {
-                    "type": "image_url",
-                    "image_url": {"url": f"data:image/jpeg;base64,{base64_image}"},
-                },
-            ]},
+            {
+                "role": "user",
+                "content": [
+                    {"type": "text", "text": prompt},
+                    {
+                        "type": "image_url",
+                        "image_url": {"url": f"data:image/jpeg;base64,{base64_image}"},
+                    },
+                ],
+            },
         ]
         request = {
             "messages": messages,
             "model": self.spec.image_to_text_model,
             "temperature": self.spec.temperature,
         }
 
-        result: ChatCompletion = await self.connection_handler.completion(request)
+        result: ChatCompletion = await self.connection_handler.completion(**request)
         print(result)
         return result.choices[0].message.content
 
-    async def text_to_image(self, call_context: CallContext, text: str, quality: Optional[str] = None, size: Tuple[int, int] = (1024, 1024), style: Optional[str] = None,
-                            image_format: Literal["jpeg", "png", "tiff", "bmp", "webp"] = "webp") -> List[FileHandle]:
+    async def text_to_image(
+        self,
+        call_context: CallContext,
+        text: str,
+        quality: Optional[str] = None,
+        size: Tuple[int, int] = (1024, 1024),
+        style: Optional[str] = None,
+        image_format: Literal["jpeg", "png", "tiff", "bmp", "webp"] = "webp",
+    ) -> List[FileHandle]:
         """
         Converts text to an image.
 
         Args:
             text (str): The text.
 
         Returns:
@@ -107,32 +122,37 @@
             "prompt": text,
             "model": self.spec.text_to_image_model,
             "response_format": "b64_json",
             "quality": quality,
             "size": f"{size_to_request[0]}x{size_to_request[1]}",
             "style": style,
         }
-        result = await self.connection_handler.generate_image(request)
+        result = await self.connection_handler.generate_image(**request)
         file_handles = []
         for i in result.data:
             image_data = base64.b64decode(i.b64_json)
             image = Image.open(BytesIO(image_data))
             image_fp = BytesIO()
             image.resize(size)
             image.save(image_fp, format=image_format)
-            file_handles.append(await AgentOS.process_file_system.write_file(call_context.process_id, image_fp.getvalue(),
-                                                                             file_md={"prompt_rewrite": i.revised_prompt, "mimetype": f"image/{image_format}"}))
+            file_handles.append(
+                await AgentOS.process_file_system.write_file(
+                    call_context.process_id,
+                    image_fp.getvalue(),
+                    file_md={"prompt_rewrite": i.revised_prompt, "mimetype": f"image/{image_format}"},
+                )
+            )
 
         return file_handles
 
     def _choose_optimal_size(self, size: Tuple[int, int], sizes: List[Tuple[int, int]]) -> Tuple[int, int]:
         desired_width, desired_height = size
         aspect_ratio = desired_width / desired_height
 
-        min_diff = float('inf')
+        min_diff = float("inf")
         optimal_size = None
 
         for width, height in sizes:
             current_aspect_ratio = width / height
             diff = abs(aspect_ratio - current_aspect_ratio)
 
             if diff < min_diff:
```

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 from eidolon_ai_sdk.cpu.call_context import CallContext
 from eidolon_ai_sdk.cpu.llm.open_ai_connection_handler import OpenAIConnectionHandler
 from eidolon_ai_sdk.cpu.llm_message import (
     LLMMessage,
     AssistantMessage,
     ToolResponseMessage,
     UserMessage,
-    SystemMessage, UserMessageText, UserMessageImage,
+    SystemMessage,
+    UserMessageText,
+    UserMessageImage,
 )
 from eidolon_ai_sdk.cpu.llm_unit import LLMUnit, LLMCallFunction, LLMModel, LLMUnitSpec
 from eidolon_ai_sdk.system.reference_model import Specable, AnnotatedReference
 from eidolon_ai_sdk.util.image_utils import scale_image
 
 logger = eidolon_logger.getChild("llm_unit")
 
@@ -101,30 +103,30 @@
     def __init__(self, **kwargs):
         LLMUnit.__init__(self, **kwargs)
         Specable.__init__(self, **kwargs)
         self.temperature = self.spec.temperature
         self.connection_handler = self.spec.connection_handler.instantiate()
 
     async def execute_llm(
-            self,
-            call_context: CallContext,
-            messages: List[LLMMessage],
-            tools: List[LLMCallFunction],
-            output_format: Union[Literal["str"], Dict[str, Any]],
+        self,
+        call_context: CallContext,
+        messages: List[LLMMessage],
+        tools: List[LLMCallFunction],
+        output_format: Union[Literal["str"], Dict[str, Any]],
     ) -> AsyncIterator[AssistantMessage]:
         can_stream_message, request = await self._build_request(call_context, messages, tools, output_format)
         request["stream"] = True
 
         logger.info("executing open ai llm request", extra=request)
         if logger.isEnabledFor(logging.DEBUG):
             logger.debug("request content:\n" + yaml.dump(request))
 
         complete_message = ""
         tools_to_call = []
-        completion = cast(AsyncStream[ChatCompletionChunk], await self.connection_handler.completion(request))
+        completion = cast(AsyncStream[ChatCompletionChunk], await self.connection_handler.completion(**request))
         async for m_chunk in completion:
             chunk = cast(ChatCompletionChunk, m_chunk)
             if not chunk.choices:
                 logger.info("open ai llm chunk has no choices, skipping")
                 continue
             message = chunk.choices[0].delta
 
@@ -143,31 +145,29 @@
                     if tool_call.function.name:
                         tools_to_call[index]["name"] = tool_call.function.name
                     if tool_call.function.arguments:
                         tools_to_call[index]["arguments"] += tool_call.function.arguments
 
             if message.content:
                 if can_stream_message:
-                    logger.debug(
-                        f"open ai llm stream response: {message.content}", extra=dict(content=message.content)
-                    )
+                    logger.debug(f"open ai llm stream response: {message.content}", extra=dict(content=message.content))
                     yield StringOutputEvent(content=message.content)
                 else:
                     complete_message += message.content
 
         logger.info(f"open ai llm tool calls: {json.dumps(tools_to_call)}", extra=dict(tool_calls=tools_to_call))
         if len(tools_to_call) > 0:
             for tool in tools_to_call:
                 tool_call = _convert_tool_call(tool)
                 yield LLMToolCallRequestEvent(tool_call=tool_call)
         if not can_stream_message:
             logger.debug(f"open ai llm object response: {complete_message}", extra=dict(content=complete_message))
             if not self.spec.force_json:
                 # message format looks like json```{...}```, parse content and pull out the json
-                complete_message = complete_message[complete_message.find("{"): complete_message.rfind("}") + 1]
+                complete_message = complete_message[complete_message.find("{") : complete_message.rfind("}") + 1]
 
             content = json.loads(complete_message) if complete_message else {}
             yield ObjectOutputEvent(content=content)
 
     async def _build_request(self, call_context: CallContext, inMessages, inTools, output_format):
         tools = await self._build_tools(inTools)
         messages = [await convert_to_openai(message, call_context.process_id) for message in inMessages]
```

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm/open_ai_speech.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm/open_ai_speech.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm_message.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm_message.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm_unit.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/logic_unit.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/logic_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/memory_unit.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/memory_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/processing_unit.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/processing_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/agent_memory.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/agent_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/chroma_vector_store.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/chroma_vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/document.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/document.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/embeddings.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/file_memory.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/file_system_vector_store.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/file_system_vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/in_memory_file_memory.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/in_memory_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/local_file_memory.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/local_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/local_symbolic_memory.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/local_symbolic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/mongo_symbolic_memory.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/mongo_symbolic_memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,20 @@
 
 from eidolon_ai_sdk.memory.semantic_memory import SymbolicMemoryBase
 from eidolon_ai_sdk.system.reference_model import Specable
 
 
 class MongoSymbolicMemoryConfig(BaseModel):
     mongo_connection_string: str = Field(
-        default=os.environ.get("MONGO_CONNECTION_STR", "mongodb://localhost:27017/?directConnection=true"), description="The connection string to the MongoDB instance."
+        default=os.environ.get("MONGO_CONNECTION_STR", "mongodb://localhost:27017/?directConnection=true"),
+        description="The connection string to the MongoDB instance.",
+    )
+    mongo_database_name: str = Field(
+        default=os.environ.get("MONGO_DATABASE_NAME", "eidolon"), description="The name of the MongoDB database to use."
     )
-    mongo_database_name: str = Field(default=os.environ.get("MONGO_DATABASE_NAME", "eidolon"), description="The name of the MongoDB database to use.")
 
 
 class MongoSymbolicMemory(SymbolicMemoryBase, Specable[MongoSymbolicMemoryConfig]):
     mongo_connection_string: Optional[str]
     mongo_database_name: str
     _database: Optional[ContextVar]
```

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/noop_memory.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/noop_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/s3_file_memory.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/s3_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/semantic_memory.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/semantic_memory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from eidolon_ai_sdk.agent_os_interfaces import SymbolicMemory
 
 
 class SymbolicMemoryBase(SymbolicMemory):
     """
     Abstract base class for a symbolic memory component within an agent.
```

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/similarity_memory.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/similarity_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/vector_store.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/authentication_processor.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/authentication_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/azure_authorizer.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/jwt_processor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,57 @@
-import os
+from abc import ABC, abstractmethod
 from typing import List, Optional, Any
 
-import httpx
-from jose import jwt
-from pydantic import BaseModel, Field
+from authlib.jose import jwt
+from fastapi import Request, FastAPI, HTTPException
 
-from eidolon_ai_sdk.security.jwt_processor import BaseJWTProcessor
+# noinspection PyPackageRequirements
+from pydantic import BaseModel
+
+from eidolon_ai_client.util.request_context import RequestContext
+from eidolon_ai_sdk.security.authentication_processor import AuthenticationProcessor
+from eidolon_ai_sdk.security.user import User
 from eidolon_ai_sdk.system.reference_model import Specable
 
 
-class AzureJWTProcessorSpec(BaseModel):
-    client_id: str = Field(
-        os.environ.get("AZURE_AD_CLIENT_ID"),
-        description="Your azure client or application ID. Defaults to the environment variable AZURE_AD_CLIENT_ID",
-    )
-    tenant_id: str = Field(
-        default=os.environ.get("AZURE_AD_TENANT_ID"),
-        description="The tenant id of the JWT. Defaults to the environment variable AZURE_AD_TENANT_ID",
-    )
-    issuer_prefix: str = Field(
-        default="https://sts.windows.net",
-        description="The issuer prefix of the JWT. Defaults to sts.windows.net.  The tenant id will be appended to this value.  For example, sts.windows.net/your_tenant_id",
-    )
+class BaseJWTProcessorSpec(BaseModel):
+    pass
 
 
-class AzureJWTProcessor(BaseJWTProcessor, Specable[AzureJWTProcessorSpec]):
+class BaseJWTProcessor(AuthenticationProcessor, ABC, Specable[BaseJWTProcessorSpec]):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.signing_keys = None
-        self.jwks_url = (
-            f"https://login.microsoftonline.com/{self.spec.tenant_id}/discovery/keys?appid={self.spec.client_id}"
-        )
 
+    async def start(self, app: FastAPI):
+        pass
+
+    @abstractmethod
     async def get_signing_keys(self):
-        if not self.signing_keys:
-            async with httpx.AsyncClient() as client:
-                resp = await client.get(self.jwks_url)
-                self.signing_keys = resp.json()["keys"]
-        return self.signing_keys
+        pass
 
-    async def get_audience_and_issuer(self):
-        return self.spec.client_id, self.spec.issuer_prefix + "/" + self.spec.tenant_id + "/"
+    @abstractmethod
+    async def get_audience_and_issuer(self) -> tuple[str, str]:
+        pass
 
+    @abstractmethod
     def get_algorithms(self) -> List[str]:
-        return ["RS256"]
+        pass
 
     async def process_token(self, token: str) -> Optional[Any]:
         jwks = await self.get_signing_keys()
-        audience, issuer = await self.get_audience_and_issuer()
-        token = jwt.decode(
-            token=token, key=jwks, algorithms=self.get_algorithms(), audience=self.spec.client_id, issuer=issuer
-        )
-        return token
+        return jwt.decode(token, jwks)
+
+    async def check_auth(self, request: Request):
+        auth_header = request.headers.get("Authorization")
+        if not auth_header:
+            raise HTTPException(status_code=401, detail="Authorization header missing")
+
+        token = auth_header[7:]
+
+        try:
+            user_info = await self.process_token(token)
+        except Exception as e:
+            raise HTTPException(status_code=401, detail=str(e)) from e
+        RequestContext.set("Authorization", auth_header, propagate=True)
+        RequestContext.set("jwt", user_info)
+        perms = [p for r in user_info.get("roles", []) for p in r.split(",")]
+        return User(id=user_info["oid"], name=user_info.get("name"), extra={"permissions": perms})
```

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/functional_authorizer.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/functional_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/google_auth.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/google_auth.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/permissions.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/permissions.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/process_authorizer.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/process_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/security_manager.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/security_manager.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/security_middleware.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/security_middleware.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/agent_contract.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/agent_contract.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/agent_controller.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/agent_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,19 @@
             raise HTTPException(
                 status_code=409,
                 detail=f'Action "{handler.name}" cannot process state "{process.state}"',
             )
         last_state = process.state
         RequestContext.set("__last_state__", last_state)
         process = await process.update(
-            check_update_time=True, agent=self.name, record_id=process_id, state="processing", data=dict(action=handler.name)
+            check_update_time=True,
+            agent=self.name,
+            record_id=process_id,
+            state="processing",
+            data=dict(action=handler.name),
         )
         parameters = inspect.signature(handler.fn).parameters
         if "process_id" in parameters:
             kwargs["process_id"] = process_id
         if "request" in parameters and parameters["request"].annotation == Request:
             kwargs["request"] = request
 
@@ -284,17 +288,15 @@
             await store_events(self.name, process.record_id, events_to_store)
             # get the latest state and if terminated, delete the process
             latest_record = await self.get_latest_process_event(process.record_id)
             if latest_record.delete_on_terminate and latest_record.state == "terminated":
                 await self._delete_process(process.record_id)
 
     async def stream_agent_iterator(
-        self,
-        stream: AsyncIterator[StreamEvent],
-        process: ProcessDoc
+        self, stream: AsyncIterator[StreamEvent], process: ProcessDoc
     ) -> AsyncIterator[StreamEvent]:
         state_change = None
         seen_end = False
         try:
             async for event in stream:
                 if event.is_root_and_type(ErrorEvent):
                     logger.warning("Error event received")
```

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/agent_machine.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/agent_machine.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,28 +173,24 @@
         :param file_bytes:
         :return: The file id that was written
         """
         file_md = None
         if mime_type:
             file_md = {"mime_type": mime_type}
         file_id = await self.process_file_system.write_file(process_id, file_bytes, file_md)
-        return JSONResponse(
-            content=file_id.model_dump(), status_code=200
-        )
+        return JSONResponse(content=file_id.model_dump(), status_code=200)
 
     async def set_metadata(self, process_id: str, file_id: str, file_md: dict):
         """
         Set metadata for a file
         :param file_id:
         :param process_id:
         """
         file_id = await self.process_file_system.set_metadata(process_id, file_id, file_md)
-        return JSONResponse(
-            content=file_id.model_dump(), status_code=200
-        )
+        return JSONResponse(content=file_id.model_dump(), status_code=200)
 
     async def download_file(self, process_id: str, file_id: str):
         """
         Download a file for this process
         :param process_id:
         :param file_id:
         :return: The file bytes
```

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/dynamic_middleware.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/dynamic_middleware.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/fn_handler.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/fn_handler.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/process_file_system.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/process_file_system.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,34 +47,35 @@
         if not exists:
             return None
         file_md = None
         if await AgentOS.file_memory.exists(path + ".md"):
             file_md = json.loads((await AgentOS.file_memory.read_file(path + ".md")).decode())
         return await AgentOS.file_memory.read_file(path), file_md
 
-    async def write_file(self, process_id: str, file_contents: bytes, file_md: Optional[Dict[str, any]] = None) -> FileHandle:
+    async def write_file(
+        self, process_id: str, file_contents: bytes, file_md: Optional[Dict[str, any]] = None
+    ) -> FileHandle:
         """
         Writes the given `file_contents` to a new file within the context of the process_id.
         :param file_md:
         :param process_id:
         :param file_contents:
         :return:
         """
         file_id = uuid4().hex
         await AgentOS.file_memory.mkdir(str(Path(self.root, process_id)), exist_ok=True)
         await AgentOS.file_memory.write_file(str(Path(self.root, process_id, file_id)), file_contents)
-        md_to_write = {
-            "process_id": process_id,
-            "file_id": file_id
-        }
+        md_to_write = {"process_id": process_id, "file_id": file_id}
         if file_md:
             md_to_write.update(file_md)
         path = str(Path(self.root, process_id, file_id + ".md"))
         await AgentOS.file_memory.write_file(path, json.dumps(md_to_write).encode())
-        return FileHandle(machineURL=AgentOS.current_machine_url(), process_id=process_id, file_id=file_id, metadata=md_to_write)
+        return FileHandle(
+            machineURL=AgentOS.current_machine_url(), process_id=process_id, file_id=file_id, metadata=md_to_write
+        )
 
     async def set_metadata(self, process_id: str, file_id: str, metadata: Dict[str, any]):
         """
         Sets the metadata for the file specified by `file_id` within the context of the process_id.
         :param process_id:
         :param file_id:
         :param metadata:
@@ -88,15 +89,17 @@
         if not exists:
             file_md = {}
         else:
             contents = await AgentOS.file_memory.read_file(path)
             file_md = json.loads(contents)
         file_md.update(metadata)
         await AgentOS.file_memory.write_file(path, json.dumps(file_md).encode())
-        return FileHandle(machineURL=AgentOS.current_machine_url(), process_id=process_id, file_id=file_id, metadata=file_md)
+        return FileHandle(
+            machineURL=AgentOS.current_machine_url(), process_id=process_id, file_id=file_id, metadata=file_md
+        )
 
     async def delete_file(self, process_id: str, file_id: str):
         """
         Deletes the file specified by `file_id` within the context of the process_id.
         :param process_id:
         :param file_id:
         :return:
```

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/processes.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/processes.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/reference_model.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/reference_model.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/resources/reference_resource.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/resources/reference_resource.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/resources/resources_base.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/resources/resources_base.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/class_utils.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/class_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/image_utils.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/image_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/replay.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/replay.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
 async def default_parser(resp):
     yield await resp
 
 
 def replayable(
-        fn, serializer=default_serializer, deserializer=default_deserializer, parser=default_parser, name_override=None
+    fn, serializer=default_serializer, deserializer=default_deserializer, parser=default_parser, name_override=None
 ):
     config = AgentOS.get_instance(ReplayConfig)
 
     async def maybe_save_args(*args, **kwargs):
         if config.save_loc:
             try:
                 existing_dirs = [os.path.split(d)[-1] for d in await AgentOS.file_memory.glob(config.save_loc + "/*")]
```

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/schema_to_model.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/schema_to_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,17 @@
                         f"{model_name}_{property_name.capitalize()}ItemModel",
                     )
                     fields[property_name] = wrap_optional(List[nested_item_model], makeFieldOrDefaultValue())
                 else:
                     python_type = get_python_type(property_name, items_schema, str)
                     fields[property_name] = wrap_optional(List[python_type], makeFieldOrDefaultValue())
             else:
-                fields[property_name] = wrap_optional(get_python_type(property_name, property_schema), makeFieldOrDefaultValue())
+                fields[property_name] = wrap_optional(
+                    get_python_type(property_name, property_schema), makeFieldOrDefaultValue()
+                )
         except Exception as e:
             raise ValueError(f"Error creating field '{property_name}': {e}")
 
     try:
         return create_model(model_name, **fields, __base__=JsonProofModel)
     except ValidationError as e:
         raise ValueError(f"Error creating model '{model_name}': {e}")
```

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/str_utils.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/str_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     for key in {*os.environ, *defaults.keys()}:
         replacement = os.environ.get(key, defaults[key]) if key in defaults else os.environ[key]
         s = s.replace(f"${{{key}}}", replacement)
     return s
 
 
 def format_frame_info(frame_info):
-    return f"File \"{frame_info.filename}\", line {frame_info.lineno}, in {frame_info.function}\n    {frame_info.code_context[0].strip()}"
+    return f'File "{frame_info.filename}", line {frame_info.lineno}, in {frame_info.function}\n    {frame_info.code_context[0].strip()}'
 
 
 def log_stack_trace():
     logger = logging.getLogger("eidolon")
 
     frames = inspect.stack()[1:]  # Exclude the current frame
     stack_trace = "\n".join(format_frame_info(inspect.getframeinfo(frame[0])) for frame in reversed(frames))
```

### Comparing `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/stream_collector.py` & `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/stream_collector.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/logging.conf` & `eidolon_ai_sdk-0.1.28/logging.conf`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.27/pyproject.toml` & `eidolon_ai_sdk-0.1.28/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eidolon-ai-sdk"
-version = "0.1.27"
+version = "0.1.28"
 description = "An Open Source Agent Services Framework"
 authors = ["Luke Lalor <lukehlalor@gmail.com>"]
 readme = "README.md"
 include = ["logging.conf"]
 
 [tool.poetry.urls]
 Github = "https://github.com/eidolon-ai/eidolon"
```

### Comparing `eidolon_ai_sdk-0.1.27/PKG-INFO` & `eidolon_ai_sdk-0.1.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eidolon-ai-sdk
-Version: 0.1.27
+Version: 0.1.28
 Summary: An Open Source Agent Services Framework
 Author: Luke Lalor
 Author-email: lukehlalor@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anthropic (>=0.21.3,<0.22.0)
```

