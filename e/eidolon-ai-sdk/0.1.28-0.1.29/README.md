# Comparing `tmp/eidolon_ai_sdk-0.1.28.tar.gz` & `tmp/eidolon_ai_sdk-0.1.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eidolon_ai_sdk-0.1.28.tar", max compression
+gzip compressed data, was "eidolon_ai_sdk-0.1.29.tar", max compression
```

## Comparing `eidolon_ai_sdk-0.1.28.tar` & `eidolon_ai_sdk-0.1.29.tar`

### file list

```diff
@@ -1,143 +1,143 @@
--rw-r--r--   0        0        0     2569 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/README.md
--rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/__init__.py
--rw-r--r--   0        0        0     2400 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/agent.py
--rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/__init__.py
--rw-r--r--   0        0        0     3025 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/document_manager.py
--rw-r--r--   0        0        0     2710 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/document_processor.py
--rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/loaders/__init__.py
--rw-r--r--   0        0        0      971 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py
--rw-r--r--   0        0        0     3405 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py
--rw-r--r--   0        0        0     4173 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py
--rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/__init__.py
--rw-r--r--   0        0        0     2817 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py
--rw-r--r--   0        0        0     4519 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py
--rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/__init__.py
--rw-r--r--   0        0        0      448 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/base_ast_generator.py
--rw-r--r--   0        0        0     3699 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py
--rw-r--r--   0        0        0     2053 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py
--rw-r--r--   0        0        0     3212 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py
--rw-r--r--   0        0        0     1647 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py
--rw-r--r--   0        0        0     1328 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py
--rw-r--r--   0        0        0     3356 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py
--rw-r--r--   0        0        0     1400 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py
--rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/transformer/__init__.py
--rw-r--r--   0        0        0     1398 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py
--rw-r--r--   0        0        0     4786 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py
--rw-r--r--   0        0        0    43465 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py
--rw-r--r--   0        0        0     4825 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/generic_agent.py
--rw-r--r--   0        0        0     1950 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/openai_whisper_agent.py
--rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/retriever_agent/__init__.py
--rw-r--r--   0        0        0     2078 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py
--rw-r--r--   0        0        0     1434 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py
--rw-r--r--   0        0        0     2329 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py
--rw-r--r--   0        0        0      559 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py
--rw-r--r--   0        0        0     2864 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/retriever_agent/retriever.py
--rw-r--r--   0        0        0     3717 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py
--rw-r--r--   0        0        0    12914 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/simple_agent.py
--rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/__init__.py
--rw-r--r--   0        0        0     1815 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/checker.py
--rw-r--r--   0        0        0     2468 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/controller.py
--rw-r--r--   0        0        0     1503 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/memory.py
--rw-r--r--   0        0        0     1423 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/prompts.py
--rw-r--r--   0        0        0      364 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/thought.py
--rw-r--r--   0        0        0     4951 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/thought_generators.py
--rw-r--r--   0        0        0     7614 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/tot_agent.py
--rw-r--r--   0        0        0     4572 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent_os.py
--rw-r--r--   0        0        0    12735 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent_os_interfaces.py
--rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/bin/__init__.py
--rwxr-xr-x   0        0        0     9444 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/bin/agent_creator.py
--rw-r--r--   0        0        0     7743 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/bin/agent_http_server.py
--rwxr-xr-x   0        0        0     3789 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/bin/replay.py
--rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/__init__.py
--rw-r--r--   0        0        0     8906 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/code_builtins.py
--rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/components/__init__.py
--rw-r--r--   0        0        0     2223 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/components/opentelemetry.py
--rw-r--r--   0        0        0     4256 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/components/usage.py
--rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/logic_units/__init__.py
--rw-r--r--   0        0        0     5662 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/logic_units/web_search.py
--rw-r--r--   0        0        0      550 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml
--rw-r--r--   0        0        0      544 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/claude_opus.yaml
--rw-r--r--   0        0        0      557 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml
--rw-r--r--   0        0        0      181 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/machine.yaml
--rw-r--r--   0        0        0      540 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/mistral_large.yaml
--rw-r--r--   0        0        0      547 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml
--rw-r--r--   0        0        0      540 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/mistral_small.yaml
--rw-r--r--   0        0        0      534 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/openai_35.yaml
--rw-r--r--   0        0        0      557 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/openai_4.yaml
--rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/__init__.py
--rw-r--r--   0        0        0     1843 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/agent_call_history.py
--rw-r--r--   0        0        0     4638 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/agent_cpu.py
--rw-r--r--   0        0        0     2562 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/agent_io.py
--rw-r--r--   0        0        0     7916 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/agents_logic_unit.py
--rw-r--r--   0        0        0     1641 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/audio_unit.py
--rw-r--r--   0        0        0      292 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/call_context.py
--rw-r--r--   0        0        0     2833 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/conversation_memory_unit.py
--rw-r--r--   0        0        0    14320 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/conversational_apu.py
--rw-r--r--   0        0        0     1891 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/image_unit.py
--rw-r--r--   0        0        0        0 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm/__init__.py
--rw-r--r--   0        0        0     9936 2024-04-17 00:51:18.212667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py
--rw-r--r--   0        0        0    11967 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py
--rw-r--r--   0        0        0     4518 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py
--rw-r--r--   0        0        0     5760 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py
--rw-r--r--   0        0        0     9430 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py
--rw-r--r--   0        0        0     3375 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm/open_ai_speech.py
--rw-r--r--   0        0        0     3930 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm_message.py
--rw-r--r--   0        0        0     2421 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm_unit.py
--rw-r--r--   0        0        0     4199 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/logic_unit.py
--rw-r--r--   0        0        0     3541 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/memory_unit.py
--rw-r--r--   0        0        0      825 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/processing_unit.py
--rw-r--r--   0        0        0        0 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/io/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/__init__.py
--rw-r--r--   0        0        0     1193 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/agent_memory.py
--rw-r--r--   0        0        0     5309 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/chroma_vector_store.py
--rw-r--r--   0        0        0      641 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/document.py
--rw-r--r--   0        0        0     2766 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/embeddings.py
--rw-r--r--   0        0        0      907 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/file_memory.py
--rw-r--r--   0        0        0     4203 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/file_system_vector_store.py
--rw-r--r--   0        0        0     3974 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/in_memory_file_memory.py
--rw-r--r--   0        0        0     5788 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/local_file_memory.py
--rw-r--r--   0        0        0     4845 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/local_symbolic_memory.py
--rw-r--r--   0        0        0     3793 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/mongo_symbolic_memory.py
--rw-r--r--   0        0        0      996 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/noop_memory.py
--rw-r--r--   0        0        0     1984 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/s3_file_memory.py
--rw-r--r--   0        0        0      974 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/semantic_memory.py
--rw-r--r--   0        0        0     2809 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/similarity_memory.py
--rw-r--r--   0        0        0     1516 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/vector_store.py
--rw-r--r--   0        0        0        0 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/__init__.py
--rw-r--r--   0        0        0      771 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/authentication_processor.py
--rw-r--r--   0        0        0     2159 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/azure_authorizer.py
--rw-r--r--   0        0        0     1277 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/functional_authorizer.py
--rw-r--r--   0        0        0     2001 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/google_auth.py
--rw-r--r--   0        0        0     1867 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/jwt_processor.py
--rw-r--r--   0        0        0      484 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/okta_authorizor.py
--rw-r--r--   0        0        0     1017 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/permissions.py
--rw-r--r--   0        0        0     2508 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/process_authorizer.py
--rw-r--r--   0        0        0     2977 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/security_manager.py
--rw-r--r--   0        0        0     1035 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/security_middleware.py
--rw-r--r--   0        0        0      428 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/user.py
--rw-r--r--   0        0        0        0 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/__init__.py
--rw-r--r--   0        0        0     1377 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/agent_contract.py
--rw-r--r--   0        0        0    21705 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/agent_controller.py
--rw-r--r--   0        0        0    14099 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/agent_machine.py
--rw-r--r--   0        0        0     1149 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/dynamic_middleware.py
--rw-r--r--   0        0        0     3432 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/fn_handler.py
--rw-r--r--   0        0        0     4904 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/process_file_system.py
--rw-r--r--   0        0        0     4275 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/processes.py
--rw-r--r--   0        0        0     6895 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/reference_model.py
--rw-r--r--   0        0        0        0 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/resources/__init__.py
--rw-r--r--   0        0        0      314 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/resources/agent_resource.py
--rw-r--r--   0        0        0      414 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/resources/machine_resource.py
--rw-r--r--   0        0        0      684 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/resources/reference_resource.py
--rw-r--r--   0        0        0     1663 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/resources/resources_base.py
--rw-r--r--   0        0        0        0 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/__init__.py
--rw-r--r--   0        0        0      509 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/async_wrapper.py
--rw-r--r--   0        0        0     2806 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/class_utils.py
--rw-r--r--   0        0        0     1604 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/image_utils.py
--rw-r--r--   0        0        0     3808 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/replay.py
--rw-r--r--   0        0        0     6521 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/schema_to_model.py
--rw-r--r--   0        0        0      898 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/str_utils.py
--rw-r--r--   0        0        0     3445 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/stream_collector.py
--rw-r--r--   0        0        0      565 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/logging.conf
--rw-r--r--   0        0        0     2030 2024-04-17 00:51:18.216667 eidolon_ai_sdk-0.1.28/pyproject.toml
--rw-r--r--   0        0        0     4807 1970-01-01 00:00:00.000000 eidolon_ai_sdk-0.1.28/PKG-INFO
+-rw-r--r--   0        0        0     2569 2024-04-17 22:17:02.294480 eidolon_ai_sdk-0.1.29/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 22:17:02.294480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 22:17:02.294480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/__init__.py
+-rw-r--r--   0        0        0     2400 2024-04-17 22:17:02.294480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/agent.py
+-rw-r--r--   0        0        0        0 2024-04-17 22:17:02.294480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/__init__.py
+-rw-r--r--   0        0        0     3025 2024-04-17 22:17:02.294480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/document_manager.py
+-rw-r--r--   0        0        0     2710 2024-04-17 22:17:02.294480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/document_processor.py
+-rw-r--r--   0        0        0        0 2024-04-17 22:17:02.294480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/loaders/__init__.py
+-rw-r--r--   0        0        0      971 2024-04-17 22:17:02.294480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py
+-rw-r--r--   0        0        0     3405 2024-04-17 22:17:02.294480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py
+-rw-r--r--   0        0        0     4173 2024-04-17 22:17:02.294480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py
+-rw-r--r--   0        0        0        0 2024-04-17 22:17:02.294480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/parsers/__init__.py
+-rw-r--r--   0        0        0     2817 2024-04-17 22:17:02.294480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py
+-rw-r--r--   0        0        0     4519 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py
+-rw-r--r--   0        0        0        0 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/__init__.py
+-rw-r--r--   0        0        0      448 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/base_ast_generator.py
+-rw-r--r--   0        0        0     3699 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py
+-rw-r--r--   0        0        0     2053 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py
+-rw-r--r--   0        0        0     3212 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py
+-rw-r--r--   0        0        0     1647 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py
+-rw-r--r--   0        0        0     1328 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py
+-rw-r--r--   0        0        0     3356 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py
+-rw-r--r--   0        0        0     1400 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py
+-rw-r--r--   0        0        0        0 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/transformer/__init__.py
+-rw-r--r--   0        0        0     1398 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py
+-rw-r--r--   0        0        0     4786 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py
+-rw-r--r--   0        0        0    43465 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py
+-rw-r--r--   0        0        0     4825 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/generic_agent.py
+-rw-r--r--   0        0        0     1936 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/openai_whisper_agent.py
+-rw-r--r--   0        0        0        0 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/retriever_agent/__init__.py
+-rw-r--r--   0        0        0     2078 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py
+-rw-r--r--   0        0        0     1434 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py
+-rw-r--r--   0        0        0     2329 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py
+-rw-r--r--   0        0        0      559 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py
+-rw-r--r--   0        0        0     2864 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/retriever_agent/retriever.py
+-rw-r--r--   0        0        0     3717 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py
+-rw-r--r--   0        0        0    12914 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/simple_agent.py
+-rw-r--r--   0        0        0        0 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/tot_agent/__init__.py
+-rw-r--r--   0        0        0     1815 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/tot_agent/checker.py
+-rw-r--r--   0        0        0     2468 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/tot_agent/controller.py
+-rw-r--r--   0        0        0     1503 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/tot_agent/memory.py
+-rw-r--r--   0        0        0     1423 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/tot_agent/prompts.py
+-rw-r--r--   0        0        0      364 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/tot_agent/thought.py
+-rw-r--r--   0        0        0     4951 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/tot_agent/thought_generators.py
+-rw-r--r--   0        0        0     7614 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/tot_agent/tot_agent.py
+-rw-r--r--   0        0        0     4572 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent_os.py
+-rw-r--r--   0        0        0    12735 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent_os_interfaces.py
+-rw-r--r--   0        0        0        0 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/bin/__init__.py
+-rwxr-xr-x   0        0        0     9444 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/bin/agent_creator.py
+-rw-r--r--   0        0        0     7743 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/bin/agent_http_server.py
+-rwxr-xr-x   0        0        0     3789 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/bin/replay.py
+-rw-r--r--   0        0        0        0 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/builtins/__init__.py
+-rw-r--r--   0        0        0     9001 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/builtins/code_builtins.py
+-rw-r--r--   0        0        0        0 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/builtins/components/__init__.py
+-rw-r--r--   0        0        0     2223 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/builtins/components/opentelemetry.py
+-rw-r--r--   0        0        0     4256 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/builtins/components/usage.py
+-rw-r--r--   0        0        0        0 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/builtins/logic_units/__init__.py
+-rw-r--r--   0        0        0     5662 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/builtins/logic_units/web_search.py
+-rw-r--r--   0        0        0      550 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml
+-rw-r--r--   0        0        0      601 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/builtins/resources/claude_opus.yaml
+-rw-r--r--   0        0        0      614 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml
+-rw-r--r--   0        0        0      181 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/builtins/resources/machine.yaml
+-rw-r--r--   0        0        0      597 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/builtins/resources/mistral_large.yaml
+-rw-r--r--   0        0        0      547 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml
+-rw-r--r--   0        0        0      540 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/builtins/resources/mistral_small.yaml
+-rw-r--r--   0        0        0      595 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/builtins/resources/openai_35.yaml
+-rw-r--r--   0        0        0      618 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/builtins/resources/openai_4.yaml
+-rw-r--r--   0        0        0        0 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/__init__.py
+-rw-r--r--   0        0        0     1843 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/agent_call_history.py
+-rw-r--r--   0        0        0     4638 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/agent_cpu.py
+-rw-r--r--   0        0        0     2562 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/agent_io.py
+-rw-r--r--   0        0        0     7916 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/agents_logic_unit.py
+-rw-r--r--   0        0        0     4062 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/audio_unit.py
+-rw-r--r--   0        0        0      292 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/call_context.py
+-rw-r--r--   0        0        0     2833 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/conversation_memory_unit.py
+-rw-r--r--   0        0        0    13845 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/conversational_apu.py
+-rw-r--r--   0        0        0     4680 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/image_unit.py
+-rw-r--r--   0        0        0        0 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/llm/__init__.py
+-rw-r--r--   0        0        0     9936 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py
+-rw-r--r--   0        0        0    11967 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py
+-rw-r--r--   0        0        0     4518 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py
+-rw-r--r--   0        0        0     5762 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py
+-rw-r--r--   0        0        0     9430 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py
+-rw-r--r--   0        0        0     3591 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/llm/open_ai_speech.py
+-rw-r--r--   0        0        0     3962 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/llm_message.py
+-rw-r--r--   0        0        0     2421 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/llm_unit.py
+-rw-r--r--   0        0        0     4199 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/logic_unit.py
+-rw-r--r--   0        0        0     3541 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/memory_unit.py
+-rw-r--r--   0        0        0      825 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/processing_unit.py
+-rw-r--r--   0        0        0        0 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/io/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/__init__.py
+-rw-r--r--   0        0        0     1193 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/agent_memory.py
+-rw-r--r--   0        0        0     5309 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/chroma_vector_store.py
+-rw-r--r--   0        0        0      641 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/document.py
+-rw-r--r--   0        0        0     2766 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/embeddings.py
+-rw-r--r--   0        0        0      907 2024-04-17 22:17:02.298480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/file_memory.py
+-rw-r--r--   0        0        0     4203 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/file_system_vector_store.py
+-rw-r--r--   0        0        0     3974 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/in_memory_file_memory.py
+-rw-r--r--   0        0        0     5788 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/local_file_memory.py
+-rw-r--r--   0        0        0     4845 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/local_symbolic_memory.py
+-rw-r--r--   0        0        0     3793 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/mongo_symbolic_memory.py
+-rw-r--r--   0        0        0      996 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/noop_memory.py
+-rw-r--r--   0        0        0     1984 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/s3_file_memory.py
+-rw-r--r--   0        0        0      974 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/semantic_memory.py
+-rw-r--r--   0        0        0     2809 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/similarity_memory.py
+-rw-r--r--   0        0        0     1516 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/vector_store.py
+-rw-r--r--   0        0        0        0 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/security/__init__.py
+-rw-r--r--   0        0        0      771 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/security/authentication_processor.py
+-rw-r--r--   0        0        0     2159 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/security/azure_authorizer.py
+-rw-r--r--   0        0        0     1277 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/security/functional_authorizer.py
+-rw-r--r--   0        0        0     2001 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/security/google_auth.py
+-rw-r--r--   0        0        0     1867 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/security/jwt_processor.py
+-rw-r--r--   0        0        0      484 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/security/okta_authorizor.py
+-rw-r--r--   0        0        0     1017 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/security/permissions.py
+-rw-r--r--   0        0        0     2508 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/security/process_authorizer.py
+-rw-r--r--   0        0        0     2977 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/security/security_manager.py
+-rw-r--r--   0        0        0     1035 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/security/security_middleware.py
+-rw-r--r--   0        0        0      428 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/security/user.py
+-rw-r--r--   0        0        0        0 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/system/__init__.py
+-rw-r--r--   0        0        0     1377 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/system/agent_contract.py
+-rw-r--r--   0        0        0    21705 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/system/agent_controller.py
+-rw-r--r--   0        0        0    14172 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/system/agent_machine.py
+-rw-r--r--   0        0        0     1149 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/system/dynamic_middleware.py
+-rw-r--r--   0        0        0     3432 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/system/fn_handler.py
+-rw-r--r--   0        0        0     4902 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/system/process_file_system.py
+-rw-r--r--   0        0        0     4275 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/system/processes.py
+-rw-r--r--   0        0        0     6895 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/system/reference_model.py
+-rw-r--r--   0        0        0        0 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/system/resources/__init__.py
+-rw-r--r--   0        0        0      314 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/system/resources/agent_resource.py
+-rw-r--r--   0        0        0      414 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/system/resources/machine_resource.py
+-rw-r--r--   0        0        0      684 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/system/resources/reference_resource.py
+-rw-r--r--   0        0        0     1663 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/system/resources/resources_base.py
+-rw-r--r--   0        0        0        0 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/util/__init__.py
+-rw-r--r--   0        0        0      509 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/util/async_wrapper.py
+-rw-r--r--   0        0        0     2806 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/util/class_utils.py
+-rw-r--r--   0        0        0     1604 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/util/image_utils.py
+-rw-r--r--   0        0        0     3808 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/util/replay.py
+-rw-r--r--   0        0        0     6521 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/util/schema_to_model.py
+-rw-r--r--   0        0        0      898 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/util/str_utils.py
+-rw-r--r--   0        0        0     3445 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/util/stream_collector.py
+-rw-r--r--   0        0        0      565 2024-04-17 22:17:02.302480 eidolon_ai_sdk-0.1.29/logging.conf
+-rw-r--r--   0        0        0     2030 2024-04-17 22:17:02.306480 eidolon_ai_sdk-0.1.29/pyproject.toml
+-rw-r--r--   0        0        0     4807 1970-01-01 00:00:00.000000 eidolon_ai_sdk-0.1.29/PKG-INFO
```

### Comparing `eidolon_ai_sdk-0.1.28/README.md` & `eidolon_ai_sdk-0.1.29/README.md`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/agent.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/document_manager.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/document_manager.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/document_processor.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/document_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/generic_agent.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/generic_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/openai_whisper_agent.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/openai_whisper_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,17 +19,15 @@
 
     def __init__(self, spec: AutonomousSpeechAgentSpec):
         super().__init__(spec=spec)
         self.speech_llm = self.spec.speech_llm.instantiate(processing_unit_locator=None)
         self.cpu = self.spec.cpu.instantiate()
 
     @register_program()
-    async def speech_to_text(
-        self, audio: Annotated[FileHandle, Body(description="The audio file", embed=True)]
-    ):
+    async def speech_to_text(self, audio: Annotated[FileHandle, Body(description="The audio file", embed=True)]):
         process_id = audio.process_id
         await ProcessDoc.set_delete_on_terminate(process_id, True)
         file, metadata = await AgentOS.process_file_system.read_file(process_id, audio.file_id)
         mimetype = "audio/wav"
         if metadata and "mimetype" in metadata:
             mimetype = metadata["mimetype"]
         # audio = AudioSegment.from_file(file)
```

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/retriever_agent/retriever.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/retriever_agent/retriever.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/simple_agent.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/simple_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/checker.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/tot_agent/checker.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/controller.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/tot_agent/controller.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/memory.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/tot_agent/memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/prompts.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/tot_agent/prompts.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/thought_generators.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/tot_agent/thought_generators.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent/tot_agent/tot_agent.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent/tot_agent/tot_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent_os.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent_os.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/agent_os_interfaces.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/agent_os_interfaces.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/bin/agent_creator.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/bin/agent_creator.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/bin/agent_http_server.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/bin/agent_http_server.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/bin/replay.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/bin/replay.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/code_builtins.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/builtins/code_builtins.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from eidolon_ai_sdk.cpu.agent_io import IOUnit
 from eidolon_ai_sdk.cpu.conversation_memory_unit import RawMemoryUnit
 from eidolon_ai_sdk.cpu.conversational_apu import ConversationalAPU
 from eidolon_ai_sdk.agent_os_interfaces import FileMemory, SymbolicMemory, SimilarityMemory, SecurityManager
 from eidolon_ai_sdk.cpu.llm.anthropic_llm_unit import AnthropicLLMUnit
 from eidolon_ai_sdk.cpu.llm.mistral_llm_unit import MistralGPT
 from eidolon_ai_sdk.cpu.llm.open_ai_connection_handler import OpenAIConnectionHandler, AzureOpenAIConnectionHandler
+from eidolon_ai_sdk.cpu.llm.open_ai_image_unit import OpenAIImageUnit
 from eidolon_ai_sdk.cpu.llm.open_ai_llm_unit import OpenAIGPT
 from eidolon_ai_sdk.cpu.llm.open_ai_speech import OpenAiSpeech
 from eidolon_ai_sdk.cpu.llm_unit import LLMUnit, LLMModel
 from eidolon_ai_sdk.cpu.memory_unit import MemoryUnit
 from eidolon_ai_sdk.memory.s3_file_memory import S3FileMemory
 from eidolon_ai_sdk.security.azure_authorizer import AzureJWTProcessor
 from eidolon_ai_sdk.security.google_auth import GoogleJWTProcessor
@@ -191,13 +192,14 @@
         ToTChecker,
         OpenAiSpeech,
         AsyncOpenAI,
         AsyncAzureOpenAI,
         UsageClient,
         OpenAIConnectionHandler,
         AzureOpenAIConnectionHandler,
+        OpenAIImageUnit,
         DefaultAzureCredential,
         EnvironmentCredential,
         # config objects
         ReplayConfig,
     ]
     return [_to_resource(maybe_tuple) for maybe_tuple in builtin_list if maybe_tuple]
```

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/components/opentelemetry.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/builtins/components/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/components/usage.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/builtins/components/usage.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/logic_units/web_search.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/builtins/logic_units/web_search.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/claude_opus.yaml` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/builtins/resources/claude_opus.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 kind: Reference
 metadata:
   name: ClaudeOpus
   annotations:
     - title: "Claude Opus"
 spec:
   implementation: APU
+  audio_unit: OpenAiSpeech
+  image_unit: OpenAIImageUnit
   llm_unit:
     implementation: AnthropicLLMUnit
     model: "claude-3-opus-20240229"
 ---
 apiVersion: eidolon/v1
 kind: Reference
 metadata:
```

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/mistral_large.yaml` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 ---
 apiVersion: eidolon/v1
 kind: Reference
 metadata:
-  name: MistralLarge
+  name: MistralMedium
   annotations:
-    - title: "Mistral Large"
+    - title: "Mistral Medium"
 spec:
   implementation: APU
   llm_unit:
     implementation: MistralGPT
-    model: "mistral-large-latest"
+    model: "mistral-medium-latest"
 ---
 apiVersion: eidolon/v1
 kind: Reference
 metadata:
-  name: "mistral-large-latest"
+  name: "mistral-medium-latest"
 spec:
   implementation: LLMModel
-  human_name: Mistral Large
-  name: "mistral-large-latest"
+  human_name: Mistral Medium
+  name: "mistral-medium-latest"
   input_context_limit: 32000
   output_context_limit: 4096
-  supports_tools: True
+  supports_tools: False
   supports_image_input: False
   supports_audio_input: False
```

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/builtins/resources/mistral_small.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 ---
 apiVersion: eidolon/v1
 kind: Reference
 metadata:
-  name: MistralMedium
+  name: MistralSmall
   annotations:
-    - title: "Mistral Medium"
+    - title: "Mistral Small"
 spec:
   implementation: APU
   llm_unit:
     implementation: MistralGPT
-    model: "mistral-medium-latest"
+    model: "mistral-small-latest"
 ---
 apiVersion: eidolon/v1
 kind: Reference
 metadata:
-  name: "mistral-medium-latest"
+  name: "mistral-small-latest"
 spec:
   implementation: LLMModel
-  human_name: Mistral Medium
-  name: "mistral-medium-latest"
+  human_name: Mistral Small
+  name: "mistral-small-latest"
   input_context_limit: 32000
   output_context_limit: 4096
   supports_tools: False
   supports_image_input: False
-  supports_audio_input: False
+  supports_audio_input: False
```

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/openai_35.yaml` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/builtins/resources/openai_35.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 kind: Reference
 metadata:
   name: GPT3.5-turbo
   annotations:
     - title: "OpenAI GPT 3.5 Turbo"
 spec:
     implementation: APU
+    audio_unit: OpenAiSpeech
+    image_unit: OpenAIImageUnit
     llm_unit:
       implementation: OpenAIGPT
       model: "gpt-3.5-turbo"
 ---
 apiVersion: eidolon/v1
 kind: Reference
 metadata:
```

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/builtins/resources/openai_4.yaml` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/builtins/resources/openai_4.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 kind: Reference
 metadata:
   name: GPT4-turbo
   annotations:
     - title: "OpenAI GPT 4.0 Turbo"
 spec:
     implementation: APU
+    audio_unit: OpenAiSpeech
+    image_unit: OpenAIImageUnit
     llm_unit:
       implementation: OpenAIGPT
       model: "gpt-4-turbo-preview"
 ---
 apiVersion: eidolon/v1
 kind: Reference
 metadata:
```

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/agent_call_history.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/agent_call_history.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/agent_cpu.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/agent_cpu.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,10 +140,10 @@
     def call_context(self) -> CallContext:
         return self._call_context
 
     async def clone(self) -> Thread:
         return await self._cpu.clone_thread(self._call_context)
 
 
-class CPUException(Exception):
+class APUException(Exception):
     def __init__(self, description):
         super().__init__("CPU Error: " + description)
```

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/agent_io.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/agent_io.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/agents_logic_unit.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/agents_logic_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/conversation_memory_unit.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/conversation_memory_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/conversational_apu.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/conversational_apu.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 )
 from eidolon_ai_client.util.logger import logger
 from eidolon_ai_client.util.stream_collector import merge_streams
 from eidolon_ai_sdk.agent.doc_manager.document_processor import DocumentProcessor
 from eidolon_ai_sdk.agent.doc_manager.loaders.base_loader import FileInfo
 from eidolon_ai_sdk.agent.doc_manager.parsers.base_parser import DataBlob
 from eidolon_ai_sdk.agent_os import AgentOS
-from eidolon_ai_sdk.cpu.agent_cpu import APU, APUSpec, Thread, CPUException, APUCapabilities
+from eidolon_ai_sdk.cpu.agent_cpu import APU, APUSpec, Thread, APUException, APUCapabilities
 from eidolon_ai_sdk.cpu.agent_io import IOUnit, CPUMessageTypes
 from eidolon_ai_sdk.cpu.audio_unit import AudioUnit
 from eidolon_ai_sdk.cpu.call_context import CallContext
 from eidolon_ai_sdk.cpu.image_unit import ImageUnit
 from eidolon_ai_sdk.cpu.llm_message import (
     AssistantMessage,
     ToolResponseMessage,
@@ -67,26 +67,30 @@
         self.memory_unit = self.spec.memory_unit.instantiate(**kwargs)
         self.llm_unit = self.spec.llm_unit.instantiate(**kwargs)
         self.logic_units = [logic_unit.instantiate(**kwargs) for logic_unit in self.spec.logic_units]
         self.audio_unit = self.spec.audio_unit.instantiate(**kwargs) if self.spec.audio_unit else None
         self.image_unit = self.spec.image_unit.instantiate(**kwargs) if self.spec.image_unit else None
         self.record_memory = self.spec.record_conversation
         self.document_processor = self.spec.document_processor.instantiate()
+        if self.audio_unit:
+            self.logic_units.append(self.audio_unit)
+        if self.image_unit:
+            self.logic_units.append(self.image_unit)
 
     def get_capabilities(self) -> APUCapabilities:
         llm_props = self.llm_unit.get_llm_capabilities()
         return APUCapabilities(
             input_context_limit=llm_props.input_context_limit,
             output_context_limit=llm_props.output_context_limit,
             supports_tools=llm_props.supports_tools,
-            supports_image_input=llm_props.supports_image_input or self.image_unit is not None,
-            supports_audio_input=llm_props.supports_audio_input or self.audio_unit is not None,
+            supports_image_input=llm_props.supports_image_input or self.spec.image_unit is not None,
+            supports_audio_input=llm_props.supports_audio_input or self.spec.audio_unit is not None,
             supports_file_search=llm_props.supports_tools and self.document_processor is not None,
-            supports_audio_generation=self.audio_unit is not None,
-            supports_image_generation=self.image_unit is not None,
+            supports_audio_generation=self.spec.audio_unit is not None,
+            supports_image_generation=self.spec.image_unit is not None,
         )
 
     def locate_unit(self, unit_type: Type[PU_T]) -> PU_T:
         for unit in self.logic_units:
             if isinstance(unit, unit_type):
                 return unit
         if isinstance(self.io_unit, unit_type):
@@ -122,19 +126,19 @@
             if self.record_memory:
                 await self.memory_unit.storeMessages(call_context, conversation_messages)
             conversation.extend(conversation_messages)
             async for event in self._llm_execution_cycle(call_context, output_format, conversation):
                 yield event
         except HTTPException as e:
             raise e
-        except CPUException as e:
+        except APUException as e:
             raise e
         except Exception as e:
             logger.exception(e)
-            raise CPUException(f"{e.__class__.__name__} while processing request") from e
+            raise APUException(f"{e.__class__.__name__} while processing request") from e
 
     async def _llm_execution_cycle(
         self,
         call_context: CallContext,
         output_format: Union[Literal["str"], Dict[str, Any]],
         conversation: List[LLMMessage],
     ) -> AsyncIterator[StreamEvent]:
@@ -143,17 +147,17 @@
         for event in conversation:
             if isinstance(event, UserMessage):
                 converted_messages = []
                 for message in event.content:
                     if isinstance(message, UserMessageFile) and message.include_directly:
                         converted_messages.extend(await self.process_file_message(call_context.process_id, message))
                     elif isinstance(message, UserMessageAudio):
-                        converted_messages.extend(await self.process_audio_message(call_context, message))
+                        converted_messages.extend(await self.process_audio_message(message))
                     elif isinstance(message, UserMessageImage):
-                        converted_messages.extend(await self.process_image_message(call_context, message))
+                        converted_messages.extend(await self.process_image_message(message))
                     else:
                         converted_messages.append(message)
                 converted_conversation.append(UserMessage(content=converted_messages))
             else:
                 converted_conversation.append(event)
 
         num_iterations = 0
@@ -163,14 +167,15 @@
                 tool_call_events = []
                 llm_facing_tools = [w.llm_message for w in tool_defs.values()]
             with tracer.start_as_current_span("llm execution"):
                 execute_llm_ = self.llm_unit.execute_llm(
                     call_context, converted_conversation, llm_facing_tools, output_format
                 )
                 # yield the events but capture the output, so it can be rolled into one event for memory.
+                # noinspection PyTypeChecker
                 stream_collector = StreamCollector(execute_llm_)
                 async for event in stream_collector:
                     if event.is_root_and_type(LLMToolCallRequestEvent):
                         tool_call_events.append(event)
                     yield event
             if stream_collector.get_content():
                 logger.info(f"LLM Response: {stream_collector.get_content()}")
@@ -190,15 +195,15 @@
                         self._call_tool(call_context, tce, tool_defs, converted_conversation) for tce in tool_call_events
                     ]
                     async for e in merge_streams(streams):
                         yield e
             else:
                 return
 
-        raise CPUException(f"exceeded maximum number of function calls ({self.spec.max_num_function_calls})")
+        raise APUException(f"exceeded maximum number of function calls ({self.spec.max_num_function_calls})")
 
     async def _call_tool(
         self,
         call_context: CallContext,
         tool_call_event: LLMToolCallRequestEvent,
         tool_defs,
         conversation: List[LLMMessage],
@@ -240,38 +245,26 @@
             result=tool_stream.get_content() or "",
             name=tc.name,
         )
         if self.record_memory:
             await self.memory_unit.storeMessages(call_context, [message])
         conversation.append(message)
 
-    async def process_audio_message(self, call_context: CallContext, message: UserMessageAudio):
+    async def process_audio_message(self, message: UserMessageAudio):
         if self.audio_unit is None:
             raise ValueError("No audio unit available")
-        audio_data, metadata = await AgentOS.process_file_system.read_file(call_context.process_id, message.file.file_id)
-        mimetype = metadata.get("mimetype")
-        path = metadata.get("path") or metadata.get("filename") or ""
-        text = await self.audio_unit.speech_to_text(audio=audio_data, mime_type=mimetype)
-        return [UserMessageText(text=f"The following text as converted from the audio file {path}:\n{text}\n\n")]
+        message = f"The user uploaded an audio clip with the file handle of {message.file.model_dump()}. Use the text_to_speech tool to process this audio file. Always process the audio file!"
+        return [UserMessageText(text=message)]
 
-    async def process_image_message(self, call_context: CallContext, message: UserMessageImage):
-        if self.get_capabilities().supports_image_input:
+    async def process_image_message(self, message: UserMessageImage):
+        if self.image_unit is not None:
+            message = f"The user uploaded an image with the file handle of {message.file.model_dump()}. Use the image_to_text tool to process this image file. Always process the image file!"
+            return [UserMessageText(text=message)]
+        elif self.get_capabilities().supports_image_input:
             return [message]
-        elif self.image_unit is not None:
-            image_data, metadata = await AgentOS.process_file_system.read_file(
-                call_context.process_id, message.file.file_id
-            )
-            path = metadata.get("path") or metadata.get("filename") or ""
-            text = await self.image_unit.image_to_text(
-                prompt="Create a detailed text description of the following image. Be sure to include as much information as needed to describe the image.  Be very verbose.",
-                image=image_data,
-            )
-            return [
-                UserMessageText(text=f"The following text is a detailed description of an image {path}:\n{text}\n\n")
-            ]
         else:
             raise ValueError("Image processing not supported")
 
     async def process_file_message(self, process_id: str, message: UserMessageFile):
         parts = []
         if message.include_directly:
             data, metadata = await AgentOS.process_file_system.read_file(process_id, message.file.file_id)
```

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             styles=[
                 "vivid",
                 "natural",
             ],
             max_prompt_size=4000,
         )
 
-    async def image_to_text(self, prompt: str, image: bytes) -> str:
+    async def _image_to_text(self, prompt: str, image: bytes) -> str:
         """
         Converts an image to text.
 
         Args:
             image (bytes): The image data.
 
         Returns:
@@ -84,15 +84,15 @@
             "temperature": self.spec.temperature,
         }
 
         result: ChatCompletion = await self.connection_handler.completion(**request)
         print(result)
         return result.choices[0].message.content
 
-    async def text_to_image(
+    async def _text_to_image(
         self,
         call_context: CallContext,
         text: str,
         quality: Optional[str] = None,
         size: Tuple[int, int] = (1024, 1024),
         style: Optional[str] = None,
         image_format: Literal["jpeg", "png", "tiff", "bmp", "webp"] = "webp",
```

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm/open_ai_speech.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/llm/open_ai_speech.py`

 * *Files 23% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     temperature: float
     llm: AsyncOpenAI = None
 
     def __init__(self, spec: OpenAiSpeechSpec, **kwargs):
         super().__init__(spec, **kwargs)
         Specable.__init__(self, spec, **kwargs)
 
-    async def text_to_speech(self, text: str, response_format: str = "mp3") -> bytes:
+    async def _text_to_speech(self, text: str, response_format: str = "mp3") -> bytes:
         """
         Converts text to speech.
 
         Args:
             text (str): The text to convert to speech.
 
         Returns:
@@ -52,15 +52,15 @@
             voice=self.spec.text_to_speech_voice,
             response_format="mp3",
             input=text,
         )
 
         return response.content
 
-    async def speech_to_text(
+    async def _speech_to_text(
         self, audio: bytes, mime_type: str, prompt: Optional[str] = None, language: Optional[str] = None
     ) -> str:
         """
         Converts speech to text.
 
         Args:
             audio (bytes): The audio data.
@@ -75,14 +75,15 @@
         """
         if not self.llm:
             self.llm = AsyncOpenAI()
         request = {
             "file": ("audio", audio, mime_type),
             "model": self.spec.speech_to_text_model,
             "temperature": self.spec.speech_to_text_temperature,
+            "extra_headers": {"Content-Type": "multipart/form-data; boundary=eidolon-boundary"},  # WTF!!!! -- openai includes a rando boundary id. Bad for tests because it causes the cassettes uniqueness to fail.
         }
 
         if language:
             request["language"] = language
 
         if prompt:
             request["prompt"] = prompt
```

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm_message.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/llm_message.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 class SystemMessage(LLMMessage):
     type: str = "system"
     content: str
 
 
 # Derived classes for different types of message content parts
 class UserMessageText(BaseModel):
-    text: str
     type: Literal["text"] = "text"
+    text: str
 
 
 class UserMessageFileHandle(BaseModel):
     type: Literal["image", "audio", "file"]
     file: FileHandle
 
     @classmethod
@@ -100,15 +100,15 @@
 
         return messages
 
 
 # Derived UserMessage class
 class UserMessage(LLMMessage):
     type: str = "user"
-    content: List[UserMessageText | UserMessageFileHandle]
+    content: List[UserMessageText | UserMessageFile | UserMessageImage | UserMessageAudio]
 
 
 # ToolCall class
 
 
 # Derived AssistantMessage class
 class AssistantMessage(LLMMessage):
```

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/llm_unit.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/logic_unit.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/logic_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/memory_unit.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/memory_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/cpu/processing_unit.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/cpu/processing_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/agent_memory.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/agent_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/chroma_vector_store.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/chroma_vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/document.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/document.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/embeddings.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/file_memory.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/file_system_vector_store.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/file_system_vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/in_memory_file_memory.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/in_memory_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/local_file_memory.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/local_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/local_symbolic_memory.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/local_symbolic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/mongo_symbolic_memory.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/mongo_symbolic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/noop_memory.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/noop_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/s3_file_memory.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/s3_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/semantic_memory.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/semantic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/similarity_memory.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/similarity_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/memory/vector_store.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/memory/vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/authentication_processor.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/security/authentication_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/azure_authorizer.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/security/azure_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/functional_authorizer.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/security/functional_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/google_auth.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/security/google_auth.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/jwt_processor.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/security/jwt_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/permissions.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/security/permissions.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/process_authorizer.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/security/process_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/security_manager.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/security/security_manager.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/security/security_middleware.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/security/security_middleware.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/agent_contract.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/system/agent_contract.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/agent_controller.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/system/agent_controller.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/agent_machine.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/system/agent_machine.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,22 +191,24 @@
     async def download_file(self, process_id: str, file_id: str):
         """
         Download a file for this process
         :param process_id:
         :param file_id:
         :return: The file bytes
         """
-        contents, metadata = await self.process_file_system.read_file(process_id, file_id)
-        if not contents:
+        file = await self.process_file_system.read_file(process_id, file_id)
+        if not file:
             return JSONResponse(content={"detail": "File Not Found"}, status_code=404)
         headers = {
             "Content-Type": "application/octet-stream",
         }
-        if metadata and "mime_type" in metadata:
-            headers["mime-type"] = metadata["mime_type"]
+        contents, metadata = file
+        if metadata and "mimetype" in metadata:
+            headers["mime-type"] = metadata["mimetype"]
+            headers["Content-Type"] = metadata["mimetype"]
         return Response(content=contents, headers=headers, status_code=200)
 
     async def _delete_file(self, process_id: str, file_id: str):
         """
         Delete a file for this process
         :param process_id:
         :param file_id:
```

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/dynamic_middleware.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/system/dynamic_middleware.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/fn_handler.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/system/fn_handler.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/process_file_system.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/system/process_file_system.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 import json
 from pathlib import Path
 from typing import Optional, Dict, Tuple
-from uuid import uuid4
 
+import bson
 from pydantic import BaseModel
 
 from eidolon_ai_client.events import FileHandle
 from eidolon_ai_sdk.agent_os import AgentOS
 from eidolon_ai_sdk.agent_os_interfaces import ProcessFileSystem
 from eidolon_ai_sdk.system.reference_model import Specable
 
@@ -57,15 +57,15 @@
         """
         Writes the given `file_contents` to a new file within the context of the process_id.
         :param file_md:
         :param process_id:
         :param file_contents:
         :return:
         """
-        file_id = uuid4().hex
+        file_id = str(bson.ObjectId())
         await AgentOS.file_memory.mkdir(str(Path(self.root, process_id)), exist_ok=True)
         await AgentOS.file_memory.write_file(str(Path(self.root, process_id, file_id)), file_contents)
         md_to_write = {"process_id": process_id, "file_id": file_id}
         if file_md:
             md_to_write.update(file_md)
         path = str(Path(self.root, process_id, file_id + ".md"))
         await AgentOS.file_memory.write_file(path, json.dumps(md_to_write).encode())
```

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/processes.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/system/processes.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/reference_model.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/system/reference_model.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/resources/reference_resource.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/system/resources/reference_resource.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/system/resources/resources_base.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/system/resources/resources_base.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/class_utils.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/util/class_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/image_utils.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/util/image_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/replay.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/util/replay.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/schema_to_model.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/util/schema_to_model.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/str_utils.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/util/str_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/eidolon_ai_sdk/util/stream_collector.py` & `eidolon_ai_sdk-0.1.29/eidolon_ai_sdk/util/stream_collector.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/logging.conf` & `eidolon_ai_sdk-0.1.29/logging.conf`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.28/pyproject.toml` & `eidolon_ai_sdk-0.1.29/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eidolon-ai-sdk"
-version = "0.1.28"
+version = "0.1.29"
 description = "An Open Source Agent Services Framework"
 authors = ["Luke Lalor <lukehlalor@gmail.com>"]
 readme = "README.md"
 include = ["logging.conf"]
 
 [tool.poetry.urls]
 Github = "https://github.com/eidolon-ai/eidolon"
```

### Comparing `eidolon_ai_sdk-0.1.28/PKG-INFO` & `eidolon_ai_sdk-0.1.29/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eidolon-ai-sdk
-Version: 0.1.28
+Version: 0.1.29
 Summary: An Open Source Agent Services Framework
 Author: Luke Lalor
 Author-email: lukehlalor@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anthropic (>=0.21.3,<0.22.0)
```

