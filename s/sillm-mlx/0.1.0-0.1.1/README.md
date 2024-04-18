# Comparing `tmp/sillm-mlx-0.1.0.tar.gz` & `tmp/sillm-mlx-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sillm-mlx-0.1.0.tar", last modified: Fri Apr 12 19:55:22 2024, max compression
+gzip compressed data, was "sillm-mlx-0.1.1.tar", last modified: Thu Apr 18 19:06:38 2024, max compression
```

## Comparing `sillm-mlx-0.1.0.tar` & `sillm-mlx-0.1.1.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-12 19:55:22.644954 sillm-mlx-0.1.0/
--rw-r--r--   0 armin      (501) staff       (20)     1071 2024-01-14 11:43:40.000000 sillm-mlx-0.1.0/LICENSE
--rw-r--r--   0 armin      (501) staff       (20)     7726 2024-04-12 19:55:22.644748 sillm-mlx-0.1.0/PKG-INFO
--rw-r--r--   0 armin      (501) staff       (20)     7061 2024-04-12 19:54:48.000000 sillm-mlx-0.1.0/README.md
--rw-r--r--   0 armin      (501) staff       (20)       88 2024-04-05 14:12:20.000000 sillm-mlx-0.1.0/pyproject.toml
--rw-r--r--   0 armin      (501) staff       (20)       38 2024-04-12 19:55:22.644995 sillm-mlx-0.1.0/setup.cfg
--rw-r--r--   0 armin      (501) staff       (20)      921 2024-04-12 19:55:08.000000 sillm-mlx-0.1.0/setup.py
-drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-12 19:55:22.638229 sillm-mlx-0.1.0/sillm/
--rw-r--r--   0 armin      (501) staff       (20)      471 2024-04-02 07:37:25.000000 sillm-mlx-0.1.0/sillm/__init__.py
--rw-r--r--   0 armin      (501) staff       (20)     4772 2024-04-10 08:05:39.000000 sillm-mlx-0.1.0/sillm/chat.py
--rw-r--r--   0 armin      (501) staff       (20)     1940 2024-04-10 11:04:13.000000 sillm-mlx-0.1.0/sillm/convert.py
-drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-12 19:55:22.639201 sillm-mlx-0.1.0/sillm/core/
--rw-r--r--   0 armin      (501) staff       (20)        0 2024-03-07 08:12:16.000000 sillm-mlx-0.1.0/sillm/core/__init__.py
--rw-r--r--   0 armin      (501) staff       (20)     3340 2024-04-02 07:37:25.000000 sillm-mlx-0.1.0/sillm/core/conversation.py
--rw-r--r--   0 armin      (501) staff       (20)    13705 2024-04-10 08:52:13.000000 sillm-mlx-0.1.0/sillm/core/llm.py
--rw-r--r--   0 armin      (501) staff       (20)    10346 2024-04-12 13:41:37.000000 sillm-mlx-0.1.0/sillm/core/loader.py
--rw-r--r--   0 armin      (501) staff       (20)     2186 2024-04-08 08:56:14.000000 sillm-mlx-0.1.0/sillm/core/template.py
--rw-r--r--   0 armin      (501) staff       (20)    12495 2024-04-10 08:03:41.000000 sillm-mlx-0.1.0/sillm/core/tokenizer.py
--rw-r--r--   0 armin      (501) staff       (20)     7079 2024-03-19 07:56:55.000000 sillm-mlx-0.1.0/sillm/dpo.py
--rw-r--r--   0 armin      (501) staff       (20)     6732 2024-04-03 11:21:15.000000 sillm-mlx-0.1.0/sillm/lora.py
-drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-12 19:55:22.640699 sillm-mlx-0.1.0/sillm/models/
--rw-r--r--   0 armin      (501) staff       (20)      252 2024-04-05 12:50:36.000000 sillm-mlx-0.1.0/sillm/models/__init__.py
--rw-r--r--   0 armin      (501) staff       (20)     5260 2024-04-10 07:23:26.000000 sillm-mlx-0.1.0/sillm/models/args.py
--rw-r--r--   0 armin      (501) staff       (20)     1550 2024-04-09 06:58:55.000000 sillm-mlx-0.1.0/sillm/models/base.py
--rw-r--r--   0 armin      (501) staff       (20)     5656 2024-04-10 07:16:05.000000 sillm-mlx-0.1.0/sillm/models/cohere.py
--rw-r--r--   0 armin      (501) staff       (20)     3586 2024-04-04 12:52:41.000000 sillm-mlx-0.1.0/sillm/models/dbrx.py
--rw-r--r--   0 armin      (501) staff       (20)     2887 2024-04-09 07:01:18.000000 sillm-mlx-0.1.0/sillm/models/gemma.py
--rw-r--r--   0 armin      (501) staff       (20)     6299 2024-04-09 06:59:25.000000 sillm-mlx-0.1.0/sillm/models/llama.py
--rw-r--r--   0 armin      (501) staff       (20)     7177 2024-04-09 07:03:02.000000 sillm-mlx-0.1.0/sillm/models/mixtral.py
--rw-r--r--   0 armin      (501) staff       (20)     4870 2024-04-09 07:03:25.000000 sillm-mlx-0.1.0/sillm/models/phi.py
--rw-r--r--   0 armin      (501) staff       (20)     3341 2024-04-09 07:03:49.000000 sillm-mlx-0.1.0/sillm/models/qwen2.py
--rw-r--r--   0 armin      (501) staff       (20)     4017 2024-04-09 07:04:14.000000 sillm-mlx-0.1.0/sillm/models/starcoder2.py
--rw-r--r--   0 armin      (501) staff       (20)     2284 2024-04-12 13:41:37.000000 sillm-mlx-0.1.0/sillm/quantize.py
--rw-r--r--   0 armin      (501) staff       (20)     2968 2024-04-02 07:54:29.000000 sillm-mlx-0.1.0/sillm/server.py
-drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-12 19:55:22.641899 sillm-mlx-0.1.0/sillm/templates/
--rw-r--r--   0 armin      (501) staff       (20)      805 2024-04-12 13:41:37.000000 sillm-mlx-0.1.0/sillm/templates/alpaca.jinja
--rw-r--r--   0 armin      (501) staff       (20)      203 2024-03-18 08:50:40.000000 sillm-mlx-0.1.0/sillm/templates/chatml.jinja
--rw-r--r--   0 armin      (501) staff       (20)     1189 2024-04-05 15:11:13.000000 sillm-mlx-0.1.0/sillm/templates/cohere.jinja
--rw-r--r--   0 armin      (501) staff       (20)      594 2024-03-18 08:50:40.000000 sillm-mlx-0.1.0/sillm/templates/gemma.jinja
--rw-r--r--   0 armin      (501) staff       (20)      791 2024-03-18 08:50:40.000000 sillm-mlx-0.1.0/sillm/templates/llama2.jinja
--rw-r--r--   0 armin      (501) staff       (20)      443 2024-03-18 08:50:40.000000 sillm-mlx-0.1.0/sillm/templates/mistral.jinja
--rw-r--r--   0 armin      (501) staff       (20)      222 2024-04-02 07:37:25.000000 sillm-mlx-0.1.0/sillm/templates/openchat.jinja
--rw-r--r--   0 armin      (501) staff       (20)      364 2024-03-18 08:50:40.000000 sillm-mlx-0.1.0/sillm/templates/phi2.jinja
--rw-r--r--   0 armin      (501) staff       (20)      448 2024-03-18 08:50:40.000000 sillm-mlx-0.1.0/sillm/templates/qwen2.jinja
-drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-12 19:55:22.642382 sillm-mlx-0.1.0/sillm/training/
--rw-r--r--   0 armin      (501) staff       (20)        0 2024-03-07 08:12:16.000000 sillm-mlx-0.1.0/sillm/training/__init__.py
--rw-r--r--   0 armin      (501) staff       (20)    15041 2024-04-03 10:12:12.000000 sillm-mlx-0.1.0/sillm/training/dataset.py
--rw-r--r--   0 armin      (501) staff       (20)     6397 2024-03-18 21:48:06.000000 sillm-mlx-0.1.0/sillm/training/dpo.py
--rw-r--r--   0 armin      (501) staff       (20)    18471 2024-04-10 09:02:01.000000 sillm-mlx-0.1.0/sillm/training/lora.py
-drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-12 19:55:22.643762 sillm-mlx-0.1.0/sillm/utils/
--rw-r--r--   0 armin      (501) staff       (20)      153 2024-03-22 08:26:17.000000 sillm-mlx-0.1.0/sillm/utils/__init__.py
--rw-r--r--   0 armin      (501) staff       (20)      393 2024-03-22 08:25:51.000000 sillm-mlx-0.1.0/sillm/utils/common.py
--rw-r--r--   0 armin      (501) staff       (20)     1332 2024-04-08 13:25:32.000000 sillm-mlx-0.1.0/sillm/utils/log.py
--rw-r--r--   0 armin      (501) staff       (20)     7726 2024-04-05 13:14:42.000000 sillm-mlx-0.1.0/sillm/utils/mapping.py
--rw-r--r--   0 armin      (501) staff       (20)     1621 2024-03-08 12:33:03.000000 sillm-mlx-0.1.0/sillm/utils/plot.py
--rw-r--r--   0 armin      (501) staff       (20)     2015 2024-04-12 13:41:37.000000 sillm-mlx-0.1.0/sillm/utils/quantization.py
-drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-12 19:55:22.644360 sillm-mlx-0.1.0/sillm_mlx.egg-info/
--rw-r--r--   0 armin      (501) staff       (20)     7726 2024-04-12 19:55:22.000000 sillm-mlx-0.1.0/sillm_mlx.egg-info/PKG-INFO
--rw-r--r--   0 armin      (501) staff       (20)     1193 2024-04-12 19:55:22.000000 sillm-mlx-0.1.0/sillm_mlx.egg-info/SOURCES.txt
--rw-r--r--   0 armin      (501) staff       (20)        1 2024-04-12 19:55:22.000000 sillm-mlx-0.1.0/sillm_mlx.egg-info/dependency_links.txt
--rw-r--r--   0 armin      (501) staff       (20)      157 2024-04-12 19:55:22.000000 sillm-mlx-0.1.0/sillm_mlx.egg-info/requires.txt
--rw-r--r--   0 armin      (501) staff       (20)        6 2024-04-12 19:55:22.000000 sillm-mlx-0.1.0/sillm_mlx.egg-info/top_level.txt
+drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-18 19:06:38.064584 sillm-mlx-0.1.1/
+-rw-r--r--   0 armin      (501) staff       (20)     1071 2024-01-14 11:43:40.000000 sillm-mlx-0.1.1/LICENSE
+-rw-r--r--   0 armin      (501) staff       (20)     7829 2024-04-18 19:06:38.064416 sillm-mlx-0.1.1/PKG-INFO
+-rw-r--r--   0 armin      (501) staff       (20)     7164 2024-04-16 14:05:30.000000 sillm-mlx-0.1.1/README.md
+-rw-r--r--   0 armin      (501) staff       (20)       38 2024-04-18 19:06:38.064614 sillm-mlx-0.1.1/setup.cfg
+-rw-r--r--   0 armin      (501) staff       (20)      921 2024-04-18 19:06:07.000000 sillm-mlx-0.1.1/setup.py
+drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-18 19:06:38.059852 sillm-mlx-0.1.1/sillm/
+-rw-r--r--   0 armin      (501) staff       (20)      471 2024-04-02 07:37:25.000000 sillm-mlx-0.1.1/sillm/__init__.py
+-rw-r--r--   0 armin      (501) staff       (20)     4772 2024-04-10 08:05:39.000000 sillm-mlx-0.1.1/sillm/chat.py
+-rw-r--r--   0 armin      (501) staff       (20)     1940 2024-04-10 11:04:13.000000 sillm-mlx-0.1.1/sillm/convert.py
+drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-18 19:06:38.060411 sillm-mlx-0.1.1/sillm/core/
+-rw-r--r--   0 armin      (501) staff       (20)        0 2024-03-07 08:12:16.000000 sillm-mlx-0.1.1/sillm/core/__init__.py
+-rw-r--r--   0 armin      (501) staff       (20)     3340 2024-04-02 07:37:25.000000 sillm-mlx-0.1.1/sillm/core/conversation.py
+-rw-r--r--   0 armin      (501) staff       (20)    14764 2024-04-18 15:24:49.000000 sillm-mlx-0.1.1/sillm/core/llm.py
+-rw-r--r--   0 armin      (501) staff       (20)    10362 2024-04-18 15:05:38.000000 sillm-mlx-0.1.1/sillm/core/loader.py
+-rw-r--r--   0 armin      (501) staff       (20)     2375 2024-04-18 18:28:05.000000 sillm-mlx-0.1.1/sillm/core/template.py
+-rw-r--r--   0 armin      (501) staff       (20)    12635 2024-04-18 18:32:39.000000 sillm-mlx-0.1.1/sillm/core/tokenizer.py
+-rw-r--r--   0 armin      (501) staff       (20)     7079 2024-03-19 07:56:55.000000 sillm-mlx-0.1.1/sillm/dpo.py
+-rw-r--r--   0 armin      (501) staff       (20)     6732 2024-04-03 11:21:15.000000 sillm-mlx-0.1.1/sillm/lora.py
+drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-18 19:06:38.061498 sillm-mlx-0.1.1/sillm/models/
+-rw-r--r--   0 armin      (501) staff       (20)      252 2024-04-05 12:50:36.000000 sillm-mlx-0.1.1/sillm/models/__init__.py
+-rw-r--r--   0 armin      (501) staff       (20)     5260 2024-04-10 07:23:26.000000 sillm-mlx-0.1.1/sillm/models/args.py
+-rw-r--r--   0 armin      (501) staff       (20)     1550 2024-04-09 06:58:55.000000 sillm-mlx-0.1.1/sillm/models/base.py
+-rw-r--r--   0 armin      (501) staff       (20)     5436 2024-04-16 08:57:26.000000 sillm-mlx-0.1.1/sillm/models/cohere.py
+-rw-r--r--   0 armin      (501) staff       (20)     3586 2024-04-04 12:52:41.000000 sillm-mlx-0.1.1/sillm/models/dbrx.py
+-rw-r--r--   0 armin      (501) staff       (20)     2887 2024-04-09 07:01:18.000000 sillm-mlx-0.1.1/sillm/models/gemma.py
+-rw-r--r--   0 armin      (501) staff       (20)     6299 2024-04-09 06:59:25.000000 sillm-mlx-0.1.1/sillm/models/llama.py
+-rw-r--r--   0 armin      (501) staff       (20)     7179 2024-04-15 20:30:32.000000 sillm-mlx-0.1.1/sillm/models/mixtral.py
+-rw-r--r--   0 armin      (501) staff       (20)     4870 2024-04-09 07:03:25.000000 sillm-mlx-0.1.1/sillm/models/phi.py
+-rw-r--r--   0 armin      (501) staff       (20)     3341 2024-04-09 07:03:49.000000 sillm-mlx-0.1.1/sillm/models/qwen2.py
+-rw-r--r--   0 armin      (501) staff       (20)     4017 2024-04-09 07:04:14.000000 sillm-mlx-0.1.1/sillm/models/starcoder2.py
+-rw-r--r--   0 armin      (501) staff       (20)     2284 2024-04-12 13:41:37.000000 sillm-mlx-0.1.1/sillm/quantize.py
+-rw-r--r--   0 armin      (501) staff       (20)     2968 2024-04-02 07:54:29.000000 sillm-mlx-0.1.1/sillm/server.py
+drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-18 19:06:38.062611 sillm-mlx-0.1.1/sillm/templates/
+-rw-r--r--   0 armin      (501) staff       (20)      785 2024-04-15 20:54:36.000000 sillm-mlx-0.1.1/sillm/templates/alpaca.jinja
+-rw-r--r--   0 armin      (501) staff       (20)      203 2024-03-18 08:50:40.000000 sillm-mlx-0.1.1/sillm/templates/chatml.jinja
+-rw-r--r--   0 armin      (501) staff       (20)     1189 2024-04-05 15:11:13.000000 sillm-mlx-0.1.1/sillm/templates/cohere.jinja
+-rw-r--r--   0 armin      (501) staff       (20)       65 2024-04-15 13:34:23.000000 sillm-mlx-0.1.1/sillm/templates/empty.jinja
+-rw-r--r--   0 armin      (501) staff       (20)      594 2024-03-18 08:50:40.000000 sillm-mlx-0.1.1/sillm/templates/gemma.jinja
+-rw-r--r--   0 armin      (501) staff       (20)      791 2024-03-18 08:50:40.000000 sillm-mlx-0.1.1/sillm/templates/llama2.jinja
+-rw-r--r--   0 armin      (501) staff       (20)      277 2024-04-18 18:20:17.000000 sillm-mlx-0.1.1/sillm/templates/llama3.jinja
+-rw-r--r--   0 armin      (501) staff       (20)      443 2024-03-18 08:50:40.000000 sillm-mlx-0.1.1/sillm/templates/mistral.jinja
+-rw-r--r--   0 armin      (501) staff       (20)      222 2024-04-02 07:37:25.000000 sillm-mlx-0.1.1/sillm/templates/openchat.jinja
+-rw-r--r--   0 armin      (501) staff       (20)      364 2024-03-18 08:50:40.000000 sillm-mlx-0.1.1/sillm/templates/phi2.jinja
+-rw-r--r--   0 armin      (501) staff       (20)      448 2024-03-18 08:50:40.000000 sillm-mlx-0.1.1/sillm/templates/qwen2.jinja
+-rw-r--r--   0 armin      (501) staff       (20)      749 2024-04-15 20:52:40.000000 sillm-mlx-0.1.1/sillm/templates/vicuna.jinja
+drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-18 19:06:38.062980 sillm-mlx-0.1.1/sillm/training/
+-rw-r--r--   0 armin      (501) staff       (20)        0 2024-03-07 08:12:16.000000 sillm-mlx-0.1.1/sillm/training/__init__.py
+-rw-r--r--   0 armin      (501) staff       (20)    15041 2024-04-03 10:12:12.000000 sillm-mlx-0.1.1/sillm/training/dataset.py
+-rw-r--r--   0 armin      (501) staff       (20)     6480 2024-04-17 07:19:26.000000 sillm-mlx-0.1.1/sillm/training/dpo.py
+-rw-r--r--   0 armin      (501) staff       (20)    18471 2024-04-10 09:02:01.000000 sillm-mlx-0.1.1/sillm/training/lora.py
+drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-18 19:06:38.063603 sillm-mlx-0.1.1/sillm/utils/
+-rw-r--r--   0 armin      (501) staff       (20)      153 2024-03-22 08:26:17.000000 sillm-mlx-0.1.1/sillm/utils/__init__.py
+-rw-r--r--   0 armin      (501) staff       (20)      393 2024-03-22 08:25:51.000000 sillm-mlx-0.1.1/sillm/utils/common.py
+-rw-r--r--   0 armin      (501) staff       (20)     1332 2024-04-08 13:25:32.000000 sillm-mlx-0.1.1/sillm/utils/log.py
+-rw-r--r--   0 armin      (501) staff       (20)     8236 2024-04-16 09:00:07.000000 sillm-mlx-0.1.1/sillm/utils/mapping.py
+-rw-r--r--   0 armin      (501) staff       (20)     1621 2024-03-08 12:33:03.000000 sillm-mlx-0.1.1/sillm/utils/plot.py
+-rw-r--r--   0 armin      (501) staff       (20)     3482 2024-04-16 07:26:30.000000 sillm-mlx-0.1.1/sillm/utils/quantization.py
+drwxr-xr-x   0 armin      (501) staff       (20)        0 2024-04-18 19:06:38.064082 sillm-mlx-0.1.1/sillm_mlx.egg-info/
+-rw-r--r--   0 armin      (501) staff       (20)     7829 2024-04-18 19:06:37.000000 sillm-mlx-0.1.1/sillm_mlx.egg-info/PKG-INFO
+-rw-r--r--   0 armin      (501) staff       (20)     1264 2024-04-18 19:06:37.000000 sillm-mlx-0.1.1/sillm_mlx.egg-info/SOURCES.txt
+-rw-r--r--   0 armin      (501) staff       (20)        1 2024-04-18 19:06:37.000000 sillm-mlx-0.1.1/sillm_mlx.egg-info/dependency_links.txt
+-rw-r--r--   0 armin      (501) staff       (20)      157 2024-04-18 19:06:37.000000 sillm-mlx-0.1.1/sillm_mlx.egg-info/requires.txt
+-rw-r--r--   0 armin      (501) staff       (20)        6 2024-04-18 19:06:37.000000 sillm-mlx-0.1.1/sillm_mlx.egg-info/top_level.txt
```

### Comparing `sillm-mlx-0.1.0/LICENSE` & `sillm-mlx-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.0/PKG-INFO` & `sillm-mlx-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sillm-mlx
-Version: 0.1.0
+Version: 0.1.1
 Summary: Running and training LLMs on Apple Silicon via MLX
 Home-page: https://github.com/armbues/SiLLM
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mlx>=0.10.0
 Requires-Dist: transformers>=4.39.3
@@ -54,14 +54,15 @@
 
 https://github.com/armbues/SiLLM/assets/4117144/833d63ab-08b1-45ca-980f-474c7e9cc284
 
 To start the web app, clone the repository and start the app using chainlit:
 ``` sh
 git clone https://github.com/armbues/SiLLM.git
 cd SiLLM/app
+pip install -r requirements.txt
 python -m chainlit run app.py -w
 ```
 Set the environment variables `SILLM_MODEL_DIR` and `SILLM_ADAPTER_DIR` to load local models/adapters.
 
 ### Command-line interface (CLI) scripts
 Run the CLI scripts with the argument -h to see a print-out of all available arguments.
 
@@ -142,22 +143,23 @@
 | Mixtral v0.1 | | | [8x7B-Instruct](https://huggingface.co/mlx-community/Mixtral-8x7B-Instruct-v0.1) |
 | Gemma | [2b](https://huggingface.co/google/gemma-2b), [2b-it](https://huggingface.co/google/gemma-7b-it), [7b](https://huggingface.co/google/gemma-7b), [7b-it](https://huggingface.co/google/gemma-7b-it) | |
 | Phi-2 | [2.7b](https://huggingface.co/microsoft/phi-2) | |
 | Qwen 1.5 | [7b-chat](https://huggingface.co/Qwen/Qwen1.5-7B-Chat), [14b-chat](https://huggingface.co/Qwen/Qwen1.5-14B-Chat) | |
 | StarCoder2 | [3b](https://huggingface.co/bigcode/starcoder2-3b), [7b](https://huggingface.co/bigcode/starcoder2-7b), [15b](https://huggingface.co/bigcode/starcoder2-15b) | |
 | CodeLlama | | [70b-instruct.Q4_0](https://huggingface.co/TheBloke/CodeLlama-70B-Instruct-GGUF), [Phind-34b-v2.Q4_0](https://huggingface.co/TheBloke/Phind-CodeLlama-34B-v2-GGUF) | |
 | DBRX | (currently not supported) | | [dbrx-instruct-4bit](https://huggingface.co/mlx-community/dbrx-instruct-4bit) |
-| Cohere | [Command-R](https://huggingface.co/CohereForAI/c4ai-command-r-v01) | |
+| Cohere | [Command-R](https://huggingface.co/CohereForAI/c4ai-command-r-v01), [Command-R+](CohereForAI/c4ai-command-r-plus) | |
 
 ## Roadmap
 
 - Repetition penalty for inference
 - Learning rate schedulers for training
 - Merging models
 - Saving models to GGUF
+- Fine tuning with ORPO
 
 ## License
 This project uses the [MIT License](LICENSE).
 
 ## Acknowledgments
 Big thanks to the Apple MLX team for implementing and maintaining the [MLX](https://github.com/ml-explore/mlx/) framework that makes it possible to unlock the power of Apple Silicon and run/train LLMs on MacBooks and other Apple devices. Thank you to all the contributors of the [MLX Examples](https://github.com/ml-explore/mlx-examples) project and developers sharing model implementations online.
 Last but not least, thank you to the larger community sharing open weights models, fine tunes, and datasets - without you all the gen AI progress would happen behind locked doors!
```

### Comparing `sillm-mlx-0.1.0/README.md` & `sillm-mlx-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 https://github.com/armbues/SiLLM/assets/4117144/833d63ab-08b1-45ca-980f-474c7e9cc284
 
 To start the web app, clone the repository and start the app using chainlit:
 ``` sh
 git clone https://github.com/armbues/SiLLM.git
 cd SiLLM/app
+pip install -r requirements.txt
 python -m chainlit run app.py -w
 ```
 Set the environment variables `SILLM_MODEL_DIR` and `SILLM_ADAPTER_DIR` to load local models/adapters.
 
 ### Command-line interface (CLI) scripts
 Run the CLI scripts with the argument -h to see a print-out of all available arguments.
 
@@ -119,22 +120,23 @@
 | Mixtral v0.1 | | | [8x7B-Instruct](https://huggingface.co/mlx-community/Mixtral-8x7B-Instruct-v0.1) |
 | Gemma | [2b](https://huggingface.co/google/gemma-2b), [2b-it](https://huggingface.co/google/gemma-7b-it), [7b](https://huggingface.co/google/gemma-7b), [7b-it](https://huggingface.co/google/gemma-7b-it) | |
 | Phi-2 | [2.7b](https://huggingface.co/microsoft/phi-2) | |
 | Qwen 1.5 | [7b-chat](https://huggingface.co/Qwen/Qwen1.5-7B-Chat), [14b-chat](https://huggingface.co/Qwen/Qwen1.5-14B-Chat) | |
 | StarCoder2 | [3b](https://huggingface.co/bigcode/starcoder2-3b), [7b](https://huggingface.co/bigcode/starcoder2-7b), [15b](https://huggingface.co/bigcode/starcoder2-15b) | |
 | CodeLlama | | [70b-instruct.Q4_0](https://huggingface.co/TheBloke/CodeLlama-70B-Instruct-GGUF), [Phind-34b-v2.Q4_0](https://huggingface.co/TheBloke/Phind-CodeLlama-34B-v2-GGUF) | |
 | DBRX | (currently not supported) | | [dbrx-instruct-4bit](https://huggingface.co/mlx-community/dbrx-instruct-4bit) |
-| Cohere | [Command-R](https://huggingface.co/CohereForAI/c4ai-command-r-v01) | |
+| Cohere | [Command-R](https://huggingface.co/CohereForAI/c4ai-command-r-v01), [Command-R+](CohereForAI/c4ai-command-r-plus) | |
 
 ## Roadmap
 
 - Repetition penalty for inference
 - Learning rate schedulers for training
 - Merging models
 - Saving models to GGUF
+- Fine tuning with ORPO
 
 ## License
 This project uses the [MIT License](LICENSE).
 
 ## Acknowledgments
 Big thanks to the Apple MLX team for implementing and maintaining the [MLX](https://github.com/ml-explore/mlx/) framework that makes it possible to unlock the power of Apple Silicon and run/train LLMs on MacBooks and other Apple devices. Thank you to all the contributors of the [MLX Examples](https://github.com/ml-explore/mlx-examples) project and developers sharing model implementations online.
 Last but not least, thank you to the larger community sharing open weights models, fine tunes, and datasets - without you all the gen AI progress would happen behind locked doors!
```

### Comparing `sillm-mlx-0.1.0/setup.py` & `sillm-mlx-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 pkg_dir = pathlib.Path(__file__).parent.resolve()
 readme = (pkg_dir / "README.md").read_text(encoding="utf-8")
 requirements = (pkg_dir / "requirements.txt").read_text(encoding="utf-8").splitlines()
 requirements_server = (pkg_dir / "requirements-server.txt").read_text(encoding="utf-8").splitlines()
 
 setup(
     name = "sillm-mlx",
-    version = "0.1.0",
+    version = "0.1.1",
     description = "Running and training LLMs on Apple Silicon via MLX",
     long_description = readme,
     long_description_content_type = "text/markdown",
     readme="README.md",
     url = "https://github.com/armbues/SiLLM",
     install_requires=requirements,
     extras_require={
```

### Comparing `sillm-mlx-0.1.0/sillm/chat.py` & `sillm-mlx-0.1.1/sillm/chat.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.0/sillm/convert.py` & `sillm-mlx-0.1.1/sillm/convert.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.0/sillm/core/conversation.py` & `sillm-mlx-0.1.1/sillm/core/conversation.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.0/sillm/core/llm.py` & `sillm-mlx-0.1.1/sillm/core/llm.py`

 * *Files 12% similar despite different names*

```diff
@@ -78,14 +78,27 @@
     def _update_names(self):
         """
         Update module names.
         """
         for name, module in self.model.named_modules():
             module.name = name
 
+    def get_size(self):
+        """
+        Get model size.
+        """
+        total_size = 0
+        for module in self.model.modules():
+            if isinstance(module, nn.QuantizedLinear):
+                total_size += module.weight.size * (32 // module.bits)
+            elif isinstance(module, nn.Linear):
+                total_size += module.weight.size
+
+        return total_size
+
     def update_weights(self,
                        weights: dict,
                        mapping: dict = None
                        ):
         """
         Update model weights.
         Args:
@@ -251,15 +264,18 @@
             quantization = {
                 "group_size": group_size,
                 "bits": bits
             }
             self._quantization = quantization
             self.args.quantization = quantization
 
-            linear_class_predicate = lambda m: isinstance(m, nn.Linear) and m.weight.shape[0] != 8 and m.name not in excluded
+            linear_class_predicate = lambda m: (isinstance(m, nn.Linear) and
+                                                m.weight.shape[0] != 8 and
+                                                ".gate." not in m.name and
+                                                m.name not in excluded)
             nn.QuantizedLinear.quantize_module(
                 model = self.model,
                 **quantization,
                 linear_class_predicate = linear_class_predicate
             )
 
             self._update_names()
@@ -377,15 +393,15 @@
     metadata = {
         "timing": timing,
         "usage": usage,
         "logprobs": [],
         "finish_reason": "length"
     }
 
-    tokens = []
+    tokens, text, buffer, prefix = [], "", [], ""
     for (token,p) , i in zip(generate_step(model, inputs, temperature, logprobs), range(max_tokens)):
         if i == 0:
             mx.eval(token)
 
             timing["eval_time"] = time.perf_counter() - start
 
         if token.item() in stop_tokens:
@@ -394,32 +410,49 @@
 
         tokens.append(token.item())
 
         if logprobs:
             metadata["logprobs"].append(p)
 
         if (len(tokens) % flush) == 0:
-            mx.eval(token)
-            s = tokenizer.decode(tokens)
+            mx.eval(tokens)
+
+            text = tokenizer.decode(tokens)
+            window = tokenizer.decode(buffer + tokens)
+            if prefix + " " + text == window:
+                prefix = text
+                text = " " + text
+            else:
+                prefix = text
+            buffer = tokens
             tokens = []
 
             timing["runtime"] = time.perf_counter() - start
             usage["completion_tokens"] = i+1
             usage["total_tokens"] = usage["prompt_tokens"] + usage["completion_tokens"]
 
-            yield s, metadata
+            yield text, metadata
 
-    mx.eval(token)
-    s = tokenizer.decode(tokens)
+    mx.eval(tokens)
+    
+    text = tokenizer.decode(tokens)
+    window = tokenizer.decode(buffer + tokens)
+    if prefix + " " + text == window:
+        prefix = text
+        text = " " + text
+    else:
+        prefix = text
+    buffer = tokens
+    tokens = []
 
     timing["runtime"] = time.perf_counter() - start
     usage["completion_tokens"] = i+1
     usage["total_tokens"] = usage["prompt_tokens"] + usage["completion_tokens"]
 
-    yield s, metadata
+    yield text, metadata
 
 def generate_step(model, inputs, temperature, logprobs=False):
     y = inputs
     cache = None
     while True:
         logits, cache = model(y[None], cache=cache)
         logits = logits[:, -1, :]
```

### Comparing `sillm-mlx-0.1.0/sillm/core/loader.py` & `sillm-mlx-0.1.1/sillm/core/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,16 @@
 
     # Verify that all model weights are present
     model.verify_weights(weights)
 
     # Update model weights
     model.update_weights(weights, mapping=mapping)
 
-    total_params = sum(v.size for v in weights.values())
+    # Print model size
+    total_params = model.get_size()
     logger.info(f"Loaded model weights with {total_params/10**9:.2f}B total parameters")
 
     return model
 
 def load_model_dir(model_path: str) -> LLM:
     """
     Load model from directory.
@@ -225,15 +226,16 @@
 
     # Verify that all model weights are present
     model.verify_weights(weights)
 
     # Update model weights
     model.update_weights(weights, mapping=mapping)
 
-    total_params = sum(v.size for v in weights.values())
+    # Print model size
+    total_params = model.get_size()
     logger.info(f"Loaded model weights with {total_params/10**9:.2f}B total parameters")
 
     return model
 
 def load_weights(weights_files,
                  load_func: callable
                  ):
@@ -288,17 +290,17 @@
     
     weights = {}
     for key, value in torch.load(weights_path, map_location="cpu").items():
         # Convert to numpy
         if value.dtype == torch.bfloat16:
             value = value.to(dtype=torch.float16).numpy()
         else:
-            v = v.numpy()
+            value = value.numpy()
 
-        weights[key] = mx.array(v, dtype=mx.float16)
+        weights[key] = mx.array(value, dtype=mx.float16)
 
     return weights
 
 ########
 # Based on:
 # https://github.com/ggerganov/llama.cpp/blob/b7b74cef36a93ae01e0b9af8986d131761742d0e/convert.py#L1182
 ########
```

### Comparing `sillm-mlx-0.1.0/sillm/core/template.py` & `sillm-mlx-0.1.1/sillm/core/template.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,15 +39,22 @@
         loader = jinja2.PackageLoader('sillm', 'templates')
 
         return loader.list_templates()
     
     @staticmethod
     def guess_template(args):
         if args.model_type and args.model_type in default_templates:
-            return default_templates[args.model_type]
+            template_name = default_templates[args.model_type]
+
+            # Hack for Llama-3
+            if args.model_type == "llama" and args.vocab_size == 128256:
+                template_name = "llama3"
+
+            return template_name
+
         return None
 
     def _raise_exception(self, msg):
         raise jinja2.exceptions.TemplateError(msg)
 
     def apply_chat_template(self,
                             messages: list,
@@ -61,10 +68,10 @@
                  ):
         self.tokenizer = tokenizer
 
         logger.info(f"Initialized built-in conversation template from tokenizer")
     
     def apply_chat_template(self,
                             messages: list,
-                            add_generation_prompt: bool = False,
+                            add_generation_prompt: bool = False
                             ):
         return self.tokenizer.apply_chat_template(messages, tokenize=False, add_generation_prompt=add_generation_prompt)
```

### Comparing `sillm-mlx-0.1.0/sillm/core/tokenizer.py` & `sillm-mlx-0.1.1/sillm/core/tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,14 +164,18 @@
         if args.pad_token_id is None:
             self.pad_id = self._model.pad_token_id
         else:
             self.pad_id = args.pad_token_id
 
         self.special_ids = set([self.bos_id, self.eos_id] + self._model.all_special_ids)
 
+        # Hack for Llama-3
+        if "<|eot_id|>" in self._model.vocab:
+            self.special_ids.add(self._model.vocab["<|eot_id|>"])
+
     def encode(self,
                s: str,
                bos: bool = True,
                eos: bool = False
                ) -> List[int]:
         """
         Encode string.
```

### Comparing `sillm-mlx-0.1.0/sillm/dpo.py` & `sillm-mlx-0.1.1/sillm/dpo.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.0/sillm/lora.py` & `sillm-mlx-0.1.1/sillm/lora.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.0/sillm/models/args.py` & `sillm-mlx-0.1.1/sillm/models/args.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.0/sillm/models/base.py` & `sillm-mlx-0.1.1/sillm/models/base.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.0/sillm/models/cohere.py` & `sillm-mlx-0.1.1/sillm/models/cohere.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,38 +37,36 @@
 
         self.wq = nn.Linear(args.dim, args.n_heads * args.head_dim, bias=False)
         self.wk = nn.Linear(args.dim, args.n_kv_heads * args.head_dim, bias=False)
         self.wv = nn.Linear(args.dim, args.n_kv_heads * args.head_dim, bias=False)
         self.wo = nn.Linear(args.n_heads * args.head_dim, args.dim, bias=False)
         
         if self.use_qk_norm:
-            self.q_norm = LayerNorm2D(self.n_heads, args.dim, eps=args.norm_eps)
-            self.k_norm = LayerNorm2D(self.n_kv_heads, args.dim, eps=args.norm_eps)
+            self.q_norm = LayerNorm2D(self.n_heads, args.head_dim, eps=args.norm_eps)
+            self.k_norm = LayerNorm2D(self.n_kv_heads, args.head_dim, eps=args.norm_eps)
 
         self.rope = nn.RoPE(args.head_dim, traditional=True, base=args.rope_theta)
 
     def __call__(self,
                  x: mx.array,
                  mask: Optional[mx.array] = None,
                  cache: Optional[Tuple[mx.array, mx.array]] = None,
                  ) -> mx.array:
         B, L, _ = x.shape
 
         queries, keys, values = self.wq(x), self.wk(x), self.wv(x)
 
+        queries = queries.reshape(B, L, self.n_heads, -1)
+        keys = keys.reshape(B, L, self.n_kv_heads, -1)
         if self.use_qk_norm:
-            queries = queries.reshape(B, L, self.n_heads, -1)
-            keys = keys.reshape(B, L, self.n_kv_heads, -1)
-            queries = self.q_norm(queries).transpose(0, 2, 1, 3)
-            keys = self.k_norm(keys).transpose(0, 2, 1, 3)
-            values = values.reshape(B, L, self.n_kv_heads, -1).transpose(0, 2, 1, 3)
-        else:
-            queries = queries.reshape(B, L, self.n_heads, -1).transpose(0, 2, 1, 3)
-            keys = keys.reshape(B, L, self.n_kv_heads, -1).transpose(0, 2, 1, 3)
-            values = values.reshape(B, L, self.n_kv_heads, -1).transpose(0, 2, 1, 3)
+            queries = self.q_norm(queries)
+            keys = self.k_norm(keys)
+        queries = queries.transpose(0, 2, 1, 3)
+        keys = keys.transpose(0, 2, 1, 3)
+        values = values.reshape(B, L, self.n_kv_heads, -1).transpose(0, 2, 1, 3)
 
         if cache is not None:
             key_cache, value_cache = cache
             queries = self.rope(queries, offset=key_cache.shape[2])
             keys = self.rope(keys, offset=key_cache.shape[2])
             keys = mx.concatenate([key_cache, keys], axis=2)
             values = mx.concatenate([value_cache, values], axis=2)
```

### Comparing `sillm-mlx-0.1.0/sillm/models/dbrx.py` & `sillm-mlx-0.1.1/sillm/models/dbrx.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.0/sillm/models/gemma.py` & `sillm-mlx-0.1.1/sillm/models/gemma.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.0/sillm/models/llama.py` & `sillm-mlx-0.1.1/sillm/models/llama.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.0/sillm/models/mixtral.py` & `sillm-mlx-0.1.1/sillm/models/mixtral.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         """
         top_k = self.num_experts_per_tok
         orig_shape = x.shape
         x = x.reshape(-1, x.shape[-1])
 
         gate_logits = self.gate(x)
         
-        expert_indices = mx.stop_gradient(mx.argpartition(-gate_logits, kth=top_k, axis=-1)[:, :top_k])
+        expert_indices = mx.stop_gradient(mx.argpartition(-gate_logits, kth=top_k-1, axis=-1)[:, :top_k])
         expert_scores = mx.softmax(mx.take_along_axis(gate_logits, expert_indices, axis=-1).astype(mx.float32), axis=-1).astype(gate_logits.dtype)
         
         if self.training:
             y = mx.zeros((x.shape[0], self.num_experts_per_tok, x.shape[-1]))
             for e, expert in enumerate(self.experts):
                 idx1, idx2 = map(mx.array, np.where(expert_indices == e))
                 if idx1.size == 0:
```

### Comparing `sillm-mlx-0.1.0/sillm/models/phi.py` & `sillm-mlx-0.1.1/sillm/models/phi.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.0/sillm/models/qwen2.py` & `sillm-mlx-0.1.1/sillm/models/qwen2.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.0/sillm/models/starcoder2.py` & `sillm-mlx-0.1.1/sillm/models/starcoder2.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.0/sillm/quantize.py` & `sillm-mlx-0.1.1/sillm/quantize.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.0/sillm/server.py` & `sillm-mlx-0.1.1/sillm/server.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.0/sillm/templates/alpaca.jinja` & `sillm-mlx-0.1.1/sillm/templates/alpaca.jinja`

 * *Files 24% similar despite different names*

```diff
@@ -1 +1 @@
-{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{% set system_message = messages[0]['content'].strip() + '\n\n' %}{% else %}{% set loop_messages = messages %}{% set system_message = '' %}{% endif %}{{ bos_token + system_message }}{% for message in loop_messages %}{% if (message['role'] == 'user') != (loop.index0 % 2 == 0) %}{{ raise_exception('Conversation roles must alternate user/assistant/user/assistant/...') }}{% endif %}{% if message['role'] == 'user' %}{{ '### Instruction:\n' + message['content'].strip() + '\n\n' }}{% elif message['role'] == 'assistant' %}{{ '### Response:\n' + message['content'].strip() + eos_token + '\n\n' }}{% endif %}{% if loop.last and message['role'] == 'user' and add_generation_prompt %}{{ '### Instruction:\n' }}{% endif %}{% endfor %}
+{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{% set system_message = messages[0]['content'].strip() + '\n\n' %}{% else %}{% set loop_messages = messages %}{% set system_message = '' %}{% endif %}{{ system_message }}{% for message in loop_messages %}{% if (message['role'] == 'user') != (loop.index0 % 2 == 0) %}{{ raise_exception('Conversation roles must alternate user/assistant/user/assistant/...') }}{% endif %}{% if message['role'] == 'user' %}{{ '### Instruction:\n' + message['content'].strip() + '\n\n' }}{% elif message['role'] == 'assistant' %}{{ '### Response:\n' + message['content'].strip() + '</s>\n\n' }}{% endif %}{% if loop.last and message['role'] == 'user' and add_generation_prompt %}{{ '### Instruction:\n' }}{% endif %}{% endfor %}
```

### Comparing `sillm-mlx-0.1.0/sillm/templates/cohere.jinja` & `sillm-mlx-0.1.1/sillm/templates/cohere.jinja`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.0/sillm/templates/gemma.jinja` & `sillm-mlx-0.1.1/sillm/templates/gemma.jinja`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.0/sillm/templates/llama2.jinja` & `sillm-mlx-0.1.1/sillm/templates/llama2.jinja`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.0/sillm/training/dataset.py` & `sillm-mlx-0.1.1/sillm/training/dataset.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.0/sillm/training/dpo.py` & `sillm-mlx-0.1.1/sillm/training/dpo.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,27 +60,28 @@
             self.reference.freeze()
             self.reference.train(mode=False)
 
         logger.info(f"Initialized DPO with reference model and loss type {loss_type}")
 
     def comparison(self,
                    prompt: str,
-                   temp: float = 0.0,
-                   num_tokens: int = 1024
+                   temperature: float = 0.0,
+                   max_tokens: int = 1024
                    ):
         """
         Generate comparison between policy and reference model completions.
         Args:
             prompt: Prompt to start generation.
-            num_tokens: Max number of tokens to generate.
+            temperature: Sampling temperature.
+            max_tokens: Max number of tokens to generate.
         Returns:
             Completions.
         """
-        reference_completion = ''.join([t[0] for t in generate(self.reference, self.tokenizer, prompt, temp=temp, num_tokens=num_tokens)])
-        policy_completion = ''.join([t[0] for t in generate(self.model, self.tokenizer, prompt, temp=temp, num_tokens=num_tokens)])
+        reference_completion = ''.join([t[0] for t in generate(self.reference, self.tokenizer, prompt, temperature==temperature, max_tokens=max_tokens)])
+        policy_completion = ''.join([t[0] for t in generate(self.model, self.tokenizer, prompt, temperature=temperature, max_tokens=max_tokens)])
 
         return reference_completion, policy_completion
 
     ########
     # References:
     # https://github.com/eric-mitchell/direct-preference-optimization
     # https://huggingface.co/docs/trl/main/en/dpo_trainer
```

### Comparing `sillm-mlx-0.1.0/sillm/training/lora.py` & `sillm-mlx-0.1.1/sillm/training/lora.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.0/sillm/utils/log.py` & `sillm-mlx-0.1.1/sillm/utils/log.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.0/sillm/utils/mapping.py` & `sillm-mlx-0.1.1/sillm/utils/mapping.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,18 +27,25 @@
         
         k = re.sub(r"^model\.layers\.", "layers.", k)
 
         k = re.sub(r"\.input_layernorm\.", ".attention_norm.", k)
         k = re.sub(r"\.post_attention_layernorm\.", ".ffn_norm.", k)
 
         k = re.sub(r"\.self_attn\.(q|k|v|o)_proj\.", r".attention.w\1.", k)
+        k = re.sub(r"\.self_attn\.(q|k)_norm\.", r".attention.\1_norm.", k)
         k = re.sub(r"\.mlp\.gate_proj\.", ".feed_forward.w1.", k)
         k = re.sub(r"\.mlp\.down_proj\.", ".feed_forward.w2.", k)
         k = re.sub(r"\.mlp\.up_proj\.", ".feed_forward.w3.", k)
 
+        # MoE
+        k = re.sub(r"\.block_sparse_moe\.gate\.", ".feed_forward.gate.", k)
+        k = re.sub(r"\.block_sparse_moe\.experts\.(\d+)\.w1.", r".feed_forward.experts.\1.w1.", k)
+        k = re.sub(r"\.block_sparse_moe\.experts\.(\d+)\.w2.", r".feed_forward.experts.\1.w2.", k)
+        k = re.sub(r"\.block_sparse_moe\.experts\.(\d+)\.w3.", r".feed_forward.experts.\1.w3.", k)
+
         # Phi mapping
         k = re.sub(r"\.self_attn\.dense\.", ".attention.wo.", k)
         k = re.sub(r"\.mlp\.fc1\.", ".feed_forward.w1.", k)
         k = re.sub(r"\.mlp\.fc2\.", ".feed_forward.w2.", k)
 
         # Starcoder2 mapping
         k = re.sub(r"\.mlp\.c_fc\.", ".feed_forward.w1.", k)
@@ -134,14 +141,16 @@
         "bos_token_id",
         "eos_token_id",
         "pad_token_id",
         "quantization",
         "moe",
         "tie_word_embeddings",
         "clip_qkv",
+        "use_qk_norm",
+        "logit_scale",
     ]
     for key in mlx_keys:
         if key in config:
             result[key] = config[key]
 
     key_map = {
         "hidden_size": "dim",
```

### Comparing `sillm-mlx-0.1.0/sillm/utils/plot.py` & `sillm-mlx-0.1.1/sillm/utils/plot.py`

 * *Files identical despite different names*

### Comparing `sillm-mlx-0.1.0/sillm_mlx.egg-info/PKG-INFO` & `sillm-mlx-0.1.1/sillm_mlx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sillm-mlx
-Version: 0.1.0
+Version: 0.1.1
 Summary: Running and training LLMs on Apple Silicon via MLX
 Home-page: https://github.com/armbues/SiLLM
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mlx>=0.10.0
 Requires-Dist: transformers>=4.39.3
@@ -54,14 +54,15 @@
 
 https://github.com/armbues/SiLLM/assets/4117144/833d63ab-08b1-45ca-980f-474c7e9cc284
 
 To start the web app, clone the repository and start the app using chainlit:
 ``` sh
 git clone https://github.com/armbues/SiLLM.git
 cd SiLLM/app
+pip install -r requirements.txt
 python -m chainlit run app.py -w
 ```
 Set the environment variables `SILLM_MODEL_DIR` and `SILLM_ADAPTER_DIR` to load local models/adapters.
 
 ### Command-line interface (CLI) scripts
 Run the CLI scripts with the argument -h to see a print-out of all available arguments.
 
@@ -142,22 +143,23 @@
 | Mixtral v0.1 | | | [8x7B-Instruct](https://huggingface.co/mlx-community/Mixtral-8x7B-Instruct-v0.1) |
 | Gemma | [2b](https://huggingface.co/google/gemma-2b), [2b-it](https://huggingface.co/google/gemma-7b-it), [7b](https://huggingface.co/google/gemma-7b), [7b-it](https://huggingface.co/google/gemma-7b-it) | |
 | Phi-2 | [2.7b](https://huggingface.co/microsoft/phi-2) | |
 | Qwen 1.5 | [7b-chat](https://huggingface.co/Qwen/Qwen1.5-7B-Chat), [14b-chat](https://huggingface.co/Qwen/Qwen1.5-14B-Chat) | |
 | StarCoder2 | [3b](https://huggingface.co/bigcode/starcoder2-3b), [7b](https://huggingface.co/bigcode/starcoder2-7b), [15b](https://huggingface.co/bigcode/starcoder2-15b) | |
 | CodeLlama | | [70b-instruct.Q4_0](https://huggingface.co/TheBloke/CodeLlama-70B-Instruct-GGUF), [Phind-34b-v2.Q4_0](https://huggingface.co/TheBloke/Phind-CodeLlama-34B-v2-GGUF) | |
 | DBRX | (currently not supported) | | [dbrx-instruct-4bit](https://huggingface.co/mlx-community/dbrx-instruct-4bit) |
-| Cohere | [Command-R](https://huggingface.co/CohereForAI/c4ai-command-r-v01) | |
+| Cohere | [Command-R](https://huggingface.co/CohereForAI/c4ai-command-r-v01), [Command-R+](CohereForAI/c4ai-command-r-plus) | |
 
 ## Roadmap
 
 - Repetition penalty for inference
 - Learning rate schedulers for training
 - Merging models
 - Saving models to GGUF
+- Fine tuning with ORPO
 
 ## License
 This project uses the [MIT License](LICENSE).
 
 ## Acknowledgments
 Big thanks to the Apple MLX team for implementing and maintaining the [MLX](https://github.com/ml-explore/mlx/) framework that makes it possible to unlock the power of Apple Silicon and run/train LLMs on MacBooks and other Apple devices. Thank you to all the contributors of the [MLX Examples](https://github.com/ml-explore/mlx-examples) project and developers sharing model implementations online.
 Last but not least, thank you to the larger community sharing open weights models, fine tunes, and datasets - without you all the gen AI progress would happen behind locked doors!
```

### Comparing `sillm-mlx-0.1.0/sillm_mlx.egg-info/SOURCES.txt` & `sillm-mlx-0.1.1/sillm_mlx.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 LICENSE
 README.md
-pyproject.toml
 setup.py
 sillm/__init__.py
 sillm/chat.py
 sillm/convert.py
 sillm/dpo.py
 sillm/lora.py
 sillm/quantize.py
@@ -25,20 +24,23 @@
 sillm/models/mixtral.py
 sillm/models/phi.py
 sillm/models/qwen2.py
 sillm/models/starcoder2.py
 sillm/templates/alpaca.jinja
 sillm/templates/chatml.jinja
 sillm/templates/cohere.jinja
+sillm/templates/empty.jinja
 sillm/templates/gemma.jinja
 sillm/templates/llama2.jinja
+sillm/templates/llama3.jinja
 sillm/templates/mistral.jinja
 sillm/templates/openchat.jinja
 sillm/templates/phi2.jinja
 sillm/templates/qwen2.jinja
+sillm/templates/vicuna.jinja
 sillm/training/__init__.py
 sillm/training/dataset.py
 sillm/training/dpo.py
 sillm/training/lora.py
 sillm/utils/__init__.py
 sillm/utils/common.py
 sillm/utils/log.py
```

