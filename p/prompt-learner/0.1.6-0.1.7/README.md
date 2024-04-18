# Comparing `tmp/prompt_learner-0.1.6.tar.gz` & `tmp/prompt_learner-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt_learner-0.1.6.tar", max compression
+gzip compressed data, was "prompt_learner-0.1.7.tar", max compression
```

## Comparing `prompt_learner-0.1.6.tar` & `prompt_learner-0.1.7.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0     1957 2024-04-13 07:01:40.160627 prompt_learner-0.1.6/README.md
--rw-r--r--   0        0        0     6148 2024-04-12 21:48:53.225544 prompt_learner-0.1.6/prompt_learner/.DS_Store
--rw-r--r--   0        0        0       28 2024-04-11 03:24:46.950449 prompt_learner-0.1.6/prompt_learner/adapters/__init__.py
--rw-r--r--   0        0        0      240 2024-04-11 03:34:45.465265 prompt_learner-0.1.6/prompt_learner/adapters/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2711 2024-04-11 03:18:16.055309 prompt_learner-0.1.6/prompt_learner/adapters/__pycache__/anthropic.cpython-311.pyc
--rw-r--r--   0        0        0     1470 2024-04-11 03:12:44.449954 prompt_learner-0.1.6/prompt_learner/adapters/__pycache__/openai.cpython-311.pyc
--rw-r--r--   0        0        0      394 2024-03-30 07:34:49.479472 prompt_learner-0.1.6/prompt_learner/adapters/adapter.py
--rw-r--r--   0        0        0     1261 2024-04-11 03:18:09.033090 prompt_learner-0.1.6/prompt_learner/adapters/anthropic.py
--rw-r--r--   0        0        0      597 2024-04-11 03:12:12.072973 prompt_learner-0.1.6/prompt_learner/adapters/openai.py
--rw-r--r--   0        0        0     1295 2024-04-12 22:29:26.768011 prompt_learner-0.1.6/prompt_learner/evals/metrics/accuracy.py
--rw-r--r--   0        0        0       29 2024-04-11 03:23:09.786151 prompt_learner-0.1.6/prompt_learner/examples/__init__.py
--rw-r--r--   0        0        0      237 2024-03-30 05:01:50.208264 prompt_learner-0.1.6/prompt_learner/examples/example.py
--rw-r--r--   0        0        0        0 2024-03-30 04:43:35.605009 prompt_learner-0.1.6/prompt_learner/examples/manipulation/__init__.py
--rw-r--r--   0        0        0        0 2024-03-30 06:22:23.812645 prompt_learner-0.1.6/prompt_learner/inference/__init__.py
--rw-r--r--   0        0        0        0 2024-03-30 06:22:57.915297 prompt_learner-0.1.6/prompt_learner/inference/predict.py
--rw-r--r--   0        0        0        0 2024-04-03 00:44:07.604053 prompt_learner-0.1.6/prompt_learner/optimizers/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 03:24:34.521211 prompt_learner-0.1.6/prompt_learner/optimizers/descriptors/__init__.py
--rw-r--r--   0        0        0      165 2024-04-03 13:24:51.204583 prompt_learner-0.1.6/prompt_learner/optimizers/descriptors/descriptor.py
--rw-r--r--   0        0        0       34 2024-03-30 05:23:18.250890 prompt_learner-0.1.6/prompt_learner/optimizers/optimizer.py
--rw-r--r--   0        0        0       30 2024-04-11 03:24:14.614552 prompt_learner-0.1.6/prompt_learner/optimizers/selectors/__init__.py
--rw-r--r--   0        0        0     1537 2024-04-12 21:34:12.452345 prompt_learner-0.1.6/prompt_learner/optimizers/selectors/diverse_sampler.py
--rw-r--r--   0        0        0      624 2024-04-12 23:18:56.744204 prompt_learner-0.1.6/prompt_learner/optimizers/selectors/random_sampler.py
--rw-r--r--   0        0        0      873 2024-04-12 23:12:29.480864 prompt_learner-0.1.6/prompt_learner/optimizers/selectors/selector.py
--rw-r--r--   0        0        0      888 2024-04-11 07:42:16.046290 prompt_learner-0.1.6/prompt_learner/optimizers/selectors/stratified_sampler.py
--rw-r--r--   0        0        0       26 2024-04-11 03:24:06.645622 prompt_learner-0.1.6/prompt_learner/prompts/__init__.py
--rw-r--r--   0        0        0      623 2024-04-11 03:17:38.543493 prompt_learner-0.1.6/prompt_learner/prompts/cot.py
--rw-r--r--   0        0        0      982 2024-04-12 23:14:38.902964 prompt_learner-0.1.6/prompt_learner/prompts/prompt.py
--rw-r--r--   0        0        0       22 2024-04-11 03:23:46.852998 prompt_learner-0.1.6/prompt_learner/tasks/__init__.py
--rw-r--r--   0        0        0      614 2024-04-11 03:43:03.066088 prompt_learner-0.1.6/prompt_learner/tasks/classification.py
--rw-r--r--   0        0        0      529 2024-04-11 03:43:06.447386 prompt_learner-0.1.6/prompt_learner/tasks/tagging.py
--rw-r--r--   0        0        0     1536 2024-04-12 22:21:38.784259 prompt_learner-0.1.6/prompt_learner/tasks/task.py
--rw-r--r--   0        0        0       30 2024-04-11 03:23:57.503062 prompt_learner-0.1.6/prompt_learner/templates/__init__.py
--rw-r--r--   0        0        0     1610 2024-04-14 19:23:58.989213 prompt_learner-0.1.6/prompt_learner/templates/anthropic_template.py
--rw-r--r--   0        0        0     1432 2024-04-11 03:43:17.180163 prompt_learner-0.1.6/prompt_learner/templates/openai_template.py
--rw-r--r--   0        0        0     1556 2024-04-14 19:25:07.177175 prompt_learner-0.1.6/prompt_learner/templates/template.py
--rw-r--r--   0        0        0      428 2024-04-14 19:46:37.477980 prompt_learner-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2582 1970-01-01 00:00:00.000000 prompt_learner-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     2140 2024-04-16 15:23:30.960382 prompt_learner-0.1.7/README.md
+-rw-r--r--   0        0        0     6148 2024-04-12 21:48:53.225544 prompt_learner-0.1.7/prompt_learner/.DS_Store
+-rw-r--r--   0        0        0       28 2024-04-11 03:24:46.950449 prompt_learner-0.1.7/prompt_learner/adapters/__init__.py
+-rw-r--r--   0        0        0      240 2024-04-11 03:34:45.465265 prompt_learner-0.1.7/prompt_learner/adapters/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2711 2024-04-11 03:18:16.055309 prompt_learner-0.1.7/prompt_learner/adapters/__pycache__/anthropic.cpython-311.pyc
+-rw-r--r--   0        0        0     1470 2024-04-11 03:12:44.449954 prompt_learner-0.1.7/prompt_learner/adapters/__pycache__/openai.cpython-311.pyc
+-rw-r--r--   0        0        0      394 2024-03-30 07:34:49.479472 prompt_learner-0.1.7/prompt_learner/adapters/adapter.py
+-rw-r--r--   0        0        0     1261 2024-04-11 03:18:09.033090 prompt_learner-0.1.7/prompt_learner/adapters/anthropic.py
+-rw-r--r--   0        0        0      597 2024-04-11 03:12:12.072973 prompt_learner-0.1.7/prompt_learner/adapters/openai.py
+-rw-r--r--   0        0        0     1295 2024-04-12 22:29:26.768011 prompt_learner-0.1.7/prompt_learner/evals/metrics/accuracy.py
+-rw-r--r--   0        0        0       29 2024-04-11 03:23:09.786151 prompt_learner-0.1.7/prompt_learner/examples/__init__.py
+-rw-r--r--   0        0        0      316 2024-04-18 07:01:26.041471 prompt_learner-0.1.7/prompt_learner/examples/example.py
+-rw-r--r--   0        0        0        0 2024-03-30 04:43:35.605009 prompt_learner-0.1.7/prompt_learner/examples/manipulation/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-30 06:22:23.812645 prompt_learner-0.1.7/prompt_learner/inference/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-30 06:22:57.915297 prompt_learner-0.1.7/prompt_learner/inference/predict.py
+-rw-r--r--   0        0        0        0 2024-04-03 00:44:07.604053 prompt_learner-0.1.7/prompt_learner/optimizers/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 03:24:34.521211 prompt_learner-0.1.7/prompt_learner/optimizers/descriptors/__init__.py
+-rw-r--r--   0        0        0      165 2024-04-03 13:24:51.204583 prompt_learner-0.1.7/prompt_learner/optimizers/descriptors/descriptor.py
+-rw-r--r--   0        0        0       34 2024-03-30 05:23:18.250890 prompt_learner-0.1.7/prompt_learner/optimizers/optimizer.py
+-rw-r--r--   0        0        0       30 2024-04-11 03:24:14.614552 prompt_learner-0.1.7/prompt_learner/optimizers/selectors/__init__.py
+-rw-r--r--   0        0        0     1537 2024-04-12 21:34:12.452345 prompt_learner-0.1.7/prompt_learner/optimizers/selectors/diverse_sampler.py
+-rw-r--r--   0        0        0      624 2024-04-12 23:18:56.744204 prompt_learner-0.1.7/prompt_learner/optimizers/selectors/random_sampler.py
+-rw-r--r--   0        0        0      873 2024-04-12 23:12:29.480864 prompt_learner-0.1.7/prompt_learner/optimizers/selectors/selector.py
+-rw-r--r--   0        0        0      888 2024-04-11 07:42:16.046290 prompt_learner-0.1.7/prompt_learner/optimizers/selectors/stratified_sampler.py
+-rw-r--r--   0        0        0       26 2024-04-11 03:24:06.645622 prompt_learner-0.1.7/prompt_learner/prompts/__init__.py
+-rw-r--r--   0        0        0      623 2024-04-11 03:17:38.543493 prompt_learner-0.1.7/prompt_learner/prompts/cot.py
+-rw-r--r--   0        0        0     1009 2024-04-18 07:04:18.022386 prompt_learner-0.1.7/prompt_learner/prompts/prompt.py
+-rw-r--r--   0        0        0       22 2024-04-11 03:23:46.852998 prompt_learner-0.1.7/prompt_learner/tasks/__init__.py
+-rw-r--r--   0        0        0      614 2024-04-18 01:51:33.806026 prompt_learner-0.1.7/prompt_learner/tasks/classification.py
+-rw-r--r--   0        0        0      400 2024-04-18 06:38:05.061557 prompt_learner-0.1.7/prompt_learner/tasks/sql_generation.py
+-rw-r--r--   0        0        0      529 2024-04-11 03:43:06.447386 prompt_learner-0.1.7/prompt_learner/tasks/tagging.py
+-rw-r--r--   0        0        0     1589 2024-04-18 07:03:05.419391 prompt_learner-0.1.7/prompt_learner/tasks/task.py
+-rw-r--r--   0        0        0       30 2024-04-11 03:23:57.503062 prompt_learner-0.1.7/prompt_learner/templates/__init__.py
+-rw-r--r--   0        0        0     3104 2024-04-18 06:59:46.552014 prompt_learner-0.1.7/prompt_learner/templates/anthropic_template.py
+-rw-r--r--   0        0        0     2746 2024-04-18 07:20:36.951484 prompt_learner-0.1.7/prompt_learner/templates/openai_template.py
+-rw-r--r--   0        0        0     1570 2024-04-18 06:49:29.458366 prompt_learner-0.1.7/prompt_learner/templates/template.py
+-rw-r--r--   0        0        0      428 2024-04-18 07:50:09.607958 prompt_learner-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2765 1970-01-01 00:00:00.000000 prompt_learner-0.1.7/PKG-INFO
```

### Comparing `prompt_learner-0.1.6/README.md` & `prompt_learner-0.1.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -18,20 +18,21 @@
 5. Instructions for output format
 
 
 See the documentation on ["Why Prompt Learner?"](https://promptlearner.attuna.xyz/why.html) to learn more.
 
 ## Getting started
 
+[![Watch our quick start guide](https://cdn.loom.com/sessions/thumbnails/94f5345736d34af3b8b6b41e1be4c2a3-with-play.gif)](https://www.loom.com/share/94f5345736d34af3b8b6b41e1be4c2a3)
+
 You can `pip install` Prompt Learner: 
 
 ```bash
 pip install prompt-learner
 ```
-
 > [!TIP]
 > See the [getting started tutorial](https://promptlearner.attuna.xyz/getting-started.html) for a detailed example of Prompt Learner in action.
 
 ## How it works
 ![Architecture](docs/concepts/images/architecture.png)
 Prompt-learner runs on the above architecture.
 Starting from the left, the user has to decide on 3 aspects -
```

### Comparing `prompt_learner-0.1.6/prompt_learner/.DS_Store` & `prompt_learner-0.1.7/prompt_learner/.DS_Store`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.6/prompt_learner/adapters/__pycache__/anthropic.cpython-311.pyc` & `prompt_learner-0.1.7/prompt_learner/adapters/__pycache__/anthropic.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.6/prompt_learner/adapters/__pycache__/openai.cpython-311.pyc` & `prompt_learner-0.1.7/prompt_learner/adapters/__pycache__/openai.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.6/prompt_learner/adapters/anthropic.py` & `prompt_learner-0.1.7/prompt_learner/adapters/anthropic.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.6/prompt_learner/adapters/openai.py` & `prompt_learner-0.1.7/prompt_learner/adapters/openai.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.6/prompt_learner/evals/metrics/accuracy.py` & `prompt_learner-0.1.7/prompt_learner/evals/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.6/prompt_learner/optimizers/selectors/diverse_sampler.py` & `prompt_learner-0.1.7/prompt_learner/optimizers/selectors/diverse_sampler.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.6/prompt_learner/optimizers/selectors/random_sampler.py` & `prompt_learner-0.1.7/prompt_learner/optimizers/selectors/random_sampler.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.6/prompt_learner/optimizers/selectors/selector.py` & `prompt_learner-0.1.7/prompt_learner/optimizers/selectors/selector.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.6/prompt_learner/optimizers/selectors/stratified_sampler.py` & `prompt_learner-0.1.7/prompt_learner/optimizers/selectors/stratified_sampler.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.6/prompt_learner/prompts/cot.py` & `prompt_learner-0.1.7/prompt_learner/prompts/cot.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.6/prompt_learner/prompts/prompt.py` & `prompt_learner-0.1.7/prompt_learner/prompts/prompt.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,10 +15,10 @@
         """Select examples for the task."""
     
     def assemble_prompt(self):
         """Assemble the prompt."""
         self.prompt = f"""{self.template.descriptor}\n{self.template.examples_preamble}
         \n{self.template.format_examples(self.selector.selected_examples)}"""
 
-    def add_inference(self, text: str):
+    def add_inference(self, text: str, context: str = ""):
         """Add inference sample"""
-        self.prompt = self.prompt + self.template.add_prediction_sample(text)
+        self.prompt = self.prompt + self.template.add_prediction_sample(text,context)
```

### Comparing `prompt_learner-0.1.6/prompt_learner/tasks/classification.py` & `prompt_learner-0.1.7/prompt_learner/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.6/prompt_learner/tasks/tagging.py` & `prompt_learner-0.1.7/prompt_learner/tasks/tagging.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.6/prompt_learner/tasks/task.py` & `prompt_learner-0.1.7/prompt_learner/tasks/task.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Generic Task class."""
 
-from typing import List
+from typing import List, Optional
 from pydantic import BaseModel, Field
 from prompt_learner.examples.example import Example
 from prompt_learner.adapters.adapter import Adapter
 
 
-class Task(BaseModel):
+class Task(BaseModel): #TO_DO enum for all task types
     """Defines the contract for a Generic task."""
     description: str = Field(description="The name of the task.")
-    allowed_labels: List[str] = Field(description="Allowed labels for task.")
+    allowed_labels: List[str] = Field(description="Allowed labels for task.", default=[])
     examples: List[Example] = []
     selected_examples: List[Example] = []
     test_examples: List[Example] = []
 
     def validate_example(self, example: Example):
         """Validate the example for the task."""
         # This method will be overridden in subclasses
```

### Comparing `prompt_learner-0.1.6/prompt_learner/templates/anthropic_template.py` & `prompt_learner-0.1.7/prompt_learner/templates/anthropic_template.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,38 +4,64 @@
 from .template import Template
 
 
 class AnthropicCompletionTemplate(Template):
     """This class generates a template for Anthropic completions"""
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
+        tasks_with_labels = ["Classification", "Tagging"]
         self.descriptor = f"""You are a helpful AI assistant.
         You are helping a user with a {self.task_type} task.
         You have to perform the following task.
-        <task_description>{self.task_description}</task_description>
-        You have to select from the following labels.
+        <task_description>{self.task_description}</task_description>"""
+        if self.allowed_labels:
+            self.descriptor += """You have to select from the following labels.
         <allowed_labels>{self.allowed_labels}</allowed_labels>"""
-        self.prediction_preamble = f"""Given the text, you have
+        if self.task_type in tasks_with_labels:
+            self.prediction_preamble = f"""Given the text, you have
         to now predict the labels from
         list of allowed labels - {self.allowed_labels}
         Output only the label(s) and close the <label> tag."""
+        elif self.task_type == "SQLGeneration":
+            self.prediction_preamble = """Given the text, you have
+        to now generate a SQL query. Only the SQL query is expected."""
+        else:  #generic preamble for prediction
+            self.prediction_preamble = """Given the text, you have to now predict."""
         self.examples_preamble = """ Here are a few examples to
         help you understand the task better."""
     
     def format_examples(self, examples: List[Example]):
         """Formats the task examples into a string."""
+        tasks_with_labels = ["Classification", "Tagging"]
         examples_str = ""
         for example in examples:
-            examples_str += f"""
-            <example>
-            <text> {example.text}</text>\n
-            <label> {example.label}</label>\n
-            </example>"""
+            if self.task_type in tasks_with_labels:
+                examples_str += f"""
+                <example>
+                <text> {example.text}</text>\n
+                <label> {example.label}</label>\n
+                </example>"""
+            elif self.task_type == "SQLGeneration":
+                examples_str += f"""
+                <example>
+                <schema> {example.context}</schema>\n
+                <text> {example.text}</text>\n
+                <SQL> {example.label}</SQL>\n
+                </example>"""
+            else:
+                examples_str += f"""
+                <example>
+                <text> {example.text}</text>\n
+                <output> {example.label}</output>\n
+                </example>"""
         return examples_str
     
-    def add_prediction_sample(self, text: str):
+    def add_prediction_sample(self, text: str, context: str):
         """Add prediction sample to task."""
-        return f"""\n
-        <text> {text} </text>\n
-        <label>
-        """
-        
+        tasks_with_labels = ["Classification", "Tagging"]
+        prediction_preamble = self.prediction_preamble + f"""\n <text> {text} <text>"""
+        if self.task_type in tasks_with_labels:
+            return prediction_preamble + "<label>"
+        elif self.task_type == "SQLGeneration":
+            return prediction_preamble + f"""\n <schema>{context} <\schema>\m <SQL>"""
+        else:
+            return prediction_preamble + "<output>"
```

### Comparing `prompt_learner-0.1.6/prompt_learner/templates/openai_template.py` & `prompt_learner-0.1.7/prompt_learner/templates/openai_template.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,36 +2,60 @@
 from typing import List
 from prompt_learner.examples.example import Example
 from .template import Template
 
 
 class OpenAICompletionTemplate(Template):
     """This class generates a template for OpenAI completions"""
-
+    
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
+        tasks_with_labels = ["Classification", "Tagging"]
         self.descriptor = f"""You are a helpful AI assistant.
         You are helping a user with a {self.task_type} task.
-        The user asks you to {self.task_description}.
-        You have to select from the following labels.
-        {self.allowed_labels}."""
-        self.prediction_preamble = f"""Given the text, 
-        you have to now predict the labels from the 
-        list of allowed labels - {self.allowed_labels}."""
+        The user asks you to {self.task_description}."""
+        if self.allowed_labels:
+            self.descriptor += """You have to select from the following labels.
+            {self.allowed_labels}."""
+        if self.task_type in tasks_with_labels:
+            self.prediction_preamble = f"""Given the text, 
+            you have to now predict the labels from the 
+            list of allowed labels - {self.allowed_labels}."""
+        elif self.task_type == "SQLGeneration":
+            self.prediction_preamble = """Given the text, 
+            you have to now generate a SQL query."""
+        else:  #generic preamble for prediction
+            self.prediction_preamble = """Given the text, 
+            you have to now predict."""
         self.examples_preamble = """Here are a few examples to help you
         understand the task better."""
        
     def format_examples(self, examples: List[Example]):
         """Formats the task examples into a string."""
+        tasks_with_labels = ["Classification", "Tagging"]
         examples_str = ""
         for example in examples:
-            # Assuming 'example' can be directly converted to string.
-            examples_str += f"""
-            text: {example.text}\n
-            label: {example.label}\n"""
+            if self.task_type in tasks_with_labels:
+                examples_str += f"""
+                text: {example.text}\n
+                label: {example.label}\n"""
+            elif self.task_type == "SQLGeneration":
+                examples_str += f"""
+                schema: {example.context}\n
+                text: {example.text}\n
+                SQL: {example.label}\n"""
+            else: #generic example format
+                examples_str += f"""
+                text: {example.text}\n
+                output: {example.label}\n"""
         return examples_str
 
-    def add_prediction_sample(self, text: str):
+    def add_prediction_sample(self, text: str, context: str = None):
         """Add prediction sample to task."""
-        return f"""\n
-        text: {text}
-        label: """
+        tasks_with_labels = ["Classification", "Tagging"]
+        prediction_preamble = self.prediction_preamble + f"""\n text: {text}"""
+        if self.task_type in tasks_with_labels:
+            return prediction_preamble + "\n label:"
+        elif self.task_type == "SQLGeneration":
+            return prediction_preamble + f"""\n schema: {context}\n SQL: """
+        else:
+            return prediction_preamble + "\n output:"
```

### Comparing `prompt_learner-0.1.6/prompt_learner/templates/template.py` & `prompt_learner-0.1.7/prompt_learner/templates/template.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,10 +28,10 @@
         self.task_type = self.task.__doc__
         self.allowed_labels = self.task.allowed_labels
         
     def format_examples(self, examples: List[Example]):
         """Add an example to the task."""
         # This method will be overridden in subclasses
 
-    def add_prediction_sample(self, text: str):
+    def add_prediction_sample(self, text: str, context: str):
         """Add inference instructions to task."""
         # This method will be overridden in subclasses
```

### Comparing `prompt_learner-0.1.6/PKG-INFO` & `prompt_learner-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-learner
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Aditya Lahiri
 Author-email: adityalahiri13@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -36,20 +36,21 @@
 5. Instructions for output format
 
 
 See the documentation on ["Why Prompt Learner?"](https://promptlearner.attuna.xyz/why.html) to learn more.
 
 ## Getting started
 
+[![Watch our quick start guide](https://cdn.loom.com/sessions/thumbnails/94f5345736d34af3b8b6b41e1be4c2a3-with-play.gif)](https://www.loom.com/share/94f5345736d34af3b8b6b41e1be4c2a3)
+
 You can `pip install` Prompt Learner: 
 
 ```bash
 pip install prompt-learner
 ```
-
 > [!TIP]
 > See the [getting started tutorial](https://promptlearner.attuna.xyz/getting-started.html) for a detailed example of Prompt Learner in action.
 
 ## How it works
 ![Architecture](docs/concepts/images/architecture.png)
 Prompt-learner runs on the above architecture.
 Starting from the left, the user has to decide on 3 aspects -
```

