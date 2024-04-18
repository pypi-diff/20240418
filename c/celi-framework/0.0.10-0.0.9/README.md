# Comparing `tmp/celi_framework-0.0.10.tar.gz` & `tmp/celi_framework-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celi_framework-0.0.10.tar", max compression
+gzip compressed data, was "celi_framework-0.0.9.tar", max compression
```

## Comparing `celi_framework-0.0.10.tar` & `celi_framework-0.0.9.tar`

### file list

```diff
@@ -1,56 +1,55 @@
--rw-r--r--   0        0        0     1084 2024-04-18 15:27:55.761727 celi_framework-0.0.10/LICENSE
--rw-r--r--   0        0        0    21895 2024-04-18 15:27:55.761727 celi_framework-0.0.10/README.md
--rw-r--r--   0        0        0    10399 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/core/job_description.py
--rw-r--r--   0        0        0    23124 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/core/monitor.py
--rw-r--r--   0        0        0    11301 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/core/mt_factory.py
--rw-r--r--   0        0        0    14719 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/core/post_monitor.py
--rw-r--r--   0        0        0    59120 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/core/processor.py
--rw-r--r--   0        0        0     3060 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/core/runner.py
--rw-r--r--   0        0        0    23630 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/core/templates.py
--rw-r--r--   0        0        0    13793 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/examples/reporting_template/job_description.py
--rw-r--r--   0        0        0    10317 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/examples/reporting_template/tools.py
--rw-r--r--   0        0        0     6133 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/examples/wikipedia/Index_cache.py
--rw-r--r--   0        0        0     7692 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/examples/wikipedia/caching_beautiful_soup_reader.py
--rw-r--r--   0        0        0     5552 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/examples/wikipedia/eval/run_eval.py
--rw-r--r--   0        0        0      530 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/examples/wikipedia/eval/test_sets.json
--rw-r--r--   0        0        0      851 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/examples/wikipedia/eval/test_sets_large.json
--rw-r--r--   0        0        0      161 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/examples/wikipedia/example_config.json
--rw-r--r--   0        0        0    13742 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/examples/wikipedia/index.py
--rw-r--r--   0        0        0    13330 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/examples/wikipedia/job_description.py
--rw-r--r--   0        0        0     7111 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/examples/wikipedia/loader.py
--rw-r--r--   0        0        0    14758 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/examples/wikipedia/tools.py
--rw-r--r--   0        0        0      549 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/examples/wikipedia/wikipedia_utils.py
--rw-r--r--   0        0        0    12668 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/experimental/embeddor.py
--rw-r--r--   0        0        0     7936 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/experimental/mapper.py
--rw-r--r--   0        0        0     1354 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/experimental/mechanic.py
--rw-r--r--   0        0        0        0 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/experimental/preprocessing/__init__.py
--rw-r--r--   0        0        0    23634 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/experimental/preprocessing/pre-processor.py
--rw-r--r--   0        0        0       94 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/experimental/preprocessing/word_pdf_extractors/__init__.py
--rw-r--r--   0        0        0     8832 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/experimental/preprocessing/word_pdf_extractors/extract_pdf_tables.py
--rw-r--r--   0        0        0     2056 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/experimental/preprocessing/word_pdf_extractors/extractor_helpers.py
--rw-r--r--   0        0        0    10669 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/experimental/preprocessing/word_pdf_extractors/pdf_extractor.py
--rw-r--r--   0        0        0     7835 2024-04-18 15:27:55.761727 celi_framework-0.0.10/celi_framework/experimental/preprocessing/word_pdf_extractors/word_extractor.py
--rw-r--r--   0        0        0     5471 2024-04-18 15:27:55.765727 celi_framework-0.0.10/celi_framework/experimental/task_builder/factory.py
--rw-r--r--   0        0        0     4242 2024-04-18 15:27:55.765727 celi_framework-0.0.10/celi_framework/experimental/task_builder/llm_helper_funcs.py
--rw-r--r--   0        0        0     4352 2024-04-18 15:27:55.765727 celi_framework-0.0.10/celi_framework/experimental/task_builder/llms.py
--rw-r--r--   0        0        0     5939 2024-04-18 15:27:55.765727 celi_framework-0.0.10/celi_framework/experimental/task_builder/template.py
--rw-r--r--   0        0        0     9914 2024-04-18 15:27:55.765727 celi_framework-0.0.10/celi_framework/experimental/utils/ada.py
--rw-r--r--   0        0        0    19041 2024-04-18 15:27:55.765727 celi_framework-0.0.10/celi_framework/experimental/utils/mapper_utils.py
--rw-r--r--   0        0        0    13615 2024-04-18 15:27:55.765727 celi_framework-0.0.10/celi_framework/experimental/utils/nougat_preprocessing/preprocess.py
--rw-r--r--   0        0        0     5118 2024-04-18 15:27:55.765727 celi_framework-0.0.10/celi_framework/experimental/utils/nougat_preprocessing/preprocessing_templates.py
--rw-r--r--   0        0        0     5458 2024-04-18 15:27:55.765727 celi_framework-0.0.10/celi_framework/experimental/utils/postprocessor_utils.py
--rw-r--r--   0        0        0     9091 2024-04-18 15:27:55.765727 celi_framework-0.0.10/celi_framework/experimental/utils/synthetic_data.py
--rw-r--r--   0        0        0     1350 2024-04-18 15:27:55.765727 celi_framework-0.0.10/celi_framework/logging_config.json
--rw-r--r--   0        0        0     2171 2024-04-18 15:27:55.765727 celi_framework-0.0.10/celi_framework/logging_setup.py
--rw-r--r--   0        0        0     6089 2024-04-18 15:27:55.765727 celi_framework-0.0.10/celi_framework/main.py
--rw-r--r--   0        0        0        0 2024-04-18 15:27:55.765727 celi_framework-0.0.10/celi_framework/utils/__init__.py
--rw-r--r--   0        0        0    10889 2024-04-18 15:27:55.765727 celi_framework-0.0.10/celi_framework/utils/codex.py
--rw-r--r--   0        0        0      461 2024-04-18 15:27:55.765727 celi_framework-0.0.10/celi_framework/utils/exceptions.py
--rw-r--r--   0        0        0    22485 2024-04-18 15:27:55.765727 celi_framework-0.0.10/celi_framework/utils/llmcore_utils.py
--rw-r--r--   0        0        0    10021 2024-04-18 15:27:55.765727 celi_framework-0.0.10/celi_framework/utils/llms.py
--rw-r--r--   0        0        0       77 2024-04-18 15:27:55.765727 celi_framework-0.0.10/celi_framework/utils/log.py
--rw-r--r--   0        0        0    10717 2024-04-18 15:27:55.765727 celi_framework-0.0.10/celi_framework/utils/sql_utils.py
--rw-r--r--   0        0        0    10871 2024-04-18 15:27:55.765727 celi_framework-0.0.10/celi_framework/utils/token_counters.py
--rw-r--r--   0        0        0    28482 2024-04-18 15:27:55.765727 celi_framework-0.0.10/celi_framework/utils/utils.py
--rw-r--r--   0        0        0     1690 2024-04-18 15:28:23.989944 celi_framework-0.0.10/pyproject.toml
--rw-r--r--   0        0        0    23331 1970-01-01 00:00:00.000000 celi_framework-0.0.10/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-07 21:41:32.138843 celi_framework-0.0.9/LICENSE
+-rw-r--r--   0        0        0    12947 2024-04-07 21:41:32.138843 celi_framework-0.0.9/README.md
+-rw-r--r--   0        0        0    10413 2024-04-07 21:41:32.138843 celi_framework-0.0.9/celi_framework/core/job_description.py
+-rw-r--r--   0        0        0    22894 2024-04-07 21:41:32.138843 celi_framework-0.0.9/celi_framework/core/monitor.py
+-rw-r--r--   0        0        0    11347 2024-04-07 21:41:32.138843 celi_framework-0.0.9/celi_framework/core/mt_factory.py
+-rw-r--r--   0        0        0    14719 2024-04-07 21:41:32.138843 celi_framework-0.0.9/celi_framework/core/post-monitor.py
+-rw-r--r--   0        0        0    59101 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/core/processor.py
+-rw-r--r--   0        0        0     3060 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/core/runner.py
+-rw-r--r--   0        0        0    21364 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/core/templates.py
+-rw-r--r--   0        0        0    17308 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/examples/study_report/template.py
+-rw-r--r--   0        0        0     9581 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/examples/study_report/tools.py
+-rw-r--r--   0        0        0     6133 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/examples/wikipedia/Index_cache.py
+-rw-r--r--   0        0        0     7692 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/examples/wikipedia/caching_beautiful_soup_reader.py
+-rw-r--r--   0        0        0     5552 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/examples/wikipedia/eval/run_eval.py
+-rw-r--r--   0        0        0      530 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/examples/wikipedia/eval/test_sets.json
+-rw-r--r--   0        0        0      851 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/examples/wikipedia/eval/test_sets_large.json
+-rw-r--r--   0        0        0      161 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/examples/wikipedia/example_config.json
+-rw-r--r--   0        0        0    13742 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/examples/wikipedia/index.py
+-rw-r--r--   0        0        0    13330 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/examples/wikipedia/job_description.py
+-rw-r--r--   0        0        0     7111 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/examples/wikipedia/loader.py
+-rw-r--r--   0        0        0    14745 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/examples/wikipedia/tools.py
+-rw-r--r--   0        0        0      549 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/examples/wikipedia/wikipedia_utils.py
+-rw-r--r--   0        0        0    12668 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/experimental/embeddor.py
+-rw-r--r--   0        0        0     7936 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/experimental/mapper.py
+-rw-r--r--   0        0        0     1354 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/experimental/mechanic.py
+-rw-r--r--   0        0        0        0 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/experimental/preprocessing/__init__.py
+-rw-r--r--   0        0        0    23551 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/experimental/preprocessing/pre-processor.py
+-rw-r--r--   0        0        0       94 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/experimental/preprocessing/word_pdf_extractors/__init__.py
+-rw-r--r--   0        0        0     2056 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/experimental/preprocessing/word_pdf_extractors/extractor_helpers.py
+-rw-r--r--   0        0        0    10669 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/experimental/preprocessing/word_pdf_extractors/pdf_extractor.py
+-rw-r--r--   0        0        0     7835 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/experimental/preprocessing/word_pdf_extractors/word_extractor.py
+-rw-r--r--   0        0        0     5479 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/experimental/task_builder/factory.py
+-rw-r--r--   0        0        0     4174 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/experimental/task_builder/llm_helper_funcs.py
+-rw-r--r--   0        0        0     4141 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/experimental/task_builder/llms.py
+-rw-r--r--   0        0        0     5930 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/experimental/task_builder/template.py
+-rw-r--r--   0        0        0     9886 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/experimental/utils/ada.py
+-rw-r--r--   0        0        0    19026 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/experimental/utils/mapper_utils.py
+-rw-r--r--   0        0        0    13615 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/experimental/utils/nougat_preprocessing/preprocess.py
+-rw-r--r--   0        0        0     5118 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/experimental/utils/nougat_preprocessing/preprocessing_templates.py
+-rw-r--r--   0        0        0     5458 2024-04-07 21:41:32.142843 celi_framework-0.0.9/celi_framework/experimental/utils/postprocessor_utils.py
+-rw-r--r--   0        0        0     9091 2024-04-07 21:41:32.146843 celi_framework-0.0.9/celi_framework/experimental/utils/synthetic_data.py
+-rw-r--r--   0        0        0     1350 2024-04-07 21:41:32.146843 celi_framework-0.0.9/celi_framework/logging_config.json
+-rw-r--r--   0        0        0     2171 2024-04-07 21:41:32.146843 celi_framework-0.0.9/celi_framework/logging_setup.py
+-rw-r--r--   0        0        0     6058 2024-04-07 21:41:32.146843 celi_framework-0.0.9/celi_framework/main.py
+-rw-r--r--   0        0        0        0 2024-04-07 21:41:32.146843 celi_framework-0.0.9/celi_framework/utils/__init__.py
+-rw-r--r--   0        0        0    10889 2024-04-07 21:41:32.146843 celi_framework-0.0.9/celi_framework/utils/codex.py
+-rw-r--r--   0        0        0      461 2024-04-07 21:41:32.146843 celi_framework-0.0.9/celi_framework/utils/exceptions.py
+-rw-r--r--   0        0        0    22402 2024-04-07 21:41:32.146843 celi_framework-0.0.9/celi_framework/utils/llmcore_utils.py
+-rw-r--r--   0        0        0     9894 2024-04-07 21:41:32.146843 celi_framework-0.0.9/celi_framework/utils/llms.py
+-rw-r--r--   0        0        0       77 2024-04-07 21:41:32.146843 celi_framework-0.0.9/celi_framework/utils/log.py
+-rw-r--r--   0        0        0    10717 2024-04-07 21:41:32.146843 celi_framework-0.0.9/celi_framework/utils/sql_utils.py
+-rw-r--r--   0        0        0    10802 2024-04-07 21:41:32.146843 celi_framework-0.0.9/celi_framework/utils/token_counters.py
+-rw-r--r--   0        0        0    28412 2024-04-07 21:41:32.146843 celi_framework-0.0.9/celi_framework/utils/utils.py
+-rw-r--r--   0        0        0     1211 2024-04-07 21:42:20.450887 celi_framework-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    14257 1970-01-01 00:00:00.000000 celi_framework-0.0.9/PKG-INFO
```

### Comparing `celi_framework-0.0.10/celi_framework/core/job_description.py` & `celi_framework-0.0.9/celi_framework/core/job_description.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 
 
 class Task(BaseModel):
     task_name: str
     details: Dict[str, str | List[str] | Dict[str, Any]]
 
     def with_references_resolved(self, task_numbering: Dict[str, str]) -> Task:
-        """Update references in each field and generates a new Task with references replaced."""
-
+        """Update references in each field, and generate a new Task with references replace."""
         updated_fields = {
             field: self._update_references(getattr(self, field), task_numbering)
             for field in self.model_fields
         }
         return type(self)(**updated_fields)  # type: ignore
 
     def _update_references(self, item: Any, task_numbering: Dict[str, str]):
@@ -70,15 +69,14 @@
         Returns concatenated text from the specified sections of the documents.
         If there is no content for the section, <empty section> will be returned.
 
         If the response contains "Error:", then there was a problem with the function call.
 
         Args:
             sections_dict_str (str): A JSON string mapping document names to their respective section numbers.  The json string will have the documents and sections in a dictionary.  The sections values should correspond to an entry in the table of contents for the specified document.
-
         '''
     """
 
     @abstractmethod
     def get_schema(self) -> Dict[str, str]:
         "This function returns a dictionary describing the document sections.  The processor will work through the sections, completing the defined tasks for each section.  Each dictionary can have any string values, but it is intended to be a section number followed by a section name."
         pass
@@ -95,15 +93,15 @@
     - `context`: Establishes the theme of "Interactive Data Collection," indicating a focus on user engagement and data-driven task generation for document drafting.
     - `task_list`: A comprehensive collection of tasks, each defined with a unique task name, a brief description, specific instructions, and examples. These tasks form the backbone of the document drafting process, guiding users or AI agents through each step required to compile a thorough and accurate document.
     - `general_comments` and `user_message`: Provide overarching guidance and specific instructions to users or AI agents undertaking the drafting tasks. These sections ensure that the drafting process is approached systematically, with clear expectations for each task's completion.
     - `pre_algo_instruct` and `post_algo_instruct`: Introductory and concluding instructions that frame the drafting tasks within a broader context, helping to orient the user or AI agent to the document's overall structure and objectives.
     - `config`: A dictionary consolidating all elements of the configuration, including the role of the user or AI agent, the context for the drafting tasks, and the structure of the task list. Additional parameters like `include_prerequisites` and `final_output_task` further customize the drafting guidance provided by the `MasterTemplateFactory`.
 
     Usage:
-    This configuration file is intended for use with the `MasterTemplateFactory` class to generate dynamic, structured instructions for drafting or analyzing documents. By defining tasks, prerequisites, and contextual guidance, it enables the automated creation of detailed documents across a variety of fields, including but not limited to technical documentation, and research reporting.
+    This configuration file is intended for use with the `MasterTemplateFactory` class to generate dynamic, structured instructions for drafting or analyzing documents. By defining tasks, prerequisites, and contextual guidance, it enables the automated creation of detailed documents across a variety of fields, including but not limited to medical writing, technical documentation, and research reporting.
 
     Example Usage:
     The configuration is dynamically loaded by the `MasterTemplateFactory` to create a tailored set of instructions and tasks based on the specific requirements of the document being drafted. The factory class utilizes the `task_list` to generate a step-by-step guide for users or AI agents, incorporating `general_comments` and `user_message` to provide additional context and clarity.
 
     By structuring the document drafting process around this configuration, the `MasterTemplateFactory` ensures that each section of the document is developed with precision, adhering to the required standards and content specifications outlined in the `task_library`.
     """
```

### Comparing `celi_framework-0.0.10/celi_framework/core/monitor.py` & `celi_framework-0.0.9/celi_framework/core/monitor.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 import json
 import time
 import queue
 from contextlib import contextmanager
 from celi_framework.core.templates import (
     make_prompt_for_secondary_analysis,
     make_prompt_for_function_call_analysis,
-    # make_prompt_for_third_analysis,
+    make_prompt_for_third_analysis,
 )
 from celi_framework.utils.exceptions import ContextLengthExceededException
 from celi_framework.utils.llms import quick_ask
 from celi_framework.utils.token_counters import TokenCounter
 from celi_framework.utils.llmcore_utils import SecondaryAnalysisReport, parse
 from celi_framework.utils.log import app_logger
 
@@ -161,36 +161,36 @@
                     print("pop_context_triggered received in Monitor")
                     # Trigger the poll_log_file logic when pop_context is called
                     # self.poll_log_file() # TODO -> Comment back in when ready
             except queue.Empty:
                 time.sleep(0.1)
 
     def analyze_prompt_completions(self, document_id):
+        """
+        Analyzes the quality of prompt completions based on the document ID. This method fetches the document
+        associated with the given ID from MongoDB, evaluates its content using secondary analysis, and updates
+        the system based on the findings.
+
+        The analysis may involve checking the completion against quality criteria, extracting insights using
+        AI models, and determining if any adjustments to the process or content are necessary. The method may
+        also flag documents for review, trigger alerts for significant issues, or recommend specific actions
+        to improve task performance and completion quality.
+
+        Args:
+            document_id (str): The unique identifier of the document to be analyzed, typically representing
+                               a prompt completion or related output from the `ProcessRunner`.
+
+        The outcomes of this analysis contribute to continuous improvement efforts, informing decisions on
+        prompt adjustments, process refinements, and strategic planning for future tasks. It underscores the
+        `MonitoringAgent`'s role in ensuring high-quality outputs through proactive and data-driven oversight.
+        """
+
         doc = self.codex.get_document_by_id(
             document_id=document_id, collection_name="process_executions"
         )
-        # """
-        # Analyzes the quality of prompt completions based on the document ID. This method fetches the document
-        # associated with the given ID from MongoDB, evaluates its content using secondary analysis, and updates
-        # the system based on the findings.
-
-        # The analysis may involve checking the completion against quality criteria, extracting insights using
-        # AI models, and determining if any adjustments to the process or content are necessary. The method may
-        # also flag documents for review, trigger alerts for significant issues, or recommend specific actions
-        # to improve task performance and completion quality.
-
-        # Args:
-        #     document_id (str): The unique identifier of the document to be analyzed, typically representing
-        #                        a prompt completion or related output from the `ProcessRunner`.
-
-        # The outcomes of this analysis contribute to continuous improvement efforts, informing decisions on
-        # prompt adjustments, process refinements, and strategic planning for future tasks. It underscores the
-        # `MonitoringAgent`'s role in ensuring high-quality outputs through proactive and data-driven oversight.
-        # """
-
         if not doc:
             app_logger.error(
                 f"Document with ID {document_id} not found.", extra={"color": "red"}
             )
             return
 
         prompt_exception = doc.get("prompt_exception", True)
@@ -299,95 +299,95 @@
             except Exception as e:
                 app_logger.error(
                     f"Failed to update document {document_id} with analysis report: {e}"
                 )
         else:
             app_logger.error("No response received from secondary analysis.")
 
-    # def periodic_review_with_third_llm(self):
-    #     """
-    #     Conducts periodic reviews of the chat interactions using a tertiary language model (LLM) to gain additional insights
-    #     and identify opportunities for improvements in the process. This method is designed to leverage a more advanced or
-    #     differently specialized LLM to analyze the accumulated chat history, evaluate the effectiveness of interactions,
-    #     and suggest modifications to the prompts or the drafting strategy.
-    #
-    #     The review process involves constructing a comprehensive prompt that summarizes the ongoing chat or highlights
-    #     specific areas of concern, then submitting this prompt to the tertiary LLM. The response from this LLM is analyzed
-    #     to extract actionable insights, such as recommendations for changing prompts, adjusting the conversation flow,
-    #     or addressing identified issues directly within the chat content.
-    #
-    #     This method allows the `MonitoringAgent` to implement a layered analysis sapproach, where multiple models contribute
-    #     to a deeper understanding and continuous refinement of the process. It underscores the system's capability for
-    #     self-improvement and adaptation, ensuring that the drafting process remains aligned with quality standards and
-    #     efficiency goals.
-    #
-    #     Returns:
-    #         None. The primary outcome of this method is the application of insights gained from the tertiary LLM analysis
-    #         to the monitoring and adjustment strategies. Any specific actions taken as a result of the review are handled
-    #         internally and reflected in the operational adjustments or recommendations provided to the `ProcessRunner`.
-    #
-    #     This method plays a critical role in maintaining a high standard of quality and efficiency in the automated drafting
-    #     process. By periodically reviewing the interaction history with an advanced analytical perspective, the
-    #     `MonitoringAgent` ensures that the system's performance evolves in response to both explicit feedback and
-    #     nuanced insights derived from AI-driven analysis.
-    #     """
-    #
-    #     # TODO -> Just testing that I can pass through the info - will uncomment and activate
-    #     # Use quick_ask for periodic review with the third LLM
-    #     secondary_ongoing_chat = copy.deepcopy(self.secondary_ongoing_chat)
-    #
-    #     prompt = make_prompt_for_third_analysis(
-    #         secondary_ongoing_chat
-    #     )  # TODO -> Create prompt func
-    #     prompt = secondary_ongoing_chat + " json"
-    #     # response_str = quick_ask(prompt, token_counter, json_output=True)
-    #     response_str = prompt
-    #     app_logger.info(
-    #         f"Response from quick ask: {response_str}", extra={"color": "blue"}
-    #     )
-    #
-    #     response_str = {}
-    #     response_str["response"] = prompt
-    #     response_str = str(response_str)
-    #
-    #     print("throughput of periodic_review_with_third_llm")
-    #     print(secondary_ongoing_chat)
-    #
-    #     try:
-    #         response = (
-    #             json.loads(response_str)
-    #             if isinstance(response_str, str)
-    #             else response_str
-    #         )
-    #     except json.JSONDecodeError:
-    #         err_msg = (
-    #             f"Error parsing response for quick ask json response: {response_str}"
-    #         )
-    #         prmpt_msg = f"Prompt was: \n{prompt}"
-    #         response = f"{err_msg}\n{prmpt_msg}"
-    #         app_logger.error("periodic_review_with_third_llm")
-    #         app_logger.error(response)
-    #
-    #     # To be uncommented
-    #     # logger.info(f"Decoded response from quick ask: {response}", extra={'color': 'blue'})
-    #
-    #     # Use the third LLM to analyze secondary_ongoing_chat
-    #     # Process the decision, e.g., stop the process_runner if needed
-    #     def enqueue_decision_based_on_analysis(self, analysis_result):
-    #         if "stop" in analysis_result.lower():
-    #             self.update_queue.put({"command": "stop"})
-    #             # Add logic here
-    #         elif "make_prompt" in analysis_result.lower():
-    #             # Assuming the analysis result contains the new prompt information
-    #             self.update_queue.put(
-    #                 {"command": "make_prompt", "data": analysis_result}
-    #             )
-    #             # Add logic here
-    #
-    #     # make_decision_based_on_chat(response)  # TBD
+    def periodic_review_with_third_llm(self):
+        """
+        Conducts periodic reviews of the chat interactions using a tertiary language model (LLM) to gain additional insights
+        and identify opportunities for improvements in the process. This method is designed to leverage a more advanced or
+        differently specialized LLM to analyze the accumulated chat history, evaluate the effectiveness of interactions,
+        and suggest modifications to the prompts or the drafting strategy.
+
+        The review process involves constructing a comprehensive prompt that summarizes the ongoing chat or highlights
+        specific areas of concern, then submitting this prompt to the tertiary LLM. The response from this LLM is analyzed
+        to extract actionable insights, such as recommendations for changing prompts, adjusting the conversation flow,
+        or addressing identified issues directly within the chat content.
+
+        This method allows the `MonitoringAgent` to implement a layered analysis sapproach, where multiple models contribute
+        to a deeper understanding and continuous refinement of the process. It underscores the system's capability for
+        self-improvement and adaptation, ensuring that the drafting process remains aligned with quality standards and
+        efficiency goals.
+
+        Returns:
+            None. The primary outcome of this method is the application of insights gained from the tertiary LLM analysis
+            to the monitoring and adjustment strategies. Any specific actions taken as a result of the review are handled
+            internally and reflected in the operational adjustments or recommendations provided to the `ProcessRunner`.
+
+        This method plays a critical role in maintaining a high standard of quality and efficiency in the automated drafting
+        process. By periodically reviewing the interaction history with an advanced analytical perspective, the
+        `MonitoringAgent` ensures that the system's performance evolves in response to both explicit feedback and
+        nuanced insights derived from AI-driven analysis.
+        """
+
+        # TODO -> Just testing that I can pass through the info - will uncomment and activate
+        # Use quick_ask for periodic review with the third LLM
+        secondary_ongoing_chat = copy.deepcopy(self.secondary_ongoing_chat)
+
+        prompt = make_prompt_for_third_analysis(
+            secondary_ongoing_chat
+        )  # TODO -> Create prompt func
+        prompt = secondary_ongoing_chat + " json"
+        # response_str = quick_ask(prompt, token_counter, json_output=True)
+        response_str = prompt
+        app_logger.info(
+            f"Response from quick ask: {response_str}", extra={"color": "blue"}
+        )
+
+        response_str = {}
+        response_str["response"] = prompt
+        response_str = str(response_str)
+
+        print("throughput of periodic_review_with_third_llm")
+        print(secondary_ongoing_chat)
+
+        try:
+            response = (
+                json.loads(response_str)
+                if isinstance(response_str, str)
+                else response_str
+            )
+        except json.JSONDecodeError:
+            err_msg = (
+                f"Error parsing response for quick ask json response: {response_str}"
+            )
+            prmpt_msg = f"Prompt was: \n{prompt}"
+            response = f"{err_msg}\n{prmpt_msg}"
+            app_logger.error("periodic_review_with_third_llm")
+            app_logger.error(response)
+
+        # To be uncommented
+        # logger.info(f"Decoded response from quick ask: {response}", extra={'color': 'blue'})
+
+        # Use the third LLM to analyze secondary_ongoing_chat
+        # Process the decision, e.g., stop the process_runner if needed
+        def enqueue_decision_based_on_analysis(self, analysis_result):
+            if "stop" in analysis_result.lower():
+                self.update_queue.put({"command": "stop"})
+                # Add logic here
+            elif "make_prompt" in analysis_result.lower():
+                # Assuming the analysis result contains the new prompt information
+                self.update_queue.put(
+                    {"command": "make_prompt", "data": analysis_result}
+                )
+                # Add logic here
+
+        # make_decision_based_on_chat(response)  # TBD
 
     def read_log_file(self, file_path):
         """
         Reads the entire log file.
 
         Args:
             file_path (str): The path to the log file.
```

### Comparing `celi_framework-0.0.10/celi_framework/core/mt_factory.py` & `celi_framework-0.0.9/celi_framework/core/mt_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 class MasterTemplateFactory:
     """
     A versatile factory class for generating structured instructions and tasks applicable to various
     document drafting or analytical processes. It abstracts the complexity of document planning into
     actionable, step-by-step guides, making it a valuable asset for automating document creation across
-    different fields.
+    different fields, including but not limited to medical writing.
 
     Attributes:
         config (dict): Configuration details including user roles, drafting contexts, and specific task lists.
         schema (dict): The schema or structural blueprint of the document to be created or analyzed.
         role (str): The intended role of the user or system utilizing the generated instructions,
                     allowing for tailored guidance.
         context (str): The overarching context or scope of the document-related tasks, ensuring
```

### Comparing `celi_framework-0.0.10/celi_framework/core/post_monitor.py` & `celi_framework-0.0.9/celi_framework/core/post-monitor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.10/celi_framework/core/processor.py` & `celi_framework-0.0.9/celi_framework/core/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -464,18 +464,18 @@
     def generate_document_ids(self, timestamp, task_list):
         """
         Generates a set of unique identifiers for a new document based on the current timestamp and task list.
         These identifiers are used to uniquely tag and track the document within the MongoDB database,
         ensuring accurate versioning and retrieval.
 
         The method produces three types of IDs:
-            1. A unique document ID that represents the specific interaction instance.
-            2. A prompt ID that identifies the set of prompts leading up to the current interaction.
-            3. A task-specific ID that links the document to a specific task within the process,
-                facilitating task-level tracking and analysis.
+        1. A unique document ID that represents the specific interaction instance.
+        2. A prompt ID that identifies the set of prompts leading up to the current interaction.
+        3. A task-specific ID that links the document to a specific task within the process,
+           facilitating task-level tracking and analysis.
 
         Args:
             timestamp (str): A string representation of the current timestamp, used for generating time-based unique IDs.
             task_list (list): A list of tasks that have been processed or are in processing, contributing to the context of the document.
 
         Returns:
             tuple: Contains three strings representing the unique document ID, prompt ID, and task-specific ID, respectively.
@@ -626,20 +626,20 @@
     def run(self):
         """
         Initiates and manages the main execution loop for drafting documents. This loop continues
         until the `keep_running` flag is set to False, indicating a request to terminate the process, either due to
         completion of all tasks or an external command to halt operations.
 
         Within each iteration of the loop, the method performs the following operations:
-            - Generates task instructions based on the current state and configuration.
-            - Retrieves a response from the language model using the current task instructions and context.
-            - Processes the language model's response, including handling any specified function calls, updating
-                the draft content, and managing the ongoing conversation context.
-            - Checks for token usage limits to ensure compliance with predefined constraints.
-            - Updates internal state and prepares for the next iteration or termination of the process.
+        - Generates task instructions based on the current state and configuration.
+        - Retrieves a response from the language model using the current task instructions and context.
+        - Processes the language model's response, including handling any specified function calls, updating
+          the draft content, and managing the ongoing conversation context.
+        - Checks for token usage limits to ensure compliance with predefined constraints.
+        - Updates internal state and prepares for the next iteration or termination of the process.
 
         The method ensures that each task is processed in accordance with the system's operational logic,
         leveraging the language model's capabilities for content generation and refinement. It maintains
         responsive interaction with the language model, adapting to its feedback and instructions to
         dynamically guide the drafting process.
 
         No parameters are required for this method, as it operates based on the class's internal state
@@ -819,16 +819,16 @@
         """
 
         app_logger.warning(
             "No message was returned and no function was called.",
             extra={"color": "red"},
         )
         return (
-            "\n\nNo message was returned from you (the writer) and no function was called.\n"
-            "As a writer, explain in detail what you want to do next."
+            "\n\nNo message was returned from you (the medical writer) and no function was called.\n"
+            "As a medical writer, explain in detail what you want to do next."
         )
 
     def handle_message_returned(self, message):
         """
         Processes and integrates the message content returned from the language model into the drafting process.
         This method is called when the language model provides actionable content or instructions within its response.
 
@@ -845,15 +845,15 @@
                  the draft document. This includes any modifications or annotations added to the original message
                  to enhance its clarity or utility.
 
         By effectively interpreting and utilizing the content provided by the language model, this method plays a
         key role in maintaining the momentum of the drafting process and ensuring that each response contributes
         towards the completion of the document.
         """
-        return f"\nPrior message from you (the writer): \n{message}"
+        return f"\nPrior message from you (the medical writer): \n{message}"
 
     def handle_function_call(self, response):
         """
         Executes specific function calls embedded within the language model's response. This method is critical
         for handling responses that contain instructions for actions beyond simple text generation, such as
         retrieving additional data, performing analysis, or modifying the draft content in a particular manner.
```

### Comparing `celi_framework-0.0.10/celi_framework/core/runner.py` & `celi_framework-0.0.9/celi_framework/core/runner.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.10/celi_framework/core/templates.py` & `celi_framework-0.0.9/celi_framework/core/templates.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,32 @@
 """
-The `templates` module provides a collection of functions designed for generating structured prompts
-and processing text data to facilitate various tasks such as document section cleanup, content analysis,
-and preparation for embedding and retrieval processes.
-
-Before the introduction of TemplateFactories, prompts were formatted and augmented with content using these
-prompt templates. While TemplateFactories offer a more dynamic and modular approach for managing templates,
-in certain scenarios, especially those involving tool calls to Large Language Models (LLMs) that require prompt
-templating, using prompt templates directly may still be convenient. This module includes examples of such templates.
-
-This module is part of a broader system aimed at automating the drafting and analysis of documents using
-language models.
+This module, `templates.templates`, currently serves as a repository for various templating functions used in the
+processing and analysis of study documents. These functions are designed to generate structured prompts
+and process text data, facilitating tasks such as cleaning up document sections, analyzing content for essential
+information, and setting up data for embedding and retrieval.
+
+However, it's important to note that this module is in the process of being deprecated. The introduction of
+TemplateFactories represents a strategic shift towards a more modular and flexible approach to handle templating needs.
+TemplateFactories will offer enhanced capabilities for dynamic template generation and management, thereby
+streamlining the overall process and reducing the reliance on hardcoded template functions.
+
+
+TODOs for Module Refactoring and Transition:
+- TODO: Assess and document the current functionalities that need to be transitioned to TemplateFactories.
+- TODO: Develop a migration plan for existing template functions to the new TemplateFactory approach.
+- TODO: Implement a deprecation warning system within the module to inform users of the upcoming changes.
+- TODO: Ensure backward compatibility where necessary during the transition phase.
+- TODO: Create a comprehensive documentation guide for the new TemplateFactories to facilitate a smooth transition for existing users.
 """
 
 from celi_framework.utils.utils import remove_text_chunk
 from celi_framework.utils.log import app_logger
 
 
 def make_cleanup_dict_prompt_template(section_content, section_heading, schema_dict):
-    """
-    Generates a prompt template for cleaning up and processing a document section's text to be suitable for sentence
-    embeddings. This template guides the analysis of document sections extracted from a mix of formats like Microsoft
-    Word and Markdown. It aims to determine if the section's content holds standalone informational value and instructs
-    on cleaning up the text while preserving the original wording as much as possible.
-
-    The template asks for the text to be analyzed within the context of the document's schema, identifying meaningful
-    content, and returning cleaned text or reasons to skip the section if it does not contain standalone information
-    or is erroneous.
-
-    Parameters:
-        section_content (str): The text of the document section to be analyzed and cleaned.
-        section_heading (str): The heading of the document section under analysis.
-        schema_dict (dict): A dictionary representing the schema or index of the study for contextual understanding.
-
-    Returns:
-        str: A formatted prompt that outlines instructions for analyzing and cleaning the section's text,
-             including handling tables and ensuring all lines are sentence-embedded ready.
-    """
-
     formatted_prompt = f"""
 
     You are analyzing a section of a scientific document.
 
     Here is the index of the study for context:
     {schema_dict}
 
@@ -86,32 +72,14 @@
 
     Analysis result (in json format):
     """
     return formatted_prompt
 
 
 def create_prompt_for_essential_section_analysis(section_content):
-    """
-    Constructs a prompt template for calling a Large Language Model (LLM) directly to determine if potential
-    source materials are indeed essential for drafting a specific document section. This template helps in identifying
-    the reference materials and guidelines necessary to create or analyze the content of a document section.
-
-    The function dynamically generates instructions based on the provided document content, including analyzing sections
-    from reference materials with minor edits and formatting, to determine their essentiality for drafting.
-
-    Parameters:
-        section_content (dict): A dictionary containing the content of the document section, reference materials,
-                                 and guidelines for analysis.
-
-    Returns:
-        str: A formatted prompt for essential source material analysis, which includes analyzing the given document
-             section in the context of provided reference materials and guidelines, and instructing on returning a JSON
-             object indicating essential sections.
-    """
-
     app_logger.info(
         "Drafting instructions to identify essential source materials...",
         extra={"color": "brown"},
     )
     if len(section_content["Document"]) > 0:
         # Ensure additional document contents are initialized if not provided
         section_content["Reference Material"] = section_content.get(
@@ -158,31 +126,14 @@
         app_logger.info(f"{formatted_prompt}", extra={"color": "green"})
         return formatted_prompt
     else:
         return "No document content provided. Skip."
 
 
 def make_draft_setting_output_prompt(content):
-    """
-    Creates a prompt instructing on formatting draft content into a specified JSON structure with additional information.
-    This function is designed for scenarios where draft content needs to be formatted in a JSON object that includes
-    headings, draft text, comments, success flags, source mappings, tables, figures, cross-references, and scope of the
-    section, among other details.
-
-    It emphasizes not changing the original wording or naming conventions and ensuring that the text is unchanged as much
-    as possible, making it suitable for embedding retrieval and further processing.
-
-    Parameters:
-        content (str): The draft content to be formatted into the structured JSON format.
-
-    Returns:
-        str: A template providing detailed instructions on how to format the provided content into the structured JSON
-             format required for the document drafting process.
-    """
-
     template = f"""
     Take the "content" below and format it into a json with the following format.
     DO NOT CHANGE THE WORDING OR NAMING CONVENTIONS. KEEP AS MUCH OF THE TEXT UNCHANGED AS POSSIBLE.
     
     Content:
     {content}
     
@@ -211,31 +162,16 @@
     
     Return:
 
     """
 
     return template
 
-def make_table_setting_output_prompt(json_content):
-    """
-    Generates a prompt for formatting content related to tables and figures into a structured JSON object. This prompt
-    is tailored for extracting and organizing information from tables and figures in the source document, ensuring
-    that each table or figure is accurately represented and referenced in the final document draft.
-
-    The prompt guides the user through formatting the content, emphasizing the preservation of headings and numbering
-    as they appear in the source document for clarity and accuracy in referencing.
-
-    Parameters:
-        json_content (str): The content to be formatted, focusing on tables and figures extracted from the document.
-
-    Returns:
-        str: A detailed prompt that outlines the expected JSON structure for organizing and referencing tables and figures,
-             aiding in the accurate representation of such content in the document drafting process.
-    """
 
+def make_table_setting_output_prompt(json_content):
     template = f"""
     Take the content below and format it into a json with the format in the following example.
     FILL IN THE TABLE/FIGURE HEADING WHERE IT SAYS "HEADING HERE", USE THE TABLE/FIGURE NUMBER AS IT IS IN THE SOURCE
     DOCUMENT.
     
     Example Return:
     {{"9.3.2":
@@ -265,36 +201,17 @@
     {json_content}
     """
 
     return template
 
 
 # TODO -> Add user message
-def make_prompt_for_secondary_analysis(system_message, ongoing_chat, prompt_completion, response):
-    """
-    Generates a prompt for secondary analysis to evaluate the outcomes of function calls made to a Large Language
-    Model (LLM). This analysis focuses on assessing the function call's relevance, accuracy, completeness, clarity,
-    integration, and contextual sufficiency based on the context of the request, the function's intended action,
-    its actual output, and handling of exceptions or errors.
-
-    This template assists in providing detailed feedback and actionable suggestions for improvement, particularly
-    in refining the execution of function calls and leveraging the cumulative context of ongoing chats more effectively.
-
-    Parameters:
-        system_message (str): The initial system message or instruction leading to the function call.
-        ongoing_chat (str): The cumulative context of all interactions prior to this function call.
-        function_name (str): The name of the executed function.
-        function_arguments (str): The arguments supplied to the function call.
-        prompt_completion (str): The output returned from the function call, including successful results or error messages.
-
-    Returns:
-        str: A structured prompt designed for secondary analysis of function call outcomes, emphasizing critical
-             evaluation and recommendations for improving task instructions and function execution.
-    """
-
+def make_prompt_for_secondary_analysis(
+    system_message, ongoing_chat, prompt_completion, response
+):
     prior_ongoing_chat = remove_text_chunk(ongoing_chat, prompt_completion)
     template = f"""
 Evaluate the language model's task completion for drafting sections of a [DOC TYPE], 
 considering both the immediate response and its integration with the cumulative context of the ongoing chat.
  This template facilitates a comprehensive assessment, feedback provision, and actionable improvement suggestions.
  Keep in mind that every prompt completion will be appended to the ongoing chat, so tasks that are sequentially after
  the current prompt will have not only the current prompt completion's output but all the previous ones too. Therefore,
@@ -444,31 +361,131 @@
        - **For Future Tasks**: Strategies for the model to enhance understanding and execution of function calls by leveraging the context more effectively.
 
     **Feedback Loop for Model Improvement**:
     - Suggest ways the model could improve its handling of function calls, focusing on context understanding, accuracy, and clarity.
     """
     return template
 
-def make_toc_prompt(pdf_extract):
-    """
-    Creates a prompt for identifying headings and subheadings from a text extract of a PDF document. The goal is to
-    analyze the extract for document structure, including section numbers, names, and corresponding page numbers,
-    and to format this information into a structured JSON object.
 
-    This prompt aids in organizing and structuring content from PDF documents, making it more accessible and easier
-    to reference in subsequent document processing and drafting tasks.
+def make_prompt_for_third_analysis():
+    print(
+        "TBD THIRD ANALYSIS TEMPLATE <----------------------------------------------------------"
+    )
 
-    Parameters:
-        pdf_extract (str): The text extract from a PDF document, containing potential headings and subheadings.
 
-    Returns:
-        str: A prompt that guides the analysis of the PDF text extract for headings and subheadings, specifying how
-             to format the identified content into a JSON object for easier reference and organization.
+def make_toc_prompt_deprecated(pdf_extract):
+    prompt = f"""
+    Identify headings and subheadings in this text based on numbering and formatting (and pages). Print them out in a json using the formatting below (section number, section name, page number)..
+
+    Text:
+    {pdf_extract}
+
+    Response Example:
+      {{{{
+          "toc": [
+            {{{{
+              "section_number": 0,
+              "section_name": "Improving Image Generation with Better Captions",
+              "page_number": 1
+            }}}},
+            {{{{
+              "section_number": 1,
+              "section_name": "Abstract",
+              "page_number": 1
+            }}}},
+            {{{{
+              "section_number": 2,
+              "section_name": "Introduction",
+              "page_number": 2
+            }}}},
+            {{{{
+              "section_number": 3,
+              "section_name": "Dataset Recaptioning",
+              "page_number": 5
+            }}}},
+            {{{{
+              "section_number": "3.1",
+              "section_name": "Building an image captioner",
+              "page_number": 5
+            }}}},
+            {{{{
+              "section_number": "3.1.1",
+              "section_name": "Fine-tuning the captioner",
+              "page_number": 6
+            }}}},
+            {{{{
+              "section_number": 4,
+              "section_name": "Evaluating the re-captioned datasets",
+              "page_number": 7
+            }}}},
+            {{{{
+              "section_number": "4.1",
+              "section_name": "Blending synthetic and ground-truth captions",
+              "page_number": 7
+            }}}},
+            {{{{
+              "section_number": "4.2",
+              "section_name": "Evaluation methodology",
+              "page_number": 7
+            }}}},
+            {{{{
+              "section_number": "4.3",
+              "section_name": "Caption type results",
+              "page_number": 8
+            }}}},
+            {{{{
+              "section_number": "4.4",
+              "section_name": "Caption blending ratios",
+              "page_number": 8
+            }}}},
+            {{{{
+              "section_number": "4.5",
+              "section_name": "Practical usage of highly descriptive captions",
+              "page_number": 9
+            }}}},
+            {{{{
+              "section_number": 5,
+              "section_name": "DALL-E 3",
+              "page_number": 10
+            }}}},
+            {{{{
+              "section_number": 6,
+              "section_name": "Limitations & Risk",
+              "page_number": 13
+            }}}},
+            {{{{
+              "section_number": "6.1",
+              "section_name": "Spatial awareness",
+              "page_number": 13
+            }}}},
+            {{{{
+              "section_number": "6.2",
+              "section_name": "Text rendering",
+              "page_number": 13
+            }}}},
+            {{{{
+              "section_number": "6.3",
+              "section_name": "Specificity",
+              "page_number": 13
+            }}}},
+            {{{{
+              "section_number": "6.4",
+              "section_name": "Safety and bias mitigations",
+              "page_number": 13
+            }}}}
+          ]
+        }}}}
     """
+    return prompt
+
 
+def make_toc_prompt(pdf_extract):
+    """
+    Constructs a prompt to identify headings and subheadings from a PDF extract.
+    """
     prompt = f"""
     **Please identify the headings and subheadings from the following text based on numbering, formatting, and pages.**
     **Then, format your response as JSON with the following structure: section number, section name, and page number.**
 
     **Text Extract:**
     {pdf_extract}
```

### Comparing `celi_framework-0.0.10/celi_framework/examples/reporting_template/job_description.py` & `celi_framework-0.0.9/celi_framework/examples/wikipedia/job_description.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,245 +1,192 @@
-"""
-This module serves as a generic template. It is designed to be adaptable for
-a broad range of reports and is not specific to any particular field.
-The tasks, function calls, and methodologies described herein are intended to provide a foundational
-structure for document analysis and drafting, which can be customized to meet the needs of various
-reporting requirements.
-"""
-
 from celi_framework.core.job_description import JobDescription, Task
-from celi_framework.examples.reporting_template.tools import ReportingToolImplementations
+
+from celi_framework.examples.wikipedia.tools import WikipediaToolImplementations
 
 task_library = [
     Task(
         task_name="Search for Document Section Text",
         details={
-            "description": "Find and retrieve the text for a specific section within the document.",
+            "description": "Find the text of the current section and all subsections in the example document.",
             "prerequisite_tasks": [],
-            "function_call": "Perform a function call to retrieve the section's text.",
-            "example_call": "{{'Document': ['Section Identifier']}}",
+            "function_call": "Call get_example_toc to get the full list of sections in the example doc and then get_text_for_sections to retrieve the text for the current section and any relevant (sub)sections.",
+            "example_call": "{{'Example Document': ['1', '1.1', '1.2']}}",
             "instructions": [
-                "Ensure every section has corresponding text, noting empty sections without modification.",
-                "If encountering an error, attempt again with different parameters.",
+                "Every section should have corresponding text, even that text is blank. If you get an error, try again with different parameters",
+                "Do not truncate or modify the retrieved text.",
+                "If text is present, print the entire text and instruct to proceed to the next task.",
+                "If a given section is empty in the example document, then you can leave that section empty in the target. In that case, you can skip all the remaining tasks and jump straight to the 'Draft New Document Section' task, which can just draft an empty section. Note that a blank section is not the same as the function returning an error.",
             ],
         },
     ),
     Task(
         task_name="Understand Differentiation",
         details={
-            "description": "Analyze the context of the document's section by comparing it with similar sections.",
+            "description": "Understand the context of the example document section by comparing it with similar sections.  Also look at any subsections and understand how they are structured.",
             "prerequisite_tasks": ["Search for Document Section Text"],
             "instructions": [
-                "Identify similar sections within the document, retrieving their text for comparison.",
-                "Document the differences to ensure uniqueness and prevent duplication.",
+                "Identify other sections of the example document that may contain content similar to the current section.",
+                "Retrieve the text of these sections along with their section identifiers.",
+                "Analyze and note down how the current section differs from these sections to prevent duplication in future work.",
             ],
-            "example": {
-                "Example Section 1": "Example text...",
-                "Example Section 2": "Another example text...",
-            },
             "additional_notes": [
-                "Keep notes concise and relevant for future use.",
-            ],
-        },
-    ),
-    Task(
-        task_name="Redraft Section for Relevant Content",
-        details={
-            "description": "Review and adjust detailed content within the section for relevance and conciseness.",
-            "prerequisite_tasks": ["Search for Document Section Text"],
-            "instructions": [
-                "If the section focuses solely on the primary topic, proceed directly to the next task.",
-                "For sections including additional detailed content, summarize or omit as necessary while maintaining coherence.",
+                "Keep your notes concise and relevant for later use.",
+                "If 'no content present' is observed in all section bodies that are retrieved, even after retrieving children/sub-sections, proceed to the next task.",
+                "If it seems like the current section is specific to the example document, and would not make sense as part of the target document, feel free to skip the section and go on to the next one.  This can happen if the example contains a section highly specific to it's topic, but not relevant to the target document.",
             ],
-            "examples": {
-                "to_exclude": [
-                    "Example of detailed content to potentially exclude or summarize.",
-                ],
-                "not_to_exclude": [
-                    "Example of essential content to retain.",
-                ],
-            },
-        },
-    ),
-    Task(
-        task_name="Identify Document Source",
-        details={
-            "description": "Determine the source materials for the document's section.",
-            "function_call": "Call the source_materials_retrieval function.",
         },
     ),
     Task(
-        task_name="Find Essential Source Materials",
+        task_name="Find the most relevant references for the target section and all the subsections",
         details={
-            "description": "Prioritize the most critical source materials for drafting the document's section.",
-            "prerequisite_tasks": ["Identify Document Source"],
-            "task": "Organize these materials by relevance in a bulleted list.",
+            "description": """Call get_corresponding_target_references_for_example_sections function with a list of the current section and all subsections to retrieve these materials. to find relevant references for the target document that correspond to the example document sections you are looking at.
+            The references may not provide you with all the information you need to draft the section.  Don't worry, you will get a chance to ask additional questions in the next task.""",
+            "example_call": "['1', '1.1', '1.2']",
         },
     ),
     Task(
-        task_name="Get Source Table of Contents",
+        task_name="Ask additional questions",
         details={
-            "description": "Retrieve the Table of Contents (TOC) for essential source documents for the current section.",
-            "function_call": "Call get_source_tocs.",
-            "example_call": "{{'current_section': 'Section Identifier'}}",
-            "instructions": [
-                "Retrieve TOCs without modification, focusing on relevance to the current section.",
-            ],
+            "description": """Determine if any additional information is required to draft the section and call the ask_question_about_target function to gather that information.
+            Feel free to ask as many questions as you need and keep working on this task until you have the information you need.  This is especially important if
+            the initial references turn out not to be useful.
+            If you don't have any questions, just move on to the next section.""",
+            "example_call": '{"prompt": "What is unusual about when this band formed?"}',
         },
     ),
     Task(
-        task_name="Map Example Document Sources to New Source ToCs",
+        task_name="Define subsections for this section",
         details={
-            "description": "Align the example source document sections with the current document's sources.",
-            "prerequisite_tasks": ["Identify Document Source"],
-            "instructions": [
-                "For each of the example document's source sections find the sections in the new document's sources "
-                "that would have the most similar content thematically (not by document numbering).",
-            ],
-        },
-    ),
-    Task(
-        task_name="Handle Document Subsections",
-        details={
-            "description": "Identify subsections of the new document source sections that may be relevant as sources "
-                           "for the new document",
-            "prerequisite_tasks": ["Map Example Document Sources to New Source ToCs"],
-        },
-    ),
-    Task(
-        task_name="New Reference Material Retrieval",
-        details={
-            "description": "Retrieve text for new source sections identified as critical.",
-            "prerequisite_tasks": ["ap Example Document Sources to New Source ToCs"],
-            "function_call": "section_text_getter",
-            "example_call": "{{ 'New Document': ['Section Identifiers'], 'New Guidelines': ['Identifiers'] }}",
+            "description": """Define what subsections should be present within this individual section.  Use the table of contents from the example document and your knowledge of the target page to structure the subsections.  Keeep in mind over differentiation of this section from other sections in the document.  It is totally fine to not have subsections, especially if the example document does not have them.
+            Also, remember that the subsections should be relevant for the target document.  The detailed structure of subsections used in the example may not be relevant for our target document.""",
         },
     ),
     Task(
         task_name="Draft New Document Section",
         details={
-            "description": "Draft a new section analogous to the revised example section content (from {{TaskRef:Redraft Section for Relevant Content}} output), ensuring alignment with its structure, format, and scope (from {{TaskRef:Understand Differentiation}} output).",
+            "description": "Draft a new section analogous to the revised example section, ensuring alignment with its structure, format, and scope (from {{TaskRef:Understand Differentiation}} output).  Use the section structure you defined in {{TaskRef:Define subsections for this section}}. However, the details should be related to the target and not the example document.",
             "guidelines": [
+                "Clearly identify the section number and section heading/title at the top of the content.",
                 "The new section should have its unique scope and purpose, distinct from the example section.",
-                "Closely align with the example section's approach for consistency.",
                 "Avoid duplicating content or including redundant information.",
-                "Aim for the new section to mirror the example section in length and detail.",
+                "Aim for the new section to mirror the example section in length and detail, but using content related to the target.",
                 "Follow the instructions set out by {{TaskRef:Understand Differentiation}} output.",
-            ],
-            "prerequisite_tasks": "All prior tasks.",
-            "considerations": [
-                "What differentiates this section from other similar sections? Refer to the output of {{TaskRef:Understand Differentiation}}.",
-                "Concentrate on content relevant to the specific section within the broader document context.",
                 "Maintain consistency in documentation methodology, using the revised example as a template.",
-                "Ensure content is derived exclusively from the newly identified source materials.",
+                "Ensure content is exclusively about the target, and not the example topic.",
             ],
             "specific_instructions": [
                 "Do not copy text verbatim. Include only text within the scope of the current section, as highlighted in the output of {{TaskRef:Understand Differentiation}}.",
                 "Include cross-references to other sections as seen in the example if applicable.",
-                "Incorporate references to tables and sections within the new reference documents as appropriate, providing context to the study's methodology and decision-making processes.",
             ],
-            "note": "Focus on the specific section, considering its role within the parent sections and its relation to the revised example section. Utilize the guidance from {{TaskRef:Understand Differentiation}} for the scope of the section",
-        },
-    ),
-    Task(
-        task_name="Final Document Review",
-        details={
-            "description": "Review the final document and provide a PASS/FAIL decision based on the success criteria.",
-            "prerequisite_tasks": ["Draft New Document Section"],
-            "instructions": [
-                "Evaluate the success of the new section draft",
-                "Document the review outcome",
-                "Print the final review output.",
-            ],
-            "success_flag_criteria": {
-                "FAIL": [
-                    "The section includes information beyond what's relevant as indicated by {{TaskRef:Understand Differentiation}}.",
-                    "Information in the new section is redundant with other sections analyzed in {{TaskRef:Understand Differentiation}}.",
-                    "The draft does not reflect the structure, format, or detail level of the revised example section (output of {{TaskRef:Redraft Section for Relevant Content}}).",
-                    "Missing or incorrectly referenced tables or figures from the new reference materials.",
-                    "Significant deviation from the new reference materials, suggesting misalignment with the report's current focus.",
-                    "Inconsistent use of verb tenses where required.",
-                ],
-                "PASS": [
-                    "The section appropriately includes information within the scope defined by {{TaskRef:Understand Differentiation}}.",
-                    "The draft logically follows what the section heading describes.",
-                    "The draft focuses exclusively on the new report's context.",
-                    "The draft meets criteria for completeness, accuracy, and is aligned with the revised example and the new reference materials.",
-                ],
-            },
-            "additional_instructions": "Offer feedback on the process of differentiating from other sections, the use of source materials, and the rationale for selected source mappings.",
-            "output_format": {
-                "Section Review": "[SECTION NUMBER] - [SECTION HEADING]",
-                "Draft Review": "[content here]",
-                "Comments": "[comments here]",
-                "Success Flag": "[FAIL/PASS]",
-                "Source Mapping Review": "[REVIEW OF UTILIZED SOURCES]",
-                "Tables": "[LIST OF REFERENCED TABLES]",
-                "Figures": "[LIST OF REFERENCED FIGURES]",
-                "Cross-References": "[REFERENCES TO OTHER DOCUMENT SECTIONS (FROM SAMPLE DOCUMENT)]",
-                "Scope of Section Review": "[REFLECTION ON FOLLOWING THE SCOPE GUIDELINES SET OUT IN {{TaskRef:Understand Differentiation}} OUTPUT]",
-            },
         },
     ),
+    # Task(
+    #     task_name="Final Section Review",
+    #     details={
+    #         "description": "Review the final text for this section and provide a PASS/FAIL decision based on the success criteria.",
+    #         "prerequisite_tasks": ["Draft New Document Section"],
+    #         "instructions": [
+    #             "Evaluate the success of the new section draft",
+    #             "Document the review outcome",
+    #             "Print the final review output.",
+    #         ],
+    #         "success_flag_criteria": {
+    #             "FAIL": [
+    #                 "The section includes information beyond what's relevant as indicated by {{TaskRef:Understand Differentiation}}.",
+    #                 "Any mention of specific drugs or combination therapies not relevant to the new study context.",
+    #                 "Information in the new section is redundant with the sections analyzed in {{TaskRef:Understand Differentiation}}.",
+    #                 "The draft does not reflect the structure, format, or detail level of the revised example section (output of {{TaskRef:Handle Treatment Details}}).",
+    #                 "Missing or incorrectly referenced tables or figures from the new reference materials.",
+    #                 "Significant deviation from the new reference materials, suggesting misalignment with the study's current focus.",
+    #                 "Inconsistent use of verb tenses where required.",
+    #             ],
+    #             "PASS": [
+    #                 "The section appropriately includes information within the scope defined by {{TaskRef:Understand Differentiation}}.",
+    #                 "The draft logically follows what the section heading describes.",
+    #                 "The draft focuses exclusively on the new study context.",
+    #                 "The draft meets criteria for completeness, accuracy, and is aligned with the revised example and the new reference materials.",
+    #             ],
+    #         },
+    #         "additional_instructions": "Offer feedback on the process of differentiating from other sections, the use of source materials, and the rationale for selected source mappings.",
+    #         "output_format": {
+    #             "Section Review": "[SECTION NUMBER] - [SECTION HEADING]",
+    #             "Draft Review": "[content here]",
+    #             "Comments": "[comments here]",
+    #             "Success Flag": "[FAIL/PASS]",
+    #             "Source Mapping Review": "[REVIEW OF UTILIZED SOURCES]",
+    #             "Tables": "[LIST OF REFERENCED TABLES]",
+    #             "Figures": "[LIST OF REFERENCED FIGURES]",
+    #             "Cross-References": "[REFERENCES TO OTHER DOCUMENT SECTIONS (FROM EXAMPLE DOCUMENT)]",
+    #             "Scope of Section Review": "[REFLECTION ON FOLLOWING THE SCOPE GUIDELINES SET OUT IN {{TaskRef:Understand Differentiation}} OUTPUT]",
+    #         },
+    #     },
+    # ),
     Task(
         task_name="Prepare for Next Document Section",
         details={
-            "description": "Conclude current tasks and prepare to draft the next document section.",
-            "prerequisite_tasks": ["Final Document Review"],
-            "function_call": "Use the pop_context function.",
-            "example_call": "{{'current_section_identifier': ['Next Section Identifier']}}",
+            "description": "SIgnal that you have completed the draft by calling the pop_context function and prepare to start drafting the next section of the document.",
+            "function_call": "Use the pop_context function with the argument value = current section identifier.",
+            "example_call": "{{'current_section_identifier': ['1.2']}}",
+            "instructions": [
+                "Announce completion: 'Proceed to the next section of the document, [current section identifier] has been completed.'"
+            ],
         },
     ),
 ]
 
 general_comments = """
 ============
-General comments:
-Start with the first section. Only do the next uncompleted task (only one task at a time).
-Explicitly print out the current section identifier.
-Explicitly print out whether the last task completed successfully or not.
-Explicitly print out the task you are completing currently.
-Explicitly print out what task you will complete next.
-Explicitly provide a detailed and appropriate response for every task.
-The most important thing for you to understand: The primary goal of the tasks is to draft a new section of the document.
-A section is considered complete once the 'Final Document Review' task has been accomplished. Do not skip the 'Final Document Review' task.
-
-If a function call returns an error then try again with parameters, or make a different function call.
-If task has not completed successfully, try again with an altered response.
-If you notice a task (or series of tasks) being repeated erroneously, devise a plan to move on to the next uncompleted task.
-If you encounter empty messages repeatedly in the chat history, reorient yourself by revisiting the last task completed. Check that the sequence of past tasks progresses in logical order. If not, assess and adjust accordingly.
-
+GENERAL COMMENTS:
+START WITH THE FIRST SECTION. ONLY DO THE NEXT UNCOMPLETED TASK (ONLY ONE TASK AT A TIME).
+EXPLICITLY print out the current section identifier.
+EXPLICITLY print out wheter the last task completed successfully or not.
+EXPLICITLY print out the task you are completing currently.
+EXPLICITLY print out what task you will complete next.
+EXPLICITLY provide a detailed and appropriate response for EVERY TASK.
+THE MOST IMPORTANT THING FOR YOU TO UNDERSTAND: THE PRIMARY GOAL OF THE TASKS IS TO DRAFT A NEW SECTION OF THE DOCUMENT
+A SECTION IS CONSIDERED COMPLETE ONCE THE LAST TASK HAS BEEN ACCOMPLISHED.
+
+IF A FUNCTION CALL RETURNS AN ERROR THEN TRY AGAIN WITH PARAMETERS, OR MAKE DIFFERENT FUNCTION CALL.
+IF TASK HAS NOT COMPLETED SUCCESSFULLY, TRY AGAIN WITH AN ALTERED RESPONSE.
+DO NOT REPEAT YOUR PREVIOUS MESSAGE.  
+IF YOU NOTICE A TASK (OR SERIES OF TASKS) BEING REPEATED ERRONEOUSLY, devise a plan to move on to the next uncompleted task.
+IF YOU ENCOUNTER REPEATED MESSAGES IN THE CHAT HISTORY, reorient yourself by revisiting the last task completed. Check that the sequence of past tasks progresses in logical order. If not, assess and adjust accordingly.
+If you are on the same task for a long time, and you are not making progress, just go to the next task and do the best you can.
 Do not ever return a tool or function call with the name 'multi_tool_use.parallel'
+
 =============
 """
 
+
 initial_user_message = """
 Please see system message for instructions. Take note of which document section is currently being worked on and which tasks have been completed. Complete the next uncompleted task.
 If you do not see any tasks completed for the current section, begin with Task #1.
 
 If all tasks for the current section have been completed, proceed to the next document section.
 If the new section draft is complete, ensure to 'Prepare for Next Document Section' as described in the tasks.
 """
 
 pre_algo_instruct = """
-I am going to give you step by step instructions on how to draft a new report document section by section.
+I am going to give you step by step instructions on how to draft a new wiki page section by section.
 Below you will find a json object that contains the index of sections that need to be drafted.
 The keys of the json are the section numbers of the document. The values include the heading title.
+
+The subsections in the target document will be different and should be based on the information in the target document.
 """
 
 post_algo_instruct = """
-We will look at a Sample Document that is similar to the document to be drafted.
-Its full content can be queried with a function (section_text_getter) and used as an example (in json format).
+We will look at an Example Document that is similar to the document to be drafted.
+Its full content can be queried with a function (get_text_for_sections) and used as an example (in json format).
 The keys of the json are the section numbers of the document and the values contain the sections' bodies.
 What I want you to do is to go section by section in the Document to be drafted, and do the following, in sequential order:
 """
 
 job_description = JobDescription(
-    role="You are a professional writing AI agent. You have the ability to call outside functions.",
+    role="You are a wiki writing AI agent. You have the ability to call outside functions.",
     context="Document to be drafted:",
     task_list=task_library,
-    tool_implementations_class=ReportingToolImplementations,
+    tool_implementations_class=WikipediaToolImplementations,
     pre_context_instruct=pre_algo_instruct,
     post_context_instruct=post_algo_instruct,
     general_comments=general_comments,
     initial_user_message=initial_user_message,
 )
```

### Comparing `celi_framework-0.0.10/celi_framework/examples/reporting_template/tools.py` & `celi_framework-0.0.9/celi_framework/examples/study_report/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-"""
-This module acts as a general template for report generation.
-It is not specific to any particular type of report or study, but rather provides a set of tools and implementations
-for handling and generating sections of a report from various source materials.
-The functionality includes reading document schemas, retrieving and formatting text from specified sections,
-and providing interfaces to external language model services for content drafting and table setting.
-
-Usage of this module can be tailored to fit the needs of any structured reporting format across different domains,
-emphasizing its versatility and adaptability.
-"""
-
 import json
 import os
 from typing import Dict
 
 from attr import dataclass
 from celi_framework.core.job_description import (
     ToolImplementations,
@@ -34,59 +23,59 @@
 
 @dataclass
 class Document:
     toc: Dict[str, str]
     content: Dict[str, str]
 
 
-class ReportingToolImplementations(ToolImplementations):
+class StudyReportToolImplementations(ToolImplementations):
     doc_dir: str
 
     def __init__(self, doc_dir: str):
         super().__init__()
         self.doc_dir = doc_dir
 
         def dir(s):
             return os.path.join(self.doc_dir, s)
 
         self.source_mappings = read_json_from_file(dir("mappings_gpt.json"))
-        self.example_doc = Document(
-            toc=read_json_from_file(dir("example_report_schema.json")),
-            content=read_json_from_file(dir("example_report_filled.json")),
+        self.sample_doc = Document(
+            toc=read_json_from_file(dir("CSR_schema.json")),
+            content=read_json_from_file(dir("CSR_filled.json")),
         )
-        self.example_doc_sources = {
-            "example_source_1": Document(
-                toc=read_json_from_file(dir("example_source_1_schema.json")),
-                content=read_json_from_file(dir("example_source_1_filled.json")),
+        self.sample_doc_sources = {
+            "Protocol": Document(
+                toc=read_json_from_file(dir("example_protocol_schema.json")),
+                content=read_json_from_file(dir("example_protocol_filled.json")),
             ),
-            "example_source_2": Document(
-                toc=read_json_from_file(dir("example_source_2_schema.json")),
-                content=read_json_from_file(dir("example_source_2_filled.json")),
+            "SAP": Document(
+                toc=read_json_from_file(dir("example_sap_schema.json")),
+                content=read_json_from_file(dir("example_sap_filled.json")),
             ),
         }
         self.new_doc_sources = {
-            "new_source_1": Document(
-                toc=read_json_from_file(dir("new_source_1_schema.json")),
-                content=read_json_from_file(dir("new_source_1_filled.json")),
+            "Protocol": Document(
+                toc=read_json_from_file(dir("new_protocol_schema.json")),
+                content=read_json_from_file(dir("new_protocol_filled.json")),
             ),
-            "new_source_2": Document(
-                toc=read_json_from_file(dir("new_source_2_schema.json")),
-                content=read_json_from_file(dir("new_source_2_filled.json")),
+            "SAP": Document(
+                toc=read_json_from_file(dir("new_sap_schema.json")),
+                content=read_json_from_file(dir("new_sap_filled.json")),
             ),
         }
 
     def get_schema(self) -> Dict[str, str]:
-        return self.example_doc.toc
+        return self.sample_doc.toc
 
     def source_sections_getter(self, section_number: str):
         """
-        Identify the documents and their sections that are source materials for the example document section.
+        Identify the documents and section that are source materials for the example document section.
 
         Args:
-            section_number (str): The section number of the document for which you want to get the source material.
+            section_number (str): The section number document for which you want to get the source material.
         """
         return self.source_mappings[section_number]
 
     def section_text_getter(
         self,
         sections_dict_str: str,
     ):
@@ -112,18 +101,18 @@
         for document_name, section_numbers in sections_dict.items():
             app_logger.info(
                 f"Processing document: {document_name} with Sections: {section_numbers}",
                 extra={"color": "cyan"},
             )
 
             # Load the document based on the document name
-            if document_name == "Example Document":
-                document = self.example_doc
-            elif document_name in self.example_doc_sources:
-                document = self.example_doc_sources[document_name]
+            if document_name == "Sample Document":
+                document = self.sample_doc
+            elif document_name in self.sample_doc_sources:
+                document = self.sample_doc_sources[document_name]
             else:
                 err_msg = f"Error: No document named {document_name} was found to extract text from"
                 app_logger.error(err_msg, extra={"color": "red"})
                 output_text += f"{err_msg}\n\n"
                 continue
 
             # Process each section for the current document
@@ -156,15 +145,15 @@
 
         Returns:
             str: A string containing the formatted tables of contents for source documents,
                 followed by an instruction to proceed to the next task.
         """
         reformatted = [
             f"{k} Table of Contexts:\n\n{format_toc(v.toc)}"
-            for k, v in self.example_doc_sources.items()
+            for k, v in self.sample_doc_sources.items()
         ]
 
         # Combine the schemas into a single string for the response
         send_to_llm = (
             "\n\n".join(reformatted)
             + "\n\nProceed to next task: Map example sources to new sources indexes"
         )
```

### Comparing `celi_framework-0.0.10/celi_framework/examples/wikipedia/Index_cache.py` & `celi_framework-0.0.9/celi_framework/examples/wikipedia/Index_cache.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.10/celi_framework/examples/wikipedia/caching_beautiful_soup_reader.py` & `celi_framework-0.0.9/celi_framework/examples/wikipedia/caching_beautiful_soup_reader.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.10/celi_framework/examples/wikipedia/eval/run_eval.py` & `celi_framework-0.0.9/celi_framework/examples/wikipedia/eval/run_eval.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.10/celi_framework/examples/wikipedia/eval/test_sets.json` & `celi_framework-0.0.9/celi_framework/examples/wikipedia/eval/test_sets.json`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.10/celi_framework/examples/wikipedia/eval/test_sets_large.json` & `celi_framework-0.0.9/celi_framework/examples/wikipedia/eval/test_sets_large.json`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.10/celi_framework/examples/wikipedia/index.py` & `celi_framework-0.0.9/celi_framework/examples/wikipedia/index.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.10/celi_framework/examples/wikipedia/job_description.py` & `celi_framework-0.0.9/celi_framework/examples/study_report/template.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,160 +1,246 @@
 from celi_framework.core.job_description import JobDescription, Task
 
-from celi_framework.examples.wikipedia.tools import WikipediaToolImplementations
+from celi_framework.examples.study_report.tools import StudyReportToolImplementations
 
 task_library = [
     Task(
         task_name="Search for Document Section Text",
         details={
-            "description": "Find the text of the current section and all subsections in the example document.",
+            "description": "Find the text of the current section in the sample document.",
             "prerequisite_tasks": [],
-            "function_call": "Call get_example_toc to get the full list of sections in the example doc and then get_text_for_sections to retrieve the text for the current section and any relevant (sub)sections.",
-            "example_call": "{{'Example Document': ['1', '1.1', '1.2']}}",
+            "function_call": "Perform a function call to retrieve the text for the current section.",
+            "example_call": "{{'Sample Document': ['1.1']}}",
             "instructions": [
                 "Every section should have corresponding text, even that text is blank. If you get an error, try again with different parameters",
                 "Do not truncate or modify the retrieved text.",
                 "If text is present, print the entire text and instruct to proceed to the next task.",
-                "If a given section is empty in the example document, then you can leave that section empty in the target. In that case, you can skip all the remaining tasks and jump straight to the 'Draft New Document Section' task, which can just draft an empty section. Note that a blank section is not the same as the function returning an error.",
+                "If a given section is empty in the sample document, then you can leave that section empty in the target. In that case, you can skip all the remaining tasks and jump straight to the 'Draft New Document Section' task, which can just draft an empty section. Note that a blank section is not the same as the function returning an error.",
             ],
         },
     ),
     Task(
         task_name="Understand Differentiation",
         details={
-            "description": "Understand the context of the example document section by comparing it with similar sections.  Also look at any subsections and understand how they are structured.",
+            "description": "Understand the context of the sample document section by comparing it with similar sections.",
             "prerequisite_tasks": ["Search for Document Section Text"],
             "instructions": [
-                "Identify other sections of the example document that may contain content similar to the current section.",
+                "Identify other sections of the sample document that may contain content similar to the current section.",
+                "Reference the 'Document to be drafted' dictionary.",
                 "Retrieve the text of these sections along with their section identifiers.",
                 "Analyze and note down how the current section differs from these sections to prevent duplication in future work.",
             ],
+            "example": {
+                "2.1.5": "Health Monitoring - Procedural topics...",
+                "2.3.1": "Health Assessment (HA) - Statistical topics...",
+            },
             "additional_notes": [
                 "Keep your notes concise and relevant for later use.",
                 "If 'no content present' is observed in all section bodies that are retrieved, even after retrieving children/sub-sections, proceed to the next task.",
-                "If it seems like the current section is specific to the example document, and would not make sense as part of the target document, feel free to skip the section and go on to the next one.  This can happen if the example contains a section highly specific to it's topic, but not relevant to the target document.",
             ],
         },
     ),
     Task(
-        task_name="Find the most relevant references for the target section and all the subsections",
+        task_name="Handle Treatment Details",
         details={
-            "description": """Call get_corresponding_target_references_for_example_sections function with a list of the current section and all subsections to retrieve these materials. to find relevant references for the target document that correspond to the example document sections you are looking at.
-            The references may not provide you with all the information you need to draft the section.  Don't worry, you will get a chance to ask additional questions in the next task.""",
-            "example_call": "['1', '1.1', '1.2']",
+            "description": "Address text related to treatment details in the sample document section.",
+            "prerequisite_tasks": ["Search for Document Section Text"],
+            "instructions": [
+                "If there is no mention of additional treatments beyond the primary investigational product in the experimental arm, print 'Proceed to next task immediately.'",
+                "If there is mention of additional treatments, list them in a numbered format and redraft the section by omitting this content. Adjust the scope of the section to be consistent with the revisions.",
+            ],
+            "examples": {
+                "to_exclude": [
+                    "In the Treatment Expansion, the investigational product and standard care were administered as outlined in Section X.Y.Z, until meeting any of the discontinuation criteria listed in Section A.B.",
+                    "Treatment Group 2=Investigational Product + Regimen 2, for subjects with Condition A; Treatment Group 3=Investigational Product + Regimen 3, for subjects with Condition B with specific risk factors; Treatment Group 4=Investigational Product + Regimen 4, for subjects with Condition C.",
+                ],
+                "not_to_exclude": [
+                    "For all Treatment Groups... Hospitalization details based on the study protocol.",
+                    "Include text about dosage details: If multiple subjects received the same dosage level without adverse effects, this may be considered the selected dose for future phases.",
+                ],
+            },
+            "additional_notes": [
+                "Omit text about any additional therapies unless the section is relevant to both the primary treatment and additional therapies. Move to the next task if this does not apply."
+            ],
         },
     ),
     Task(
-        task_name="Ask additional questions",
+        task_name="Identify Document Source",
         details={
-            "description": """Determine if any additional information is required to draft the section and call the ask_question_about_target function to gather that information.
-            Feel free to ask as many questions as you need and keep working on this task until you have the information you need.  This is especially important if
-            the initial references turn out not to be useful.
-            If you don't have any questions, just move on to the next section.""",
-            "example_call": '{"prompt": "What is unusual about when this band formed?"}',
+            "description": "Identify the section source materials for the sample document section.",
+            "function_call": "Call the source_sections_getter function to retrieve these materials.",
         },
     ),
     Task(
-        task_name="Define subsections for this section",
+        task_name="Find Essential Source Materials",
         details={
-            "description": """Define what subsections should be present within this individual section.  Use the table of contents from the example document and your knowledge of the target page to structure the subsections.  Keeep in mind over differentiation of this section from other sections in the document.  It is totally fine to not have subsections, especially if the example document does not have them.
-            Also, remember that the subsections should be relevant for the target document.  The detailed structure of subsections used in the example may not be relevant for our target document.""",
+            "description": "Identify the most critical source materials needed for drafting the sample document section.",
+            "prerequisite_tasks": ["Identify Document Source"],
+            "task": "Organize these materials in descending order of relevance and present them as a bulleted list.",
+            "example": [
+                "Sample Document Section S1: Outlines the general study framework, including major phases, medication schedules, and methods to address potential adverse effects.",
+                "Sample Reference Section R1: Provides a summary of the study structure, with details on specific phases and medication schedules relevant to the investigational product.",
+            ],
+        },
+    ),
+    Task(
+        task_name="Get source table of contents",
+        details={
+            "description": "Retrieve the TOCs of the new SAP and Protocol documents for the current section.",
+            "function_call": "Call get_source_tocs.",
+            "example_call": "{{'current_section_number': '9.1.a'}}.",
+            "instructions": [
+                "Retrieve the TOCs for the new SAP and new Protocol documents with function call.",
+                "Do not modify the new source TOCs that you retrieve in any way.",
+                "Do not hallucinate new TOCs.",
+            ],
+        },
+    ),
+    Task(
+        task_name="Map Document Sources to New Indexes",
+        details={
+            "description": "Align sections of the new reference documents with the identified source sections of the sample document.",
+            "prerequisite_tasks": [
+                "Identify Document Source",
+                "New target sources indexes",
+            ],
+            "instructions": [
+                "Utilize the new indexes provided by the output of the previous task.",
+                "Focus on the content and headings of the document sections rather than strict numbering conventions.",
+                "Pay attention to overarching sections, like 'Study Overview', 'Data Analysis Methods', etc.",
+            ],
+        },
+    ),
+    Task(
+        task_name="Handle Document Subsections",
+        details={
+            "description": "Ensure that both main sections and their nested subsections are appropriately mapped when necessary.",
+            "prerequisite_tasks": ["Map Document Sources to New Indexes"],
+            "instructions": [
+                "Ensure alignment between the main section and any nested subsections that share relevant content.",
+                "Comprehend the structure of sections and subsections by their sequence and thematic connection.",
+            ],
+        },
+    ),
+    Task(
+        task_name="New Reference Material Retrieval",
+        details={
+            "description": "Retrieve the text for new reference document sections identified in previous tasks.",
+            "prerequisite_tasks": ["Map Document Sources to New Indexes"],
+            "instructions": [
+                "Utilize the section text retrieval function to fetch the text for specified sections.",
+                "Limit the retrieval to a maximum of 8 sections. If there are more than 8 sections identified as critical, prioritize based on importance.",
+            ],
+            "example_call": "{{ 'New Reference Document': ['1.1', '1.1.1'], 'New Guidelines': ['G2.2'] }}",
         },
     ),
     Task(
         task_name="Draft New Document Section",
         details={
-            "description": "Draft a new section analogous to the revised example section, ensuring alignment with its structure, format, and scope (from {{TaskRef:Understand Differentiation}} output).  Use the section structure you defined in {{TaskRef:Define subsections for this section}}. However, the details should be related to the target and not the example document.",
+            "description": "Draft a new section analogous to the revised example section (from {{TaskRef:Handle Treatment Details}} output), ensuring alignment with its structure, format, and scope (from {{TaskRef:Understand Differentiation}} output).",
+            "prerequisite_tasks": [
+                "Search for Document Section Text",
+                "Understand Differentiation",
+                "Map Document Sources to New Indexes",
+                "New Reference Material Retrieval",
+            ],
             "guidelines": [
-                "Clearly identify the section number and section heading/title at the top of the content.",
                 "The new section should have its unique scope and purpose, distinct from the example section.",
+                "Closely align with the example section's approach for consistency.",
                 "Avoid duplicating content or including redundant information.",
-                "Aim for the new section to mirror the example section in length and detail, but using content related to the target.",
+                "Aim for the new section to mirror the example section in length and detail.",
                 "Follow the instructions set out by {{TaskRef:Understand Differentiation}} output.",
+            ],
+            "considerations": [
+                "What differentiates this section from other similar sections? Refer to the output of {{TaskRef:Understand Differentiation}}.",
+                "Concentrate on content relevant to the specific section within the broader document context.",
                 "Maintain consistency in documentation methodology, using the revised example as a template.",
-                "Ensure content is exclusively about the target, and not the example topic.",
+                "Ensure content is derived exclusively from the newly identified source materials.",
             ],
             "specific_instructions": [
                 "Do not copy text verbatim. Include only text within the scope of the current section, as highlighted in the output of {{TaskRef:Understand Differentiation}}.",
                 "Include cross-references to other sections as seen in the example if applicable.",
+                "Incorporate references to tables and sections within the new reference documents as appropriate, providing context to the study's methodology and decision-making processes.",
+            ],
+            "note": "Focus on the specific section, considering its role within the parent sections and its relation to the revised example section. Utilize the guidance from {{TaskRef:Understand Differentiation}} for the scope of the section",
+        },
+    ),
+    Task(
+        task_name="Final Document Review",
+        details={
+            "description": "Review the final document and provide a PASS/FAIL decision based on the success criteria.",
+            "prerequisite_tasks": ["Draft New Document Section"],
+            "instructions": [
+                "Evaluate the success of the new section draft",
+                "Document the review outcome",
+                "Print the final review output.",
             ],
+            "success_flag_criteria": {
+                "FAIL": [
+                    "The section includes information beyond what's relevant as indicated by {{TaskRef:Understand Differentiation}}.",
+                    "Any mention of specific drugs or combination therapies not relevant to the new study context.",
+                    "Information in the new section is redundant with the sections analyzed in {{TaskRef:Understand Differentiation}}.",
+                    "The draft does not reflect the structure, format, or detail level of the revised example section (output of {{TaskRef:Handle Treatment Details}}).",
+                    "Missing or incorrectly referenced tables or figures from the new reference materials.",
+                    "Significant deviation from the new reference materials, suggesting misalignment with the study's current focus.",
+                    "Inconsistent use of verb tenses where required.",
+                ],
+                "PASS": [
+                    "The section appropriately includes information within the scope defined by {{TaskRef:Understand Differentiation}}.",
+                    "The draft logically follows what the section heading describes.",
+                    "The draft focuses exclusively on the new study context.",
+                    "The draft meets criteria for completeness, accuracy, and is aligned with the revised example and the new reference materials.",
+                ],
+            },
+            "additional_instructions": "Offer feedback on the process of differentiating from other sections, the use of source materials, and the rationale for selected source mappings.",
+            "output_format": {
+                "Section Review": "[SECTION NUMBER] - [SECTION HEADING]",
+                "Draft Review": "[content here]",
+                "Comments": "[comments here]",
+                "Success Flag": "[FAIL/PASS]",
+                "Source Mapping Review": "[REVIEW OF UTILIZED SOURCES]",
+                "Tables": "[LIST OF REFERENCED TABLES]",
+                "Figures": "[LIST OF REFERENCED FIGURES]",
+                "Cross-References": "[REFERENCES TO OTHER DOCUMENT SECTIONS (FROM SAMPLE DOCUMENT)]",
+                "Scope of Section Review": "[REFLECTION ON FOLLOWING THE SCOPE GUIDELINES SET OUT IN {{TaskRef:Understand Differentiation}} OUTPUT]",
+            },
         },
     ),
-    # Task(
-    #     task_name="Final Section Review",
-    #     details={
-    #         "description": "Review the final text for this section and provide a PASS/FAIL decision based on the success criteria.",
-    #         "prerequisite_tasks": ["Draft New Document Section"],
-    #         "instructions": [
-    #             "Evaluate the success of the new section draft",
-    #             "Document the review outcome",
-    #             "Print the final review output.",
-    #         ],
-    #         "success_flag_criteria": {
-    #             "FAIL": [
-    #                 "The section includes information beyond what's relevant as indicated by {{TaskRef:Understand Differentiation}}.",
-    #                 "Any mention of specific drugs or combination therapies not relevant to the new study context.",
-    #                 "Information in the new section is redundant with the sections analyzed in {{TaskRef:Understand Differentiation}}.",
-    #                 "The draft does not reflect the structure, format, or detail level of the revised example section (output of {{TaskRef:Handle Treatment Details}}).",
-    #                 "Missing or incorrectly referenced tables or figures from the new reference materials.",
-    #                 "Significant deviation from the new reference materials, suggesting misalignment with the study's current focus.",
-    #                 "Inconsistent use of verb tenses where required.",
-    #             ],
-    #             "PASS": [
-    #                 "The section appropriately includes information within the scope defined by {{TaskRef:Understand Differentiation}}.",
-    #                 "The draft logically follows what the section heading describes.",
-    #                 "The draft focuses exclusively on the new study context.",
-    #                 "The draft meets criteria for completeness, accuracy, and is aligned with the revised example and the new reference materials.",
-    #             ],
-    #         },
-    #         "additional_instructions": "Offer feedback on the process of differentiating from other sections, the use of source materials, and the rationale for selected source mappings.",
-    #         "output_format": {
-    #             "Section Review": "[SECTION NUMBER] - [SECTION HEADING]",
-    #             "Draft Review": "[content here]",
-    #             "Comments": "[comments here]",
-    #             "Success Flag": "[FAIL/PASS]",
-    #             "Source Mapping Review": "[REVIEW OF UTILIZED SOURCES]",
-    #             "Tables": "[LIST OF REFERENCED TABLES]",
-    #             "Figures": "[LIST OF REFERENCED FIGURES]",
-    #             "Cross-References": "[REFERENCES TO OTHER DOCUMENT SECTIONS (FROM EXAMPLE DOCUMENT)]",
-    #             "Scope of Section Review": "[REFLECTION ON FOLLOWING THE SCOPE GUIDELINES SET OUT IN {{TaskRef:Understand Differentiation}} OUTPUT]",
-    #         },
-    #     },
-    # ),
     Task(
         task_name="Prepare for Next Document Section",
         details={
-            "description": "SIgnal that you have completed the draft by calling the pop_context function and prepare to start drafting the next section of the document.",
+            "description": "Complete current tasks and prepare to start drafting the next section of the document.",
+            "prerequisite_tasks": ["Final Document Review"],
             "function_call": "Use the pop_context function with the argument value = current section identifier.",
             "example_call": "{{'current_section_identifier': ['1.2']}}",
             "instructions": [
                 "Announce completion: 'Proceed to the next section of the document, [current section identifier] has been completed.'"
             ],
+            "caution": "If the draft for the new section was not finalized in any prior tasks, then call pop_context with current_section_identifier = None",
         },
     ),
 ]
 
 general_comments = """
 ============
 GENERAL COMMENTS:
 START WITH THE FIRST SECTION. ONLY DO THE NEXT UNCOMPLETED TASK (ONLY ONE TASK AT A TIME).
 EXPLICITLY print out the current section identifier.
 EXPLICITLY print out wheter the last task completed successfully or not.
 EXPLICITLY print out the task you are completing currently.
 EXPLICITLY print out what task you will complete next.
 EXPLICITLY provide a detailed and appropriate response for EVERY TASK.
 THE MOST IMPORTANT THING FOR YOU TO UNDERSTAND: THE PRIMARY GOAL OF THE TASKS IS TO DRAFT A NEW SECTION OF THE DOCUMENT
-A SECTION IS CONSIDERED COMPLETE ONCE THE LAST TASK HAS BEEN ACCOMPLISHED.
+A SECTION IS CONSIDERED COMPLETE ONCE THE 'Final Document Review' TASK HAS BEEN ACCOMPLISHED.  DSO NOT SKIP THE 'Final Document Review' task.
 
 IF A FUNCTION CALL RETURNS AN ERROR THEN TRY AGAIN WITH PARAMETERS, OR MAKE DIFFERENT FUNCTION CALL.
-IF TASK HAS NOT COMPLETED SUCCESSFULLY, TRY AGAIN WITH AN ALTERED RESPONSE.
-DO NOT REPEAT YOUR PREVIOUS MESSAGE.  
+IF TASK HAS NOT COMPLETED SUCCESSFULLY, TRY AGAIN WITH AN ALTERED RESPONSE
 IF YOU NOTICE A TASK (OR SERIES OF TASKS) BEING REPEATED ERRONEOUSLY, devise a plan to move on to the next uncompleted task.
-IF YOU ENCOUNTER REPEATED MESSAGES IN THE CHAT HISTORY, reorient yourself by revisiting the last task completed. Check that the sequence of past tasks progresses in logical order. If not, assess and adjust accordingly.
-If you are on the same task for a long time, and you are not making progress, just go to the next task and do the best you can.
+IF YOU ENCOUNTER EMPTY MESSAGES REPEATEDLY IN THE CHAT HISTORY, reorient yourself by revisiting the last task completed. Check that the sequence of past tasks progresses in logical order. If not, assess and adjust accordingly.
+
 Do not ever return a tool or function call with the name 'multi_tool_use.parallel'
 
 =============
 """
 
 
 initial_user_message = """
@@ -162,31 +248,29 @@
 If you do not see any tasks completed for the current section, begin with Task #1.
 
 If all tasks for the current section have been completed, proceed to the next document section.
 If the new section draft is complete, ensure to 'Prepare for Next Document Section' as described in the tasks.
 """
 
 pre_algo_instruct = """
-I am going to give you step by step instructions on how to draft a new wiki page section by section.
+I am going to give you step by step instructions on how to draft a new study report document section by section.
 Below you will find a json object that contains the index of sections that need to be drafted.
 The keys of the json are the section numbers of the document. The values include the heading title.
-
-The subsections in the target document will be different and should be based on the information in the target document.
 """
 
 post_algo_instruct = """
-We will look at an Example Document that is similar to the document to be drafted.
-Its full content can be queried with a function (get_text_for_sections) and used as an example (in json format).
+We will look at a Sample Document that is similar to the document to be drafted.
+Its full content can be queried with a function (section_text_getter) and used as an example (in json format).
 The keys of the json are the section numbers of the document and the values contain the sections' bodies.
 What I want you to do is to go section by section in the Document to be drafted, and do the following, in sequential order:
 """
 
 job_description = JobDescription(
-    role="You are a wiki writing AI agent. You have the ability to call outside functions.",
+    role="You are a medical writing AI agent. You have the ability to call outside functions.",
     context="Document to be drafted:",
     task_list=task_library,
-    tool_implementations_class=WikipediaToolImplementations,
+    tool_implementations_class=StudyReportToolImplementations,
     pre_context_instruct=pre_algo_instruct,
     post_context_instruct=post_algo_instruct,
     general_comments=general_comments,
     initial_user_message=initial_user_message,
 )
```

### Comparing `celi_framework-0.0.10/celi_framework/examples/wikipedia/loader.py` & `celi_framework-0.0.9/celi_framework/examples/wikipedia/loader.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.10/celi_framework/examples/wikipedia/tools.py` & `celi_framework-0.0.9/celi_framework/examples/wikipedia/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,12 +348,12 @@
                 RecreatedNode(node_id=id, metadata=metadata, text=doc)
                 for id, metadata, doc in by_node
             ]
         else:
             try:
                 return [
                     _
-                    for _ in self.example_index.docstore.docs.values()
+                    for _ in index.docstore.docs.values()
                     if _.metadata.get("celi_section_number", None) == section_number
                 ]
             except IndexError:
                 raise ValueError(f"Example section {section_number} not found.")
```

### Comparing `celi_framework-0.0.10/celi_framework/examples/wikipedia/wikipedia_utils.py` & `celi_framework-0.0.9/celi_framework/examples/wikipedia/wikipedia_utils.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.10/celi_framework/experimental/embeddor.py` & `celi_framework-0.0.9/celi_framework/experimental/embeddor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.10/celi_framework/experimental/mapper.py` & `celi_framework-0.0.9/celi_framework/experimental/mapper.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.10/celi_framework/experimental/mechanic.py` & `celi_framework-0.0.9/celi_framework/experimental/mechanic.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.10/celi_framework/experimental/preprocessing/pre-processor.py` & `celi_framework-0.0.9/celi_framework/experimental/preprocessing/pre-processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,39 +14,36 @@
 - `test_load_json_files`: Confirms JSON file integrity, crucial for successful loading and embedding.
 - `rid_new_line_sections_dict`: Purges sections of unnecessary newlines, reducing noise before embedding.
 - `process_files_in_directory_new_line`: Implements newline cleanup across multiple files in preparation for embedding.
 - `clean_up_dict`: Applies an in-depth content cleanup, utilizing AI models to polish text for optimal embedding results.
 - `process_files_in_directory`: Coordinates the document processing workflow, ensuring each file is systematically cleaned and ready for the celi_framework.embeddor module.
 
 This script is built to be adaptable, enabling users to tailor its functions to meet the unique requirements of their projects. It serves as an exemplar for document preprocessing, showcasing Python's capabilities for automating the preparation of textual data for intricate analysis and model training.
-
 """
 
-# TODO -> We manually had chatGPT take table of contents and turn it into a dictionary "schema" for our experimentation.
-#  Do this programatically at some point
-
-
 import re
 import subprocess
 import time
 import os
 import json
 from celi_framework.utils.token_counters import token_counter_og
 from celi_framework.utils.llms import quick_ask
 from celi_framework.core.templates import make_cleanup_dict_prompt_template
 from celi_framework.utils.utils import (
     load_json,
     save_json,
     filter_empty_sections,
+    logger,
     read_txt,
 )
-from celi_framework.utils.log import app_logger as logger  # TODO: Check that the logger works correctly
 
 
 # STEP 1
+
+
 def convert_docx_to_markdown(input_file, output_file):
     """
     Converts a DOCX file to Markdown format using Pandoc.
 
     Args:
     input_file (str): Path to the input DOCX file.
     output_file (str): Path for the output Markdown file.
@@ -66,14 +63,19 @@
 
         # Executing the command
         subprocess.run(command, check=True)
         print(f"Conversion successful: {input_file} to {output_file}")
     except subprocess.CalledProcessError as e:
         logger.error(f"An error occurred during conversion: {e}")
 
+
+# TODO -> You manually had chatGPT take table of contents and turn it into a dictionary ("schema") for all three document types
+#  do this programattically at some point
+
+
 def process_markdown_fill_flat_2(file_path, section_dict):
     """
     Process a markdown file and store sections in a dictionary based on a provided section dictionary.
     This version uses regular expressions to match markdown headings and considers their levels.
 
     Args:
     file_path (str): Path to the markdown file.
```

### Comparing `celi_framework-0.0.10/celi_framework/experimental/preprocessing/word_pdf_extractors/extractor_helpers.py` & `celi_framework-0.0.9/celi_framework/experimental/preprocessing/word_pdf_extractors/extractor_helpers.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.10/celi_framework/experimental/preprocessing/word_pdf_extractors/pdf_extractor.py` & `celi_framework-0.0.9/celi_framework/experimental/preprocessing/word_pdf_extractors/pdf_extractor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.10/celi_framework/experimental/preprocessing/word_pdf_extractors/word_extractor.py` & `celi_framework-0.0.9/celi_framework/experimental/preprocessing/word_pdf_extractors/word_extractor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.10/celi_framework/experimental/task_builder/factory.py` & `celi_framework-0.0.9/celi_framework/experimental/task_builder/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 The `templates.task_builder.factory` module is part of a larger framework designed to automate and simplify the process of document drafting and analysis. At the heart of this module is the `InteractiveDocumentTemplate` class, which extends the `MasterTemplateFactory` to provide a more interactive and user-centric approach to document creation. This module leverages a configurable task library to generate detailed, numbered tasks and a comprehensive system message that guides users through each step of the document drafting or analysis process.
 
-The `InteractiveDocumentTemplate` class is specifically tailored to support a variety of document types and requirements, making it a versatile tool for projects ranging from writing to technical documentation. It ensures that users or AI agents can follow a clear, sequential path through the drafting process, enhancing understanding and efficiency.
+The `InteractiveDocumentTemplate` class is specifically tailored to support a variety of document types and requirements, making it a versatile tool for projects ranging from medical writing to technical documentation. It ensures that users or AI agents can follow a clear, sequential path through the drafting process, enhancing understanding and efficiency.
 
 Key Features:
 - Inherits and extends the `MasterTemplateFactory` class to support interactive document drafting.
 - Dynamically numbers tasks and enriches them with detailed descriptions for clarity.
 - Generates a comprehensive system message that includes the user role, context, detailed tasks, general comments, and a user message.
 - Utilizes a configuration and schema to tailor the drafting guide to specific document types and drafting goals.
 """
```

### Comparing `celi_framework-0.0.10/celi_framework/experimental/task_builder/llm_helper_funcs.py` & `celi_framework-0.0.9/celi_framework/experimental/task_builder/llm_helper_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,14 @@
     document_sampler_handler(directory: str = "input", sample_count: int = 5) -> str:
         Randomly selects documents from the specified directory and extracts text samples, particularly supporting PDFs and potentially other formats. This sampling is instrumental in gauging the content's nature and scope, serving as a basis for tailoring subsequent drafting tasks to the document's specific needs.
 
 Usage Scenario:
 These helper functions are integral to the operation of the `InteractiveDocumentTemplate`, enhancing its ability to interactively engage with users and utilize the content of documents in the drafting process. By leveraging these functions, the template builder can dynamically generate tasks that are directly informed by user goals and the specific content of the documents under consideration.
 """
 
-# TODO: Use the ToolImplementations class for the tools.
-
-import os
 
 def interactive_input_handler(question):
     user_input = input(f"{question}: ")
     # Simulate LLM response based on user input (replace with actual LLM call)
     llm_response = f"LLM simulated response based on '{user_input}'"
     print(f"LLM says: {llm_response}")
     return user_input, llm_response
```

### Comparing `celi_framework-0.0.10/celi_framework/experimental/task_builder/llms.py` & `celi_framework-0.0.9/celi_framework/experimental/task_builder/llms.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,14 @@
 Purpose:
 The primary objective of this module is to act as a reference for the `InteractiveDocumentTemplate` class, aiding in the identification and invocation of functions that LLMs can execute to enhance the interactive drafting process. By providing a clear list of available function calls, it ensures that LLMs can effectively contribute to task generation, user interaction, and content analysis, making the document drafting process more adaptive and user-focused.
 
 Note:
 This module is specific to the interactive task builder's context and should be used in conjunction with the `InteractiveDocumentTemplate` class to dynamically generate tasks that respond to user inputs and document content, enhancing the document creation workflow.
 """
 
-# TODO: We no longer need to list and describe available tools separately from llm_helper_funcs.
-#  The descriptions are automatically pulled from the tool definition docstrings if you use ToolImplementations.
-
 functions = [
     # Existing function entries...
     # Interactive Input Handler
     {
         "name": "interactive_input_handler",
         "description": "Interactively collects user input based on a provided question and simulates an LLM response.",
         "parameters": {
```

### Comparing `celi_framework-0.0.10/celi_framework/experimental/task_builder/template.py` & `celi_framework-0.0.9/celi_framework/experimental/task_builder/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 3. The system assesses the files and samples text data to inform the drafting process further.
 4. Based on the sampled text and user inputs, the system proposes a rephrased intent for the user's confirmation, ensuring alignment with the user's goals.
 5. A complete list of tasks is generated, outlining a customized approach to achieve the defined document drafting objectives.
 
 This configuration empowers the `InteractiveDocumentTemplate` to create an interactive guide for document drafting, enhancing user engagement and ensuring the drafting process is responsive to the user's specific needs and the document's content requirements.
 """
 
-from celi_framework.core.job_description import JobDescription, Task
+import os
+
+from job_description import JobDescription, Task
 
 # TODO:
 #  Have the user define the expected output format, have them give the required input data,
 #  and then have tasks generated from that
 
 job_description = JobDescription(
     role="You are tasked with gathering specific information for document drafting.",
```

### Comparing `celi_framework-0.0.10/celi_framework/experimental/utils/ada.py` & `celi_framework-0.0.9/celi_framework/experimental/utils/ada.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,18 +33,19 @@
 
 
 import numpy as np
 import openai
 import pandas as pd
 from sklearn.metrics.pairwise import cosine_similarity
 
-from celi_framework.utils.llms import get_openai_client
 from celi_framework.utils.token_counters import token_counter_og
 from celi_framework.utils.log import app_logger
 
+client = openai.OpenAI(api_key=os.environ["OPENAI_API_KEY"])
+
 EMBEDDING_MODEL = "text-embedding-ada-002"
 EMBEDDING_TOKEN_LIMIT = 8100
 EMBEDDING_CHUNK_OVERLAP = 500
 
 SAMPLE_SIZE = 50  # Number of samples to determine token-to-length ratio
 
 
@@ -87,16 +88,15 @@
     """
     text = text.replace("\n", " ")
 
     for retry in range(retries):
         try:
             if len(text) > 0 and text != "[Empty Section]":
                 response = (
-                    get_openai_client()
-                    .embeddings.create(input=[text], model=model)
+                    client.embeddings.create(input=[text], model=model)
                     .data[0]
                     .embedding
                 )
                 return response
             else:
                 return None
         except Exception as e:
```

### Comparing `celi_framework-0.0.10/celi_framework/experimental/utils/mapper_utils.py` & `celi_framework-0.0.9/celi_framework/experimental/utils/mapper_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import json
 import os
 from collections import defaultdict, Counter
 import numpy as np
 import pandas as pd
 from sklearn.metrics.pairwise import cosine_similarity
 from celi_framework.experimental.utils.ada import get_openai_embedding_sync_timeouts
-from celi_framework.utils.llms import quick_ask
+from utils.llms import quick_ask
 from celi_framework.core.templates import create_prompt_for_essential_section_analysis
 from celi_framework.utils.token_counters import get_master_counter_instance
 from celi_framework.utils.utils import load_json, get_section_context_as_text
 from celi_framework.utils.log import app_logger
 
 TOKEN_LIMIT_PER_MINUTE = 120000
```

### Comparing `celi_framework-0.0.10/celi_framework/experimental/utils/nougat_preprocessing/preprocess.py` & `celi_framework-0.0.9/celi_framework/experimental/utils/nougat_preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.10/celi_framework/experimental/utils/nougat_preprocessing/preprocessing_templates.py` & `celi_framework-0.0.9/celi_framework/experimental/utils/nougat_preprocessing/preprocessing_templates.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.10/celi_framework/experimental/utils/postprocessor_utils.py` & `celi_framework-0.0.9/celi_framework/experimental/utils/postprocessor_utils.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.10/celi_framework/experimental/utils/synthetic_data.py` & `celi_framework-0.0.9/celi_framework/experimental/utils/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.10/celi_framework/logging_config.json` & `celi_framework-0.0.9/celi_framework/logging_config.json`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.10/celi_framework/logging_setup.py` & `celi_framework-0.0.9/celi_framework/logging_setup.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.10/celi_framework/main.py` & `celi_framework-0.0.9/celi_framework/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,16 +72,15 @@
         "EXTERNAL_DB",
         "Set to True if using an existing mongo server.",
     )
     parser.add_argument(
         "--job-description",
         type=str,
         default=os.getenv(
-            "JOB_DESCRIPTION",
-            "celi_framework.examples.wikipedia.job_description.job_description",
+            "JOB_DESCRIPTION", "templates.study_report.template.job_description"
         ),
         help="Fully qualified name of a JobDescription instance with information on the task to perform",
     )
     parser.add_argument(
         "--tool-config-json",
         type=str,
         default=os.getenv("TOOL_CONFIG_JSON"),
```

### Comparing `celi_framework-0.0.10/celi_framework/utils/codex.py` & `celi_framework-0.0.9/celi_framework/utils/codex.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.10/celi_framework/utils/llmcore_utils.py` & `celi_framework-0.0.9/celi_framework/utils/llmcore_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,47 +2,46 @@
 The `utils.llmcore_utils` module serves as a comprehensive toolkit for leveraging Large Language Models (LLMs)
 such as OpenAI's models and LLaMA CPP for natural language processing tasks within a broader application context.
 This module integrates core components from the `llm_core` library, providing functionality for parsing textual
 messages, conducting error analysis, performing secondary analysis, generating dense summaries, and processing
 content through specialized LLM assistants.
 
 Features:
-    - Data class definitions for structured representation of messages, errors, function returns, analysis reports,
-        and output summaries, enabling type-safe operations and clarity in data handling.
-    - Utility functions for parsing textual inputs into structured data classes using OpenAI's and LLaMA CPP's parsers,
-        facilitating the extraction of meaningful information from free-text responses.
-    - Integration with MongoDB for data persistence, demonstrating how LLM outputs can be stored, retrieved, and processed
-        for applications requiring database interactions.
-    - Implementation of question-answering workflows and content verification methods that employ LLMs to validate,
-        analyze, and enhance textual content based on specific criteria such as relevance, accuracy, and clarity.
-    - Techniques for reducing hallucinations and improving the reliability of LLM responses through the Chain of Verification
-        (CoV) and summarization strategies aimed at condensing extensive content into more manageable forms.
+- Data class definitions for structured representation of messages, errors, function returns, analysis reports,
+  and output summaries, enabling type-safe operations and clarity in data handling.
+- Utility functions for parsing textual inputs into structured data classes using OpenAI's and LLaMA CPP's parsers,
+  facilitating the extraction of meaningful information from free-text responses.
+- Integration with MongoDB for data persistence, demonstrating how LLM outputs can be stored, retrieved, and processed
+  for applications requiring database interactions.
+- Implementation of question-answering workflows and content verification methods that employ LLMs to validate,
+  analyze, and enhance textual content based on specific criteria such as relevance, accuracy, and clarity.
+- Techniques for reducing hallucinations and improving the reliability of LLM responses through the Chain of Verification
+  (CoV) and summarization strategies aimed at condensing extensive content into more manageable forms.
 
 Usage:
 This module is designed to be utilized in applications that require sophisticated text processing capabilities,
 including but not limited to content creation, document analysis, error detection in automated outputs,
 and the generation of actionable insights from unstructured data. It exemplifies the integration of LLMs
 into practical workflows, offering a blend of parsing, summarization, and content enhancement utilities
 that can be adapted to various domains and use cases.
 
 Dependencies:
-    - llm_core: A library providing core functionalities for interacting with LLMs.
-    - dotenv: For loading environment variables that may include API keys or database connection strings.
-    - requests: Used for making HTTP requests to external services, particularly when interacting with LLM APIs.
-    - dataclasses: For defining structured data types that facilitate the organization and manipulation of complex data.
+- llm_core: A library providing core functionalities for interacting with LLMs.
+- dotenv: For loading environment variables that may include API keys or database connection strings.
+- requests: Used for making HTTP requests to external services, particularly when interacting with LLM APIs.
+- dataclasses: For defining structured data types that facilitate the organization and manipulation of complex data.
 
 Note:
-    - The module includes placeholders and TODO comments indicating areas where customization and further development
-        are required to adapt the utilities to specific application needs or to integrate with different LLMs and databases.
+- The module includes placeholders and TODO comments indicating areas where customization and further development
+  are required to adapt the utilities to specific application needs or to integrate with different LLMs and databases.
 
 Examples:
-    - Parsing structured data from LLM responses for document analysis tasks.
-    - Conducting secondary analysis on textual content to assess its quality and relevance.
-    - Generating dense summaries of extensive articles or reports to extract key insights.
-
+- Parsing structured data from LLM responses for document analysis tasks.
+- Conducting secondary analysis on textual content to assess its quality and relevance.
+- Generating dense summaries of extensive articles or reports to extract key insights.
 """
 
 import codecs
 from dataclasses import asdict, dataclass, field
 import json
 from typing import Callable, List, Optional, Type, TypeVar
 
@@ -102,16 +101,17 @@
     tables: List[str] = field(default_factory=list)
     figures: List[str] = field(default_factory=list)
     cross_references: List[str] = field(default_factory=list)
 
 
 def patch_llm_core(llm: LLMBase):
     """llm_core ignores history when  calculating the context size for parsing.
-
-    This function monkey-patches and LLMBase object.  It can be removed once this PR is merged and celi is upgraded to a new version of llm-core.  PR: https://github.com/advanced-stack/py-llm-core/pull/12
+    This function monkey-patches and LLMBase object.
+     It can be removed once this PR is merged and celi is upgraded to a new version of llm-core.
+    PR: https://github.com/advanced-stack/py-llm-core/pull/12
     """
 
     def patched_sanitize_prompt(
         self,
         prompt,
         history=None,
         schema=None,
```

### Comparing `celi_framework-0.0.10/celi_framework/utils/llms.py` & `celi_framework-0.0.9/celi_framework/utils/llms.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,52 +3,49 @@
 such as OpenAI's GPT models. It provides utility functions that abstract away the complexities
 of sending prompts to the model, receiving responses, and handling various edge cases like
 rate limits or excessive context lengths. This module is particularly useful for applications
 that require robust and efficient interaction with LLMs for generating text, parsing information,
 or conducting analysis based on model responses.
 
 Features and Functionalities:
-    - `ask_split` and `quick_ask`: Core functions for sending prompts to OpenAI's API, with built-in
-        token counting, retries on failure, and verbose logging. `ask_split` is designed for more complex
-        interactions involving system messages and user prompts, while `quick_ask` offers a streamlined
-        approach for simple prompt-response cycles.
-    - Token Counter Decorators: Decorators that wrap around the core functions to enforce token limits,
-        ensuring that each query adheres to predefined constraints to manage costs and API usage efficiently.
-    - Custom Error Handling: Implements error handling mechanisms to gracefully recover from common
-        issues such as network timeouts, API rate limits, and context length exceedance. The
-        `ContextLengthExceededException` specifically addresses scenarios where the prompt exceeds
-        the maximum allowed context length, enabling the application to respond appropriately.
-    - Memory Tracking: Utilizes the `tracemalloc` library to monitor memory allocation and identify
-        potential inefficiencies, which is critical for applications processing large volumes of text
-        or managing numerous concurrent interactions with the LLM.
-
+- `ask_split` and `quick_ask`: Core functions for sending prompts to OpenAI's API, with built-in
+  token counting, retries on failure, and verbose logging. `ask_split` is designed for more complex
+  interactions involving system messages and user prompts, while `quick_ask` offers a streamlined
+  approach for simple prompt-response cycles.
+- Token Counter Decorators: Decorators that wrap around the core functions to enforce token limits,
+  ensuring that each query adheres to predefined constraints to manage costs and API usage efficiently.
+- Custom Error Handling: Implements error handling mechanisms to gracefully recover from common
+  issues such as network timeouts, API rate limits, and context length exceedance. The
+  `ContextLengthExceededException` specifically addresses scenarios where the prompt exceeds
+  the maximum allowed context length, enabling the application to respond appropriately.
+- Memory Tracking: Utilizes the `tracemalloc` library to monitor memory allocation and identify
+  potential inefficiencies, which is critical for applications processing large volumes of text
+  or managing numerous concurrent interactions with the LLM.
 """
 
-import functools
 import os
 import time
 from typing import Optional, Dict, List, Any, Tuple
 from pydantic import BaseModel
 import openai
 from openai.types.chat import ChatCompletion
 from requests import HTTPError
-
 from celi_framework.utils.codex import MongoDBUtilitySingleton
 from celi_framework.utils.token_counters import (
     token_counter_decorator_ask_split,
     token_counter_decorator_quick_ask,
 )
 from celi_framework.utils.log import app_logger
 from celi_framework.utils.exceptions import ContextLengthExceededException
+import tracemalloc
 
+tracemalloc.start()
 
 # Initialize the OpenAI client, using the OPENAI_API_KEY environment variable.
-@functools.lru_cache(1)
-def get_openai_client():
-    return openai.OpenAI(api_key=os.environ["OPENAI_API_KEY"])
+client = openai.OpenAI(api_key=os.environ["OPENAI_API_KEY"])
 
 
 class ToolDescription(BaseModel):
     name: str
     description: str
     parameters: Dict[str, Any]
 
@@ -248,12 +245,12 @@
     if codex:
         ret = codex.check_llm_cache(**kwargs)
         if ret:
             app_logger.debug("Using cached LLM response")
             return ChatCompletion.model_validate(ret["completion"])
         else:
             app_logger.debug("Caching LLM response")
-            result = get_openai_client().chat.completions.create(**kwargs)
+            result = client.chat.completions.create(**kwargs)
             codex.cache_llm_response(response={"completion": result.dict()}, **kwargs)
             return result
     else:
-        return get_openai_client().chat.completions.create(**kwargs)
+        return client.chat.completions.create(**kwargs)
```

### Comparing `celi_framework-0.0.10/celi_framework/utils/sql_utils.py` & `celi_framework-0.0.9/celi_framework/utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.10/celi_framework/utils/token_counters.py` & `celi_framework-0.0.9/celi_framework/utils/token_counters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 """
 The `utils.token_counters` module provides a set of tools for counting and managing tokens in text strings.
 This is particularly useful for applications interfacing with language models like GPT-4, where understanding
 and monitoring token usage is crucial for optimizing API calls and managing computational resources efficiently.
 
 Key Components:
-    - `token_counter_og`: A function that returns the exact number of tokens in a text string for a specified API,
-        using the `tiktoken` library for encoding. It's designed for cases where accuracy is paramount.
-    - `token_counter_est`: Provides a quick estimation of token count based on word count, using a heuristic approach.
-        This function is useful for scenarios where performance is a consideration, and an exact token count is less critical.
-    - `TokenCounter`: A singleton class that tracks the number of tokens in requests and responses. It supports
-        multiple instances (e.g., 'master', 'monitor') for different monitoring purposes within the same application,
-        ensuring that only one instance of each type is created.
-    - `get_master_counter_instance` and `get_monitor_counter_instance`: Factory functions that return singleton instances
-        of the `TokenCounter` class for specific purposes ('master' and 'monitor', respectively), ensuring application-wide
-        consistency in token counting.
-    - `token_counter_decorator_ask_split` and `token_counter_decorator_quick_ask`: Decorators designed to wrap API call
-        functions, counting tokens in both the request and response phases. These are particularly useful for integrating
-        token counting into existing API interactions, providing a seamless way to monitor and manage token usage.
+- `token_counter_og`: A function that returns the exact number of tokens in a text string for a specified API,
+  using the `tiktoken` library for encoding. It's designed for cases where accuracy is paramount.
+- `token_counter_est`: Provides a quick estimation of token count based on word count, using a heuristic approach.
+  This function is useful for scenarios where performance is a consideration, and an exact token count is less critical.
+- `TokenCounter`: A singleton class that tracks the number of tokens in requests and responses. It supports
+  multiple instances (e.g., 'master', 'monitor') for different monitoring purposes within the same application,
+  ensuring that only one instance of each type is created.
+- `get_master_counter_instance` and `get_monitor_counter_instance`: Factory functions that return singleton instances
+  of the `TokenCounter` class for specific purposes ('master' and 'monitor', respectively), ensuring application-wide
+  consistency in token counting.
+- `token_counter_decorator_ask_split` and `token_counter_decorator_quick_ask`: Decorators designed to wrap API call
+  functions, counting tokens in both the request and response phases. These are particularly useful for integrating
+  token counting into existing API interactions, providing a seamless way to monitor and manage token usage.
 
 Usage:
 This module is intended to be used in applications that require detailed monitoring and management of token usage,
 especially when interfacing with language models. It provides both precise and estimated token counting functions,
 along with a mechanism to track token usage throughout the application lifecycle via the `TokenCounter` class and
 its singleton instances. The decorators offer a convenient way to add token counting to API calls without significant
 modification to existing code.
 
-Example::
-
-    from utils.token_counters import get_master_counter_instance, token_counter_decorator_quick_ask
-
-    # Retrieve the master token counter instance
-    master_counter = get_master_counter_instance()
-
-    # Example API call function
-    @api_call_function
-    def fetch_data(api_endpoint, data):
-        return "Simulated response"
-
-    # Wrap the API call function with token counting
-    fetch_data_decorated = token_counter_decorator_quick_ask(fetch_data)
-
-    # Use the decorated function as normal
-    response = fetch_data_decorated(api_endpoint="http://example.com/api", data={"query": "example"}, token_counter=master_counter)
+Example:
+```python
+from utils.token_counters import get_master_counter_instance, token_counter_decorator_quick_ask
+
+# Retrieve the master token counter instance
+master_counter = get_master_counter_instance()
+
+# Example API call function
+@api_call_function
+def fetch_data(api_endpoint, data):
+    # Simulated API call logic
+    return "Simulated response"
+
+# Wrap the API call function with token counting
+fetch_data_decorated = token_counter_decorator_quick_ask(fetch_data)
+
+# Use the decorated function as normal
+response = fetch_data_decorated(api_endpoint="http://example.com/api", data={"query": "example"}, token_counter=master_counter)
+'''
 
 This module is a comprehensive solution for managing token usage, crucial for optimizing interactions with language models and other token-based APIs.
 """
 
 import functools
 import tiktoken
 from celi_framework.utils.log import app_logger
```

### Comparing `celi_framework-0.0.10/celi_framework/utils/utils.py` & `celi_framework-0.0.9/celi_framework/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 """
 The `utils.utils` module encapsulates a variety of utility functions and classes designed to support and enhance
 the development of Python applications. This module includes functionalities for colorized logging, JSON and text
 file manipulation, dynamic content generation, and more, offering a robust toolkit for developers.
 
 Features:
-    - Colorized Logging: Utilizes ANSI escape codes to colorize log messages for enhanced readability. Includes a custom
-        logging handler `ColorizingStreamHandler` that integrates with MongoDB for advanced logging purposes.
-    - JSON File Manipulation: Provides functions `load_json`, `save_json` for loading and saving JSON data, streamlining
-        data handling and storage.
-    - Text Processing: Offers utilities for reading text files (`read_txt`), manipulating JSON objects (`remove_newlines_from_json`,
-        `is_json_cleaned_of_newline`), and more, facilitating the processing and analysis of textual data.
-    - Dynamic Content Generation: Contains methods for generating hash IDs (`generate_hash_id`), creating and manipulating
-        data structures (`shuffle_json_ordering`, `transform_dict_to_flat_schema`), and comparing JSON files (`compare_json_files`,
-        `detailed_compare_json_files`), aiding in the creation and management of dynamic content.
-    - File and Directory Operations: Includes functions for working with files and directories (`find_latest_file`,
-        `make_list_of_dirs`), enabling efficient file system navigation and organization.
-    - Miscellaneous Utilities: Offers a variety of additional tools, such as a decorator for measuring function execution
-        time (`time_it`), and methods for modifying text and data structures to meet specific criteria (`remove_text_chunk`,
-        `dequeue_all_matching`).
-
+- Colorized Logging: Utilizes ANSI escape codes to colorize log messages for enhanced readability. Includes a custom
+  logging handler (`ColorizingStreamHandler`) that integrates with MongoDB for advanced logging purposes.
+- JSON File Manipulation: Provides functions (`load_json`, `save_json`) for loading and saving JSON data, streamlining
+  data handling and storage.
+- Text Processing: Offers utilities for reading text files (`read_txt`), manipulating JSON objects (`remove_newlines_from_json`,
+  `is_json_cleaned_of_newline`), and more, facilitating the processing and analysis of textual data.
+- Dynamic Content Generation: Contains methods for generating hash IDs (`generate_hash_id`), creating and manipulating
+  data structures (`shuffle_json_ordering`, `transform_dict_to_flat_schema`), and comparing JSON files (`compare_json_files`,
+  `detailed_compare_json_files`), aiding in the creation and management of dynamic content.
+- File and Directory Operations: Includes functions for working with files and directories (`find_latest_file`,
+  `make_list_of_dirs`), enabling efficient file system navigation and organization.
+- Miscellaneous Utilities: Offers a variety of additional tools, such as a decorator for measuring function execution
+  time (`time_it`), and methods for modifying text and data structures to meet specific criteria (`remove_text_chunk`,
+  `dequeue_all_matching`).
 
 Usage:
 This module is designed to be imported and used in Python applications that require advanced logging capabilities,
 efficient data handling, and manipulation, as well as dynamic content generation. Its modular design allows for
 easy integration into existing projects, enhancing functionality without significant refactoring.
-
 """
 
 import importlib
 from pathlib import Path
 import random
 from datetime import datetime
 import hashlib
```

### Comparing `celi_framework-0.0.10/pyproject.toml` & `celi_framework-0.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "celi-framework"
-version = "0.0.10"
+version = "0.0.9"
 description = "Controller-Embedded Language Interactions - facilitates the entire lifecycle of document processing, from pre-processing and embedding to post-monitoring and quality assessment."
 authors = ["Jan-Samuel Wagner <jwab@genmab.com>","Dave DeCaprio <daved@alum.mit.edu>"]
-license = "MIT"
+license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/x3n0cr4735/celi"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
@@ -20,36 +20,24 @@
 evaluate = ">=0.4.1"
 py-llm-core = ">=2.8.2"
 pymongo = ">=4.6.2"
 python-dotenv = ">=1.0.0"
 requests-cache = ">=1.2.0"
 llama-index = ">=0.10.23"
 llama-index-vector-stores-chroma = "^0.1.6"
-scikit-learn = "^1.4.2"
-pymupdf = "^1.24.1"
-python-docx = "^1.1.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = ">=7.4.4"
 pytest-asyncio = ">=0.23.3"
 
+
+
 [tool.poetry.group.dev.dependencies]
 ipykernel = ">=6.29.3"
 
-[tool.poetry.group.docs.dependencies]
-sphinx = "^7.2.6"
-myst-parser = "^2.0.0"
-furo = "^2023.9.10"
-sphinxext-opengraph = "^0.9.1"
-sphinx-copybutton = "^0.5.2"
-sphinx-autobuild = "^2021.3.14"
-protobuf = ">=4.21.6" # Added to address build issues with readthedocs.
-cffi = ">=1.10.0" # Added to address build issues with readthedocs. pyo3_runtime.PanicException: Python API call failed
-sphinx-autodoc-typehints = "^2.0.0"
-
 [tool.pytest.ini_options]
 log_level="DEBUG"
 log_cli=true
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

