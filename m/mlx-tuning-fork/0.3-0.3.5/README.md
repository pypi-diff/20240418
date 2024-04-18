# Comparing `tmp/mlx-tuning-fork-0.3.tar.gz` & `tmp/mlx_tuning_fork-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlx-tuning-fork-0.3.tar", last modified: Fri Mar 15 21:14:48 2024, max compression
+gzip compressed data, was "mlx_tuning_fork-0.3.5.tar", last modified: Thu Apr 18 15:11:45 2024, max compression
```

## Comparing `mlx-tuning-fork-0.3.tar` & `mlx_tuning_fork-0.3.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 chimezie  (1000) chimezie  (1000)        0 2024-03-15 21:14:48.638599 mlx-tuning-fork-0.3/
--rw-rw-r--   0 chimezie  (1000) chimezie  (1000)     1069 2024-01-31 21:45:51.000000 mlx-tuning-fork-0.3/LICENSE
--rw-r--r--   0 chimezie  (1000) chimezie  (1000)    11500 2024-03-15 21:14:48.638599 mlx-tuning-fork-0.3/PKG-INFO
--rw-rw-r--   0 chimezie  (1000) chimezie  (1000)     9595 2024-03-14 19:29:10.000000 mlx-tuning-fork-0.3/README.md
--rw-rw-r--   0 chimezie  (1000) chimezie  (1000)      780 2024-03-14 20:30:34.000000 mlx-tuning-fork-0.3/pyproject.toml
--rw-rw-r--   0 chimezie  (1000) chimezie  (1000)       38 2024-03-15 21:14:48.638599 mlx-tuning-fork-0.3/setup.cfg
-drwxrwxr-x   0 chimezie  (1000) chimezie  (1000)        0 2024-03-15 21:14:48.626598 mlx-tuning-fork-0.3/src/
-drwxrwxr-x   0 chimezie  (1000) chimezie  (1000)        0 2024-03-15 21:14:48.630598 mlx-tuning-fork-0.3/src/mlx_tuning_fork/
--rw-rw-r--   0 chimezie  (1000) chimezie  (1000)       19 2024-03-14 19:29:10.000000 mlx-tuning-fork-0.3/src/mlx_tuning_fork/__init__.py
--rw-rw-r--   0 chimezie  (1000) chimezie  (1000)     1361 2024-03-14 20:16:40.000000 mlx-tuning-fork-0.3/src/mlx_tuning_fork/config.py
--rw-rw-r--   0 chimezie  (1000) chimezie  (1000)      558 2024-03-14 19:33:53.000000 mlx-tuning-fork-0.3/src/mlx_tuning_fork/dataset.py
-drwxrwxr-x   0 chimezie  (1000) chimezie  (1000)        0 2024-03-15 21:14:48.638599 mlx-tuning-fork-0.3/src/mlx_tuning_fork/prompt_templates/
--rw-rw-r--   0 chimezie  (1000) chimezie  (1000)        0 2024-01-31 21:48:49.000000 mlx-tuning-fork-0.3/src/mlx_tuning_fork/prompt_templates/__init__.py
--rw-rw-r--   0 chimezie  (1000) chimezie  (1000)      417 2024-02-14 20:20:23.000000 mlx-tuning-fork-0.3/src/mlx_tuning_fork/prompt_templates/chatml.py
--rw-rw-r--   0 chimezie  (1000) chimezie  (1000)      590 2024-02-14 20:20:25.000000 mlx-tuning-fork-0.3/src/mlx_tuning_fork/prompt_templates/mistral.py
--rw-rw-r--   0 chimezie  (1000) chimezie  (1000)      799 2024-03-14 19:29:10.000000 mlx-tuning-fork-0.3/src/mlx_tuning_fork/reporting.py
--rw-rw-r--   0 chimezie  (1000) chimezie  (1000)    16444 2024-03-14 19:29:10.000000 mlx-tuning-fork-0.3/src/mlx_tuning_fork/training.py
-drwxrwxr-x   0 chimezie  (1000) chimezie  (1000)        0 2024-03-15 21:14:48.638599 mlx-tuning-fork-0.3/src/mlx_tuning_fork/tuning/
--rw-rw-r--   0 chimezie  (1000) chimezie  (1000)        0 2024-02-05 22:25:35.000000 mlx-tuning-fork-0.3/src/mlx_tuning_fork/tuning/__init__.py
-drwxrwxr-x   0 chimezie  (1000) chimezie  (1000)        0 2024-03-15 21:14:48.638599 mlx-tuning-fork-0.3/src/mlx_tuning_fork/tuning/dynamic_learning/
--rw-rw-r--   0 chimezie  (1000) chimezie  (1000)     2949 2024-03-14 19:29:10.000000 mlx-tuning-fork-0.3/src/mlx_tuning_fork/tuning/dynamic_learning/__init__.py
--rw-rw-r--   0 chimezie  (1000) chimezie  (1000)     4332 2024-03-14 19:34:15.000000 mlx-tuning-fork-0.3/src/mlx_tuning_fork/wandb_sweep.py
-drwxrwxr-x   0 chimezie  (1000) chimezie  (1000)        0 2024-03-15 21:14:48.638599 mlx-tuning-fork-0.3/src/mlx_tuning_fork.egg-info/
--rw-r--r--   0 chimezie  (1000) chimezie  (1000)    11500 2024-03-15 21:14:48.000000 mlx-tuning-fork-0.3/src/mlx_tuning_fork.egg-info/PKG-INFO
--rw-rw-r--   0 chimezie  (1000) chimezie  (1000)      709 2024-03-15 21:14:48.000000 mlx-tuning-fork-0.3/src/mlx_tuning_fork.egg-info/SOURCES.txt
--rw-rw-r--   0 chimezie  (1000) chimezie  (1000)        1 2024-03-15 21:14:48.000000 mlx-tuning-fork-0.3/src/mlx_tuning_fork.egg-info/dependency_links.txt
--rw-rw-r--   0 chimezie  (1000) chimezie  (1000)       51 2024-03-15 21:14:48.000000 mlx-tuning-fork-0.3/src/mlx_tuning_fork.egg-info/requires.txt
--rw-rw-r--   0 chimezie  (1000) chimezie  (1000)       16 2024-03-15 21:14:48.000000 mlx-tuning-fork-0.3/src/mlx_tuning_fork.egg-info/top_level.txt
-drwxrwxr-x   0 chimezie  (1000) chimezie  (1000)        0 2024-03-15 21:14:48.638599 mlx-tuning-fork-0.3/tests/
--rw-rw-r--   0 chimezie  (1000) chimezie  (1000)     1451 2024-03-14 19:58:25.000000 mlx-tuning-fork-0.3/tests/test_scheduler_config.py
+drwxrwxr-x   0 chimezie  (1000) chimezie  (1000)        0 2024-04-18 15:11:45.096595 mlx_tuning_fork-0.3.5/
+-rw-rw-r--   0 chimezie  (1000) chimezie  (1000)     1069 2024-01-31 21:45:51.000000 mlx_tuning_fork-0.3.5/LICENSE
+-rw-r--r--   0 chimezie  (1000) chimezie  (1000)    11691 2024-04-18 15:11:45.096595 mlx_tuning_fork-0.3.5/PKG-INFO
+-rw-rw-r--   0 chimezie  (1000) chimezie  (1000)     9784 2024-04-18 14:53:46.000000 mlx_tuning_fork-0.3.5/README.md
+-rw-rw-r--   0 chimezie  (1000) chimezie  (1000)      782 2024-04-18 14:53:46.000000 mlx_tuning_fork-0.3.5/pyproject.toml
+-rw-rw-r--   0 chimezie  (1000) chimezie  (1000)       38 2024-04-18 15:11:45.096595 mlx_tuning_fork-0.3.5/setup.cfg
+drwxrwxr-x   0 chimezie  (1000) chimezie  (1000)        0 2024-04-18 15:11:45.084595 mlx_tuning_fork-0.3.5/src/
+drwxrwxr-x   0 chimezie  (1000) chimezie  (1000)        0 2024-04-18 15:11:45.092595 mlx_tuning_fork-0.3.5/src/mlx_tuning_fork/
+-rw-rw-r--   0 chimezie  (1000) chimezie  (1000)       21 2024-04-18 14:53:46.000000 mlx_tuning_fork-0.3.5/src/mlx_tuning_fork/__init__.py
+-rw-rw-r--   0 chimezie  (1000) chimezie  (1000)     1354 2024-04-06 16:00:50.000000 mlx_tuning_fork-0.3.5/src/mlx_tuning_fork/config.py
+-rw-rw-r--   0 chimezie  (1000) chimezie  (1000)      558 2024-03-14 19:33:53.000000 mlx_tuning_fork-0.3.5/src/mlx_tuning_fork/dataset.py
+drwxrwxr-x   0 chimezie  (1000) chimezie  (1000)        0 2024-04-18 15:11:45.092595 mlx_tuning_fork-0.3.5/src/mlx_tuning_fork/prompt_templates/
+-rw-rw-r--   0 chimezie  (1000) chimezie  (1000)        0 2024-01-31 21:48:49.000000 mlx_tuning_fork-0.3.5/src/mlx_tuning_fork/prompt_templates/__init__.py
+-rw-rw-r--   0 chimezie  (1000) chimezie  (1000)      417 2024-02-14 20:20:23.000000 mlx_tuning_fork-0.3.5/src/mlx_tuning_fork/prompt_templates/chatml.py
+-rw-rw-r--   0 chimezie  (1000) chimezie  (1000)      590 2024-02-14 20:20:25.000000 mlx_tuning_fork-0.3.5/src/mlx_tuning_fork/prompt_templates/mistral.py
+-rw-rw-r--   0 chimezie  (1000) chimezie  (1000)     1399 2024-03-28 21:43:55.000000 mlx_tuning_fork-0.3.5/src/mlx_tuning_fork/reporting.py
+-rw-rw-r--   0 chimezie  (1000) chimezie  (1000)    16103 2024-04-15 20:36:17.000000 mlx_tuning_fork-0.3.5/src/mlx_tuning_fork/training.py
+drwxrwxr-x   0 chimezie  (1000) chimezie  (1000)        0 2024-04-18 15:11:45.092595 mlx_tuning_fork-0.3.5/src/mlx_tuning_fork/tuning/
+-rw-rw-r--   0 chimezie  (1000) chimezie  (1000)        0 2024-02-05 22:25:35.000000 mlx_tuning_fork-0.3.5/src/mlx_tuning_fork/tuning/__init__.py
+drwxrwxr-x   0 chimezie  (1000) chimezie  (1000)        0 2024-04-18 15:11:45.092595 mlx_tuning_fork-0.3.5/src/mlx_tuning_fork/tuning/dynamic_learning/
+-rw-rw-r--   0 chimezie  (1000) chimezie  (1000)     3046 2024-03-22 14:35:50.000000 mlx_tuning_fork-0.3.5/src/mlx_tuning_fork/tuning/dynamic_learning/__init__.py
+-rw-rw-r--   0 chimezie  (1000) chimezie  (1000)     9339 2024-04-17 19:48:11.000000 mlx_tuning_fork-0.3.5/src/mlx_tuning_fork/wandb_sweep.py
+drwxrwxr-x   0 chimezie  (1000) chimezie  (1000)        0 2024-04-18 15:11:45.096595 mlx_tuning_fork-0.3.5/src/mlx_tuning_fork.egg-info/
+-rw-r--r--   0 chimezie  (1000) chimezie  (1000)    11691 2024-04-18 15:11:45.000000 mlx_tuning_fork-0.3.5/src/mlx_tuning_fork.egg-info/PKG-INFO
+-rw-rw-r--   0 chimezie  (1000) chimezie  (1000)      709 2024-04-18 15:11:45.000000 mlx_tuning_fork-0.3.5/src/mlx_tuning_fork.egg-info/SOURCES.txt
+-rw-rw-r--   0 chimezie  (1000) chimezie  (1000)        1 2024-04-18 15:11:45.000000 mlx_tuning_fork-0.3.5/src/mlx_tuning_fork.egg-info/dependency_links.txt
+-rw-rw-r--   0 chimezie  (1000) chimezie  (1000)       51 2024-04-18 15:11:45.000000 mlx_tuning_fork-0.3.5/src/mlx_tuning_fork.egg-info/requires.txt
+-rw-rw-r--   0 chimezie  (1000) chimezie  (1000)       16 2024-04-18 15:11:45.000000 mlx_tuning_fork-0.3.5/src/mlx_tuning_fork.egg-info/top_level.txt
+drwxrwxr-x   0 chimezie  (1000) chimezie  (1000)        0 2024-04-18 15:11:45.096595 mlx_tuning_fork-0.3.5/tests/
+-rw-rw-r--   0 chimezie  (1000) chimezie  (1000)     1417 2024-04-18 15:04:52.000000 mlx_tuning_fork-0.3.5/tests/test_scheduler_config.py
```

### Comparing `mlx-tuning-fork-0.3/LICENSE` & `mlx_tuning_fork-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mlx-tuning-fork-0.3/PKG-INFO` & `mlx_tuning_fork-0.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx-tuning-fork
-Version: 0.3
+Version: 0.3.5
 Summary: Basic framework for LLM (Q)LoRA fine-tuning using mlx, mlx_lm, and OgbujiPT.
 Author-email: Chimezie Ogbuji <chimezie@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Chime Ogbuji
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,18 +46,18 @@
 Large Language Model (Q)LoRa fine-tuning with MLX.  It uses [mlx](https://github.com/ml-explore/mlx), [mlx_lm](https://github.com/ml-explore/mlx-examples/tree/main/llms/mlx_lm), 
 and [OgbujiPT](https://github.com/OoriData/OgbujiPT), and is based primarily on the excellent mlx-example libraries
 but adds very minimal architecture for systematic running of easily parameterized fine tunes, hyperparameter sweeping,
 declarative prompt construction, an equivalent of HF's [train on completions](https://huggingface.co/docs/trl/sft_trainer#train-on-completions-only), and other capabilities.  
 
 ## Installation
 
-For now, can be installed by cloning the repository and running (in the local working copy)
+Can be installed via:
 
 ```bash
-$ pip install .
+$ pip install mlx-tuning-fork
 ```
 
 Currently just has a single Mistral prompt format (-f/ --prompt-format) module, but with mlx-lm and OgbujiPT you can do something similar with other models:
 
 * Llama
 * Mixtral
 * Qwen
@@ -166,15 +166,16 @@
 the user prompt.  If two values are provided, they should be quoted and separated by spaces.  The first refers to 
 a table that provides the system prompt and the second refers to the user prompt.  Finally, if three values are provided
 they are assumed to be system prompt, context, and user prompt.
 
 If they are not specified via ``--build-prompt``, the system prompt is assumed to be specified in a table named 
 **system_prompt**, the context is from a table named **context**, and the user prompt is from a table named **question**.
 
-
+If any of the table header name of the context is of the form ``[filename.txt]`` the contents of the specified filename are used
+for the instead.
 
 If any of the text values in the corresponding tables have curly braces, the ``--loom-markers`` option can be used
 to provide values for the names specified in between the braces.  It is expected to be a string in the format: 
 ``name=[.. value ..]``.
 
 So, the following command-line:
 
@@ -235,14 +236,16 @@
 
 ```commandline
 $ python -m mlx_tuning_fork.wandb_sweep --help
 Usage: python -m mlx_tuning_fork.wandb_sweep [OPTIONS] CONFIG_FILE
 
 Options:
   --verbose / --no-verbose
-  --wandb-project TEXT      Wandb project name
-  --help                    Show this message and exit.
+  --wandb-project TEXT            Wandb project name
+  --train-type [completion-only|self-supervised]
+  -f, --prompt-format [mistral|chatml]
+  --help                          Show this message and exit.
 ```
 
 It takes a single argument which is a [Wandb sweep configuration (YAML) file](https://docs.wandb.ai/guides/sweeps/define-sweep-configuration)
  .  The `--wandb-project` options refers to a Wandb project where the sweep output is be stored.
```

### Comparing `mlx-tuning-fork-0.3/README.md` & `mlx_tuning_fork-0.3.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 Large Language Model (Q)LoRa fine-tuning with MLX.  It uses [mlx](https://github.com/ml-explore/mlx), [mlx_lm](https://github.com/ml-explore/mlx-examples/tree/main/llms/mlx_lm), 
 and [OgbujiPT](https://github.com/OoriData/OgbujiPT), and is based primarily on the excellent mlx-example libraries
 but adds very minimal architecture for systematic running of easily parameterized fine tunes, hyperparameter sweeping,
 declarative prompt construction, an equivalent of HF's [train on completions](https://huggingface.co/docs/trl/sft_trainer#train-on-completions-only), and other capabilities.  
 
 ## Installation
 
-For now, can be installed by cloning the repository and running (in the local working copy)
+Can be installed via:
 
 ```bash
-$ pip install .
+$ pip install mlx-tuning-fork
 ```
 
 Currently just has a single Mistral prompt format (-f/ --prompt-format) module, but with mlx-lm and OgbujiPT you can do something similar with other models:
 
 * Llama
 * Mixtral
 * Qwen
@@ -123,15 +123,16 @@
 the user prompt.  If two values are provided, they should be quoted and separated by spaces.  The first refers to 
 a table that provides the system prompt and the second refers to the user prompt.  Finally, if three values are provided
 they are assumed to be system prompt, context, and user prompt.
 
 If they are not specified via ``--build-prompt``, the system prompt is assumed to be specified in a table named 
 **system_prompt**, the context is from a table named **context**, and the user prompt is from a table named **question**.
 
-
+If any of the table header name of the context is of the form ``[filename.txt]`` the contents of the specified filename are used
+for the instead.
 
 If any of the text values in the corresponding tables have curly braces, the ``--loom-markers`` option can be used
 to provide values for the names specified in between the braces.  It is expected to be a string in the format: 
 ``name=[.. value ..]``.
 
 So, the following command-line:
 
@@ -192,14 +193,16 @@
 
 ```commandline
 $ python -m mlx_tuning_fork.wandb_sweep --help
 Usage: python -m mlx_tuning_fork.wandb_sweep [OPTIONS] CONFIG_FILE
 
 Options:
   --verbose / --no-verbose
-  --wandb-project TEXT      Wandb project name
-  --help                    Show this message and exit.
+  --wandb-project TEXT            Wandb project name
+  --train-type [completion-only|self-supervised]
+  -f, --prompt-format [mistral|chatml]
+  --help                          Show this message and exit.
 ```
 
 It takes a single argument which is a [Wandb sweep configuration (YAML) file](https://docs.wandb.ai/guides/sweeps/define-sweep-configuration)
  .  The `--wandb-project` options refers to a Wandb project where the sweep output is be stored.
```

### Comparing `mlx-tuning-fork-0.3/pyproject.toml` & `mlx_tuning_fork-0.3.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mlx-tuning-fork"
-version = "0.3"
+version = "0.3.5"
 dependencies = [
     "mlx",
     "click",
     "tqdm",
     "ogbujipt",
     "numpy",
     "mlx-lm",
```

### Comparing `mlx-tuning-fork-0.3/src/mlx_tuning_fork/config.py` & `mlx_tuning_fork-0.3.5/src/mlx_tuning_fork/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     "iters": -1,
     "epochs": -1,
     "val_batches": 25,
     "learning_rate": 1e-5,
     "steps_per_report": 10,
     "steps_per_eval": 200,
     "resume_adapter_file": None,
-    "adapter_file": "adapters.npz",
     "test": False,
     "test_batches": 500,
     "max_seq_length": 2048,
     "seed": 0,
     "max_tokens": 100,
     "save_every": 100,
     "validation_scale": 5,
@@ -43,9 +42,9 @@
     "validation_interval_proportion": 0.2, #200/1000
     "validations_per_train_item": .5,
     "adapter_save_interval_proportion": .1,
     "ignore_chat_template": False,
     "colorize": False,
     "trust_remote_code": False,
     "lora_parameters": {"rank": 8, "alpha": 16, "dropout": 0.0, "scale": 10.0},
-
-}
+    "grad_checkpoint": False
+}
```

### Comparing `mlx-tuning-fork-0.3/src/mlx_tuning_fork/dataset.py` & `mlx_tuning_fork-0.3.5/src/mlx_tuning_fork/dataset.py`

 * *Files identical despite different names*

### Comparing `mlx-tuning-fork-0.3/src/mlx_tuning_fork/prompt_templates/mistral.py` & `mlx_tuning_fork-0.3.5/src/mlx_tuning_fork/prompt_templates/mistral.py`

 * *Files identical despite different names*

### Comparing `mlx-tuning-fork-0.3/src/mlx_tuning_fork/training.py` & `mlx_tuning_fork-0.3.5/src/mlx_tuning_fork/training.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import warnings
 
 import mlx.optimizers as optim
 import numpy as np
-from mlx_lm.tuner.trainer import TrainingArgs, default_loss, evaluate, train
+from mlx_lm.tuner.trainer import TrainingArgs, default_loss, evaluate, train, iterate_batches
 from mlx_lm.tuner.utils import linear_to_lora_layers
-from mlx_lm.utils import load, generate
+from mlx_lm.utils import load, generate, save_config
+from mlx_lm.lora import print_trainable_parameters
 from mlx_lm.generate import colorprint_by_t0
-from mlx_lm import lora
+from mlx_lm.tuner.datasets import Dataset as mlx_lm_dataset
 from types import SimpleNamespace
 import mlx.core as mx
 from tqdm import tqdm
 import mlx.nn as nn
 import click
 import yaml
 import math
@@ -37,21 +38,29 @@
     ce = nn.losses.cross_entropy(logits, shifted_labels) * mask
     ntoks = mask.sum()
     ce = ce.sum() / ntoks
     return ce, ntoks
 
 
 def completions_only_iterate_batches(dataset, tokenizer, batch_size, max_seq_length, train=False):
+    #idx = sorted(range(len(dataset)), key=lambda idx: len(dataset[idx]))
+    #See https://github.com/ml-explore/mlx-examples/issues/583
+    idx = range(len(dataset))
+
+    # Make the batches:
+    batch_idx = [
+        idx[i: i + batch_size] for i in range(0, len(idx) - batch_size + 1, batch_size)
+    ]
     while True:
-        indices = np.random.permutation(np.arange(len(dataset)))
-        for i in range(0, len(indices) - batch_size + 1, batch_size):
+        indices = np.random.permutation(len(batch_idx))
+        for i in indices:
             input_text = []
             output_text = []
-            for j in range(batch_size):
-                record = dataset[indices[i + j]]
+            for j in batch_idx[i]:
+                record = dataset[j]
                 input_text.append(prompt_formatter.get_input(record))
                 output_text.append(prompt_formatter.get_output(record))
 
             input_batch = [tokenizer.encode(record) for record in input_text]
             output_batch = [tokenizer.encode(record, add_special_tokens=False) +
                             [tokenizer.eos_token_id] for record in output_text]
 
@@ -63,74 +72,32 @@
 
             if max(lengths) > max_seq_length:
                 print(
                     f"[WARNING] Some sequences are longer than {max_seq_length} tokens. "
                     f"The longest sentence {max(lengths)} will be truncated to {max_seq_length}. "
                     "Consider pre-splitting your data to save memory."
                 )
+            pad_to = 8
+            max_length_in_batch = pad_to * ((max(lengths) + pad_to - 1) // pad_to)
+            max_length_in_batch = min(max_length_in_batch, max_seq_length)
 
-            max_width = min(max(lengths), max_seq_length)
-
-            batch_arr = np.zeros((batch_size, max_width), np.int32)
+            batch_arr = np.zeros((batch_size, max_length_in_batch), np.int32)
             adjusted_lengths = []
             for j in range(batch_size):
                 input_length = input_lengths[j]
-                full_ids_end_idx = input_length + min(output_lengths[j], max_width - input_length)
+                full_ids_end_idx = input_length + min(output_lengths[j], max_length_in_batch - input_length)
                 adjusted_lengths.append(full_ids_end_idx)
                 batch_arr[j, :full_ids_end_idx] = full_labels[j][:full_ids_end_idx]
             batch = mx.array(batch_arr)
-            if train:
-                pbar.update(1)
             yield batch, mx.array(input_lengths), mx.array(adjusted_lengths)
 
         if not train:
             break
 
 
-def iterate_batches(dataset, tokenizer, batch_size, max_seq_length, train=False):
-    while True:
-        # Shuffle indices
-        indices = np.arange(len(dataset))
-        indices = np.random.permutation(indices)
-        # Collect batches from dataset
-        for i in range(0, len(indices) - batch_size + 1, batch_size):
-            # Encode batch
-            batch = [
-                tokenizer.encode(
-                    prompt_formatter.get_input(dataset[indices[i + j]]) +
-                    prompt_formatter.get_output(dataset[indices[i + j]])
-                ) for j in range(batch_size)
-            ]
-            lengths = [len(x) for x in batch]
-
-            if max(lengths) > max_seq_length:
-                print(
-                    f"[WARNING] Some sequences are longer than {max_seq_length} tokens. "
-                    f"The longest sentence {max(lengths)} will be truncated to {max_seq_length}. "
-                    "Consider pre-splitting your data to save memory."
-                )
-
-            # Pad to the max length
-            max_length_in_batch = min(max(lengths), max_seq_length)
-            batch_arr = np.zeros((batch_size, max_length_in_batch), np.int32)
-
-            for j in range(batch_size):
-                truncated_length = min(lengths[j], max_seq_length)
-                batch_arr[j, :truncated_length] = batch[j][:truncated_length]
-                lengths[j] = (
-                    truncated_length  # Update lengths to match truncated lengths
-                )
-            batch = mx.array(batch_arr)
-
-            yield batch[:, :-1], batch[:, 1:], mx.array(lengths)
-
-        if not train:
-            break
-
-
 def generate_prompt_from_loom(loom_file, loom_markers, prompt_formatter, build_prompt):
     with open(loom_file, mode='rb') as fp:
         loom = word_loom.load(fp)
         if build_prompt is not None:
             loom_sections = build_prompt.split(' ')
             num_loom_sections = len(loom_sections)
             if num_loom_sections not in [1, 2, 3]:
@@ -149,15 +116,19 @@
                 question_section = loom_sections[2]
         else:
             system_section = 'system_prompt'
             extra_context_section = 'context'
             question_section = 'question'
         question = loom[question_section]
         system = loom.get(system_section, '')
-        extra_context = loom.get(extra_context_section, '')
+        if extra_context_section[0] == '[' and extra_context_section[-1] == ']':
+            with open(extra_context_section[1:-1], 'r') as f:
+                extra_context = f.read()
+        else:
+            extra_context = loom.get(extra_context_section, '')
         if loom_markers is not None:
             marker, value = loom_markers.split('=')
             question = question.format(**{marker: value})
         return format(question, preamble=system, contexts=extra_context, delimiters=prompt_formatter.get_delimiters())
 
 @click.command()
 @click.option('--verbose/--no-verbose', default=False)
@@ -189,24 +160,22 @@
               help='Sampling top-p')
 @click.option('--build-prompt', default=None, type=str,
               help='Which word loom sections to use in building the claim (space-separated list of sections)')
 @click.argument('config_file')
 def main(verbose, summary, loom_file, loom_markers, prompt, temperature, num_tokens, train_type, prompt_format, adapter,
          wandb_project, wandb_run, repetition_penalty, repetition_context_size, top_p, config_file,
          build_prompt):
-    global pbar, prompt_formatter
+    global prompt_formatter
     if prompt_format == 'mistral':
         from mlx_tuning_fork.prompt_templates.mistral import TrainingRecordHandler
         prompt_formatter = TrainingRecordHandler
     elif prompt_format == 'chatml':
         from mlx_tuning_fork.prompt_templates.chatml import TrainingRecordHandler
         prompt_formatter = TrainingRecordHandler
 
-    lora.Dataset = Dataset
-
     with open(config_file, "r") as file:
         config = yaml.load(file, yaml_loader)
         param_dict = {k: v for k, v in config.items()}
         if "model" not in param_dict:
             raise SyntaxError('Missing required "model" parameter')
         for key, default in CONFIG_DEFAULTS.items():
             if key not in param_dict:
@@ -216,45 +185,50 @@
             param_dict["prompt"] = generate_prompt_from_loom(loom_file, loom_markers, prompt_formatter, build_prompt)
             param_dict["test"] = param_dict["train"] = False
             param_dict["ignore_chat_template"] = True
         if prompt:
             param_dict["prompt"] = prompt
             param_dict["test"] = param_dict["train"] = False
         if temperature:
-            param_dict["temperature"] = temperature
+            param_dict["temp"] = temperature
         if adapter:
-            param_dict["adapter_file"] = adapter
+            param_dict["adapter_path"] = adapter
         if num_tokens and num_tokens != -1:
-            param_dict["num_tokens"] = num_tokens
+            param_dict["max_tokens"] = num_tokens
         pprint(param_dict)
         args = SimpleNamespace(**param_dict)
 
     print("Loading pretrained model")
     tokenizer_config = {"trust_remote_code": True if args.trust_remote_code else None}
     # if args.eos_token is not None:
     #     tokenizer_config["eos_token"] = args.eos_token
     model, tokenizer = load(args.model, tokenizer_config=tokenizer_config)
     model.freeze()
     # Convert linear layers to lora layers and unfreeze in the process
     linear_to_lora_layers(model, args.lora_layers, args.lora_parameters)
 
+    print_trainable_parameters(model)
+
     training_callback = None
     if wandb_project:
         if wandb_run is None:
             raise RuntimeError("Specify the name of a Wandb run to use with --wandb-run ")
         try:
             import wandb
         except ImportError:
             raise ImportError('wandb module not available.  Install with `pip install wandb`')
         wandb.init(project=wandb_project, name=wandb_run, config=config)
-        training_callback = WandbCallback()
 
     print("Loading datasets")
     names = ("train", "valid", "test")
-    train_set, valid_set, test_set = (lora.Dataset(Path(args.data) / f"{n}.jsonl") for n in names)
+    if train_type == 'completion-only':
+        dataset = Dataset
+    else:
+        dataset = mlx_lm_dataset
+    train_set, valid_set, test_set = (dataset(Path(args.data) / f"{n}.jsonl") for n in names)
     if args.train and len(train_set) == 0:
         raise ValueError(
             "Training set not found or empty. Must provide training set for fine-tuning."
         )
     if args.train and len(valid_set) == 0:
         warnings.warn(
             "Validation set not found or empty. Should provide validation set for fine-tuning."
@@ -267,18 +241,21 @@
     epoch_num_steps = (len(train_set) + args.batch_size - 1) // args.batch_size
     if args.epochs == -1:
         num_iterations = epoch_num_steps if args.iters == -1 else args.iters
     else:
         num_iterations = epoch_num_steps * args.epochs
     num_iterations = int(num_iterations)
 
+    if wandb_project:
+        training_callback = WandbCallback(tqdm(total=num_iterations))
+
     print(
         f"{num_iterations:,} iterations at {epoch_num_steps:,} iterations per epoch on a dataset of "
         f"{len(train_set):,} records, {args.batch_size} at a time and with a validation set of "
-        f"{len(valid_set):,} records, training {args.lora_layers} layers out of {len(model.model.layers)} using qLoRa."
+        f"{len(valid_set):,} records, training {args.lora_layers} layers out of {len(model.layers)} using qLoRa."
     )
 
     scaled_steps_per_report = int(args.reporting_interval_proportion * num_iterations)
     scaled_steps_per_eval = int(num_iterations * args.validation_interval_proportion)
     scaled_val_batches = int(args.validations_per_train_item * args.validation_interval_proportion * num_iterations)
     scaled_save_every = int(args.adapter_save_interval_proportion * num_iterations)
 
@@ -292,30 +269,40 @@
 
         if "learning_schedule" in config:
             scheduler = SCHEDULE_CONFIGURATION_TYPE_TO_CLASS[
                 config["learning_schedule"]["type"]].from_configuration(args.learning_rate, config, num_iterations)
         else:
             scheduler = args.learning_rate
 
+        # Resume training the given adapters.
+        if args.resume_adapter_file is not None:
+            print(f"Loading pretrained adapters from {args.resume_adapter_file}")
+            model.load_weights(args.resume_adapter_file, strict=False)
+
+        adapter_path = Path(args.adapter_path)
+        adapter_path.mkdir(parents=True, exist_ok=True)
+        save_config(vars(args), adapter_path / "adapter_config.json")
+        adapter_file = adapter_path / "adapters.safetensors"
+
         training_args = TrainingArgs(
             batch_size=args.batch_size,
             iters=num_iterations,
             val_batches=scaled_val_batches,
             steps_per_report=scaled_steps_per_report,
             steps_per_eval=scaled_steps_per_eval,
             steps_per_save=scaled_save_every,
-            adapter_file=args.adapter_file,
-            max_seq_length=args.max_seq_length
+            adapter_file=adapter_file,
+            max_seq_length=args.max_seq_length,
+            grad_checkpoint=args.grad_checkpoint,
         )
 
         if args.train:
             print("Training")
             model.train()
             opt = optim.Adam(learning_rate=scheduler)
-            pbar = tqdm(total=num_iterations)
 
             train(
                 model,
                 tokenizer,
                 opt,
                 train_set,
                 valid_set,
@@ -323,19 +310,20 @@
                 loss=completions_only_loss if train_type == 'completion-only' else default_loss,
                 iterate_batches=completions_only_iterate_batches if train_type == 'completion-only'
                 else iterate_batches,
                 training_callback=training_callback
             )
 
         # Load the LoRA adapter weights which we assume should exist by this point
-        if not Path(args.adapter_file).is_file():
+        if not adapter_file.is_file():
             raise ValueError(
-                f"Adapter file {args.adapter_file} missing. "
+                f"Adapter file {adapter_file} missing. "
+                "Use --train to learn and save the adapters"
             )
-        model.load_weights(args.adapter_file, strict=False)
+        model.load_weights(str(adapter_file), strict=False)
         print(f"Loaded weights from {args.adapter_file}")
 
         if args.test:
             print(f"Testing ({len(test_set):,} records)")
             model.eval()
 
             test_loss = evaluate(
```

### Comparing `mlx-tuning-fork-0.3/src/mlx_tuning_fork/tuning/dynamic_learning/__init__.py` & `mlx_tuning_fork-0.3.5/src/mlx_tuning_fork/tuning/dynamic_learning/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,21 +40,22 @@
 
 
 class CosineWithWarmup:
     @classmethod
     def from_configuration(cls, learning_rate, config, total_iterations):
         param_dict = {k: v for k, v in config["learning_schedule"].items()}
         min_lr = param_dict["min_lr"]
+        min_cos_lr = param_dict["min_cos_lr"] if "min_cos_lr" in param_dict else 0.0
         max_lr = param_dict["max_lr"] if "max_lr" in param_dict else learning_rate
         cycle_length = param_dict["cycle_length"]
         cycle_length = total_iterations if cycle_length == -1 else cycle_length
         length = param_dict["length"] if "length" in param_dict else int(param_dict["warmup_proportion"] *
                                                                          total_iterations)
         warmup_schedule = mlx_schedulers.linear_schedule(min_lr, max_lr, length)
-        cosine_schedule = mlx_schedulers.cosine_decay(max_lr, cycle_length)
+        cosine_schedule = mlx_schedulers.cosine_decay(max_lr, cycle_length, min_cos_lr)
         cosine_w_warmup_schedule = mlx_schedulers.join_schedules([warmup_schedule, cosine_schedule], [length])
         return cosine_w_warmup_schedule
 
 
 class Cosine:
     @classmethod
     def from_configuration(cls, learning_rate, config, total_iterations):
```

### Comparing `mlx-tuning-fork-0.3/src/mlx_tuning_fork.egg-info/PKG-INFO` & `mlx_tuning_fork-0.3.5/src/mlx_tuning_fork.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx-tuning-fork
-Version: 0.3
+Version: 0.3.5
 Summary: Basic framework for LLM (Q)LoRA fine-tuning using mlx, mlx_lm, and OgbujiPT.
 Author-email: Chimezie Ogbuji <chimezie@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Chime Ogbuji
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,18 +46,18 @@
 Large Language Model (Q)LoRa fine-tuning with MLX.  It uses [mlx](https://github.com/ml-explore/mlx), [mlx_lm](https://github.com/ml-explore/mlx-examples/tree/main/llms/mlx_lm), 
 and [OgbujiPT](https://github.com/OoriData/OgbujiPT), and is based primarily on the excellent mlx-example libraries
 but adds very minimal architecture for systematic running of easily parameterized fine tunes, hyperparameter sweeping,
 declarative prompt construction, an equivalent of HF's [train on completions](https://huggingface.co/docs/trl/sft_trainer#train-on-completions-only), and other capabilities.  
 
 ## Installation
 
-For now, can be installed by cloning the repository and running (in the local working copy)
+Can be installed via:
 
 ```bash
-$ pip install .
+$ pip install mlx-tuning-fork
 ```
 
 Currently just has a single Mistral prompt format (-f/ --prompt-format) module, but with mlx-lm and OgbujiPT you can do something similar with other models:
 
 * Llama
 * Mixtral
 * Qwen
@@ -166,15 +166,16 @@
 the user prompt.  If two values are provided, they should be quoted and separated by spaces.  The first refers to 
 a table that provides the system prompt and the second refers to the user prompt.  Finally, if three values are provided
 they are assumed to be system prompt, context, and user prompt.
 
 If they are not specified via ``--build-prompt``, the system prompt is assumed to be specified in a table named 
 **system_prompt**, the context is from a table named **context**, and the user prompt is from a table named **question**.
 
-
+If any of the table header name of the context is of the form ``[filename.txt]`` the contents of the specified filename are used
+for the instead.
 
 If any of the text values in the corresponding tables have curly braces, the ``--loom-markers`` option can be used
 to provide values for the names specified in between the braces.  It is expected to be a string in the format: 
 ``name=[.. value ..]``.
 
 So, the following command-line:
 
@@ -235,14 +236,16 @@
 
 ```commandline
 $ python -m mlx_tuning_fork.wandb_sweep --help
 Usage: python -m mlx_tuning_fork.wandb_sweep [OPTIONS] CONFIG_FILE
 
 Options:
   --verbose / --no-verbose
-  --wandb-project TEXT      Wandb project name
-  --help                    Show this message and exit.
+  --wandb-project TEXT            Wandb project name
+  --train-type [completion-only|self-supervised]
+  -f, --prompt-format [mistral|chatml]
+  --help                          Show this message and exit.
 ```
 
 It takes a single argument which is a [Wandb sweep configuration (YAML) file](https://docs.wandb.ai/guides/sweeps/define-sweep-configuration)
  .  The `--wandb-project` options refers to a Wandb project where the sweep output is be stored.
```

### Comparing `mlx-tuning-fork-0.3/src/mlx_tuning_fork.egg-info/SOURCES.txt` & `mlx_tuning_fork-0.3.5/src/mlx_tuning_fork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlx-tuning-fork-0.3/tests/test_scheduler_config.py` & `mlx_tuning_fork-0.3.5/tests/test_scheduler_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 import yaml
 from mlx_tuning_fork.config import yaml_loader
 from mlx_tuning_fork.tuning.dynamic_learning import SCHEDULE_CONFIGURATION_TYPE_TO_CLASS
 
 
 def load_config(yaml_string, total_iterations):
     config = yaml.load(yaml_string, yaml_loader)
-    learning_rate = config["learning_rate"]
     return SCHEDULE_CONFIGURATION_TYPE_TO_CLASS[
-        config["learning_schedule"]["type"]].from_configuration(learning_rate, config, total_iterations)
+        config["learning_schedule"]["type"]].from_configuration(config.get("learning_rate"), config, total_iterations)
 
 
 class TestCosineWithWarmup:
     TEST_YAML1 = """
     learning_rate: 1e-5
     learning_schedule:
         type: cosine_w_warmup
@@ -45,8 +44,8 @@
 
     def test_basic(self):
         load_config(self.TEST_YAML1, 10000)
         load_config(self.TEST_YAML2, 10000)
         load_config(self.TEST_YAML3, 10000)
         with pytest.raises(KeyError) as excinfo:
             load_config(self.TEST_YAML4, 10000)
-        assert "cycle_length in " in str(excinfo.value)
+        assert "cycle_length" in str(excinfo.value)
```

