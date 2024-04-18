# Comparing `tmp/surveyeval-0.1.5.tar.gz` & `tmp/surveyeval-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surveyeval-0.1.5.tar", last modified: Wed Apr 17 18:39:30 2024, max compression
+gzip compressed data, was "surveyeval-0.1.6.tar", last modified: Thu Apr 18 15:46:35 2024, max compression
```

## Comparing `surveyeval-0.1.5.tar` & `surveyeval-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-17 18:39:30.946281 surveyeval-0.1.5/
--rw-r--r--   0 crobert    (501) staff       (20)    11357 2023-11-29 20:42:10.000000 surveyeval-0.1.5/LICENSE
--rw-r--r--   0 crobert    (501) staff       (20)    11239 2024-04-17 18:39:30.946018 surveyeval-0.1.5/PKG-INFO
--rw-r--r--   0 crobert    (501) staff       (20)    10689 2024-04-16 21:14:57.000000 surveyeval-0.1.5/README.rst
--rw-r--r--   0 crobert    (501) staff       (20)       38 2024-04-17 18:39:30.946342 surveyeval-0.1.5/setup.cfg
--rw-r--r--   0 crobert    (501) staff       (20)     1349 2024-04-17 18:39:29.000000 surveyeval-0.1.5/setup.py
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-17 18:39:30.940681 surveyeval-0.1.5/src/
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-17 18:39:30.943627 surveyeval-0.1.5/src/surveyeval/
--rw-r--r--   0 crobert    (501) staff       (20)     1058 2024-04-17 18:39:29.000000 surveyeval-0.1.5/src/surveyeval/__init__.py
--rw-r--r--   0 crobert    (501) staff       (20)    49441 2024-04-14 15:33:38.000000 surveyeval-0.1.5/src/surveyeval/core_evaluation_lenses.py
--rw-r--r--   0 crobert    (501) staff       (20)    33231 2024-04-14 16:03:22.000000 surveyeval-0.1.5/src/surveyeval/evaluation_engine.py
--rw-r--r--   0 crobert    (501) staff       (20)    56480 2024-04-14 15:27:21.000000 surveyeval-0.1.5/src/surveyeval/survey_parser.py
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-17 18:39:30.945609 surveyeval-0.1.5/src/surveyeval.egg-info/
--rw-r--r--   0 crobert    (501) staff       (20)    11239 2024-04-17 18:39:30.000000 surveyeval-0.1.5/src/surveyeval.egg-info/PKG-INFO
--rw-r--r--   0 crobert    (501) staff       (20)      352 2024-04-17 18:39:30.000000 surveyeval-0.1.5/src/surveyeval.egg-info/SOURCES.txt
--rw-r--r--   0 crobert    (501) staff       (20)        1 2024-04-17 18:39:30.000000 surveyeval-0.1.5/src/surveyeval.egg-info/dependency_links.txt
--rw-r--r--   0 crobert    (501) staff       (20)      118 2024-04-17 18:39:30.000000 surveyeval-0.1.5/src/surveyeval.egg-info/requires.txt
--rw-r--r--   0 crobert    (501) staff       (20)       11 2024-04-17 18:39:30.000000 surveyeval-0.1.5/src/surveyeval.egg-info/top_level.txt
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-18 15:46:35.341433 surveyeval-0.1.6/
+-rw-r--r--   0 crobert    (501) staff       (20)    11357 2023-11-29 20:42:10.000000 surveyeval-0.1.6/LICENSE
+-rw-r--r--   0 crobert    (501) staff       (20)    11239 2024-04-18 15:46:35.341079 surveyeval-0.1.6/PKG-INFO
+-rw-r--r--   0 crobert    (501) staff       (20)    10689 2024-04-16 21:14:57.000000 surveyeval-0.1.6/README.rst
+-rw-r--r--   0 crobert    (501) staff       (20)       38 2024-04-18 15:46:35.341496 surveyeval-0.1.6/setup.cfg
+-rw-r--r--   0 crobert    (501) staff       (20)     1349 2024-04-18 15:46:33.000000 surveyeval-0.1.6/setup.py
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-18 15:46:35.336487 surveyeval-0.1.6/src/
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-18 15:46:35.338781 surveyeval-0.1.6/src/surveyeval/
+-rw-r--r--   0 crobert    (501) staff       (20)     1058 2024-04-17 18:39:29.000000 surveyeval-0.1.6/src/surveyeval/__init__.py
+-rw-r--r--   0 crobert    (501) staff       (20)    49929 2024-04-18 15:46:33.000000 surveyeval-0.1.6/src/surveyeval/core_evaluation_lenses.py
+-rw-r--r--   0 crobert    (501) staff       (20)    35091 2024-04-18 15:46:33.000000 surveyeval-0.1.6/src/surveyeval/evaluation_engine.py
+-rw-r--r--   0 crobert    (501) staff       (20)    56480 2024-04-14 15:27:21.000000 surveyeval-0.1.6/src/surveyeval/survey_parser.py
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-18 15:46:35.340573 surveyeval-0.1.6/src/surveyeval.egg-info/
+-rw-r--r--   0 crobert    (501) staff       (20)    11239 2024-04-18 15:46:35.000000 surveyeval-0.1.6/src/surveyeval.egg-info/PKG-INFO
+-rw-r--r--   0 crobert    (501) staff       (20)      352 2024-04-18 15:46:35.000000 surveyeval-0.1.6/src/surveyeval.egg-info/SOURCES.txt
+-rw-r--r--   0 crobert    (501) staff       (20)        1 2024-04-18 15:46:35.000000 surveyeval-0.1.6/src/surveyeval.egg-info/dependency_links.txt
+-rw-r--r--   0 crobert    (501) staff       (20)      118 2024-04-18 15:46:35.000000 surveyeval-0.1.6/src/surveyeval.egg-info/requires.txt
+-rw-r--r--   0 crobert    (501) staff       (20)       11 2024-04-18 15:46:35.000000 surveyeval-0.1.6/src/surveyeval.egg-info/top_level.txt
```

### Comparing `surveyeval-0.1.5/LICENSE` & `surveyeval-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.5/PKG-INFO` & `surveyeval-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surveyeval
-Version: 0.1.5
+Version: 0.1.6
 Summary: A toolkit for survey evaluation
 Home-page: https://github.com/higherbar-ai/survey-eval
 Author: Christopher Robert
 Author-email: crobert@higherbar.ai
 License: Apache 2.0
 Project-URL: Documentation, https://surveyeval.readthedocs.io/
 Requires-Python: >=3.10
```

### Comparing `surveyeval-0.1.5/README.rst` & `surveyeval-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.5/setup.py` & `surveyeval-0.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from setuptools import setup
 
 with open('README.rst') as file:
     readme = file.read()
 
 setup(
     name='surveyeval',
-    version='0.1.5',
+    version='0.1.6',
     packages=['surveyeval'],
     python_requires='>=3.10',
     install_requires=[
         'tiktoken~=0.5.2',
         'openai~=1.10.0',
         'langchain~=0.1.15',
         'langchain-openai~=0.0.5',
```

### Comparing `surveyeval-0.1.5/src/surveyeval/__init__.py` & `surveyeval-0.1.6/src/surveyeval/__init__.py`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.5/src/surveyeval/core_evaluation_lenses.py` & `surveyeval-0.1.6/src/surveyeval/core_evaluation_lenses.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
         # call super constructor
         super().__init__(lens_system_prompt_template, lens_question_template, lens_followups, evaluation_engine)
 
     @overrides
     def evaluate(self, chat_history: list = None, survey_context: str = "", survey_locations: str = "",
                  survey_excerpt: str = "", survey_question: str = "", **kwargs) \
-            -> list:
+            -> dict:
         """
         Override default evaluate method.
 
         :param chat_history: Chat history to use for the evaluation chain (or None for none).
         :type chat_history: list
         :param survey_context: Information about the survey context.
         :type survey_context: str
@@ -134,28 +134,29 @@
         :type survey_locations: str
         :param survey_excerpt: Excerpt from the survey instrument (for context).
         :type survey_excerpt: str
         :param survey_question: Specific question to focus on.
         :type survey_question: str
         :param kwargs: Keyword arguments to use for formatting the task system prompt and question.
         :type kwargs: Any
-        :return: A list with, first, the evaluation result (a dict), and then a list with the full history of the
-            evaluation chain (each of which is a list with two strings, a prompt and a response).
-        :rtype: list
+        :return: A dict with result ("success" or "error"), error (if result is "error"), response (a dict),
+            and history (a list with the full history of the evaluation chain, each item of which is a list with two
+            strings, a prompt and a response).
+        :rtype: dict
         """
 
         return super().evaluate(chat_history=chat_history, survey_context=survey_context,
                                 survey_locations=survey_locations,
                                 survey_excerpt=EvaluationEngine.clean_whitespace(survey_excerpt),
                                 survey_question=EvaluationEngine.clean_whitespace(survey_question), **kwargs)
 
     @overrides
     async def a_evaluate(self, chat_history: list = None, survey_context: str = "", survey_locations: str = "",
                          survey_excerpt: str = "", survey_question: str = "", **kwargs) \
-            -> list:
+            -> dict:
         """
         Override default a_evaluate method.
 
         :param chat_history: Chat history to use for the evaluation chain (or None for none).
         :type chat_history: list
         :param survey_context: Information about the survey context.
         :type survey_context: str
@@ -163,17 +164,18 @@
         :type survey_locations: str
         :param survey_excerpt: Excerpt from the survey instrument to evaluate.
         :type survey_excerpt: str
         :param survey_question: Specific question to focus on.
         :type survey_question: str
         :param kwargs: Keyword arguments to use for formatting the task system prompt and question.
         :type kwargs: Any
-        :return: A list with, first, the evaluation result (a dict), and then a list with the full history of the
-            evaluation chain (each of which is a list with two strings, a prompt and a response).
-        :rtype: list
+        :return: A dict with result ("success" or "error"), error (if result is "error"), response (a dict),
+            and history (a list with the full history of the evaluation chain, each item of which is a list with two
+            strings, a prompt and a response).
+        :rtype: dict
         """
 
         return await super().a_evaluate(chat_history=chat_history, survey_context=survey_context,
                                         survey_locations=survey_locations,
                                         survey_excerpt=EvaluationEngine.clean_whitespace(survey_excerpt),
                                         survey_question=EvaluationEngine.clean_whitespace(survey_question),
                                         **kwargs)
@@ -371,56 +373,58 @@
         ]
 
         # call super constructor
         super().__init__(lens_system_prompt_template, lens_question_template, lens_followups, evaluation_engine)
 
     @overrides
     def evaluate(self, chat_history: list = None, survey_context: str = "", survey_locations: str = "",
-                 survey_excerpt: str = "", **kwargs) -> list:
+                 survey_excerpt: str = "", **kwargs) -> dict:
         """
         Override default evaluate method.
 
         :param chat_history: Chat history to use for the evaluation chain (or None for none).
         :type chat_history: list
         :param survey_context: Information about the survey context.
         :type survey_context: str
         :param survey_locations: Information about the survey location(s).
         :type survey_locations: str
         :param survey_excerpt: Excerpt from the survey instrument to evaluate.
         :type survey_excerpt: str
         :param kwargs: Keyword arguments to use for formatting the task system prompt and question.
         :type kwargs: Any
-        :return: A list with, first, the evaluation result (a dict), and then a list with the full history of the
-            evaluation chain (each of which is a list with two strings, a prompt and a response).
-        :rtype: list
+        :return: A dict with result ("success" or "error"), error (if result is "error"), response (a dict),
+            and history (a list with the full history of the evaluation chain, each item of which is a list with two
+            strings, a prompt and a response).
+        :rtype: dict
         """
 
         return super().evaluate(chat_history=chat_history, survey_context=survey_context,
                                 survey_locations=survey_locations,
                                 survey_excerpt=EvaluationEngine.clean_whitespace(survey_excerpt), **kwargs)
 
     @overrides
     async def a_evaluate(self, chat_history: list = None, survey_context: str = "", survey_locations: str = "",
-                         survey_excerpt: str = "", **kwargs) -> list:
+                         survey_excerpt: str = "", **kwargs) -> dict:
         """
         Override default a_evaluate method.
 
         :param chat_history: Chat history to use for the evaluation chain (or None for none).
         :type chat_history: list
         :param survey_context: Information about the survey context.
         :type survey_context: str
         :param survey_locations: Information about the survey location(s).
         :type survey_locations: str
         :param survey_excerpt: Excerpt from the survey instrument to evaluate.
         :type survey_excerpt: str
         :param kwargs: Keyword arguments to use for formatting the task system prompt and question.
         :type kwargs: Any
-        :return: A list with, first, the evaluation result (a dict), and then a list with the full history of the
-            evaluation chain (each of which is a list with two strings, a prompt and a response).
-        :rtype: list
+        :return: A dict with result ("success" or "error"), error (if result is "error"), response (a dict),
+            and history (a list with the full history of the evaluation chain, each item of which is a list with two
+            strings, a prompt and a response).
+        :rtype: dict
         """
 
         return await super().a_evaluate(chat_history=chat_history, survey_context=survey_context,
                                         survey_locations=survey_locations,
                                         survey_excerpt=EvaluationEngine.clean_whitespace(survey_excerpt), **kwargs)
 
     def format_result(self, result: dict | None = None) -> str:
@@ -590,56 +594,58 @@
         ]
 
         # call super constructor
         super().__init__(lens_system_prompt_template, lens_question_template, lens_followups, evaluation_engine)
 
     @overrides
     def evaluate(self, chat_history: list = None, survey_context: str = "", survey_locations: str = "",
-                 survey_excerpt: str = "", **kwargs) -> list:
+                 survey_excerpt: str = "", **kwargs) -> dict:
         """
         Override default evaluate method.
 
         :param chat_history: Chat history to use for the evaluation chain (or None for none).
         :type chat_history: list
         :param survey_context: Information about the survey context.
         :type survey_context: str
         :param survey_locations: Information about the survey location(s).
         :type survey_locations: str
         :param survey_excerpt: Excerpt from the survey instrument to evaluate.
         :type survey_excerpt: str
         :param kwargs: Keyword arguments to use for formatting the task system prompt and question.
         :type kwargs: Any
-        :return: A list with, first, the evaluation result (a dict), and then a list with the full history of the
-            evaluation chain (each of which is a list with two strings, a prompt and a response).
-        :rtype: list
+        :return: A dict with result ("success" or "error"), error (if result is "error"), response (a dict),
+            and history (a list with the full history of the evaluation chain, each item of which is a list with two
+            strings, a prompt and a response).
+        :rtype: dict
         """
 
         return super().evaluate(chat_history=chat_history, survey_context=survey_context,
                                 survey_locations=survey_locations,
                                 survey_excerpt=EvaluationEngine.clean_whitespace(survey_excerpt), **kwargs)
 
     @overrides
     async def a_evaluate(self, chat_history: list = None, survey_context: str = "", survey_locations: str = "",
-                         survey_excerpt: str = "", **kwargs) -> list:
+                         survey_excerpt: str = "", **kwargs) -> dict:
         """
         Override default a_evaluate method.
 
         :param chat_history: Chat history to use for the evaluation chain (or None for none).
         :type chat_history: list
         :param survey_context: Information about the survey context.
         :type survey_context: str
         :param survey_locations: Information about the survey location(s).
         :type survey_locations: str
         :param survey_excerpt: Excerpt from the survey instrument to evaluate.
         :type survey_excerpt: str
         :param kwargs: Keyword arguments to use for formatting the task system prompt and question.
         :type kwargs: Any
-        :return: A list with, first, the evaluation result (a dict), and then a list with the full history of the
-            evaluation chain (each of which is a list with two strings, a prompt and a response).
-        :rtype: list
+        :return: A dict with result ("success" or "error"), error (if result is "error"), response (a dict),
+            and history (a list with the full history of the evaluation chain, each item of which is a list with two
+            strings, a prompt and a response).
+        :rtype: dict
         """
 
         return await super().a_evaluate(chat_history=chat_history, survey_context=survey_context,
                                         survey_locations=survey_locations,
                                         survey_excerpt=EvaluationEngine.clean_whitespace(survey_excerpt), **kwargs)
 
     def format_result(self, result: dict | None = None) -> str:
@@ -772,56 +778,58 @@
         ]
 
         # call super constructor
         super().__init__(lens_system_prompt_template, lens_question_template, lens_followups, evaluation_engine)
 
     @overrides
     def evaluate(self, chat_history: list = None, survey_context: str = "", survey_locations: str = "",
-                 survey_excerpt: str = "", **kwargs) -> list:
+                 survey_excerpt: str = "", **kwargs) -> dict:
         """
         Override default evaluate method.
 
         :param chat_history: Chat history to use for the evaluation chain (or None for none).
         :type chat_history: list
         :param survey_context: Information about the survey context.
         :type survey_context: str
         :param survey_locations: Information about the survey location(s).
         :type survey_locations: str
         :param survey_excerpt: Excerpt from the survey instrument to evaluate.
         :type survey_excerpt: str
         :param kwargs: Keyword arguments to use for formatting the task system prompt and question.
         :type kwargs: Any
-        :return: A list with, first, the evaluation result (a dict), and then a list with the full history of the
-            evaluation chain (each of which is a list with two strings, a prompt and a response).
-        :rtype: list
+        :return: A dict with result ("success" or "error"), error (if result is "error"), response (a dict),
+            and history (a list with the full history of the evaluation chain, each item of which is a list with two
+            strings, a prompt and a response).
+        :rtype: dict
         """
 
         return super().evaluate(chat_history=chat_history, survey_context=survey_context,
                                 survey_locations=survey_locations,
                                 survey_excerpt=EvaluationEngine.clean_whitespace(survey_excerpt), **kwargs)
 
     @overrides
     async def a_evaluate(self, chat_history: list = None, survey_context: str = "", survey_locations: str = "",
-                         survey_excerpt: str = "", **kwargs) -> list:
+                         survey_excerpt: str = "", **kwargs) -> dict:
         """
         Override default a_evaluate method.
 
         :param chat_history: Chat history to use for the evaluation chain (or None for none).
         :type chat_history: list
         :param survey_context: Information about the survey context.
         :type survey_context: str
         :param survey_locations: Information about the survey location(s).
         :type survey_locations: str
         :param survey_excerpt: Excerpt from the survey instrument to evaluate.
         :type survey_excerpt: str
         :param kwargs: Keyword arguments to use for formatting the task system prompt and question.
         :type kwargs: Any
-        :return: A list with, first, the evaluation result (a dict), and then a list with the full history of the
-            evaluation chain (each of which is a list with two strings, a prompt and a response).
-        :rtype: list
+        :return: A dict with result ("success" or "error"), error (if result is "error"), response (a dict),
+            and history (a list with the full history of the evaluation chain, each item of which is a list with two
+            strings, a prompt and a response).
+        :rtype: dict
         """
 
         return await super().a_evaluate(chat_history=chat_history, survey_context=survey_context,
                                         survey_locations=survey_locations,
                                         survey_excerpt=EvaluationEngine.clean_whitespace(survey_excerpt), **kwargs)
 
     def format_result(self, result: dict | None = None) -> str:
```

### Comparing `surveyeval-0.1.5/src/surveyeval/evaluation_engine.py` & `surveyeval-0.1.6/src/surveyeval/evaluation_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,14 +134,30 @@
             # if so, truncate the tokens list and convert it back to a string
             tokens = tokens[:max_tokens]
             s = self.tokenizer.decode(tokens)
 
         return s
 
     @staticmethod
+    def trim_json(json_str: str) -> str:
+        """
+        Trim common leading and trailing characters from JSON string.
+
+        :param json_str: JSON string to trim
+        :type json_str: str
+        :return: Trimmed JSON string
+        :rtype: str
+        """
+
+        # TBD
+        trimmed_json = json_str
+
+        return trimmed_json
+
+    @staticmethod
     def clean_whitespace(s: str) -> str:
         """
         Strip whitespace from prompt string in order to economize on tokens.
 
         :param s: Prompt string to clean.
         :type s: str
         :return: Cleaned prompt string.
@@ -262,15 +278,15 @@
         # create and return conversation chain
         llm_chain = ConversationChain(
             llm=conversation_llm, prompt=chat_prompt, memory=memory, input_key="question", output_key="answer"
         )
         return llm_chain
 
     async def a_run_evaluation_chain(self, task_system_prompt: str, question: str, followups: list[dict],
-                                     chat_history: list = None) -> list:
+                                     chat_history: list = None) -> dict:
         """
         Run an evaluation chain (asynchronously).
 
         :param task_system_prompt: System prompt template to use for the evaluation chain. This can include the
             {survey_context} and {survey_locations} variables to include information about the survey context. It
             should specify a specific JSON format for all responses.
         :type task_system_prompt: str
@@ -285,22 +301,27 @@
             "condition_key": the key in the response dict to check;
             "condition_value": the value to check against the one in the response dict;
             "prompt_template": the template for the follow-up question to ask (which can include variables from
             the response dict).
         :type followups: list[dict]
         :param chat_history: Chat history to use for the evaluation chain (or None for none).
         :type chat_history: list
-        :return: A list with, first, the evaluation result (a dict), and then a list with the full history of the
-            evaluation chain (each of which is a list with two strings, a prompt and a response).
-        :rtype: list
+        :return: A dict with result ("success" or "error"), error (if result is "error"), response (a dict),
+            and history (a list with the full history of the evaluation chain, each item of which is a list with two
+            strings, a prompt and a response).
+        :rtype: dict
         """
 
         # initialize new evaluation chain
         llm_chain = self.get_chain(system_prompt=task_system_prompt, starting_chat_history=chat_history,
                                    max_history_tokens=6000)
+
+        # initialize results
+        result_dict = {"result": None, "error": None, "response": None, "history": None}
+        response_dict = None
         full_history = []
 
         # ask our question to the LLM, retrying the appropriate number of times
         attempt = 0
         while True:
             attempt += 1
             try:
@@ -321,38 +342,47 @@
         # get prompt and response, record in history
         prompt = result["question"].strip()
         json_response = result["answer"].strip()
         full_history.append([prompt, json_response])
 
         # parse result as JSON
         try:
-            response_dict = json.loads(json_response)
+            response_dict = json.loads(EvaluationEngine.trim_json(json_response))
         except Exception as e:
-            self.logger.error(f"Error occurred parsing JSON ({str(e)}); raw JSON: {json_response}")
-            return [None, full_history]
-
-        # ask follow-up questions
-        for followup in followups:
-            updated_data = await self.a_followup_question(**followup, response_dict=response_dict, llm_chain=llm_chain,
-                                                          chat_history=chat_history)
-            # parse response
-            updated_response = updated_data[0]
-            prompt = updated_data[1]
-            json_response = updated_data[2]
-            # if we actually asked a follow-up, include it in the history
-            if prompt:
-                full_history.append([prompt, json_response])
-            # if we actually got a parsed response, update the response dict
-            if updated_response:
-                response_dict.update(updated_response)
+            error_message = f"Error occurred parsing LLM's JSON response ({str(e)}); raw JSON: {json_response}"
+            self.logger.error(error_message)
+            result_dict["result"] = "error"
+            result_dict["error"] = error_message
+        else:
+            # unless something goes wrong later, presume we're successful
+            result_dict["result"] = "success"
 
-        return [response_dict, full_history]
+            # ask follow-up questions
+            for followup in followups:
+                followup_result = await self.a_followup_question(**followup, response_dict=response_dict,
+                                                                 llm_chain=llm_chain, chat_history=chat_history)
+
+                # if we actually asked a follow-up, include it in the history
+                if followup_result["result"] != "skipped":
+                    full_history.append([prompt, json_response])
+                if followup_result["result"] == "success" and followup_result["response"]:
+                    # if we actually got a parsed response, update the response dict
+                    response_dict.update(followup_result["response"])
+                elif followup_result["result"] == "error":
+                    # otherwise, if we got an error, update the result dict to reflect that
+                    result_dict["error"] = followup_result["error"]
+                    result_dict["result"] = "error"
+
+        # assemble and return results
+        result_dict["response"] = response_dict
+        result_dict["history"] = full_history
+        return result_dict
 
     def run_evaluation_chain(self, task_system_prompt: str, question: str, followups: list[dict],
-                             chat_history: list = None) -> list:
+                             chat_history: list = None) -> dict:
         """
         Run an evaluation chain (synchronously).
 
         :param task_system_prompt: System prompt template to use for the evaluation chain. This can include the
             {survey_context} and {survey_locations} variables to include information about the survey context. It
             should specify a specific JSON format for all responses.
         :type task_system_prompt: str
@@ -367,17 +397,18 @@
             "condition_key": the key in the response dict to check;
             "condition_value": the value to check against the one in the response dict;
             "prompt_template": the template for the follow-up question to ask (which can include variables from
             the response dict).
         :type followups: list[dict]
         :param chat_history: Chat history to use for the evaluation chain (or None for none).
         :type chat_history: list
-        :return: A list with, first, the evaluation result (a dict), and then a list with the full history of the
-            evaluation chain (each of which is a list with two strings, a prompt and a response).
-        :rtype: list
+        :return: A dict with result ("success" or "error"), error (if result is "error"), response (a dict),
+            and history (a list with the full history of the evaluation chain, each item of which is a list with two
+            strings, a prompt and a response).
+        :rtype: dict
         """
 
         # run asynchronous process synchronously
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
             self.a_run_evaluation_chain(
                 task_system_prompt=task_system_prompt,
@@ -385,15 +416,15 @@
                 followups=followups,
                 chat_history=chat_history
             )
         )
 
     async def a_followup_question(self, condition_func: callable, condition_key: str, condition_value,
                                   prompt_template: str, response_dict: dict, llm_chain: ConversationChain,
-                                  chat_history: list = None) -> list:
+                                  chat_history: list = None) -> dict:
         """
         Ask a follow-up question (asynchronously).
 
         :param condition_func: Function to call to evaluate whether the follow-up should be asked (True) or not (False).
         :type condition_func: callable
         :param condition_key: Key to check in the response dictionary.
         :type condition_key: str
@@ -404,24 +435,28 @@
         :type prompt_template: str
         :param response_dict: Full response dictionary.
         :type response_dict: dict
         :param llm_chain: Conversation chain to use for asking the follow-up question.
         :type llm_chain: ConversationChain
         :param chat_history: Chat history to use for the evaluation chain (or None for none).
         :type chat_history: list
-        :return: A list with the updated response dictionary (if any), the prompt that was asked ('' if follow-up not
-            asked), and the response that was received.
-        :rtype: list
+        :return: A dict with result ("success", "error", or "skipped"), error (if result is "error"), prompt (a str),
+            response_json (a str), and response (a dict).
+        :rtype: dict
         """
 
+        # initialize results
+        result_dict = {"result": None, "error": None, "prompt": None, "response_json": None, "response": None}
+
         # check to see if we meet the criteria for this follow-up
         if condition_func(response_dict, condition_key, condition_value):
             # if so, format the question
             followup_question = prompt_template.format(**response_dict)
             prompt = followup_question.strip()
+            result_dict["prompt"] = prompt
 
             # ask question to the LLM, retrying the appropriate number of times
             attempt = 0
             while True:
                 attempt += 1
                 try:
                     # ask our question and record the result
@@ -436,33 +471,39 @@
                         await asyncio.sleep(5)
                     else:
                         # maximum attempts reached, raise exception
                         raise RuntimeError(f"Max retries reached asking follow-up. Last error: {str(e)}") from e
 
             # parse result as JSON
             json_response = result["answer"].strip()
+            result_dict["response_json"] = json_response
             if json_response != "{}":
                 try:
-                    return [json.loads(json_response), prompt, json_response]
+                    result_dict["response"] = json.loads(EvaluationEngine.trim_json(json_response))
+                    result_dict["result"] = "success"
                 except Exception as e:
-                    self.logger.error(f"Error occurred parsing JSON ({str(e)}); raw JSON: {json_response}")
-            return [None, prompt, json_response]
+                    error_message = f"Error occurred parsing LLM's JSON response ({str(e)}); raw JSON: {json_response}"
+                    self.logger.error(error_message)
+                    result_dict["error"] = error_message
+                    result_dict["result"] = "error"
+        else:
+            result_dict["result"] = "skipped"
 
-        # return empty values if we don't meet the criteria for this follow-up
-        return [None, '', '']
+        # return assembled result
+        return result_dict
 
 
 class EvaluationLens:
     """Class for instrument evaluation lens, which is used to conduct a particular type of evaluation."""
 
     evaluation_engine: EvaluationEngine
     task_system_prompt_template: str
     question_template: str
     followups: list[dict]
-    evaluation_result: list
+    evaluation_result: dict
 
     def __init__(self, task_system_prompt_template: str, question_template: str, followups: list[dict],
                  evaluation_engine: EvaluationEngine):
         """
         Initialize evaluation lens.
 
         :param task_system_prompt_template: System prompt template to use for the evaluation chain. This can include the
@@ -490,47 +531,49 @@
         self.task_system_prompt_template = task_system_prompt_template
         if evaluation_engine.extra_evaluation_instructions:
             self.task_system_prompt_template += (f"\n\nAlso follow these additional instructions:\n\n"
                                                  f"{evaluation_engine.extra_evaluation_instructions}")
         self.question_template = question_template
         self.followups = followups
         self.evaluation_engine = evaluation_engine
-        self.evaluation_result = []
+        self.evaluation_result = {}
 
-    def evaluate(self, chat_history=None, **kwargs) -> list:
+    def evaluate(self, chat_history=None, **kwargs) -> dict:
         """
         Run an evaluation chain (synchronously).
 
         :param chat_history: Chat history to use for the evaluation chain (or None for none).
         :type chat_history: list
         :param kwargs: Keyword arguments to use for formatting the task system prompt and question.
         :type kwargs: Any
-        :return: A list with, first, the evaluation result (a dict), and then a list with the full history of the
-            evaluation chain (each of which is a list with two strings, a prompt and a response).
-        :rtype: list
+        :return: A dict with result ("success" or "error"), error (if result is "error"), response (a dict),
+            and history (a list with the full history of the evaluation chain, each item of which is a list with two
+            strings, a prompt and a response).
+        :rtype: dict
         """
 
         # call evaluation engine to run evaluation chain
         self.evaluation_result = self.evaluation_engine.run_evaluation_chain(
             task_system_prompt=self.task_system_prompt_template.format(**kwargs),
             question=self.question_template.format(**kwargs),
             followups=self.followups, chat_history=chat_history)
         return self.evaluation_result
     
-    async def a_evaluate(self, chat_history=None, **kwargs) -> list:
+    async def a_evaluate(self, chat_history=None, **kwargs) -> dict:
         """
         Run an evaluation chain (asynchronously).
 
         :param chat_history: Chat history to use for the evaluation chain (or None for none).
         :type chat_history: list
         :param kwargs: Keyword arguments to use for formatting the task system prompt and question.
         :type kwargs: Any
-        :return: A list with, first, the evaluation result (a dict), and then a list with the full history of the
-            evaluation chain (each of which is a list with two strings, a prompt and a response).
-        :rtype: list
+        :return: A dict with result ("success" or "error"), error (if result is "error"), response (a dict),
+            and history (a list with the full history of the evaluation chain, each item of which is a list with two
+            strings, a prompt and a response).
+        :rtype: dict
         """
 
         # call evaluation engine to run evaluation chain
         self.evaluation_result = await self.evaluation_engine.a_run_evaluation_chain(
             task_system_prompt=self.task_system_prompt_template.format(**kwargs),
             question=self.question_template.format(**kwargs),
             followups=self.followups, chat_history=chat_history)
@@ -546,15 +589,15 @@
         :rtype: str
         """
 
         # use evaluation_result attribute if no result is passed
         if result is not None:
             result_to_format = result
         else:
-            result_to_format = self.evaluation_result
+            result_to_format = self.evaluation_result[0]
 
         # return empty string if no result is available to format
         if result_to_format is None:
             return ""
 
         # format result as a list of key-value pairs
         formatted_results = []
```

### Comparing `surveyeval-0.1.5/src/surveyeval/survey_parser.py` & `surveyeval-0.1.6/src/surveyeval/survey_parser.py`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.5/src/surveyeval.egg-info/PKG-INFO` & `surveyeval-0.1.6/src/surveyeval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surveyeval
-Version: 0.1.5
+Version: 0.1.6
 Summary: A toolkit for survey evaluation
 Home-page: https://github.com/higherbar-ai/survey-eval
 Author: Christopher Robert
 Author-email: crobert@higherbar.ai
 License: Apache 2.0
 Project-URL: Documentation, https://surveyeval.readthedocs.io/
 Requires-Python: >=3.10
```

