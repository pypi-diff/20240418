# Comparing `tmp/moviechat-0.1.0.tar.gz` & `tmp/moviechat-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moviechat-0.1.0.tar", last modified: Wed Apr 17 07:44:40 2024, max compression
+gzip compressed data, was "moviechat-0.2.0.tar", last modified: Thu Apr 18 15:37:49 2024, max compression
```

## Comparing `moviechat-0.1.0.tar` & `moviechat-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,75 @@
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-17 07:44:40.116592 moviechat-0.1.0/
--rw-rw-r--   0 exs       (1016) exs       (1016)     1501 2024-04-17 05:16:47.000000 moviechat-0.1.0/LICENSE
--rw-rw-r--   0 exs       (1016) exs       (1016)     1502 2024-04-17 05:16:51.000000 moviechat-0.1.0/LICENSE_Lavis.md
--rw-rw-r--   0 exs       (1016) exs       (1016)     1497 2024-04-17 05:16:51.000000 moviechat-0.1.0/LICENSE_Minigpt4.md
--rw-rw-r--   0 exs       (1016) exs       (1016)     1532 2024-04-17 05:16:51.000000 moviechat-0.1.0/LICENSE_videollama
--rw-r--r--   0 exs       (1016) exs       (1016)     2274 2024-04-17 07:44:40.112592 moviechat-0.1.0/PKG-INFO
--rw-rw-r--   0 exs       (1016) exs       (1016)     1901 2024-04-17 07:38:23.000000 moviechat-0.1.0/pyproject.toml
--rw-rw-r--   0 exs       (1016) exs       (1016)       38 2024-04-17 07:44:40.116592 moviechat-0.1.0/setup.cfg
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-17 07:44:40.112592 moviechat-0.1.0/src/
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-17 07:44:40.112592 moviechat-0.1.0/src/MovieChat.egg-info/
--rw-r--r--   0 exs       (1016) exs       (1016)     2274 2024-04-17 07:44:40.000000 moviechat-0.1.0/src/MovieChat.egg-info/PKG-INFO
--rw-rw-r--   0 exs       (1016) exs       (1016)      262 2024-04-17 07:44:40.000000 moviechat-0.1.0/src/MovieChat.egg-info/SOURCES.txt
--rw-rw-r--   0 exs       (1016) exs       (1016)        1 2024-04-17 07:44:40.000000 moviechat-0.1.0/src/MovieChat.egg-info/dependency_links.txt
--rw-rw-r--   0 exs       (1016) exs       (1016)      974 2024-04-17 07:44:40.000000 moviechat-0.1.0/src/MovieChat.egg-info/requires.txt
--rw-rw-r--   0 exs       (1016) exs       (1016)       44 2024-04-17 07:44:40.000000 moviechat-0.1.0/src/MovieChat.egg-info/top_level.txt
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-18 15:37:49.663462 moviechat-0.2.0/
+-rw-rw-r--   0 exs       (1016) exs       (1016)     1501 2024-04-17 05:16:47.000000 moviechat-0.2.0/LICENSE
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-18 15:37:49.655462 moviechat-0.2.0/MovieChat/
+-rw-rw-r--   0 exs       (1016) exs       (1016)      956 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/__init__.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-18 15:37:49.655462 moviechat-0.2.0/MovieChat/common/
+-rw-rw-r--   0 exs       (1016) exs       (1016)        0 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/common/__init__.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    15080 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/common/config.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     3620 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/common/dist_utils.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)      815 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/common/gradcam.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     6002 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/common/logger.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     3517 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/common/optims.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     9928 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/common/registry.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    13808 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/common/utils.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-18 15:37:49.655462 moviechat-0.2.0/MovieChat/conversation/
+-rw-rw-r--   0 exs       (1016) exs       (1016)        0 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/conversation/__init__.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    10954 2024-04-17 09:12:13.000000 moviechat-0.2.0/MovieChat/conversation/conversation_video.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-18 15:37:49.655462 moviechat-0.2.0/MovieChat/datasets/
+-rw-rw-r--   0 exs       (1016) exs       (1016)        0 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/datasets/__init__.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-18 15:37:49.655462 moviechat-0.2.0/MovieChat/datasets/builders/
+-rw-rw-r--   0 exs       (1016) exs       (1016)     2162 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/datasets/builders/__init__.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     8109 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/datasets/builders/base_dataset_builder.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     3004 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/datasets/builders/image_text_pair_builder.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     2393 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/datasets/builders/instruct_builder.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)      987 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/datasets/builders/video_caption_builder.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     6283 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/datasets/data_utils.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-18 15:37:49.659462 moviechat-0.2.0/MovieChat/datasets/datasets/
+-rw-rw-r--   0 exs       (1016) exs       (1016)        0 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/datasets/datasets/__init__.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     2067 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/datasets/datasets/base_dataset.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     2602 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/datasets/datasets/caption_datasets.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     1669 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/datasets/datasets/cc_sbu_dataset.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     4214 2024-04-17 09:11:31.000000 moviechat-0.2.0/MovieChat/datasets/datasets/dataloader_utils.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     1175 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/datasets/datasets/laion_dataset.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     8785 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/datasets/datasets/llava_instruct_dataset.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     9701 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/datasets/datasets/video_instruct_dataset.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     4437 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/datasets/datasets/webvid_datasets.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-18 15:37:49.659462 moviechat-0.2.0/MovieChat/models/
+-rw-rw-r--   0 exs       (1016) exs       (1016)    48450 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/models/Qformer.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     4294 2024-04-17 07:00:49.000000 moviechat-0.2.0/MovieChat/models/__init__.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     7147 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/models/base_model.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     7795 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/models/blip2.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     2331 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/models/blip2_outputs.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     9161 2024-04-18 14:38:08.000000 moviechat-0.2.0/MovieChat/models/chat_model.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    18684 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/models/eva_vit.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    14489 2024-04-17 09:11:15.000000 moviechat-0.2.0/MovieChat/models/eva_vit_with_tome.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     3989 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/models/helpers.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    33326 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/models/modeling_llama.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    32438 2024-04-18 14:38:48.000000 moviechat-0.2.0/MovieChat/models/moviechat.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    23136 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/models/multimodal_preprocessors.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    11438 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/models/process_video_data.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-18 15:37:49.659462 moviechat-0.2.0/MovieChat/processors/
+-rw-rw-r--   0 exs       (1016) exs       (1016)      999 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/processors/__init__.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)      610 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/processors/base_processor.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     4008 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/processors/blip_processors.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     3924 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/processors/functional_video.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    10960 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/processors/randaugment.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     5017 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/processors/transforms_video.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     6959 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/processors/video_processor.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-18 15:37:49.659462 moviechat-0.2.0/MovieChat/runners/
+-rw-rw-r--   0 exs       (1016) exs       (1016)      307 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/runners/__init__.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    22856 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/runners/runner_base.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)        0 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/runners/test.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-18 15:37:49.659462 moviechat-0.2.0/MovieChat/tasks/
+-rw-rw-r--   0 exs       (1016) exs       (1016)      837 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/tasks/__init__.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     8799 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/tasks/base_task.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)      540 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/tasks/image_text_pretrain.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)      540 2024-04-17 05:16:51.000000 moviechat-0.2.0/MovieChat/tasks/video_text_pretrain.py
+-rw-r--r--   0 exs       (1016) exs       (1016)     2047 2024-04-18 15:37:49.663462 moviechat-0.2.0/PKG-INFO
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-18 15:37:49.659462 moviechat-0.2.0/moviechat.egg-info/
+-rw-r--r--   0 exs       (1016) exs       (1016)     2047 2024-04-18 15:37:49.000000 moviechat-0.2.0/moviechat.egg-info/PKG-INFO
+-rw-rw-r--   0 exs       (1016) exs       (1016)     2166 2024-04-18 15:37:49.000000 moviechat-0.2.0/moviechat.egg-info/SOURCES.txt
+-rw-rw-r--   0 exs       (1016) exs       (1016)        1 2024-04-18 15:37:49.000000 moviechat-0.2.0/moviechat.egg-info/dependency_links.txt
+-rw-rw-r--   0 exs       (1016) exs       (1016)      905 2024-04-18 15:37:49.000000 moviechat-0.2.0/moviechat.egg-info/requires.txt
+-rw-rw-r--   0 exs       (1016) exs       (1016)       10 2024-04-18 15:37:49.000000 moviechat-0.2.0/moviechat.egg-info/top_level.txt
+-rw-rw-r--   0 exs       (1016) exs       (1016)     1804 2024-04-18 15:03:39.000000 moviechat-0.2.0/pyproject.toml
+-rw-rw-r--   0 exs       (1016) exs       (1016)       38 2024-04-18 15:37:49.663462 moviechat-0.2.0/setup.cfg
```

### Comparing `moviechat-0.1.0/LICENSE` & `moviechat-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moviechat-0.1.0/PKG-INFO` & `moviechat-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
-Name: MovieChat
-Version: 0.1.0
+Name: moviechat
+Version: 0.2.0
 Summary: Long video understanding
 Author-email: Enxin Song <enxin.song.dut@gmail.com>
 License: MIT License
 Project-URL: homepage, https://rese1f.github.io/MovieChat/
 Project-URL: repository, https://github.com/rese1f/MovieChat
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-License-File: LICENSE_Lavis.md
-License-File: LICENSE_Minigpt4.md
-License-File: LICENSE_videollama
 Requires-Dist: pip>=23.1.2
 Requires-Dist: torch==2.0.1
 Requires-Dist: pytorch-mutex==1.0; extra == "cuda"
 Requires-Dist: torchaudio==2.0.2
 Requires-Dist: torchvision==0.15.2
 Requires-Dist: accelerate==0.16.0
 Requires-Dist: aiohttp==3.8.4
@@ -34,15 +31,14 @@
 Requires-Dist: importlib-resources==5.12.0
 Requires-Dist: kiwisolver==1.4.4
 Requires-Dist: matplotlib==3.7.0
 Requires-Dist: multidict==6.0.4
 Requires-Dist: openai==0.27.0
 Requires-Dist: packaging==23.0
 Requires-Dist: psutil==5.9.4
-Requires-Dist: pycocotools==2.0.6
 Requires-Dist: pyparsing==3.0.9
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: pyyaml==6.0
 Requires-Dist: regex==2022.10.31
 Requires-Dist: tokenizers==0.13.2
 Requires-Dist: tqdm==4.64.1
 Requires-Dist: transformers==4.28.0
@@ -54,17 +50,14 @@
 Requires-Dist: yarl==1.8.2
 Requires-Dist: zipp==3.14.0
 Requires-Dist: omegaconf==2.3.0
 Requires-Dist: opencv-python==4.7.0.72
 Requires-Dist: iopath==0.1.10
 Requires-Dist: decord==0.6.0
 Requires-Dist: tenacity==8.2.2
-Requires-Dist: gradio==3.24.1
-Requires-Dist: gradio-client==0.0.8
-Requires-Dist: wandb==0.16.0
 Requires-Dist: einops==0.6.1
 Requires-Dist: SentencePiece==0.1.99
 Requires-Dist: ftfy==6.1.1
 Requires-Dist: pytorchvideo==0.1.5
 Requires-Dist: GPUtil==1.4.0
 Requires-Dist: moviepy==1.0.3
 Requires-Dist: scikit-image==0.21.0
```

### Comparing `moviechat-0.1.0/pyproject.toml` & `moviechat-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
-name = "MovieChat"
-version = "0.1.0"
+name = "moviechat"
+version = "0.2.0"
 description = "Long video understanding"
 authors = [
     { name = "Enxin Song", email = "enxin.song.dut@gmail.com" },
 ]
 license = {text = "MIT License"}
 readme = "README.md"
 requires-python = ">=3.7"
@@ -35,15 +35,14 @@
     "importlib-resources==5.12.0",
     "kiwisolver==1.4.4",
     "matplotlib==3.7.0",
     "multidict==6.0.4",
     "openai==0.27.0",
     "packaging==23.0",
     "psutil==5.9.4",
-    "pycocotools==2.0.6",
     "pyparsing==3.0.9",
     "python-dateutil==2.8.2",
     "pyyaml==6.0",
     "regex==2022.10.31",
     "tokenizers==0.13.2",
     "tqdm==4.64.1",
     "transformers==4.28.0",
@@ -55,17 +54,14 @@
     "yarl==1.8.2",
     "zipp==3.14.0",
     "omegaconf==2.3.0",
     "opencv-python==4.7.0.72",
     "iopath==0.1.10",
     "decord==0.6.0",
     "tenacity==8.2.2",
-    "gradio==3.24.1",
-    "gradio-client==0.0.8",
-    "wandb==0.16.0",
     "einops==0.6.1",
     "SentencePiece==0.1.99",
     "ftfy==6.1.1",
     "pytorchvideo==0.1.5",
     "GPUtil==1.4.0",
     "moviepy==1.0.3",
     "scikit-image==0.21.0",
```

### Comparing `moviechat-0.1.0/src/MovieChat.egg-info/PKG-INFO` & `moviechat-0.2.0/moviechat.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
-Name: MovieChat
-Version: 0.1.0
+Name: moviechat
+Version: 0.2.0
 Summary: Long video understanding
 Author-email: Enxin Song <enxin.song.dut@gmail.com>
 License: MIT License
 Project-URL: homepage, https://rese1f.github.io/MovieChat/
 Project-URL: repository, https://github.com/rese1f/MovieChat
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-License-File: LICENSE_Lavis.md
-License-File: LICENSE_Minigpt4.md
-License-File: LICENSE_videollama
 Requires-Dist: pip>=23.1.2
 Requires-Dist: torch==2.0.1
 Requires-Dist: pytorch-mutex==1.0; extra == "cuda"
 Requires-Dist: torchaudio==2.0.2
 Requires-Dist: torchvision==0.15.2
 Requires-Dist: accelerate==0.16.0
 Requires-Dist: aiohttp==3.8.4
@@ -34,15 +31,14 @@
 Requires-Dist: importlib-resources==5.12.0
 Requires-Dist: kiwisolver==1.4.4
 Requires-Dist: matplotlib==3.7.0
 Requires-Dist: multidict==6.0.4
 Requires-Dist: openai==0.27.0
 Requires-Dist: packaging==23.0
 Requires-Dist: psutil==5.9.4
-Requires-Dist: pycocotools==2.0.6
 Requires-Dist: pyparsing==3.0.9
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: pyyaml==6.0
 Requires-Dist: regex==2022.10.31
 Requires-Dist: tokenizers==0.13.2
 Requires-Dist: tqdm==4.64.1
 Requires-Dist: transformers==4.28.0
@@ -54,17 +50,14 @@
 Requires-Dist: yarl==1.8.2
 Requires-Dist: zipp==3.14.0
 Requires-Dist: omegaconf==2.3.0
 Requires-Dist: opencv-python==4.7.0.72
 Requires-Dist: iopath==0.1.10
 Requires-Dist: decord==0.6.0
 Requires-Dist: tenacity==8.2.2
-Requires-Dist: gradio==3.24.1
-Requires-Dist: gradio-client==0.0.8
-Requires-Dist: wandb==0.16.0
 Requires-Dist: einops==0.6.1
 Requires-Dist: SentencePiece==0.1.99
 Requires-Dist: ftfy==6.1.1
 Requires-Dist: pytorchvideo==0.1.5
 Requires-Dist: GPUtil==1.4.0
 Requires-Dist: moviepy==1.0.3
 Requires-Dist: scikit-image==0.21.0
```

### Comparing `moviechat-0.1.0/src/MovieChat.egg-info/requires.txt` & `moviechat-0.2.0/moviechat.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 importlib-resources==5.12.0
 kiwisolver==1.4.4
 matplotlib==3.7.0
 multidict==6.0.4
 openai==0.27.0
 packaging==23.0
 psutil==5.9.4
-pycocotools==2.0.6
 pyparsing==3.0.9
 python-dateutil==2.8.2
 pyyaml==6.0
 regex==2022.10.31
 tokenizers==0.13.2
 tqdm==4.64.1
 transformers==4.28.0
@@ -39,17 +38,14 @@
 yarl==1.8.2
 zipp==3.14.0
 omegaconf==2.3.0
 opencv-python==4.7.0.72
 iopath==0.1.10
 decord==0.6.0
 tenacity==8.2.2
-gradio==3.24.1
-gradio-client==0.0.8
-wandb==0.16.0
 einops==0.6.1
 SentencePiece==0.1.99
 ftfy==6.1.1
 pytorchvideo==0.1.5
 GPUtil==1.4.0
 moviepy==1.0.3
 scikit-image==0.21.0
```

