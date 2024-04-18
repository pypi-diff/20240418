# Comparing `tmp/langtrace_python_sdk-1.3.3.tar.gz` & `tmp/langtrace_python_sdk-1.3.4.tar.gz`

## Comparing `langtrace_python_sdk-1.3.3.tar` & `langtrace_python_sdk-1.3.4.tar`

### file list

```diff
@@ -1,88 +1,88 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/__init__.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/run_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/examples/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/examples/anthropic_example/__init__.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/examples/anthropic_example/completion.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/examples/chroma_example/__init__.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/examples/chroma_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/examples/cohere_example/__init__.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/examples/cohere_example/chat.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/examples/cohere_example/chat_stream.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/examples/cohere_example/embed_create.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/examples/fastapi_example/basic_route.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/examples/hiveagent_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/examples/langchain_example/__init__.py
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/examples/langchain_example/basic.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/examples/langchain_example/tool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/examples/llamaindex_example/__init__.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/examples/llamaindex_example/agent.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/examples/llamaindex_example/basic.py
--rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/examples/llamaindex_example/data/abramov.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/examples/openai/__init__.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/examples/openai/chat_completion.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/examples/openai/embeddings_create.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/examples/openai/function_calling.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/examples/openai/images_generate.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/examples/perplexity_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/examples/pinecone_example/__init__.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/examples/pinecone_example/basic.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/__init__.py
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/langtrace.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/constants/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/constants/instrumentation/__init__.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/constants/instrumentation/chroma.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/constants/instrumentation/cohere.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/constants/instrumentation/common.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/constants/instrumentation/openai.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/extensions/__init__.py
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/extensions/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
--rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/chroma/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
--rw-r--r--   0        0        0    16631 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/cohere/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/langchain/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
--rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
--rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
--rw-r--r--   0        0        0     7959 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
--rw-r--r--   0        0        0    31587 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/openai/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/utils/__init__.py
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/utils/llm.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/utils/with_root_span.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/tests/__init__.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/tests/utils.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/tests/anthropic/test_anthropic.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/tests/chroma/test_chroma.py
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/tests/langchain/test_langchain.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/tests/langchain/test_langchain_community.py
--rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/tests/langchain/test_langchain_core.py
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/tests/openai/test_chat_completion.py
--rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/tests/openai/test_image_generation.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/src/tests/pinecone/test_pinecone.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/LICENSE
--rw-r--r--   0        0        0     8031 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/README.md
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/__init__.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/run_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/examples/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/examples/anthropic_example/__init__.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/examples/anthropic_example/completion.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/examples/chroma_example/__init__.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/examples/chroma_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/examples/cohere_example/__init__.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/examples/cohere_example/chat.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/examples/cohere_example/chat_stream.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/examples/cohere_example/embed_create.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/examples/fastapi_example/basic_route.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/examples/hiveagent_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/examples/langchain_example/__init__.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/examples/langchain_example/basic.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/examples/langchain_example/tool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/examples/llamaindex_example/__init__.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/examples/llamaindex_example/agent.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/examples/llamaindex_example/basic.py
+-rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/examples/llamaindex_example/data/abramov.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/examples/openai/__init__.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/examples/openai/chat_completion.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/examples/openai/embeddings_create.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/examples/openai/function_calling.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/examples/openai/images_generate.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/examples/perplexity_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/examples/pinecone_example/__init__.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/examples/pinecone_example/basic.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/__init__.py
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/langtrace.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/constants/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/constants/instrumentation/__init__.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/constants/instrumentation/chroma.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/constants/instrumentation/cohere.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/constants/instrumentation/common.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/constants/instrumentation/openai.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/extensions/__init__.py
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/extensions/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
+-rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/chroma/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
+-rw-r--r--   0        0        0    16631 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/cohere/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/langchain/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
+-rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
+-rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
+-rw-r--r--   0        0        0     7959 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
+-rw-r--r--   0        0        0    31587 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/openai/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/utils/llm.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/utils/with_root_span.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/tests/__init__.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/tests/utils.py
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/tests/anthropic/test_anthropic.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/tests/chroma/test_chroma.py
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/tests/langchain/test_langchain.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/tests/langchain/test_langchain_community.py
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/tests/langchain/test_langchain_core.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/tests/openai/test_chat_completion.py
+-rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/tests/openai/test_image_generation.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/src/tests/pinecone/test_pinecone.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/LICENSE
+-rw-r--r--   0        0        0     8031 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/README.md
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     9094 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.4/PKG-INFO
```

### Comparing `langtrace_python_sdk-1.3.3/src/run_example.py` & `langtrace_python_sdk-1.3.4/src/run_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/examples/anthropic_example/completion.py` & `langtrace_python_sdk-1.3.4/src/examples/anthropic_example/completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/examples/chroma_example/basic.py` & `langtrace_python_sdk-1.3.4/src/examples/chroma_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/examples/cohere_example/chat.py` & `langtrace_python_sdk-1.3.4/src/examples/cohere_example/chat.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/examples/cohere_example/chat_stream.py` & `langtrace_python_sdk-1.3.4/src/examples/cohere_example/chat_stream.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/examples/cohere_example/embed_create.py` & `langtrace_python_sdk-1.3.4/src/examples/cohere_example/embed_create.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/examples/fastapi_example/basic_route.py` & `langtrace_python_sdk-1.3.4/src/examples/fastapi_example/basic_route.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/examples/langchain_example/basic.py` & `langtrace_python_sdk-1.3.4/src/examples/langchain_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/examples/langchain_example/tool.py` & `langtrace_python_sdk-1.3.4/src/examples/langchain_example/tool.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/examples/llamaindex_example/agent.py` & `langtrace_python_sdk-1.3.4/src/examples/llamaindex_example/agent.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/examples/llamaindex_example/basic.py` & `langtrace_python_sdk-1.3.4/src/examples/llamaindex_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/examples/llamaindex_example/data/abramov.txt` & `langtrace_python_sdk-1.3.4/src/examples/llamaindex_example/data/abramov.txt`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/examples/openai/chat_completion.py` & `langtrace_python_sdk-1.3.4/src/examples/openai/chat_completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/examples/openai/embeddings_create.py` & `langtrace_python_sdk-1.3.4/src/examples/openai/embeddings_create.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/examples/openai/function_calling.py` & `langtrace_python_sdk-1.3.4/src/examples/openai/function_calling.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/examples/perplexity_example/basic.py` & `langtrace_python_sdk-1.3.4/src/examples/perplexity_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/examples/pinecone_example/basic.py` & `langtrace_python_sdk-1.3.4/src/examples/pinecone_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/langtrace.py` & `langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/langtrace.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/constants/instrumentation/chroma.py` & `langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/constants/instrumentation/chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/constants/instrumentation/common.py` & `langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/constants/instrumentation/common.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/constants/instrumentation/openai.py` & `langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/constants/instrumentation/openai.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/extensions/langtrace_exporter.py` & `langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/extensions/langtrace_exporter.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py` & `langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/anthropic/patch.py` & `langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/anthropic/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py` & `langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/chroma/patch.py` & `langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/chroma/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py` & `langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/cohere/patch.py` & `langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/cohere/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py` & `langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/langchain/patch.py` & `langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/langchain/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py` & `langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py` & `langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py` & `langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py` & `langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py` & `langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py` & `langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py` & `langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/openai/patch.py` & `langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/openai/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py` & `langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/instrumentation/pinecone/patch.py` & `langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/instrumentation/pinecone/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/utils/llm.py` & `langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/utils/llm.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/langtrace_python_sdk/utils/with_root_span.py` & `langtrace_python_sdk-1.3.4/src/langtrace_python_sdk/utils/with_root_span.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/tests/utils.py` & `langtrace_python_sdk-1.3.4/src/tests/utils.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/tests/anthropic/test_anthropic.py` & `langtrace_python_sdk-1.3.4/src/tests/anthropic/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/tests/chroma/test_chroma.py` & `langtrace_python_sdk-1.3.4/src/tests/chroma/test_chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/tests/langchain/test_langchain.py` & `langtrace_python_sdk-1.3.4/src/tests/langchain/test_langchain.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/tests/langchain/test_langchain_community.py` & `langtrace_python_sdk-1.3.4/src/tests/langchain/test_langchain_community.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/tests/langchain/test_langchain_core.py` & `langtrace_python_sdk-1.3.4/src/tests/langchain/test_langchain_core.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/tests/openai/test_chat_completion.py` & `langtrace_python_sdk-1.3.4/src/tests/openai/test_chat_completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/tests/openai/test_image_generation.py` & `langtrace_python_sdk-1.3.4/src/tests/openai/test_image_generation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/src/tests/pinecone/test_pinecone.py` & `langtrace_python_sdk-1.3.4/src/tests/pinecone/test_pinecone.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/.gitignore` & `langtrace_python_sdk-1.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/LICENSE` & `langtrace_python_sdk-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/README.md` & `langtrace_python_sdk-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.3/pyproject.toml` & `langtrace_python_sdk-1.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 license = "Apache-2.0"
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  'trace-attributes',
+  'trace-attributes==1.0.32',
   'opentelemetry-api',
   'opentelemetry-sdk',
   'opentelemetry-instrumentation',
   'pinecone-client',
   'tiktoken'
 ]
```

### Comparing `langtrace_python_sdk-1.3.3/PKG-INFO` & `langtrace_python_sdk-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.3
 Name: langtrace-python-sdk
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python SDK for LangTrace
 Project-URL: Homepage, https://github.com/Scale3-Labs/langtrace-python-sdk
 Author-email: Scale3 Labs <engineering@scale3labs.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Requires-Dist: opentelemetry-api
 Requires-Dist: opentelemetry-instrumentation
 Requires-Dist: opentelemetry-sdk
 Requires-Dist: pinecone-client
 Requires-Dist: tiktoken
-Requires-Dist: trace-attributes
+Requires-Dist: trace-attributes==1.0.32
 Provides-Extra: dev
 Requires-Dist: anthropic; extra == 'dev'
 Requires-Dist: chromadb; extra == 'dev'
 Requires-Dist: cohere; extra == 'dev'
 Requires-Dist: langchain; extra == 'dev'
 Requires-Dist: langchain-openai; extra == 'dev'
 Requires-Dist: llama-index; extra == 'dev'
```

