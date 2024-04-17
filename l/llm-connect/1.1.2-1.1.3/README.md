# Comparing `tmp/llm_connect-1.1.2.tar.gz` & `tmp/llm_connect-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_connect-1.1.2.tar", last modified: Fri Jan 19 15:35:58 2024, max compression
+gzip compressed data, was "llm_connect-1.1.3.tar", last modified: Sat Jan 20 00:27:36 2024, max compression
```

## Comparing `llm_connect-1.1.2.tar` & `llm_connect-1.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 ahtshamzafar   (501) staff       (20)        0 2024-01-19 15:35:58.056577 llm_connect-1.1.2/
--rw-r--r--   0 ahtshamzafar   (501) staff       (20)     4254 2024-01-19 15:35:58.056386 llm_connect-1.1.2/PKG-INFO
--rw-r--r--   0 ahtshamzafar   (501) staff       (20)     3908 2024-01-18 16:15:11.000000 llm_connect-1.1.2/README.md
-drwxr-xr-x   0 ahtshamzafar   (501) staff       (20)        0 2024-01-19 15:35:58.056065 llm_connect-1.1.2/llm_connect.egg-info/
--rw-r--r--   0 ahtshamzafar   (501) staff       (20)     4254 2024-01-19 15:35:58.000000 llm_connect-1.1.2/llm_connect.egg-info/PKG-INFO
--rw-r--r--   0 ahtshamzafar   (501) staff       (20)      616 2024-01-19 15:35:58.000000 llm_connect-1.1.2/llm_connect.egg-info/SOURCES.txt
--rw-r--r--   0 ahtshamzafar   (501) staff       (20)        1 2024-01-19 15:35:58.000000 llm_connect-1.1.2/llm_connect.egg-info/dependency_links.txt
--rw-r--r--   0 ahtshamzafar   (501) staff       (20)       43 2024-01-19 15:35:58.000000 llm_connect-1.1.2/llm_connect.egg-info/entry_points.txt
--rw-r--r--   0 ahtshamzafar   (501) staff       (20)       91 2024-01-19 15:35:58.000000 llm_connect-1.1.2/llm_connect.egg-info/requires.txt
--rw-r--r--   0 ahtshamzafar   (501) staff       (20)       16 2024-01-19 15:35:58.000000 llm_connect-1.1.2/llm_connect.egg-info/top_level.txt
-drwxr-xr-x   0 ahtshamzafar   (501) staff       (20)        0 2024-01-19 15:35:58.053721 llm_connect-1.1.2/llm_connect_api/
--rw-r--r--   0 ahtshamzafar   (501) staff       (20)       18 2024-01-15 18:28:28.000000 llm_connect-1.1.2/llm_connect_api/__init__.py
--rw-r--r--   0 ahtshamzafar   (501) staff       (20)     3434 2024-01-17 16:50:48.000000 llm_connect-1.1.2/llm_connect_api/cli.py
-drwxr-xr-x   0 ahtshamzafar   (501) staff       (20)        0 2024-01-19 15:35:58.055767 llm_connect-1.1.2/llm_connect_api/commands/
--rw-r--r--   0 ahtshamzafar   (501) staff       (20)        0 2023-11-30 18:49:22.000000 llm_connect-1.1.2/llm_connect_api/commands/__init__.py
--rw-r--r--   0 ahtshamzafar   (501) staff       (20)     4014 2024-01-18 16:03:43.000000 llm_connect-1.1.2/llm_connect_api/commands/add_model.py
--rw-r--r--   0 ahtshamzafar   (501) staff       (20)     8549 2024-01-19 15:30:30.000000 llm_connect-1.1.2/llm_connect_api/commands/execute.py
--rw-r--r--   0 ahtshamzafar   (501) staff       (20)      448 2024-01-02 15:09:51.000000 llm_connect-1.1.2/llm_connect_api/commands/fetch_result.py
--rw-r--r--   0 ahtshamzafar   (501) staff       (20)     3955 2024-01-18 15:59:49.000000 llm_connect-1.1.2/llm_connect_api/commands/hardware.py
--rw-r--r--   0 ahtshamzafar   (501) staff       (20)     1605 2024-01-18 15:56:05.000000 llm_connect-1.1.2/llm_connect_api/commands/list_models.py
--rw-r--r--   0 ahtshamzafar   (501) staff       (20)      760 2024-01-18 15:59:49.000000 llm_connect-1.1.2/llm_connect_api/commands/list_tasks.py
--rw-r--r--   0 ahtshamzafar   (501) staff       (20)     2461 2024-01-18 15:56:05.000000 llm_connect-1.1.2/llm_connect_api/commands/remove_model.py
--rw-r--r--   0 ahtshamzafar   (501) staff       (20)      122 2024-01-02 15:09:51.000000 llm_connect-1.1.2/llm_connect_api/config.py
--rw-r--r--   0 ahtshamzafar   (501) staff       (20)       38 2024-01-19 15:35:58.056618 llm_connect-1.1.2/setup.cfg
--rw-r--r--   0 ahtshamzafar   (501) staff       (20)      625 2024-01-19 15:35:05.000000 llm_connect-1.1.2/setup.py
+drwxr-xr-x   0 ahtshamzafar   (501) staff       (20)        0 2024-01-20 00:27:36.207055 llm_connect-1.1.3/
+-rw-r--r--   0 ahtshamzafar   (501) staff       (20)     4089 2024-01-20 00:27:36.206869 llm_connect-1.1.3/PKG-INFO
+-rw-r--r--   0 ahtshamzafar   (501) staff       (20)     3743 2024-01-20 00:26:51.000000 llm_connect-1.1.3/README.md
+drwxr-xr-x   0 ahtshamzafar   (501) staff       (20)        0 2024-01-20 00:27:36.206673 llm_connect-1.1.3/llm_connect.egg-info/
+-rw-r--r--   0 ahtshamzafar   (501) staff       (20)     4089 2024-01-20 00:27:36.000000 llm_connect-1.1.3/llm_connect.egg-info/PKG-INFO
+-rw-r--r--   0 ahtshamzafar   (501) staff       (20)      616 2024-01-20 00:27:36.000000 llm_connect-1.1.3/llm_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 ahtshamzafar   (501) staff       (20)        1 2024-01-20 00:27:36.000000 llm_connect-1.1.3/llm_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 ahtshamzafar   (501) staff       (20)       43 2024-01-20 00:27:36.000000 llm_connect-1.1.3/llm_connect.egg-info/entry_points.txt
+-rw-r--r--   0 ahtshamzafar   (501) staff       (20)       91 2024-01-20 00:27:36.000000 llm_connect-1.1.3/llm_connect.egg-info/requires.txt
+-rw-r--r--   0 ahtshamzafar   (501) staff       (20)       16 2024-01-20 00:27:36.000000 llm_connect-1.1.3/llm_connect.egg-info/top_level.txt
+drwxr-xr-x   0 ahtshamzafar   (501) staff       (20)        0 2024-01-20 00:27:36.204920 llm_connect-1.1.3/llm_connect_api/
+-rw-r--r--   0 ahtshamzafar   (501) staff       (20)       18 2024-01-15 18:28:28.000000 llm_connect-1.1.3/llm_connect_api/__init__.py
+-rw-r--r--   0 ahtshamzafar   (501) staff       (20)     3434 2024-01-17 16:50:48.000000 llm_connect-1.1.3/llm_connect_api/cli.py
+drwxr-xr-x   0 ahtshamzafar   (501) staff       (20)        0 2024-01-20 00:27:36.206387 llm_connect-1.1.3/llm_connect_api/commands/
+-rw-r--r--   0 ahtshamzafar   (501) staff       (20)        0 2023-11-30 18:49:22.000000 llm_connect-1.1.3/llm_connect_api/commands/__init__.py
+-rw-r--r--   0 ahtshamzafar   (501) staff       (20)     4014 2024-01-18 16:03:43.000000 llm_connect-1.1.3/llm_connect_api/commands/add_model.py
+-rw-r--r--   0 ahtshamzafar   (501) staff       (20)     8546 2024-01-19 20:34:15.000000 llm_connect-1.1.3/llm_connect_api/commands/execute.py
+-rw-r--r--   0 ahtshamzafar   (501) staff       (20)      448 2024-01-02 15:09:51.000000 llm_connect-1.1.3/llm_connect_api/commands/fetch_result.py
+-rw-r--r--   0 ahtshamzafar   (501) staff       (20)     3955 2024-01-18 15:59:49.000000 llm_connect-1.1.3/llm_connect_api/commands/hardware.py
+-rw-r--r--   0 ahtshamzafar   (501) staff       (20)     1605 2024-01-18 15:56:05.000000 llm_connect-1.1.3/llm_connect_api/commands/list_models.py
+-rw-r--r--   0 ahtshamzafar   (501) staff       (20)      760 2024-01-18 15:59:49.000000 llm_connect-1.1.3/llm_connect_api/commands/list_tasks.py
+-rw-r--r--   0 ahtshamzafar   (501) staff       (20)     2461 2024-01-18 15:56:05.000000 llm_connect-1.1.3/llm_connect_api/commands/remove_model.py
+-rw-r--r--   0 ahtshamzafar   (501) staff       (20)      122 2024-01-02 15:09:51.000000 llm_connect-1.1.3/llm_connect_api/config.py
+-rw-r--r--   0 ahtshamzafar   (501) staff       (20)       38 2024-01-20 00:27:36.207096 llm_connect-1.1.3/setup.cfg
+-rw-r--r--   0 ahtshamzafar   (501) staff       (20)      625 2024-01-20 00:27:22.000000 llm_connect-1.1.3/setup.py
```

### Comparing `llm_connect-1.1.2/PKG-INFO` & `llm_connect-1.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 Metadata-Version: 2.1
 Name: llm_connect
-Version: 1.1.2
+Version: 1.1.3
 Summary: LLM Connect API
 Author: CeADAR Connect Group
 Description-Content-Type: text/markdown
 Requires-Dist: click==8.1.7
 Requires-Dist: setuptools~=68.2.0
 Requires-Dist: transformers
 Requires-Dist: torch~=2.1.0
 Requires-Dist: accelerate
 Requires-Dist: bitsandbytes
 Requires-Dist: colorama
 
 # LLMConnect API
 
 ## Table of Contents
-- [Introduction](#introduction)
+- [Introduction](#Introduction)
 - [Features](#features)
 - [Installation](#installation)
   - [Prerequisites](#prerequisites)
-  - [Installation Steps](#installation-steps)
 - [Commands](#commands)
-- [Command examples](#Commandexamples)
-- [Author](#Author)
-- [License](#license)
+- [Predefined tasks](#predefined-tasks)
+  - [Command]()
+  - [Output]()
+- [Command examples]()
+- [Author]()
+- [License]()
 
 ## Introduction
-LLMConnect API is a developer-friendly Python-based CLI utility designed to manage and execute Large Language Models (LLMs) on local servers or clusters. It enables users to run a variety of standard and custom tasks with popular models such as Llama-2, Mistral, Falcon, etc., and also supports the integration of new LLMs.
+LLMConnect API is a developer-friendly Python-based CLI utility designed to manage and evaluate Language Models including LLMs and SLMs on local servers or clusters. It enables users to run a variety of standard and custom tasks with popular models such as Llama-2, Mistral, Falcon, etc., and also supports the integration of new LLMs.
 
 
 ## Features
 - Task Versatility: Execute predefined tasks like NER, Sentiment Analysis, Summarisation, or craft your own.
-- LLM Selection: Choose from an array of predefined models or add your custom LLMs.
-- Configurable Parameters: Adjust model settings like token limits and temperature for optimal performance.
+- Model Selection: Choose and add your custom LLMs and SLMs from HuggingFace.
 - Adaptable Environments: Operate seamlessly on local servers and extend to local network clusters.
 - Hardware Compatibility: Ensure efficient LLM functioning with GPU compatibility checks and memory monitoring.
 
 CLI Interface:
 - Navigate tasks, models, and hardware diagnostics with simple, intuitive commands.
-:female-technologist: Development & Security:
-- Developed in Python 3.x, emphasising seamless LLM integration, comprehensive testing (via pytest), and detailed documentation.
+
+Development & Security:
+- Developed in Python 3.x, emphasising seamless LLM integration, and detailed documentation.
 - Features enhanced input validation for secure, reliable operations.
 
 Deployment:
 - Eager to experience the power of Large Language Models through a Python-based Command Line Interface? LLMConnect API is your gateway to harnessing this technology on your local systems!
 
 ## Installation
```

### Comparing `llm_connect-1.1.2/README.md` & `llm_connect-1.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 # LLMConnect API
 
 ## Table of Contents
-- [Introduction](#introduction)
+- [Introduction](#Introduction)
 - [Features](#features)
 - [Installation](#installation)
   - [Prerequisites](#prerequisites)
-  - [Installation Steps](#installation-steps)
 - [Commands](#commands)
-- [Command examples](#Commandexamples)
-- [Author](#Author)
-- [License](#license)
+- [Predefined tasks](#predefined-tasks)
+  - [Command]()
+  - [Output]()
+- [Command examples]()
+- [Author]()
+- [License]()
 
 ## Introduction
-LLMConnect API is a developer-friendly Python-based CLI utility designed to manage and execute Large Language Models (LLMs) on local servers or clusters. It enables users to run a variety of standard and custom tasks with popular models such as Llama-2, Mistral, Falcon, etc., and also supports the integration of new LLMs.
+LLMConnect API is a developer-friendly Python-based CLI utility designed to manage and evaluate Language Models including LLMs and SLMs on local servers or clusters. It enables users to run a variety of standard and custom tasks with popular models such as Llama-2, Mistral, Falcon, etc., and also supports the integration of new LLMs.
 
 
 ## Features
 - Task Versatility: Execute predefined tasks like NER, Sentiment Analysis, Summarisation, or craft your own.
-- LLM Selection: Choose from an array of predefined models or add your custom LLMs.
-- Configurable Parameters: Adjust model settings like token limits and temperature for optimal performance.
+- Model Selection: Choose and add your custom LLMs and SLMs from HuggingFace.
 - Adaptable Environments: Operate seamlessly on local servers and extend to local network clusters.
 - Hardware Compatibility: Ensure efficient LLM functioning with GPU compatibility checks and memory monitoring.
 
 CLI Interface:
 - Navigate tasks, models, and hardware diagnostics with simple, intuitive commands.
-:female-technologist: Development & Security:
-- Developed in Python 3.x, emphasising seamless LLM integration, comprehensive testing (via pytest), and detailed documentation.
+
+Development & Security:
+- Developed in Python 3.x, emphasising seamless LLM integration, and detailed documentation.
 - Features enhanced input validation for secure, reliable operations.
 
 Deployment:
 - Eager to experience the power of Large Language Models through a Python-based Command Line Interface? LLMConnect API is your gateway to harnessing this technology on your local systems!
 
 ## Installation
```

### Comparing `llm_connect-1.1.2/llm_connect.egg-info/PKG-INFO` & `llm_connect-1.1.3/llm_connect.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 Metadata-Version: 2.1
 Name: llm_connect
-Version: 1.1.2
+Version: 1.1.3
 Summary: LLM Connect API
 Author: CeADAR Connect Group
 Description-Content-Type: text/markdown
 Requires-Dist: click==8.1.7
 Requires-Dist: setuptools~=68.2.0
 Requires-Dist: transformers
 Requires-Dist: torch~=2.1.0
 Requires-Dist: accelerate
 Requires-Dist: bitsandbytes
 Requires-Dist: colorama
 
 # LLMConnect API
 
 ## Table of Contents
-- [Introduction](#introduction)
+- [Introduction](#Introduction)
 - [Features](#features)
 - [Installation](#installation)
   - [Prerequisites](#prerequisites)
-  - [Installation Steps](#installation-steps)
 - [Commands](#commands)
-- [Command examples](#Commandexamples)
-- [Author](#Author)
-- [License](#license)
+- [Predefined tasks](#predefined-tasks)
+  - [Command]()
+  - [Output]()
+- [Command examples]()
+- [Author]()
+- [License]()
 
 ## Introduction
-LLMConnect API is a developer-friendly Python-based CLI utility designed to manage and execute Large Language Models (LLMs) on local servers or clusters. It enables users to run a variety of standard and custom tasks with popular models such as Llama-2, Mistral, Falcon, etc., and also supports the integration of new LLMs.
+LLMConnect API is a developer-friendly Python-based CLI utility designed to manage and evaluate Language Models including LLMs and SLMs on local servers or clusters. It enables users to run a variety of standard and custom tasks with popular models such as Llama-2, Mistral, Falcon, etc., and also supports the integration of new LLMs.
 
 
 ## Features
 - Task Versatility: Execute predefined tasks like NER, Sentiment Analysis, Summarisation, or craft your own.
-- LLM Selection: Choose from an array of predefined models or add your custom LLMs.
-- Configurable Parameters: Adjust model settings like token limits and temperature for optimal performance.
+- Model Selection: Choose and add your custom LLMs and SLMs from HuggingFace.
 - Adaptable Environments: Operate seamlessly on local servers and extend to local network clusters.
 - Hardware Compatibility: Ensure efficient LLM functioning with GPU compatibility checks and memory monitoring.
 
 CLI Interface:
 - Navigate tasks, models, and hardware diagnostics with simple, intuitive commands.
-:female-technologist: Development & Security:
-- Developed in Python 3.x, emphasising seamless LLM integration, comprehensive testing (via pytest), and detailed documentation.
+
+Development & Security:
+- Developed in Python 3.x, emphasising seamless LLM integration, and detailed documentation.
 - Features enhanced input validation for secure, reliable operations.
 
 Deployment:
 - Eager to experience the power of Large Language Models through a Python-based Command Line Interface? LLMConnect API is your gateway to harnessing this technology on your local systems!
 
 ## Installation
```

### Comparing `llm_connect-1.1.2/llm_connect.egg-info/SOURCES.txt` & `llm_connect-1.1.3/llm_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llm_connect-1.1.2/llm_connect_api/cli.py` & `llm_connect-1.1.3/llm_connect_api/cli.py`

 * *Files identical despite different names*

### Comparing `llm_connect-1.1.2/llm_connect_api/commands/add_model.py` & `llm_connect-1.1.3/llm_connect_api/commands/add_model.py`

 * *Files identical despite different names*

### Comparing `llm_connect-1.1.2/llm_connect_api/commands/execute.py` & `llm_connect-1.1.3/llm_connect_api/commands/execute.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                 sentiment_text = input_text if input_text is not None else input(
                     f"    {magenta}Enter text to analyse sentiment{reset}\n")
                 prompt = f"Analyze the sentiment of the following text: {sentiment_text}."
 
             elif task.lower() == 'detectbias':
                 bias_text = input_text if input_text is not None else input(
                     f"    {magenta}Enter text to detect bias{reset}\n")
-                prompt = f"Analyze the following article for any biases: {bias_text}."
+                prompt = f"Analyze the following text for any biases: {bias_text}."
 
             def generate_text():
                 time = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
 
                 pipe = pipeline(task="text-generation", model=model, tokenizer=tokenizer, max_length=2800)
                 result = pipe(prompt, pad_token_id=pipe.tokenizer.eos_token_id)
                 generated_text = result[0]['generated_text'].replace(prompt, "").strip()
```

### Comparing `llm_connect-1.1.2/llm_connect_api/commands/hardware.py` & `llm_connect-1.1.3/llm_connect_api/commands/hardware.py`

 * *Files identical despite different names*

### Comparing `llm_connect-1.1.2/llm_connect_api/commands/list_models.py` & `llm_connect-1.1.3/llm_connect_api/commands/list_models.py`

 * *Files identical despite different names*

### Comparing `llm_connect-1.1.2/llm_connect_api/commands/list_tasks.py` & `llm_connect-1.1.3/llm_connect_api/commands/list_tasks.py`

 * *Files identical despite different names*

### Comparing `llm_connect-1.1.2/llm_connect_api/commands/remove_model.py` & `llm_connect-1.1.3/llm_connect_api/commands/remove_model.py`

 * *Files identical despite different names*

### Comparing `llm_connect-1.1.2/setup.py` & `llm_connect-1.1.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text(encoding="utf-8")
 
 setup(
     name='llm_connect',
-    version='1.1.2',
+    version='1.1.3',
     packages=find_packages(),
     install_requires=['click==8.1.7', 'setuptools~=68.2.0', 'transformers','torch~=2.1.0','accelerate', 'bitsandbytes','colorama'],
     description="LLM Connect API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="CeADAR Connect Group",
     entry_points={
```

