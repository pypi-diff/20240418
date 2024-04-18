# Comparing `tmp/llmkira-1.0.0.tar.gz` & `tmp/llmkira-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmkira-1.0.0.tar", last modified: Wed Apr 17 06:20:08 2024, max compression
+gzip compressed data, was "llmkira-1.0.1.tar", last modified: Wed Apr 17 15:13:00 2024, max compression
```

## Comparing `llmkira-1.0.0.tar` & `llmkira-1.0.1.tar`

### file list

```diff
@@ -1,54 +1,58 @@
--rw-r--r--   0        0        0    11357 2024-04-17 06:19:52.611194 llmkira-1.0.0/LICENSE
--rw-r--r--   0        0        0     1030 2024-04-17 06:19:52.611194 llmkira-1.0.0/NOTICE.MD
--rw-r--r--   0        0        0     6859 2024-04-17 06:19:52.611194 llmkira-1.0.0/README.md
--rw-r--r--   0        0        0      730 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/__init__.py
--rw-r--r--   0        0        0      209 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/_exception.py
--rw-r--r--   0        0        0     3760 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/cache/__init__.py
--rw-r--r--   0        0        0     1216 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/cache/elara_runtime.py
--rw-r--r--   0        0        0     1426 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/cache/redis_runtime.py
--rw-r--r--   0        0        0     1118 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/cache/runtime_schema.py
--rw-r--r--   0        0        0     4235 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/doc_manager/__init__.py
--rw-r--r--   0        0        0      127 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/extra/plugins/__init__.py
--rw-r--r--   0        0        0     6726 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/extra/plugins/alarm/__init__.py
--rw-r--r--   0        0        0     6510 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/extra/plugins/search/__init__.py
--rw-r--r--   0        0        0     1774 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/extra/plugins/search/engine.py
--rw-r--r--   0        0        0        0 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/kv_manager/__init__.py
--rw-r--r--   0        0        0      626 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/kv_manager/_base.py
--rw-r--r--   0        0        0     1750 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/kv_manager/env.py
--rw-r--r--   0        0        0     4405 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/kv_manager/file.py
--rw-r--r--   0        0        0      929 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/kv_manager/instruction.py
--rw-r--r--   0        0        0     1070 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/kv_manager/tool_call.py
--rw-r--r--   0        0        0      637 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/memory/__init__.py
--rw-r--r--   0        0        0      729 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/memory/_base.py
--rw-r--r--   0        0        0     2324 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/memory/local_storage.py
--rw-r--r--   0        0        0     1070 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/memory/redis_storage/LICENSE
--rw-r--r--   0        0        0     2840 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/memory/redis_storage/__init__.py
--rw-r--r--   0        0        0     6192 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/memory/redis_storage/utils.py
--rw-r--r--   0        0        0      522 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/openai/__init__.py
--rw-r--r--   0        0        0     3431 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/openai/_excption.py
--rw-r--r--   0        0        0     7440 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/openai/cell.py
--rw-r--r--   0        0        0     7811 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/openai/request.py
--rw-r--r--   0        0        0      130 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/openapi/__init__.py
--rw-r--r--   0        0        0     2729 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/openapi/fuse/__init__.py
--rw-r--r--   0        0        0     4285 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/openapi/transducer/__init__.py
--rw-r--r--   0        0        0      799 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/openapi/transducer/default_factory.py
--rw-r--r--   0        0        0     1229 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/openapi/transducer/schema.py
--rw-r--r--   0        0        0     2079 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/openapi/trigger/__init__.py
--rw-r--r--   0        0        0      419 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/openapi/trigger/default_trigger.py
--rw-r--r--   0        0        0      321 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/sdk/__init__.py
--rw-r--r--   0        0        0     1069 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/sdk/tools/LICENSE
--rw-r--r--   0        0        0     4501 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/sdk/tools/__init__.py
--rw-r--r--   0        0        0      496 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/sdk/tools/error.py
--rw-r--r--   0        0        0     3373 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/sdk/tools/loader.py
--rw-r--r--   0        0        0     9551 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/sdk/tools/model.py
--rw-r--r--   0        0        0     3286 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/sdk/tools/register.py
--rw-r--r--   0        0        0    10397 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/sdk/tools/schema.py
--rw-r--r--   0        0        0     4233 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/sdk/utils.py
--rw-r--r--   0        0        0     4848 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/task/__init__.py
--rw-r--r--   0        0        0    22287 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/task/schema.py
--rw-r--r--   0        0        0      219 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/task/snapshot/__init__.py
--rw-r--r--   0        0        0      422 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/task/snapshot/_base.py
--rw-r--r--   0        0        0     1237 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/task/snapshot/local.py
--rw-r--r--   0        0        0     2835 2024-04-17 06:20:08.495237 llmkira-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1485 2024-04-17 06:19:52.635193 llmkira-1.0.0/tests/pydantic_error.py
--rw-r--r--   0        0        0    10079 1970-01-01 00:00:00.000000 llmkira-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-17 15:12:46.807127 llmkira-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1030 2024-04-17 15:12:46.807127 llmkira-1.0.1/NOTICE.MD
+-rw-r--r--   0        0        0     7325 2024-04-17 15:12:46.807127 llmkira-1.0.1/README.md
+-rw-r--r--   0        0        0      730 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/__init__.py
+-rw-r--r--   0        0        0      209 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/_exception.py
+-rw-r--r--   0        0        0     3760 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/cache/__init__.py
+-rw-r--r--   0        0        0     1216 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/cache/elara_runtime.py
+-rw-r--r--   0        0        0     1426 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/cache/redis_runtime.py
+-rw-r--r--   0        0        0     1118 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/cache/runtime_schema.py
+-rw-r--r--   0        0        0     4583 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/doc_manager/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/extra/plugins/__init__.py
+-rw-r--r--   0        0        0     6726 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/extra/plugins/alarm/__init__.py
+-rw-r--r--   0        0        0     6510 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/extra/plugins/search/__init__.py
+-rw-r--r--   0        0        0     1774 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/extra/plugins/search/engine.py
+-rw-r--r--   0        0        0     3473 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/extra/voice/__init__.py
+-rw-r--r--   0        0        0     3192 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/extra/voice_hook.py
+-rw-r--r--   0        0        0        0 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/kv_manager/__init__.py
+-rw-r--r--   0        0        0      626 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/kv_manager/_base.py
+-rw-r--r--   0        0        0     2193 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/kv_manager/env.py
+-rw-r--r--   0        0        0     4419 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/kv_manager/file.py
+-rw-r--r--   0        0        0      929 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/kv_manager/instruction.py
+-rw-r--r--   0        0        0     1512 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/kv_manager/time.py
+-rw-r--r--   0        0        0     1070 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/kv_manager/tool_call.py
+-rw-r--r--   0        0        0      637 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/memory/__init__.py
+-rw-r--r--   0        0        0      733 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/memory/_base.py
+-rw-r--r--   0        0        0     2381 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/memory/local_storage.py
+-rw-r--r--   0        0        0     1070 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/memory/redis_storage/LICENSE
+-rw-r--r--   0        0        0     2819 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/memory/redis_storage/__init__.py
+-rw-r--r--   0        0        0     6192 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/memory/redis_storage/utils.py
+-rw-r--r--   0        0        0      522 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/openai/__init__.py
+-rw-r--r--   0        0        0     3431 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/openai/_excption.py
+-rw-r--r--   0        0        0     7440 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/openai/cell.py
+-rw-r--r--   0        0        0     7845 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/openai/request.py
+-rw-r--r--   0        0        0      130 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/openapi/__init__.py
+-rw-r--r--   0        0        0     2729 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/openapi/fuse/__init__.py
+-rw-r--r--   0        0        0     1610 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/openapi/hook/__init__.py
+-rw-r--r--   0        0        0     4285 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/openapi/transducer/__init__.py
+-rw-r--r--   0        0        0      799 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/openapi/transducer/default_factory.py
+-rw-r--r--   0        0        0     1229 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/openapi/transducer/schema.py
+-rw-r--r--   0        0        0     2143 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/openapi/trigger/__init__.py
+-rw-r--r--   0        0        0      419 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/openapi/trigger/default_trigger.py
+-rw-r--r--   0        0        0      321 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/sdk/__init__.py
+-rw-r--r--   0        0        0     1069 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/sdk/tools/LICENSE
+-rw-r--r--   0        0        0     4501 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/sdk/tools/__init__.py
+-rw-r--r--   0        0        0      496 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/sdk/tools/error.py
+-rw-r--r--   0        0        0     3373 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/sdk/tools/loader.py
+-rw-r--r--   0        0        0     9551 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/sdk/tools/model.py
+-rw-r--r--   0        0        0     3286 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/sdk/tools/register.py
+-rw-r--r--   0        0        0    10397 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/sdk/tools/schema.py
+-rw-r--r--   0        0        0     4233 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/sdk/utils.py
+-rw-r--r--   0        0        0     4848 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/task/__init__.py
+-rw-r--r--   0        0        0    22287 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/task/schema.py
+-rw-r--r--   0        0        0      219 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/task/snapshot/__init__.py
+-rw-r--r--   0        0        0      422 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/task/snapshot/_base.py
+-rw-r--r--   0        0        0     1237 2024-04-17 15:12:46.827127 llmkira-1.0.1/llmkira/task/snapshot/local.py
+-rw-r--r--   0        0        0     2855 2024-04-17 15:13:00.807209 llmkira-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1485 2024-04-17 15:12:46.831127 llmkira-1.0.1/tests/pydantic_error.py
+-rw-r--r--   0        0        0    10580 1970-01-01 00:00:00.000000 llmkira-1.0.1/PKG-INFO
```

### Comparing `llmkira-1.0.0/LICENSE` & `llmkira-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/NOTICE.MD` & `llmkira-1.0.1/NOTICE.MD`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/README.md` & `llmkira-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 ------------------
 
 <p align="center">
 <a href="https://hub.docker.com/repository/docker/sudoskys/llmbot/general">
     <img src="https://img.shields.io/docker/pulls/sudoskys/llmbot" alt="docker">
 </a>
-<a href="https://github.com/llmkira/openaibot/actions/workflows/docker-ci.yaml">
-    <img src="https://github.com/llmkira/openaibot/actions/workflows/docker-ci.yaml/badge.svg" alt="docker workflow">
+<a href="https://badge.fury.io/py/llmkira">
+    <img src="https://badge.fury.io/py/llmkira.svg" alt="docker workflow">
 </a>
 <br />
 <a href="https://t.me/Openai_LLM">
     <img src="https://img.shields.io/badge/Join-Telegram-blue" alt="telegram">
 </a>
 <a href="https://discord.gg/6QHNdwhdE5">
     <img src="https://img.shields.io/badge/Join-Discord-blue" alt="discord">
@@ -44,22 +44,26 @@
 
 The model adheres to the Openai Schema, other models are not supported. Please adapt using gateways independently.
 
 | Demo                              |
 |-----------------------------------|
 | ![sticker](./docs/chain_chat.gif) |
 
-## 🍔 Roadmap
+## 🔨 Roadmap
 
 - [x] Removal of legacy code
 - [x] Deletion of metric system
 - [x] Deletion of model selection system, unified to OpenAI Schema
 - [x] Implementation of a more robust plugin system
 - [x] Project structure simplification
 - [x] Elimination of the Provider system
+- [x] Hook support.
+- [x] Access to TTS.
+- [ ] Add LLM reference support to the plugin environment. (extract && search in text)
+- [ ] Add standalone support for Openai's new Schema. (vision)
 
 ## 📦 Features
 
 - 🍪 A comprehensive plugin development ecosystem, adopting a classic design, and seamless integration with plugins
   through `pip` installation
 - 📝 Message system with no time or sender constraints, offering fully decoupled logics
 - 📬 Offers Login via a URL mechanism, providing a flexible and expandable authentication development solution
@@ -67,17 +71,17 @@
 - 📦 Support for plugins to access files
 - 🍟 Multi-platform support – extend new platforms by inheriting the base class
 - 🍔 Plugins can determine their appearance in new sessions dynamically, preventing performance degradation despite large
   amounts of plugins
 
 ### 🍔 Login Modes
 
-- `Login via url`: Use `/login token#https://provider.com` to Login. The program posts the token to the interface to
+- `Login via url`: Use `/login token$https://provider.com` to Login. The program posts the token to the interface to
   retrieve configuration information
-- `Login`: Use `/login https://api.com/v1#key#model` to login
+- `Login`: Use `/login https://api.com/v1$key$model` to login
 
 ### 🧀 Plugin Previews
 
 | Sticker Converter                   | Timer Function                  | Translate Function                           |
 |-------------------------------------|---------------------------------|----------------------------------------------|
 | ![sticker](./docs/sticker_func.gif) | ![timer](./docs/timer_func.gif) | ![translate](./docs/translate_file_func.gif) |
 
@@ -164,14 +168,27 @@
 ```
 
 ## 💻 How to Develop Plugins?
 
 Refer to the example plugins in the `plugins` directory and
 the [🧀 Plugin Development Document](https://llmkira.github.io/Docs/dev/basic) for plugin development documentation.
 
+### Hooks
+
+Hooks control the EventMessage in sender and receiver. For example, we have `voice_hook` in built-in hooks.
+
+you can enable it by setting `VOICE_REPLY_ME=true` in `.env`.
+
+```shell
+/env VOICE_REPLY_ME=true
+/env REECHO_VOICE_KEY=<key in dev.reecho.ai>
+```
+
+check the source code in `llmkira/extra/voice_hook.py`, learn to write your own hooks.
+
 ## 🧀 Sponsor
 
 [![sponsor](./.github/sponsor_ohmygpt.png)](https://www.ohmygpt.com)
 
 ## 📜 Notice
 
 > This project, named OpenAiBot, signifying "Open Artificial Intelligence Robot", is not officially affiliated with
```

#### html2text {}

```diff
@@ -5,66 +5,73 @@
                             _[_l_i_c_e_n_s_e_]_[_d_o_c_k_e_r_ _b_u_i_l_d_]
               _ð___©_ _D_e_p_l_o_y_ _D_o_c_s & _ð__§__ _D_e_v_ _D_o_c_s & _ð__¤__ _C_o_n_t_r_i_b_u_t_e
 > Don't hesitate to Star â­ï¸, Issue ð, and PR ð ï¸ > Python>=3.9 This
 project uses the ToolCall feature. It integrates a message queuing and snapshot
 system, offering plugin mechanisms and authentication prior to plugin
 execution. The model adheres to the Openai Schema, other models are not
 supported. Please adapt using gateways independently. | Demo | |---------------
---------------------| | ![sticker](./docs/chain_chat.gif) | ## ð Roadmap -
+--------------------| | ![sticker](./docs/chain_chat.gif) | ## ð¨ Roadmap -
 [x] Removal of legacy code - [x] Deletion of metric system - [x] Deletion of
 model selection system, unified to OpenAI Schema - [x] Implementation of a more
 robust plugin system - [x] Project structure simplification - [x] Elimination
-of the Provider system ## ð¦ Features - ðª A comprehensive plugin
-development ecosystem, adopting a classic design, and seamless integration with
-plugins through `pip` installation - ð Message system with no time or sender
-constraints, offering fully decoupled logics - ð¬ Offers Login via a URL
-mechanism, providing a flexible and expandable authentication development
-solution - ð° Empowers users to authorize plugin execution. Users can
-configure plugin environment variables at their discretion - ð¦ Support for
-plugins to access files - ð Multi-platform support â extend new platforms
-by inheriting the base class - ð Plugins can determine their appearance in
-new sessions dynamically, preventing performance degradation despite large
-amounts of plugins ### ð Login Modes - `Login via url`: Use `/login
-token#https://provider.com` to Login. The program posts the token to the
-interface to retrieve configuration information - `Login`: Use `/login https://
-api.com/v1#key#model` to login ### ð§ Plugin Previews | Sticker Converter |
-Timer Function | Translate Function | |-------------------------------------|--
--------------------------------|----------------------------------------------
-| | ![sticker](./docs/sticker_func.gif) | ![timer](./docs/timer_func.gif) | !
-[translate](./docs/translate_file_func.gif) | ### ð¬ Platform Support |
-Platform | Support | File System | Remarks | |----------|---------|------------
--|----------------------------------------| | Telegram | â | â | | |
-Discord | â | â | | | Kook | â | â | Does not support `triggering by
-reply` | | Slack | â | â | Does not support `triggering by reply` | | QQ |
-â | | | | Wechat | â | | | | Twitter | â | | | | Matrix | â | | | | IRC
-| â | | | | ... | | | Create Issue/PR | ## ð¦ Quick Start Refer to the
-[ð§ Deployment Document](https://llmkira.github.io/Docs/) for more
-information. ```shell # Install RabbitMQ docker pull rabbitmq:3.10-management
-docker run -d -p 5672:5672 -p 15672:15672 \ -e RABBITMQ_DEFAULT_USER=admin \ -
-e RABBITMQ_DEFAULT_PASS=8a8a8a \ --hostname myRabbit \ --name rabbitmq \
-rabbitmq:3.10-management docker ps -l # Install Project pip install pdm pdm
-install -G bot cp .env.exp .env && nano .env # Test pdm run python3
-start_sender.py pdm run python3 start_receiver.py # Host pdm start pm2.json ```
-### ð¥£ Docker Build Hub: [sudoskys/llmbot](https://hub.docker.com/repository/
-docker/sudoskys/llmbot/general) #### Automatic Docker/Docker-compose
-Installation If you are using a brand new server, you can use the following
-shell to automatically install this project. This script automatically installs
-the required services and maps ports using Docker methods. If you have deployed
-`redis`, `rabbitmq`, `mongodb`, please modify the `docker-compose.yml` file
-accordingly. ```shell curl -sSL https://raw.githubusercontent.com/LLMKira/
-Openaibot/main/deploy.sh | bash ``` #### Manual Docker-compose Installation
-```shell git clone https://github.com/LlmKira/Openaibot.git cd Openaibot cp
-.env.exp .env&&nano .env docker-compose -f docker-compose.yml up -d ``` Update
-image using `docker-compose pull`. Use `docker exec -it llmbot /bin/bash` to
-view Shell in Docker, enter `exit` to exit. ## ðª Slash Commands ```shell
-clear - Deletes chat records help - Displays documentation chat - Conversation
-task - Use a function to converse ask - Disable function-based conversations
-tool - Lists all functions login - Login auth - Authorize a function env -
-Environment variables of the function ``` ## ð» How to Develop Plugins? Refer
-to the example plugins in the `plugins` directory and the [ð§ Plugin
-Development Document](https://llmkira.github.io/Docs/dev/basic) for plugin
-development documentation. ## ð§ Sponsor [![sponsor](./.github/
+of the Provider system - [x] Hook support. - [x] Access to TTS. - [ ] Add LLM
+reference support to the plugin environment. (extract && search in text) - [ ]
+Add standalone support for Openai's new Schema. (vision) ## ð¦ Features -
+ðª A comprehensive plugin development ecosystem, adopting a classic design,
+and seamless integration with plugins through `pip` installation - ð Message
+system with no time or sender constraints, offering fully decoupled logics -
+ð¬ Offers Login via a URL mechanism, providing a flexible and expandable
+authentication development solution - ð° Empowers users to authorize plugin
+execution. Users can configure plugin environment variables at their discretion
+- ð¦ Support for plugins to access files - ð Multi-platform support â
+extend new platforms by inheriting the base class - ð Plugins can determine
+their appearance in new sessions dynamically, preventing performance
+degradation despite large amounts of plugins ### ð Login Modes - `Login via
+url`: Use `/login token$https://provider.com` to Login. The program posts the
+token to the interface to retrieve configuration information - `Login`: Use `/
+login https://api.com/v1$key$model` to login ### ð§ Plugin Previews | Sticker
+Converter | Timer Function | Translate Function | |----------------------------
+---------|---------------------------------|-----------------------------------
+-----------| | ![sticker](./docs/sticker_func.gif) | ![timer](./docs/
+timer_func.gif) | ![translate](./docs/translate_file_func.gif) | ### ð¬
+Platform Support | Platform | Support | File System | Remarks | |----------|---
+------|-------------|----------------------------------------| | Telegram | â
+| â | | | Discord | â | â | | | Kook | â | â | Does not support
+`triggering by reply` | | Slack | â | â | Does not support `triggering by
+reply` | | QQ | â | | | | Wechat | â | | | | Twitter | â | | | | Matrix |
+â | | | | IRC | â | | | | ... | | | Create Issue/PR | ## ð¦ Quick Start
+Refer to the [ð§ Deployment Document](https://llmkira.github.io/Docs/) for
+more information. ```shell # Install RabbitMQ docker pull rabbitmq:3.10-
+management docker run -d -p 5672:5672 -p 15672:15672 \ -
+e RABBITMQ_DEFAULT_USER=admin \ -e RABBITMQ_DEFAULT_PASS=8a8a8a \ --hostname
+myRabbit \ --name rabbitmq \ rabbitmq:3.10-management docker ps -l # Install
+Project pip install pdm pdm install -G bot cp .env.exp .env && nano .env # Test
+pdm run python3 start_sender.py pdm run python3 start_receiver.py # Host pdm
+start pm2.json ``` ### ð¥£ Docker Build Hub: [sudoskys/llmbot](https://
+hub.docker.com/repository/docker/sudoskys/llmbot/general) #### Automatic
+Docker/Docker-compose Installation If you are using a brand new server, you can
+use the following shell to automatically install this project. This script
+automatically installs the required services and maps ports using Docker
+methods. If you have deployed `redis`, `rabbitmq`, `mongodb`, please modify the
+`docker-compose.yml` file accordingly. ```shell curl -sSL https://
+raw.githubusercontent.com/LLMKira/Openaibot/main/deploy.sh | bash ``` ####
+Manual Docker-compose Installation ```shell git clone https://github.com/
+LlmKira/Openaibot.git cd Openaibot cp .env.exp .env&&nano .env docker-compose -
+f docker-compose.yml up -d ``` Update image using `docker-compose pull`. Use
+`docker exec -it llmbot /bin/bash` to view Shell in Docker, enter `exit` to
+exit. ## ðª Slash Commands ```shell clear - Deletes chat records help -
+Displays documentation chat - Conversation task - Use a function to converse
+ask - Disable function-based conversations tool - Lists all functions login -
+Login auth - Authorize a function env - Environment variables of the function
+``` ## ð» How to Develop Plugins? Refer to the example plugins in the
+`plugins` directory and the [ð§ Plugin Development Document](https://
+llmkira.github.io/Docs/dev/basic) for plugin development documentation. ###
+Hooks Hooks control the EventMessage in sender and receiver. For example, we
+have `voice_hook` in built-in hooks. you can enable it by setting
+`VOICE_REPLY_ME=true` in `.env`. ```shell /env VOICE_REPLY_ME=true /env
+REECHO_VOICE_KEY= ``` check the source code in `llmkira/extra/voice_hook.py`,
+learn to write your own hooks. ## ð§ Sponsor [![sponsor](./.github/
 sponsor_ohmygpt.png)](https://www.ohmygpt.com) ## ð Notice > This project,
 named OpenAiBot, signifying "Open Artificial Intelligence Robot", is not
 officially affiliated with > OpenAI. [![FOSSA Status](https://app.fossa.com/
 api/projects/git%2Bgithub.com%2Fsudoskys%2FOpenaibot.svg?type=small)](https://
 app.fossa.com/projects/git%2Bgithub.com%2Fsudoskys%2FOpenaibot?ref=badge_small)
```

### Comparing `llmkira-1.0.0/llmkira/__init__.py` & `llmkira-1.0.1/llmkira/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/cache/__init__.py` & `llmkira-1.0.1/llmkira/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/cache/elara_runtime.py` & `llmkira-1.0.1/llmkira/cache/elara_runtime.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/cache/redis_runtime.py` & `llmkira-1.0.1/llmkira/cache/redis_runtime.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/cache/runtime_schema.py` & `llmkira-1.0.1/llmkira/cache/runtime_schema.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/doc_manager/__init__.py` & `llmkira-1.0.1/llmkira/doc_manager/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -107,19 +107,26 @@
     @model_validator(mode="after")
     def mongodb_validator(self):
         try:
             client = MongoClient(
                 self.mongodb_dsn, serverSelectionTimeoutMS=1000
             )  # 设置超时时间
             client.admin.command("ping")
+            # 获取服务器信息
+            client.server_info()
+            # 尝试执行需要管理员权限的命令
+            client.admin.command("listDatabases")
         except ServerSelectionTimeoutError:
             self.available = False
             logger.warning(
                 f"\n🍀MongoDB Connection Error -- timeout when connecting to {self.mongodb_dsn}"
             )
+        except pymongo.errors.OperationFailure:
+            self.available = False
+            logger.warning("\n🍀MongoDB Connection Error -- insufficient permissions")
         except Exception as e:
             self.available = False
             logger.warning(f"\n🍀MongoDB Connection Error -- error {e}")
         else:
             logger.success(f"\n🍀MongoDB Connection Success --dsn {self.mongodb_dsn}")
         return self
```

### Comparing `llmkira-1.0.0/llmkira/extra/plugins/alarm/__init__.py` & `llmkira-1.0.1/llmkira/extra/plugins/alarm/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/extra/plugins/search/__init__.py` & `llmkira-1.0.1/llmkira/extra/plugins/search/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/extra/plugins/search/engine.py` & `llmkira-1.0.1/llmkira/extra/plugins/search/engine.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/kv_manager/_base.py` & `llmkira-1.0.1/llmkira/kv_manager/_base.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/kv_manager/env.py` & `llmkira-1.0.1/llmkira/kv_manager/env.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,53 +8,65 @@
 
 
 def parse_env_string(env_string) -> Dict[str, str]:
     if not env_string.endswith(";"):
         env_string = env_string + ";"
     pattern = r"(\w+)\s*=\s*(.*?)\s*;"
     matches = re.findall(pattern, env_string, re.MULTILINE)
-    _env_table = {}
+    env_table = {}
     for match in matches:
-        _key = match[0]
-        _value = match[1]
-        _value = _value.strip().strip('"')
-        _key = _key.upper()
-        _env_table[_key] = _value
-    return _env_table
+        env_key = f"{match[0]}"
+        env_value = f"{match[1]}"
+        env_value = env_value.strip().strip('"')
+        env_key = env_key.upper()
+        if env_value.lower() == "none":
+            env_value = None
+        env_table[env_key] = env_value
+    return env_table
 
 
 class EnvManager(KvManager):
     def __init__(self, user_id: str):
         self.user_id = str(user_id)
 
     def prefix(self, key: str) -> str:
         return f"env:{key}"
 
+    async def get_env(self, env_name, default) -> Optional[str]:
+        result = await self.read_env()
+        if not result:
+            return default
+        return result.get(env_name, default)
+
     async def read_env(self) -> Optional[dict]:
         result = await self.read_data(self.user_id)
         if not result:
             return None
         try:
+            if isinstance(result, dict):
+                return result
             return json.loads(result)
         except Exception as e:
             logger.error(
                 f"operation failed: env string cant be parsed by json.loads {e}"
             )
             return None
 
     async def set_env(
-        self, env_value: Union[dict, str], update=False
+        self, env_value: Union[dict, str], update=False, return_all=False
     ) -> Dict[str, str]:
         current_env = {}
         if update:
             current_env = await self.read_env()
             if not current_env:
                 current_env = {}
         if isinstance(env_value, str):
             env_map = parse_env_string(env_value)
         elif isinstance(env_value, dict):
             env_map = env_value
         else:
             raise ValueError("Env String Should be dict or str")
         current_env.update(env_map)
         await self.save_data(self.user_id, json.dumps(current_env))
+        if return_all:
+            return current_env
         return env_map
```

### Comparing `llmkira-1.0.0/llmkira/kv_manager/file.py` & `llmkira-1.0.1/llmkira/kv_manager/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     return short_id
 
 
 class File(BaseModel):
     creator: str = Field(description="创建用户")
     file_name: str = Field(description="文件名")
     file_key: str = Field(description="文件 Key")
-    caption: Optional[str] = Field(description="文件描述")
+    caption: Optional[str] = Field(default=None, description="文件描述")
 
     async def download_file(self) -> Optional[bytes]:
         """
         Download the file from the cache.
         If the file is not found in the cache, the method will return None.
         :return: The file data if found, otherwise None.
         """
```

### Comparing `llmkira-1.0.0/llmkira/kv_manager/instruction.py` & `llmkira-1.0.1/llmkira/kv_manager/instruction.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/kv_manager/tool_call.py` & `llmkira-1.0.1/llmkira/kv_manager/tool_call.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/memory/__init__.py` & `llmkira-1.0.1/llmkira/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/memory/_base.py` & `llmkira-1.0.1/llmkira/memory/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,19 +13,19 @@
         return self
 
     @abstractmethod
     async def read(self, lines: int) -> List[str]:
         ...
 
     @abstractmethod
-    async def append(self, message: List[BaseModel]):
-        _json_lines = [m.model_dump_json(indent=None) for m in message]
+    async def append(self, messages: List[BaseModel]):
+        _json_lines = [m.model_dump_json(indent=None) for m in messages]
         ...
 
     @abstractmethod
-    async def write(self, message: List[BaseModel]):
-        _json_lines = [m.model_dump_json(indent=None) for m in message]
+    async def write(self, messages: List[BaseModel]):
+        _json_lines = [m.model_dump_json(indent=None) for m in messages]
         ...
 
     @abstractmethod
     async def clear(self):
         ...
```

### Comparing `llmkira-1.0.0/llmkira/memory/local_storage.py` & `llmkira-1.0.1/llmkira/memory/local_storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,21 +49,23 @@
             if not self.path.exists():
                 return result
             with FileReadBackwards(str(self.path), encoding="utf-8") as frb:
                 for i, line in enumerate(frb):
                     if i >= lines:
                         break
                     result.append(line)
+            # 逆序
+            result = result[::-1]
             return result
 
-    async def write(self, message: List[BaseModel]):
+    async def write(self, messages: List[BaseModel]):
         async with self.lock:
             async with AIOFile(str(self.path), "w") as afp:
                 writer = Writer(afp)
-                for m in message:
+                for m in messages:
                     _json_line = m.model_dump_json(indent=None)
                     await writer(_json_line + "\n")
                 await afp.fsync()
 
     async def clear(self):
         async with self.lock:
             if not self.path.exists():
```

### Comparing `llmkira-1.0.0/llmkira/memory/redis_storage/LICENSE` & `llmkira-1.0.1/llmkira/memory/redis_storage/LICENSE`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/memory/redis_storage/__init__.py` & `llmkira-1.0.1/llmkira/memory/redis_storage/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf-8 -*-
 # Source: https://github.com/langchain-ai/langchain/blob/master/libs/langchain/langchain/utilities/redis.py
 from __future__ import annotations
 
-import json
 from typing import List
 
 import redis
 from loguru import logger
 from pydantic import BaseModel
 from pydantic import Field, model_validator
 from pydantic_settings import BaseSettings, SettingsConfigDict
@@ -60,23 +59,23 @@
 
     @property
     def key(self) -> str:
         return self.key_prefix + self.session_id
 
     async def read(self, lines: int) -> List[str]:
         _items = self.redis_client.lrange(self.key, 0, lines - 1)
-        items = [json.loads(m.decode("utf-8")) for m in _items[::-1]]
+        items = [m.decode("utf-8") for m in _items[::-1]]
         return items
 
-    async def append(self, message: List[BaseModel]):
-        for m in message:
-            message_json = m.json()
-            await self.redis_client.lpush(self.key, message_json)
+    async def append(self, messages: List[BaseModel]):
+        for m in messages:
+            message_json = m.model_dump_json()
+            self.redis_client.lpush(self.key, message_json)
             if self.ttl:
-                await self.redis_client.expire(self.key, self.ttl)
+                self.redis_client.expire(self.key, self.ttl)
 
-    async def write(self, message: List[BaseModel]):
+    async def write(self, messages: List[BaseModel]):
         self.clear()
-        await self.append(message)
+        self.append(messages)
 
-    def clear(self) -> None:
+    async def clear(self) -> None:
         self.redis_client.delete(self.key)
```

### Comparing `llmkira-1.0.0/llmkira/memory/redis_storage/utils.py` & `llmkira-1.0.1/llmkira/memory/redis_storage/utils.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/openai/__init__.py` & `llmkira-1.0.1/llmkira/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/openai/_excption.py` & `llmkira-1.0.1/llmkira/openai/_excption.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/openai/cell.py` & `llmkira-1.0.1/llmkira/openai/cell.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/openai/request.py` & `llmkira-1.0.1/llmkira/openai/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     ToolChoice,
     Message,
     AssistantMessage,
     CommonTool,
     ToolCall,
     ToolMessage,
     UserMessage,
+    SystemMessage,
 )
 
 
 class OpenAICredential(BaseModel):
     api_key: SecretStr
     base_url: str = "https://api.openai.com/v1"
     default_headers: dict = {"x-foo": "true"}
@@ -94,17 +95,17 @@
 
 
 class OpenAI(BaseModel):
     class ResponseFormat(BaseModel):
         type: Literal["json_object", "text"] = "text"
 
     model: str
-    messages: List[Union[Message, AssistantMessage, ToolMessage, UserMessage]] = Field(
-        ..., description="Messages"
-    )
+    messages: List[
+        Union[Message, AssistantMessage, ToolMessage, UserMessage, SystemMessage]
+    ] = Field(..., description="Messages")
 
     @field_validator("messages")
     def check_messages(cls, v):
         if not v:
             raise ValueError("messages cannot be empty")
         return v
```

### Comparing `llmkira-1.0.0/llmkira/openapi/fuse/__init__.py` & `llmkira-1.0.1/llmkira/openapi/fuse/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/openapi/transducer/__init__.py` & `llmkira-1.0.1/llmkira/openapi/transducer/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/openapi/transducer/default_factory.py` & `llmkira-1.0.1/llmkira/openapi/transducer/default_factory.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/openapi/transducer/schema.py` & `llmkira-1.0.1/llmkira/openapi/transducer/schema.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/openapi/trigger/__init__.py` & `llmkira-1.0.1/llmkira/openapi/trigger/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,18 +9,22 @@
 # 管道前置触发管理器，注册触发词或禁止触发词
 ######
 
 
 import inspect
 from functools import wraps
 from typing import Literal, List, Callable
+from typing import TYPE_CHECKING
 
 from loguru import logger
 from pydantic import BaseModel, Field
 
+if TYPE_CHECKING:
+    pass
+
 
 class Trigger(BaseModel):
     on_func: Callable = None
     on_platform: str
     action: Literal["allow", "deny"] = "allow"
     priority: int = Field(default=0, ge=-100, le=100)
     message: str = Field(default="Trigger deny your message")
@@ -33,15 +37,15 @@
 
 __trigger_phrases__: List[Trigger] = []
 
 
 async def get_trigger_loop(platform_name: str, message: str, uid: str = None):
     """
     receiver builder
-    message: "RawMessage"
+    message: Message Content
     :return 如果有触发，则返回触发的action，否则返回None 代表没有操作
     """
     sorted(__trigger_phrases__, key=lambda x: x.priority)
     if not message:
         message = ""
     for trigger in __trigger_phrases__:
         if trigger.on_platform == platform_name:
```

### Comparing `llmkira-1.0.0/llmkira/sdk/tools/LICENSE` & `llmkira-1.0.1/llmkira/sdk/tools/LICENSE`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/sdk/tools/__init__.py` & `llmkira-1.0.1/llmkira/sdk/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/sdk/tools/loader.py` & `llmkira-1.0.1/llmkira/sdk/tools/loader.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/sdk/tools/model.py` & `llmkira-1.0.1/llmkira/sdk/tools/model.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/sdk/tools/register.py` & `llmkira-1.0.1/llmkira/sdk/tools/register.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/sdk/tools/schema.py` & `llmkira-1.0.1/llmkira/sdk/tools/schema.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/sdk/utils.py` & `llmkira-1.0.1/llmkira/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/task/__init__.py` & `llmkira-1.0.1/llmkira/task/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/task/schema.py` & `llmkira-1.0.1/llmkira/task/schema.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/llmkira/task/snapshot/local.py` & `llmkira-1.0.1/llmkira/task/snapshot/local.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/pyproject.toml` & `llmkira-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llmkira"
-version = "1.0.0"
+version = "1.0.1"
 description = "A chain message bot based on OpenAI"
 authors = [
     { name = "sudoskys", email = "me@dianas.cyou" },
     { name = "llmkira", email = "me@dianas.cyou" },
 ]
 dependencies = [
     "pathlib>=1.0.1",
@@ -58,32 +58,32 @@
     "curl-cffi>=0.6.2",
     "deprecated>=1.2.14",
     "aiofile>=3.8.8",
     "file-read-backwards>=3.0.0",
     "apscheduler>=3.10.4",
     "montydb[lmdb]>=2.5.2",
     "pymongo>=4.6.3",
+    "fast-langdetect>=0.1.0",
 ]
 requires-python = ">=3.9,<3.12"
 readme = "README.md"
 keywords = [
     "llmbot",
     "llmkira",
     "openai",
     "chatgpt",
-    "telegram",
-    "bot",
+    "llm",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
 ]
 
 [project.license]
-text = "GPL3"
+text = "Apache-2.0"
 
 [project.urls]
 homepage = "https://llmkira.github.io/Docs/"
 repository = "https://github.com/LlmKira/Openaibot"
 
 [project.optional-dependencies]
 bot = [
```

### Comparing `llmkira-1.0.0/tests/pydantic_error.py` & `llmkira-1.0.1/tests/pydantic_error.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.0/PKG-INFO` & `llmkira-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: llmkira
-Version: 1.0.0
+Version: 1.0.1
 Summary: A chain message bot based on OpenAI
-Keywords: llmbot,llmkira,openai,chatgpt,telegram,bot
+Keywords: llmbot,llmkira,openai,chatgpt,llm
 Home-page: https://llmkira.github.io/Docs/
 Author-Email: sudoskys <me@dianas.cyou>, llmkira <me@dianas.cyou>
-License: GPL3
+License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Project-URL: Homepage, https://llmkira.github.io/Docs/
 Project-URL: Repository, https://github.com/LlmKira/Openaibot
 Requires-Python: <3.12,>=3.9
 Requires-Dist: pathlib>=1.0.1
 Requires-Dist: pydantic>=2.0.0
@@ -62,14 +62,15 @@
 Requires-Dist: curl-cffi>=0.6.2
 Requires-Dist: deprecated>=1.2.14
 Requires-Dist: aiofile>=3.8.8
 Requires-Dist: file-read-backwards>=3.0.0
 Requires-Dist: apscheduler>=3.10.4
 Requires-Dist: montydb[lmdb]>=2.5.2
 Requires-Dist: pymongo>=4.6.3
+Requires-Dist: fast-langdetect>=0.1.0
 Requires-Dist: hikari==2.0.0.dev121; extra == "bot"
 Requires-Dist: hikari-crescent<1.0.0,>=0.6.4; extra == "bot"
 Requires-Dist: khl-py<1.0.0,>=0.3.17; extra == "bot"
 Requires-Dist: slack-bolt<2.0.0,>=1.18.0; extra == "bot"
 Requires-Dist: hikari==2.0.0.dev121; extra == "testing"
 Requires-Dist: hikari-crescent<1.0.0,>=0.6.4; extra == "testing"
 Requires-Dist: khl-py<1.0.0,>=0.3.17; extra == "testing"
@@ -83,16 +84,16 @@
 
 ------------------
 
 <p align="center">
 <a href="https://hub.docker.com/repository/docker/sudoskys/llmbot/general">
     <img src="https://img.shields.io/docker/pulls/sudoskys/llmbot" alt="docker">
 </a>
-<a href="https://github.com/llmkira/openaibot/actions/workflows/docker-ci.yaml">
-    <img src="https://github.com/llmkira/openaibot/actions/workflows/docker-ci.yaml/badge.svg" alt="docker workflow">
+<a href="https://badge.fury.io/py/llmkira">
+    <img src="https://badge.fury.io/py/llmkira.svg" alt="docker workflow">
 </a>
 <br />
 <a href="https://t.me/Openai_LLM">
     <img src="https://img.shields.io/badge/Join-Telegram-blue" alt="telegram">
 </a>
 <a href="https://discord.gg/6QHNdwhdE5">
     <img src="https://img.shields.io/badge/Join-Discord-blue" alt="discord">
@@ -125,22 +126,26 @@
 
 The model adheres to the Openai Schema, other models are not supported. Please adapt using gateways independently.
 
 | Demo                              |
 |-----------------------------------|
 | ![sticker](./docs/chain_chat.gif) |
 
-## 🍔 Roadmap
+## 🔨 Roadmap
 
 - [x] Removal of legacy code
 - [x] Deletion of metric system
 - [x] Deletion of model selection system, unified to OpenAI Schema
 - [x] Implementation of a more robust plugin system
 - [x] Project structure simplification
 - [x] Elimination of the Provider system
+- [x] Hook support.
+- [x] Access to TTS.
+- [ ] Add LLM reference support to the plugin environment. (extract && search in text)
+- [ ] Add standalone support for Openai's new Schema. (vision)
 
 ## 📦 Features
 
 - 🍪 A comprehensive plugin development ecosystem, adopting a classic design, and seamless integration with plugins
   through `pip` installation
 - 📝 Message system with no time or sender constraints, offering fully decoupled logics
 - 📬 Offers Login via a URL mechanism, providing a flexible and expandable authentication development solution
@@ -148,17 +153,17 @@
 - 📦 Support for plugins to access files
 - 🍟 Multi-platform support – extend new platforms by inheriting the base class
 - 🍔 Plugins can determine their appearance in new sessions dynamically, preventing performance degradation despite large
   amounts of plugins
 
 ### 🍔 Login Modes
 
-- `Login via url`: Use `/login token#https://provider.com` to Login. The program posts the token to the interface to
+- `Login via url`: Use `/login token$https://provider.com` to Login. The program posts the token to the interface to
   retrieve configuration information
-- `Login`: Use `/login https://api.com/v1#key#model` to login
+- `Login`: Use `/login https://api.com/v1$key$model` to login
 
 ### 🧀 Plugin Previews
 
 | Sticker Converter                   | Timer Function                  | Translate Function                           |
 |-------------------------------------|---------------------------------|----------------------------------------------|
 | ![sticker](./docs/sticker_func.gif) | ![timer](./docs/timer_func.gif) | ![translate](./docs/translate_file_func.gif) |
 
@@ -245,14 +250,27 @@
 ```
 
 ## 💻 How to Develop Plugins?
 
 Refer to the example plugins in the `plugins` directory and
 the [🧀 Plugin Development Document](https://llmkira.github.io/Docs/dev/basic) for plugin development documentation.
 
+### Hooks
+
+Hooks control the EventMessage in sender and receiver. For example, we have `voice_hook` in built-in hooks.
+
+you can enable it by setting `VOICE_REPLY_ME=true` in `.env`.
+
+```shell
+/env VOICE_REPLY_ME=true
+/env REECHO_VOICE_KEY=<key in dev.reecho.ai>
+```
+
+check the source code in `llmkira/extra/voice_hook.py`, learn to write your own hooks.
+
 ## 🧀 Sponsor
 
 [![sponsor](./.github/sponsor_ohmygpt.png)](https://www.ohmygpt.com)
 
 ## 📜 Notice
 
 > This project, named OpenAiBot, signifying "Open Artificial Intelligence Robot", is not officially affiliated with
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: llmkira Version: 1.0.0 Summary: A chain message bot
-based on OpenAI Keywords: llmbot,llmkira,openai,chatgpt,telegram,bot Home-page:
-https://llmkira.github.io/Docs/ Author-Email: sudoskys
+Metadata-Version: 2.1 Name: llmkira Version: 1.0.1 Summary: A chain message bot
+based on OpenAI Keywords: llmbot,llmkira,openai,chatgpt,llm Home-page: https://
+llmkira.github.io/Docs/ Author-Email: sudoskys
 dianas.cyou>, llmkira
-dianas.cyou> License: GPL3 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9 Project-URL: Homepage, https:
-//llmkira.github.io/Docs/ Project-URL: Repository, https://github.com/LlmKira/
-Openaibot Requires-Python: <3.12,>=3.9 Requires-Dist: pathlib>=1.0.1 Requires-
-Dist: pydantic>=2.0.0 Requires-Dist: loguru>=0.5.3 Requires-Dist: httpx>=0.24.1
-Requires-Dist: socksio<2.0.0,>=1.0.0 Requires-Dist: python-dotenv<2.0.0,>=1.0.0
-Requires-Dist: redis>=4.5.4 Requires-Dist: aio-pika<10.0.0,>=9.3.0 Requires-
-Dist: arclet-alconna<2.0.0,>=1.7.26 Requires-Dist: shortuuid<2.0.0,>=1.0.11
-Requires-Dist: tiktoken<1.0.0,>=0.5.1 Requires-Dist: nest-asyncio<2.0.0,>=1.5.8
-Requires-Dist: contextvars<3.0,>=2.4 Requires-Dist:
+dianas.cyou> License: Apache-2.0 Classifier: Programming Language :: Python ::
+3 Classifier: Programming Language :: Python :: 3.9 Project-URL: Homepage,
+https://llmkira.github.io/Docs/ Project-URL: Repository, https://github.com/
+LlmKira/Openaibot Requires-Python: <3.12,>=3.9 Requires-Dist: pathlib>=1.0.1
+Requires-Dist: pydantic>=2.0.0 Requires-Dist: loguru>=0.5.3 Requires-Dist:
+httpx>=0.24.1 Requires-Dist: socksio<2.0.0,>=1.0.0 Requires-Dist: python-
+dotenv<2.0.0,>=1.0.0 Requires-Dist: redis>=4.5.4 Requires-Dist: aio-
+pika<10.0.0,>=9.3.0 Requires-Dist: arclet-alconna<2.0.0,>=1.7.26 Requires-Dist:
+shortuuid<2.0.0,>=1.0.11 Requires-Dist: tiktoken<1.0.0,>=0.5.1 Requires-Dist:
+nest-asyncio<2.0.0,>=1.5.8 Requires-Dist: contextvars<3.0,>=2.4 Requires-Dist:
 pytz<2024.0.0,>=2023.3.post1 Requires-Dist: numpy<2.0.0,>=1.24.0 Requires-Dist:
 fasttext-wheel<1.0.0,>=0.9.2 Requires-Dist: tenacity<9.0.0,>=8.2.3 Requires-
 Dist: pysocks<2.0.0,>=1.7.1 Requires-Dist: flask-sqlalchemy<4.0.0,>=3.1.1
 Requires-Dist: emoji<3.0.0,>=2.8.0 Requires-Dist: websocket<1.0.0,>=0.2.1
 Requires-Dist: wrapt<2.0.0,>=1.11.0 Requires-Dist: dynaconf<4.0.0,>=3.2.3
 Requires-Dist: rich<14.0.0,>=13.6.0 Requires-Dist: importlib-
 metadata<7.0.0,>=6.8.0 Requires-Dist: sentry-sdk<2.0.0,>=1.34.0 Requires-Dist:
@@ -29,86 +29,94 @@
 Requires-Dist: inscriptis<3.0.0,>=2.3.2 Requires-Dist: aiohttp<4.0.0,>=3.8.6
 Requires-Dist: pytelegrambotapi<5.0.0,>=4.14.0 Requires-Dist: ffmpeg-
 python<1.0.0,>=0.2.0 Requires-Dist: duckduckgo-search<4.0.0,>=3.9.5 Requires-
 Dist: flask<4.0.0,>=3.0.0 Requires-Dist: telegramify-markdown>=0.1.2 Requires-
 Dist: json-repair>=0.13.0 Requires-Dist: curl-cffi>=0.6.2 Requires-Dist:
 deprecated>=1.2.14 Requires-Dist: aiofile>=3.8.8 Requires-Dist: file-read-
 backwards>=3.0.0 Requires-Dist: apscheduler>=3.10.4 Requires-Dist: montydb
-[lmdb]>=2.5.2 Requires-Dist: pymongo>=4.6.3 Requires-Dist:
-hikari==2.0.0.dev121; extra == "bot" Requires-Dist: hikari-
-crescent<1.0.0,>=0.6.4; extra == "bot" Requires-Dist: khl-py<1.0.0,>=0.3.17;
-extra == "bot" Requires-Dist: slack-bolt<2.0.0,>=1.18.0; extra == "bot"
-Requires-Dist: hikari==2.0.0.dev121; extra == "testing" Requires-Dist: hikari-
-crescent<1.0.0,>=0.6.4; extra == "testing" Requires-Dist: khl-
-py<1.0.0,>=0.3.17; extra == "testing" Requires-Dist: slack-bolt<2.0.0,>=1.18.0;
-extra == "testing" Requires-Dist: pre-commit<3.5.0,>=2.15.0; extra == "testing"
-Provides-Extra: bot Provides-Extra: testing Description-Content-Type: text/
-markdown ![cover](https://raw.githubusercontent.com/LlmKira/.github/main/
-llmbot/project_cover.png) ------------------
+[lmdb]>=2.5.2 Requires-Dist: pymongo>=4.6.3 Requires-Dist: fast-
+langdetect>=0.1.0 Requires-Dist: hikari==2.0.0.dev121; extra == "bot" Requires-
+Dist: hikari-crescent<1.0.0,>=0.6.4; extra == "bot" Requires-Dist: khl-
+py<1.0.0,>=0.3.17; extra == "bot" Requires-Dist: slack-bolt<2.0.0,>=1.18.0;
+extra == "bot" Requires-Dist: hikari==2.0.0.dev121; extra == "testing"
+Requires-Dist: hikari-crescent<1.0.0,>=0.6.4; extra == "testing" Requires-Dist:
+khl-py<1.0.0,>=0.3.17; extra == "testing" Requires-Dist: slack-
+bolt<2.0.0,>=1.18.0; extra == "testing" Requires-Dist: pre-
+commit<3.5.0,>=2.15.0; extra == "testing" Provides-Extra: bot Provides-Extra:
+testing Description-Content-Type: text/markdown ![cover](https://
+raw.githubusercontent.com/LlmKira/.github/main/llmbot/project_cover.png) ------
+------------
                            _[_d_o_c_k_e_r_]_[_d_o_c_k_e_r_ _w_o_r_k_f_l_o_w_]
                               _[_t_e_l_e_g_r_a_m_]_[_d_i_s_c_o_r_d_]
                             _[_l_i_c_e_n_s_e_]_[_d_o_c_k_e_r_ _b_u_i_l_d_]
               _ð___©_ _D_e_p_l_o_y_ _D_o_c_s & _ð__§__ _D_e_v_ _D_o_c_s & _ð__¤__ _C_o_n_t_r_i_b_u_t_e
 > Don't hesitate to Star â­ï¸, Issue ð, and PR ð ï¸ > Python>=3.9 This
 project uses the ToolCall feature. It integrates a message queuing and snapshot
 system, offering plugin mechanisms and authentication prior to plugin
 execution. The model adheres to the Openai Schema, other models are not
 supported. Please adapt using gateways independently. | Demo | |---------------
---------------------| | ![sticker](./docs/chain_chat.gif) | ## ð Roadmap -
+--------------------| | ![sticker](./docs/chain_chat.gif) | ## ð¨ Roadmap -
 [x] Removal of legacy code - [x] Deletion of metric system - [x] Deletion of
 model selection system, unified to OpenAI Schema - [x] Implementation of a more
 robust plugin system - [x] Project structure simplification - [x] Elimination
-of the Provider system ## ð¦ Features - ðª A comprehensive plugin
-development ecosystem, adopting a classic design, and seamless integration with
-plugins through `pip` installation - ð Message system with no time or sender
-constraints, offering fully decoupled logics - ð¬ Offers Login via a URL
-mechanism, providing a flexible and expandable authentication development
-solution - ð° Empowers users to authorize plugin execution. Users can
-configure plugin environment variables at their discretion - ð¦ Support for
-plugins to access files - ð Multi-platform support â extend new platforms
-by inheriting the base class - ð Plugins can determine their appearance in
-new sessions dynamically, preventing performance degradation despite large
-amounts of plugins ### ð Login Modes - `Login via url`: Use `/login
-token#https://provider.com` to Login. The program posts the token to the
-interface to retrieve configuration information - `Login`: Use `/login https://
-api.com/v1#key#model` to login ### ð§ Plugin Previews | Sticker Converter |
-Timer Function | Translate Function | |-------------------------------------|--
--------------------------------|----------------------------------------------
-| | ![sticker](./docs/sticker_func.gif) | ![timer](./docs/timer_func.gif) | !
-[translate](./docs/translate_file_func.gif) | ### ð¬ Platform Support |
-Platform | Support | File System | Remarks | |----------|---------|------------
--|----------------------------------------| | Telegram | â | â | | |
-Discord | â | â | | | Kook | â | â | Does not support `triggering by
-reply` | | Slack | â | â | Does not support `triggering by reply` | | QQ |
-â | | | | Wechat | â | | | | Twitter | â | | | | Matrix | â | | | | IRC
-| â | | | | ... | | | Create Issue/PR | ## ð¦ Quick Start Refer to the
-[ð§ Deployment Document](https://llmkira.github.io/Docs/) for more
-information. ```shell # Install RabbitMQ docker pull rabbitmq:3.10-management
-docker run -d -p 5672:5672 -p 15672:15672 \ -e RABBITMQ_DEFAULT_USER=admin \ -
-e RABBITMQ_DEFAULT_PASS=8a8a8a \ --hostname myRabbit \ --name rabbitmq \
-rabbitmq:3.10-management docker ps -l # Install Project pip install pdm pdm
-install -G bot cp .env.exp .env && nano .env # Test pdm run python3
-start_sender.py pdm run python3 start_receiver.py # Host pdm start pm2.json ```
-### ð¥£ Docker Build Hub: [sudoskys/llmbot](https://hub.docker.com/repository/
-docker/sudoskys/llmbot/general) #### Automatic Docker/Docker-compose
-Installation If you are using a brand new server, you can use the following
-shell to automatically install this project. This script automatically installs
-the required services and maps ports using Docker methods. If you have deployed
-`redis`, `rabbitmq`, `mongodb`, please modify the `docker-compose.yml` file
-accordingly. ```shell curl -sSL https://raw.githubusercontent.com/LLMKira/
-Openaibot/main/deploy.sh | bash ``` #### Manual Docker-compose Installation
-```shell git clone https://github.com/LlmKira/Openaibot.git cd Openaibot cp
-.env.exp .env&&nano .env docker-compose -f docker-compose.yml up -d ``` Update
-image using `docker-compose pull`. Use `docker exec -it llmbot /bin/bash` to
-view Shell in Docker, enter `exit` to exit. ## ðª Slash Commands ```shell
-clear - Deletes chat records help - Displays documentation chat - Conversation
-task - Use a function to converse ask - Disable function-based conversations
-tool - Lists all functions login - Login auth - Authorize a function env -
-Environment variables of the function ``` ## ð» How to Develop Plugins? Refer
-to the example plugins in the `plugins` directory and the [ð§ Plugin
-Development Document](https://llmkira.github.io/Docs/dev/basic) for plugin
-development documentation. ## ð§ Sponsor [![sponsor](./.github/
+of the Provider system - [x] Hook support. - [x] Access to TTS. - [ ] Add LLM
+reference support to the plugin environment. (extract && search in text) - [ ]
+Add standalone support for Openai's new Schema. (vision) ## ð¦ Features -
+ðª A comprehensive plugin development ecosystem, adopting a classic design,
+and seamless integration with plugins through `pip` installation - ð Message
+system with no time or sender constraints, offering fully decoupled logics -
+ð¬ Offers Login via a URL mechanism, providing a flexible and expandable
+authentication development solution - ð° Empowers users to authorize plugin
+execution. Users can configure plugin environment variables at their discretion
+- ð¦ Support for plugins to access files - ð Multi-platform support â
+extend new platforms by inheriting the base class - ð Plugins can determine
+their appearance in new sessions dynamically, preventing performance
+degradation despite large amounts of plugins ### ð Login Modes - `Login via
+url`: Use `/login token$https://provider.com` to Login. The program posts the
+token to the interface to retrieve configuration information - `Login`: Use `/
+login https://api.com/v1$key$model` to login ### ð§ Plugin Previews | Sticker
+Converter | Timer Function | Translate Function | |----------------------------
+---------|---------------------------------|-----------------------------------
+-----------| | ![sticker](./docs/sticker_func.gif) | ![timer](./docs/
+timer_func.gif) | ![translate](./docs/translate_file_func.gif) | ### ð¬
+Platform Support | Platform | Support | File System | Remarks | |----------|---
+------|-------------|----------------------------------------| | Telegram | â
+| â | | | Discord | â | â | | | Kook | â | â | Does not support
+`triggering by reply` | | Slack | â | â | Does not support `triggering by
+reply` | | QQ | â | | | | Wechat | â | | | | Twitter | â | | | | Matrix |
+â | | | | IRC | â | | | | ... | | | Create Issue/PR | ## ð¦ Quick Start
+Refer to the [ð§ Deployment Document](https://llmkira.github.io/Docs/) for
+more information. ```shell # Install RabbitMQ docker pull rabbitmq:3.10-
+management docker run -d -p 5672:5672 -p 15672:15672 \ -
+e RABBITMQ_DEFAULT_USER=admin \ -e RABBITMQ_DEFAULT_PASS=8a8a8a \ --hostname
+myRabbit \ --name rabbitmq \ rabbitmq:3.10-management docker ps -l # Install
+Project pip install pdm pdm install -G bot cp .env.exp .env && nano .env # Test
+pdm run python3 start_sender.py pdm run python3 start_receiver.py # Host pdm
+start pm2.json ``` ### ð¥£ Docker Build Hub: [sudoskys/llmbot](https://
+hub.docker.com/repository/docker/sudoskys/llmbot/general) #### Automatic
+Docker/Docker-compose Installation If you are using a brand new server, you can
+use the following shell to automatically install this project. This script
+automatically installs the required services and maps ports using Docker
+methods. If you have deployed `redis`, `rabbitmq`, `mongodb`, please modify the
+`docker-compose.yml` file accordingly. ```shell curl -sSL https://
+raw.githubusercontent.com/LLMKira/Openaibot/main/deploy.sh | bash ``` ####
+Manual Docker-compose Installation ```shell git clone https://github.com/
+LlmKira/Openaibot.git cd Openaibot cp .env.exp .env&&nano .env docker-compose -
+f docker-compose.yml up -d ``` Update image using `docker-compose pull`. Use
+`docker exec -it llmbot /bin/bash` to view Shell in Docker, enter `exit` to
+exit. ## ðª Slash Commands ```shell clear - Deletes chat records help -
+Displays documentation chat - Conversation task - Use a function to converse
+ask - Disable function-based conversations tool - Lists all functions login -
+Login auth - Authorize a function env - Environment variables of the function
+``` ## ð» How to Develop Plugins? Refer to the example plugins in the
+`plugins` directory and the [ð§ Plugin Development Document](https://
+llmkira.github.io/Docs/dev/basic) for plugin development documentation. ###
+Hooks Hooks control the EventMessage in sender and receiver. For example, we
+have `voice_hook` in built-in hooks. you can enable it by setting
+`VOICE_REPLY_ME=true` in `.env`. ```shell /env VOICE_REPLY_ME=true /env
+REECHO_VOICE_KEY= ``` check the source code in `llmkira/extra/voice_hook.py`,
+learn to write your own hooks. ## ð§ Sponsor [![sponsor](./.github/
 sponsor_ohmygpt.png)](https://www.ohmygpt.com) ## ð Notice > This project,
 named OpenAiBot, signifying "Open Artificial Intelligence Robot", is not
 officially affiliated with > OpenAI. [![FOSSA Status](https://app.fossa.com/
 api/projects/git%2Bgithub.com%2Fsudoskys%2FOpenaibot.svg?type=small)](https://
 app.fossa.com/projects/git%2Bgithub.com%2Fsudoskys%2FOpenaibot?ref=badge_small)
```

