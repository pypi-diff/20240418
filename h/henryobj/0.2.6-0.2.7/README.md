# Comparing `tmp/henryobj-0.2.6.tar.gz` & `tmp/henryobj-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "henryobj-0.2.6.tar", last modified: Mon Apr 15 10:24:13 2024, max compression
+gzip compressed data, was "henryobj-0.2.7.tar", last modified: Thu Apr 18 07:34:23 2024, max compression
```

## Comparing `henryobj-0.2.6.tar` & `henryobj-0.2.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-15 10:24:13.974694 henryobj-0.2.6/
--rw-r--r--   0 henry      (501) staff       (20)     3115 2024-04-15 10:24:13.974515 henryobj-0.2.6/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)     2976 2024-01-24 08:03:39.000000 henryobj-0.2.6/README.md
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-15 10:24:13.973530 henryobj-0.2.6/henryobj/
--rw-r--r--   0 henry      (501) staff       (20)      224 2024-04-09 07:08:41.000000 henryobj-0.2.6/henryobj/__init__.py
--rw-r--r--   0 henry      (501) staff       (20)    22625 2024-04-11 08:30:24.000000 henryobj-0.2.6/henryobj/base.py
--rw-r--r--   0 henry      (501) staff       (20)     1543 2024-04-10 09:35:13.000000 henryobj-0.2.6/henryobj/config.py
--rw-r--r--   0 henry      (501) staff       (20)    13971 2024-04-11 08:30:55.000000 henryobj-0.2.6/henryobj/gpt.py
--rw-r--r--   0 henry      (501) staff       (20)    29910 2024-04-11 13:11:10.000000 henryobj-0.2.6/henryobj/oai.py
--rw-r--r--   0 henry      (501) staff       (20)    14269 2024-04-15 10:23:49.000000 henryobj-0.2.6/henryobj/web.py
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-15 10:24:13.974309 henryobj-0.2.6/henryobj.egg-info/
--rw-r--r--   0 henry      (501) staff       (20)     3115 2024-04-15 10:24:13.000000 henryobj-0.2.6/henryobj.egg-info/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      282 2024-04-15 10:24:13.000000 henryobj-0.2.6/henryobj.egg-info/SOURCES.txt
--rw-r--r--   0 henry      (501) staff       (20)        1 2024-04-15 10:24:13.000000 henryobj-0.2.6/henryobj.egg-info/dependency_links.txt
--rw-r--r--   0 henry      (501) staff       (20)       60 2024-04-15 10:24:13.000000 henryobj-0.2.6/henryobj.egg-info/requires.txt
--rw-r--r--   0 henry      (501) staff       (20)        9 2024-04-15 10:24:13.000000 henryobj-0.2.6/henryobj.egg-info/top_level.txt
--rw-r--r--   0 henry      (501) staff       (20)       38 2024-04-15 10:24:13.974742 henryobj-0.2.6/setup.cfg
--rw-r--r--   0 henry      (501) staff       (20)      574 2024-04-15 10:24:02.000000 henryobj-0.2.6/setup.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-18 07:34:23.893001 henryobj-0.2.7/
+-rw-r--r--   0 henry      (501) staff       (20)     3115 2024-04-18 07:34:23.892851 henryobj-0.2.7/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)     2976 2024-01-24 08:03:39.000000 henryobj-0.2.7/README.md
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-18 07:34:23.891800 henryobj-0.2.7/henryobj/
+-rw-r--r--   0 henry      (501) staff       (20)      224 2024-04-09 07:08:41.000000 henryobj-0.2.7/henryobj/__init__.py
+-rw-r--r--   0 henry      (501) staff       (20)    22625 2024-04-11 08:30:24.000000 henryobj-0.2.7/henryobj/base.py
+-rw-r--r--   0 henry      (501) staff       (20)     1563 2024-04-18 07:33:26.000000 henryobj-0.2.7/henryobj/config.py
+-rw-r--r--   0 henry      (501) staff       (20)    13971 2024-04-11 08:30:55.000000 henryobj-0.2.7/henryobj/gpt.py
+-rw-r--r--   0 henry      (501) staff       (20)    30005 2024-04-18 07:33:58.000000 henryobj-0.2.7/henryobj/oai.py
+-rw-r--r--   0 henry      (501) staff       (20)    14269 2024-04-15 10:23:49.000000 henryobj-0.2.7/henryobj/web.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-18 07:34:23.892660 henryobj-0.2.7/henryobj.egg-info/
+-rw-r--r--   0 henry      (501) staff       (20)     3115 2024-04-18 07:34:23.000000 henryobj-0.2.7/henryobj.egg-info/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      282 2024-04-18 07:34:23.000000 henryobj-0.2.7/henryobj.egg-info/SOURCES.txt
+-rw-r--r--   0 henry      (501) staff       (20)        1 2024-04-18 07:34:23.000000 henryobj-0.2.7/henryobj.egg-info/dependency_links.txt
+-rw-r--r--   0 henry      (501) staff       (20)       60 2024-04-18 07:34:23.000000 henryobj-0.2.7/henryobj.egg-info/requires.txt
+-rw-r--r--   0 henry      (501) staff       (20)        9 2024-04-18 07:34:23.000000 henryobj-0.2.7/henryobj.egg-info/top_level.txt
+-rw-r--r--   0 henry      (501) staff       (20)       38 2024-04-18 07:34:23.893063 henryobj-0.2.7/setup.cfg
+-rw-r--r--   0 henry      (501) staff       (20)      574 2024-04-18 07:34:20.000000 henryobj-0.2.7/setup.py
```

### Comparing `henryobj-0.2.6/PKG-INFO` & `henryobj-0.2.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1
-Name: henryobj
-Version: 0.2.6
-Home-page: https://github.com/HenryObj/mypip
-Description-Content-Type: text/markdown
-
 # PIP Package henryobj Overview - 24th of January
 
 This codebase is a Python package designed to facilitate web scraping, interactions with OpenAI's API, and provide a suite of utility functions. It is structured to be modular, allowing each component to function independently or in conjunction with others, promoting maintainability and scalability.
 
 ## Module Descriptions
 
 ### `web.py`
@@ -49,8 +43,8 @@
 ### `__init__.py`
 
 - **Purpose:** Serves as the package initializer, importing all necessary modules for user accessibility.
 - **Interactions:** Critical for package integrity, enabling module imports upon package usage without housing direct functionality.
 
 ## Additional Notes
 
-This ReadME was generated automatically. See gpt.py to use it for your repos.
+This ReadME was generated automatically. See gpt.py to use it for your repos.
```

### Comparing `henryobj-0.2.6/README.md` & `henryobj-0.2.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Metadata-Version: 2.1
+Name: henryobj
+Version: 0.2.7
+Home-page: https://github.com/HenryObj/mypip
+Description-Content-Type: text/markdown
+
 # PIP Package henryobj Overview - 24th of January
 
 This codebase is a Python package designed to facilitate web scraping, interactions with OpenAI's API, and provide a suite of utility functions. It is structured to be modular, allowing each component to function independently or in conjunction with others, promoting maintainability and scalability.
 
 ## Module Descriptions
 
 ### `web.py`
@@ -43,8 +49,8 @@
 ### `__init__.py`
 
 - **Purpose:** Serves as the package initializer, importing all necessary modules for user accessibility.
 - **Interactions:** Critical for package integrity, enabling module imports upon package usage without housing direct functionality.
 
 ## Additional Notes
 
-This ReadME was generated automatically. See gpt.py to use it for your repos.
+This ReadME was generated automatically. See gpt.py to use it for your repos.
```

### Comparing `henryobj-0.2.6/henryobj/base.py` & `henryobj-0.2.7/henryobj/base.py`

 * *Files identical despite different names*

### Comparing `henryobj-0.2.6/henryobj/config.py` & `henryobj-0.2.7/henryobj/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 MAX_TOKEN_OUTPUT_DEFAULT = 300
 MAX_TOKEN_OUTPUT_DEFAULT_HUGE = 3000
 
 MAX_TOKEN_WINDOW_OLD = 4096 
 MAX_TOKEN_WINDOW_GPT4_TURBO = 128000
 MAX_TOKEN_WINDOW_GPT35_TURBO = 16385
 MAX_TOKEN_WINDOW_GPT4 = 8192
+WINDOW_BUFFER = 100
 
 # ****** MODELS
 MODEL_GPT4_TURBO = r"gpt-4-1106-preview" #Max 128,000 token context window total with 4,096 output
 MODEL_GPT4_STABLE = r"gpt-4" # 8K context window and 4,096 output
 
 MODEL_CHAT_BACKUP = r"gpt-3.5-turbo-1106" # Context 16,385 tokens - Reply 4,096
 MODEL_CHAT = r"gpt-3.5-turbo-0125"
```

### Comparing `henryobj-0.2.6/henryobj/gpt.py` & `henryobj-0.2.7/henryobj/gpt.py`

 * *Files identical despite different names*

### Comparing `henryobj-0.2.6/henryobj/oai.py` & `henryobj-0.2.7/henryobj/oai.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # All that is related ot Open AI
 
 from .config import (
     ERROR_MESSAGE, OPEN_AI_ISSUE, MAX_TOKEN_OUTPUT_DEFAULT, MAX_TOKEN_OUTPUT_DEFAULT_HUGE, MAX_TOKEN_WINDOW_GPT4, 
     MAX_TOKEN_WINDOW_GPT4_TURBO, MAX_TOKEN_WINDOW_OLD, MAX_TOKEN_WINDOW_GPT35_TURBO, MODEL_GPT4_TURBO,
-    MODEL_GPT4_STABLE, MODEL_CHAT, MODEL_EMB_LARGE, MODEL_CHAT_STABLE, MODEL_CHAT_BACKUP
+    MODEL_GPT4_STABLE, MODEL_CHAT, MODEL_EMB_LARGE, MODEL_CHAT_STABLE, MODEL_CHAT_BACKUP, WINDOW_BUFFER
 )
 from .base import log_warning, log_issue, split_into_sentences, custom_round, check_co
 
 
 from typing import Optional
 
 import tiktoken
@@ -502,19 +502,19 @@
         verbose (bool, optional): Will print information in the console.
         json_on (bool, optional): Whether to force the output in JSON format // UNUSED FOR NOW
 
     Returns:
         str: The model's reply to the question.
     """
     max_token_window = {
-        MODEL_GPT4_TURBO: MAX_TOKEN_WINDOW_GPT4_TURBO,
-        MODEL_GPT4_STABLE: MAX_TOKEN_WINDOW_GPT4,
-        MODEL_CHAT: MAX_TOKEN_WINDOW_GPT35_TURBO,
-        MODEL_CHAT_STABLE: MAX_TOKEN_WINDOW_GPT35_TURBO,
-    }.get(model, MAX_TOKEN_WINDOW_OLD)
+        MODEL_GPT4_TURBO: MAX_TOKEN_WINDOW_GPT4_TURBO - WINDOW_BUFFER,
+        MODEL_GPT4_STABLE: MAX_TOKEN_WINDOW_GPT4 - WINDOW_BUFFER,
+        MODEL_CHAT: MAX_TOKEN_WINDOW_GPT35_TURBO - WINDOW_BUFFER,
+        MODEL_CHAT_STABLE: MAX_TOKEN_WINDOW_GPT35_TURBO - WINDOW_BUFFER,
+    }.get(model, MAX_TOKEN_WINDOW_OLD - WINDOW_BUFFER)
     initial_token_usage = calculate_token(role) + calculate_token(question)
     if initial_token_usage > max_token_window:
         print("Your input is too large for the query regardless of the max_tokens for the reply.")
         return ""
     elif initial_token_usage + max_tokens > max_token_window:
         max_tokens_adjusted = max_token_window - initial_token_usage
         print(f"Your input + the requested tokens for the answer exceed the maximum amount of {max_token_window}.\n Please adjust the max_tokens to a MAXIMUM of {max_tokens_adjusted}")
```

### Comparing `henryobj-0.2.6/henryobj/web.py` & `henryobj-0.2.7/henryobj/web.py`

 * *Files identical despite different names*

### Comparing `henryobj-0.2.6/henryobj.egg-info/PKG-INFO` & `henryobj-0.2.7/henryobj.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henryobj
-Version: 0.2.6
+Version: 0.2.7
 Home-page: https://github.com/HenryObj/mypip
 Description-Content-Type: text/markdown
 
 # PIP Package henryobj Overview - 24th of January
 
 This codebase is a Python package designed to facilitate web scraping, interactions with OpenAI's API, and provide a suite of utility functions. It is structured to be modular, allowing each component to function independently or in conjunction with others, promoting maintainability and scalability.
```

### Comparing `henryobj-0.2.6/setup.py` & `henryobj-0.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="henryobj",
-    version="0.2.6", # need to increment this everytime otherwise Pypi will not accept the new version
+    version="0.2.7", # need to increment this everytime otherwise Pypi will not accept the new version
      url='https://github.com/HenryObj/mypip',
     packages=find_packages(),
     install_requires=[
         "openai>=1.9.0",
         "tiktoken>=0.5.2",
         "requests>=2.31.0",
         "bs4",
```

