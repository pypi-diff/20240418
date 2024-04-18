# Comparing `tmp/equivalent_llm-0.1.0.tar.gz` & `tmp/equivalent_llm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equivalent_llm-0.1.0.tar", last modified: Mon Apr  8 06:38:40 2024, max compression
+gzip compressed data, was "equivalent_llm-0.2.0.tar", last modified: Thu Apr 18 07:32:27 2024, max compression
```

## Comparing `equivalent_llm-0.1.0.tar` & `equivalent_llm-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1469 2024-04-04 07:47:09.583011 equivalent_llm-0.1.0/LICENSE
--rw-r--r--   0        0        0     4629 2024-04-05 07:32:17.227264 equivalent_llm-0.1.0/README.md
--rw-r--r--   0        0        0     2050 2024-04-08 06:38:40.342827 equivalent_llm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     9089 2024-04-04 07:47:09.590699 equivalent_llm-0.1.0/src/equivalent_llm/__init__.py
--rw-r--r--   0        0        0     5813 2024-04-04 07:47:09.591909 equivalent_llm-0.1.0/src/equivalent_llm/function/__init__.py
--rw-r--r--   0        0        0     7484 2024-04-04 07:47:09.592935 equivalent_llm-0.1.0/src/equivalent_llm/function_call/__init__.py
--rw-r--r--   0        0        0    13045 2024-04-04 07:47:09.593555 equivalent_llm-0.1.0/src/equivalent_llm/function_call/v1/__init__.py
--rw-r--r--   0        0        0     4203 2024-04-04 07:47:09.594100 equivalent_llm-0.1.0/src/equivalent_llm/function_call/v2/__init__.py
--rw-r--r--   0        0        0     8024 2024-04-04 07:47:09.594504 equivalent_llm-0.1.0/src/equivalent_llm/reservation.py
--rw-r--r--   0        0        0    14442 2024-04-04 07:47:09.595119 equivalent_llm-0.1.0/src/equivalent_llm/testers/__init__.py
--rw-r--r--   0        0        0     2479 2024-04-04 07:47:09.595469 equivalent_llm-0.1.0/src/equivalent_llm/user.py
--rw-r--r--   0        0        0        0 2024-04-05 07:32:17.228429 equivalent_llm-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     5514 1970-01-01 00:00:00.000000 equivalent_llm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1469 2024-04-18 07:32:09.404541 equivalent_llm-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5155 2024-04-18 07:32:09.404541 equivalent_llm-0.2.0/README.md
+-rw-r--r--   0        0        0     2050 2024-04-18 07:32:27.192814 equivalent_llm-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9641 2024-04-18 07:32:09.408542 equivalent_llm-0.2.0/src/equivalent_llm/__init__.py
+-rw-r--r--   0        0        0     5896 2024-04-18 07:32:09.408542 equivalent_llm-0.2.0/src/equivalent_llm/function/__init__.py
+-rw-r--r--   0        0        0     7487 2024-04-18 07:32:09.408542 equivalent_llm-0.2.0/src/equivalent_llm/function_call/__init__.py
+-rw-r--r--   0        0        0    13831 2024-04-18 07:32:09.408542 equivalent_llm-0.2.0/src/equivalent_llm/function_call/v1/__init__.py
+-rw-r--r--   0        0        0     4203 2024-04-18 07:32:09.408542 equivalent_llm-0.2.0/src/equivalent_llm/function_call/v2/__init__.py
+-rw-r--r--   0        0        0     8506 2024-04-18 07:32:09.408542 equivalent_llm-0.2.0/src/equivalent_llm/reservation.py
+-rw-r--r--   0        0        0    14507 2024-04-18 07:32:09.408542 equivalent_llm-0.2.0/src/equivalent_llm/testers/__init__.py
+-rw-r--r--   0        0        0     2738 2024-04-18 07:32:09.408542 equivalent_llm-0.2.0/src/equivalent_llm/user.py
+-rw-r--r--   0        0        0        0 2024-04-18 07:32:09.408542 equivalent_llm-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     6040 1970-01-01 00:00:00.000000 equivalent_llm-0.2.0/PKG-INFO
```

### Comparing `equivalent_llm-0.1.0/LICENSE` & `equivalent_llm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `equivalent_llm-0.1.0/README.md` & `equivalent_llm-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,48 @@
 # Validation tool to compare a generated context by sLLM to reference context
 
 생성된 문장(Function call 또는 Reservation Board (a.k.a Formatted output))과 기준이 되는 문장을 비교하여 두 문자열이 동일한지 여부를 확인합니다.
 
+## Validataion criteria
+
+### Equivalence test
+
+tests whether the generated sentence is equivalent to the reference sentence or not
+
+### Consistency test
+
+tests whether the generated sentence is consistent with the given information or not
+
+### Grammar test
+
+tests whether the generated sentence is grammatically correct or not
+
+### Elegant test
+
+tests whether the generated sentence is firmly well-structed to human readablity or not
+
+### Etc
+
+-   Function name matching
+-   Arugments matching
+-   Required arguments
+
 ## Input data format
 
+### JSON string
+
 ```json
 {
-    "context": "<s>[INST] <<SYS>>\nYou are a helpful and respectful movie ticketing assistant.\nYou"re actively involved in a three-way conversation with "user", "function" (the function helper other than you), ...",
+    "context": "<s>[INST] <<SYS>>\nYou are a helpful and respectful movie ticketing assistant.\nYou\"re actively involved in a three-way conversation with \"user\", \"function\" (the function helper other than you), ...",
     "answer": "{\"function_call\": {\"name\": \"extract_date_time\", \"arguments\": \"{\\\"query\\\":\\\"현재 시간을 알려주세요~\\\"}\"}, \"role\": \"assistant\", \"content\": null} ",
     "generated": "{\"function_call\": {\"name\": \"extract_date_time\", \"arguments\": \"{\\\"query\\\":\\\"현재 시간을 알려주세요\\\"}\"}, \"role\": \"assistant\", \"content\": null} "
 }
 ```
 
-## Load data from CSV file
+### CSV file
 
 ```csv
 index, context, answer, generated
 0,<s>[INST] <<SYS>>\nYou are a...,{"function_call": {...,{"function_call": {...
 ```
 
 ## Installation
```

### Comparing `equivalent_llm-0.1.0/pyproject.toml` & `equivalent_llm-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 max-complexity = 10
 
 [tool.pdm]
 distribution = true
 
 [project]
 name = "equivalent_llm"
-version = "0.1.0"
+version = "0.2.0"
 description = "Validation tool to compare a generated context by sLLM to reference context"
 authors = [
     { name = "Sung Gon Yi", email = "skonmeme@sk.com" },
 ]
 dependencies = [
     "langchain-core~=0.1.30",
     "langchain>=0.1.11",
```

### Comparing `equivalent_llm-0.1.0/src/equivalent_llm/__init__.py` & `equivalent_llm-0.2.0/src/equivalent_llm/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from langchain_openai import ChatOpenAI
 
 from equivalent_llm import function, function_call, reservation, user
 
 class EquvalentLLM:
 
     configurations = {
-        'temperature': 0.7,
+        'temperature': 0.15,
         'model': 'gpt-4-0125-preview',
         'prompt_engine': 'OpenAI',
         'parse_instruction': True,
         'test_consistency': True,
         'test_grammar': True,
         'test_elegance': True,
         'api': 'v1',
@@ -138,17 +138,36 @@
             self.parse_instructions()
         if self.parsed_reference is None:
             self.parsed_reference = self.parse_llm(self.reference, True)
         if self.parsed_generated is None:
             self.parsed_generated = self.parse_llm(self.generated)
 
         if self.parsed_reference.get('status') == 'fail':
-            return { 'passed': False, 'count': {'passed': 0, 'total': 1}, 'status': 'fail', 'source': 'reference', 'error': f"Failed to parse reference (invalid JSON string): {self.parsed_reference['error']}" }
+            return {
+                'target': 'Unknown',
+                'passed': False,
+                'count': {'passed': 0, 'total': 1},
+                'status': 'fail',
+                'source': 'reference',
+                'raw_reference': self.reference,
+                'raw_generated': self.generated,
+                'error': f"Failed to parse reference (invalid JSON string): {self.parsed_reference['error']}"
+            }
         if self.parsed_generated.get('status') == 'fail':
-            return { 'passed': False, 'count': {'passed': 0, 'total': 1}, 'status': 'fail', 'source': 'generated', 'error': f"Failed to parse generated (invalid JSON string): {self.parsed_generated['error']}" }
+            target = 'reservation' if self.validation_type == 'reservation' else 'function call'
+            return {
+                'target': target,
+                'passed': False,
+                'count': {'passed': 0, 'total': 1},
+                'status': 'fail',
+                'source': 'generated',
+                'reference': self.parsed_reference,
+                'raw_generated': self.generated,
+                'error': f"Failed to parse generated (invalid JSON string): {self.parsed_generated['error']}"
+            }
 
         if self.validation_type == 'function_call':
             validation_reports = function_call.validate(
                 self.parsed_reference['name'],
                 self.parsed_generated,
                 self.parsed_reference,
                 self.parsed_instructions,
```

### Comparing `equivalent_llm-0.1.0/src/equivalent_llm/function/__init__.py` & `equivalent_llm-0.2.0/src/equivalent_llm/function/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,17 +136,20 @@
             'movie_theater': __get_entity(movie_theater, content),
             'movie_schedules': __get_entity(movie_schedules, content),
         },
         'role': 'function',
     }
 
 def book_movie_tickets(content: str, instructions: list, prompt_engine: Any) -> dict:
+    url = r"(?<=URL:\s).*"
     return {
         'name': 'book_movie_tickets',
-        'parameters': {},
+        'parameters': {
+            'url': __get_entity(url, content),
+        },
         'role': 'function',
     }
 
 def search_movie_information(content: str, instructions: list, prompt_engine: Any) -> dict:
     movie_title = r"(?<='title':\s).*(?=\s)"
     movie_snippet = r"(?<=snippet:\s).*"
```

### Comparing `equivalent_llm-0.1.0/src/equivalent_llm/function_call/__init__.py` & `equivalent_llm-0.2.0/src/equivalent_llm/function_call/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,16 @@
                     'not_in_required': p,
                 },
             }
     return {'passed': True}
 
 def check_paired_arguments(generated_keys: dict, reference_keys: dict) -> dict:
     if generated_keys != reference_keys:
-        not_in_reference = list(filter(lambda v: v not in generated_keys, reference_keys))
-        not_in_generated = list(filter(lambda v: v not in reference_keys, generated_keys))
+        not_in_generated = list(filter(lambda v: v not in generated_keys, reference_keys))
+        not_in_reference = list(filter(lambda v: v not in reference_keys, generated_keys))
         return {
             'passed': False,
             'level': 'severe',
             'evidance': {
                 'not_in_reference': not_in_reference,
                 'not_in_generated': not_in_generated,
             }
@@ -113,28 +113,28 @@
         match(api_version):
             case 'v1':
                 DEFINITION = getattr(v1, function_name.upper())
             case _:
                 DEFINITION = getattr(v2, function_name.upper())
     except AttributeError:
         logger.error(f'Function {function_name} not found in equivalent_llm')
-        return {'passed': False, 'count': {'total': {'passed': 0, 'total': 1}}, 'tests': {}, 'reason': 'Function not found', 'level': 'fatal'}
+        return {'passed': False, 'counts': {'total': {'passed': 0, 'total': 1}}, 'tests': {}, 'reason': 'Function not found', 'level': 'fatal'}
 
     reports = {
         'target': function_name,
         'tests': {
             'equivalence': [],
             'consistency': [],
             'grammar': [],
             'elegance': [],
         },
     }
 
     if generated['type'] is not reference['type']:
-        return {'passed': False, 'count': {'total': {'passed': 0, 'total': 1}}, 'tests': {}, 'reason': 'function call is not generated', 'level': 'fatal'}
+        return {'passed': False, 'counts': {'total': {'passed': 0, 'total': 1}}, 'tests': {}, 'reason': 'function call is not generated', 'level': 'fatal'}
 
     # counters
 
     equivalence_counter = testers.TestCounter()
     consistency_counter = testers.TestCounter()
     grammar_counter = testers.TestCounter()
     elegance_counter = testers.TestCounter()
@@ -210,15 +210,15 @@
             )
             reports['tests']['elegance'].append({'argument': name, **elegance_result})
             elegance_counter.count(elegance_result)
 
     total_counter = equivalence_counter + consistency_counter + grammar_counter + elegance_counter
 
     reports['passed'] = total_counter.fully_passed()
-    reports['count'] = {
+    reports['counts'] = {
         'total': total_counter.settlement(),
         'equivalence': equivalence_counter.settlement(),
         'consistency': consistency_counter.settlement(),
         'grammar': grammar_counter.settlement(),
         'elegance': elegance_counter.settlement(),
         'etc': etc_counter.settlement(),
     }
```

### Comparing `equivalent_llm-0.1.0/src/equivalent_llm/function_call/v1/__init__.py` & `equivalent_llm-0.2.0/src/equivalent_llm/function_call/v1/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                 'tester': 'get_grammar_tester',
             },
         }
     }
 }
 
 EXTRACT_COORDINATES = {
-    'required': ['query'],
+    'required': [],
     'parameters': {
         'query': {
             'name': 'query',
             'equivalence': {
                 'tester': 'get_equivalence_tester',
                 'category': 'date, time, time range, date range',
             },
@@ -41,15 +41,15 @@
                 'tester': 'get_grammar_tester',
             },
         }
     }
 }
 
 GET_MOVIE_THEATERS = {
-    'required': ['latitude', 'longitude'],
+    'required': [],
     'parameters': {
         'movie_title': {
             'name': 'movie_title',
             'equivalence': {
                 'tester': 'get_equivalence_tester',
                 'category': 'movie title',
             },
@@ -88,28 +88,28 @@
             'equivalence': {
                 'tester': 'get_equivalence_tester',
                 'category': 'datetime, YYYY-mm-dd HH:MM:SS',
             },
             'consistency': {
                 'tester': 'get_category_consistency_tester',
                 'category': 'datetime, YYYY-mm-dd HH:MM:SS',
-                'comment': 'If the start time is not provided explicitly, it should be inferred from the compound of the current time and user request.',
+                'comment': 'Start point of time range. If the start time is not provided explicitly, it should be inferred from the compound of the current time and user request. Also, if there is not stated time, base time is kept as 00:00:00.',
                 'instruction': 'all',
             },
         },
         'end_time': {
             'name': 'end_time',
             'equivalence': {
                 'tester': 'get_equivalence_tester',
                 'category': 'datetime, YYYY-mm-dd HH:MM:SS',
             },
             'consistency': {
                 'tester': 'get_category_consistency_tester',
                 'category': 'datetime, YYYY-mm-dd HH:MM:SS',
-                'comment': 'If the end time is not provided explicitly, it should be inferred from the compound of the current time and user request.',
+                'comment': 'End point of time range. If the end time is not provided explicitly, it should be inferred from the compound of the current time and user request. Also, if there is not stated time, base time is kept as 23:59:59.',
                 'instruction': 'all',
             },
         },
         'selected_benefit': {
             'name': 'selected_benefit',
             'equivalence': {
                 'tester': 'get_equivalence_tester',
@@ -132,63 +132,65 @@
             'equivalence': {
                 'tester': 'get_equivalence_tester',
                 'category': 'datetime, YYYY-mm-dd HH:MM:SS',
             },
             'consistency': {
                 'tester': 'get_category_consistency_tester',
                 'category': 'datetime, YYYY-mm-dd HH:MM:SS',
-                'comment': 'If the start time is not provided explicitly, it should be inferred from the compound of the current time and user request.',
+                'comment': 'Start point of time range. If the start time is not provided explicitly, it should be inferred from the compound of the current time and user request. Also, if there is not stated time, base time is kept as 00:00:00.',
                 'instruction': 'all',
             },
         },
         'end_time': {
             'name': 'end_time',
             'equivalence': {
                 'tester': 'get_equivalence_tester',
                 'category': 'datetime, YYYY-mm-dd HH:MM:SS',
             },
             'consistency': {
                 'tester': 'get_category_consistency_tester',
                 'category': 'datetime, YYYY-mm-dd HH:MM:SS',
-                'comment': 'If the end time is not provided explicitly, it should be inferred from the compound of the current time and user request.',
+                'comment': 'End point of time range. If the end time is not provided explicitly, it should be inferred from the compound of the current time and user request. Also, if there is not stated time, base time is kept as 23:59:59.',
                 'instruction': 'all',
             },
         },
         'movie_theater': {
             'name': 'movie_theater',
             'equivalence': {
                 'tester': 'get_equivalence_tester',
                 'category': 'theater name',
             },
             'consistency': {
                 'tester': 'get_category_consistency_tester',
                 'category': 'theater name',
+                'comment': 'Ignore words like "극장", "상영관", "영화관", and "theater"',
                 'instruction': 'all',
             },
         },
         'query': {
             'name': 'query',
             'equivalence': {
                 'tester': 'get_equivalence_tester',
-                'category': 'movie title',
+                'category': 'actor, movie title, movie series, movie genre, country',
             },
             'consistency': {
                 'tester': 'get_category_consistency_tester',
-                'category': 'movie title',
+                'category': 'actor, movie title, movie series, movie genre, country',
+                'comment': 'Ignore words like "영화", and "movie"',
                 'instruction': 'latest',
             },
             'grammar': {
                 'tester': 'get_grammar_tester',
             },
         },
     },
 }
 
 GET_MOVIE_SCHEDULES = {
-    'required' : ['movie_title', 'movie_theater'],
+    'required' : ['movie_title', 'movie_theater', 'start_time'],
     'parameters': {
         'movie_title': {
             'name': 'movie_title',
             'equivalence': {
                 'tester': 'get_equivalence_tester',
                 'category': 'movie title',
             },
@@ -215,28 +217,28 @@
             'equivalence': {
                 'tester': 'get_equivalence_tester',
                 'category': 'datetime, YYYY-mm-dd HH:MM:SS',
             },
             'consistency': {
                 'tester': 'get_category_consistency_tester',
                 'category': 'datetime, YYYY-mm-dd HH:MM:SS',
-                'comment': 'If the start time is not provided explicitly, it should be inferred from the compound of the current time and user request.',
+                'comment': 'Start point of time range. If the start time is not provided explicitly, it should be inferred from the compound of the current time and user request. Also, if there is not stated time, base time is kept as 00:00:00.',
                 'instruction': 'all',
             },
         },
         'end_time': {
             'name': 'end_time',
             'equivalence': {
                 'tester': 'get_equivalence_tester',
                 'category': 'datetime, YYYY-mm-dd HH:MM:SS',
             },
             'consistency': {
                 'tester': 'get_category_consistency_tester',
                 'category': 'datetime, YYYY-mm-dd HH:MM:SS',
-                'comment': 'If the end time is not provided explicitly, it should be inferred from the compound of the current time and user request.',
+                'comment': 'End point of time range. If the end time is not provided explicitly, it should be inferred from the compound of the current time and user request. Also, if there is not stated time, base time is kept as 23:59:59.',
                 'instruction': 'all',
             },
         },
         'selected_benefit': {
             'name': 'selected_benefit',
             'equivalence': {
                 'tester': 'get_equivalence_tester',
@@ -294,15 +296,15 @@
             'name': 'user_consent',
             'equivalence': {
                 'tester': 'get_equivalence_tester',
                 'category': 'consent',
             },
             'consistency': {
                 'tester': 'get_enum_consistency_tester',
-                'items': ["true", "false"],
+                'items': [True, False],
                 'instruction': 'all',
             },
         },
     }
 }
 
 SEARCH_MOVIE_INFORMATION = {
```

### Comparing `equivalent_llm-0.1.0/src/equivalent_llm/function_call/v2/__init__.py` & `equivalent_llm-0.2.0/src/equivalent_llm/function_call/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `equivalent_llm-0.1.0/src/equivalent_llm/reservation.py` & `equivalent_llm-0.2.0/src/equivalent_llm/reservation.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 RESERVATION_BOARD = {
     'answer': {
         'name': 'answer',
         'equivalence': {
             'tester': 'get_equivalence_tester',
             'category': 'answer for a question or a request of user, suggestion of related to movie reservation, or confirmation of reservation',
+            #'comment': 'Consider seriously whether the country of production of the movie is included. If the country of production is not specified, targeting movies MUST be regraded as movies from all countries.',
+            'comment': '영화의 평가에 있어 제작 국가 및 개봉 국가의 구분은 중요합니다. 제작 국가가 명시되지 않은 경우, 해당 영화를 모든 국가의 영화로 간주하며, 이는 평가 시 고려되어야 합니다.',
         },
         'consistency': {
             'tester': 'get_category_consistency_tester',
             'instruction': 'all',
             'category': 'answer for a question or a request of user, suggestion of related to movie reservation, or confirmation of reservation',
         },
         'grammar': {
@@ -159,15 +161,15 @@
         'selected_schedule',
         'selected_time',
         'reference_number',
         'template',
     ]
 
     if generated['type'] is not reference['type']:
-        return {'passed': False, 'count': {'total': {'passed': 0, 'total': 1}}, 'tests': {}, 'reason': 'reservation is not generated ', 'level': 'fatal'}
+        return {'passed': False, 'counts': {'total': {'passed': 0, 'total': 1}}, 'tests': {}, 'reason': 'reservation is not generated ', 'level': 'fatal'}
 
     equivalence_counter = testers.TestCounter()
     consistency_counter = testers.TestCounter()
     grammar_counter = testers.TestCounter()
     elegance_counter = testers.TestCounter()
 
     for element in elements:
@@ -230,15 +232,15 @@
                 )
                 reports['tests']['elegance'].append({'element': element, **elegance_result})
                 elegance_counter.count(elegance_result)
 
     total_counter = equivalence_counter + consistency_counter + grammar_counter + elegance_counter
 
     reports['passed'] = total_counter.fully_passed()
-    reports['count'] = {
+    reports['counts'] = {
         'total': total_counter.settlement(),
         'equivalence': equivalence_counter.settlement(),
         'consistency': consistency_counter.settlement(),
         'grammar': grammar_counter.settlement(),
         'elegance': elegance_counter.settlement(),
     }
     return reports
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `equivalent_llm-0.1.0/src/equivalent_llm/testers/__init__.py` & `equivalent_llm-0.2.0/src/equivalent_llm/testers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,16 @@
     def settlement(self):
         return {'passed': self.passed, 'total': self.total}
 
 
 FormatTemplate = """- format instructions: {format_instructions}"""
 PreknowledgeTemplate = """- Related categories: {category}
 - given information: {information}"""
-EquivalenceTemplate = """- reference sentence: {reference}
+EquivalenceTemplate = """{comment}
+- reference sentence: {reference}
 - target sentence: {generated}
 Question: Is target sentence equivalent to reference sentence?
 """
 class EquivalenceResult(BaseModel):
     passed: bool = Field(description="Whether equivalent or not")
     score: int = Field(description="Equivalence score from 0 to 100")
     evidence: str = Field(description="The evidence of passed value")
@@ -63,14 +64,15 @@
             prompt_template = ChatPromptTemplate.from_messages(
                 [system_template, ai_template, human_template]
             )
             final_prompt = prompt_template.format_prompt(
                 reference=reference_value,
                 generated=value,
                 category=definition['category'],
+                comment=definition.get('comment', ''),
                 information=instructions if instructions is not None else "No information",
                 format_instructions=equivalence_parser.get_format_instructions(),
             ).to_messages()
             logger.debug(f"Equivalence Prompt: {final_prompt}")
             result = prompt_engine(final_prompt)
 
             # markdown json format
@@ -198,15 +200,15 @@
             human_template = HumanMessagePromptTemplate.from_template(EnumConsistencyTemplate)
             prompt_template = ChatPromptTemplate.from_messages(
                 [system_template, ai_template, human_template]
             )
             final_prompt = prompt_template.format_prompt(
                 generated=value,
                 given_information=instructions if instructions is not None else "No information",
-                enum_items=definition['itmes'],
+                enum_items=definition['items'],
                 comment=definition.get('comment', ''),
                 format_instructions=equivalence_parser.get_format_instructions(),
             ).to_messages()
             logger.debug(f"Enum Consistency Prompt: {final_prompt}")
             result = prompt_engine(final_prompt)
             # markdown json format
             if result.content.startswith("```json"):
```

### Comparing `equivalent_llm-0.1.0/src/equivalent_llm/user.py` & `equivalent_llm-0.2.0/src/equivalent_llm/user.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,20 +7,24 @@
 
 from pydantic.v1 import BaseModel, Field
 
 __system_template = '''
 - format instructions: {format_instructions}
 - When you reserve a movie at movie theater, you should think following considerations.
 - DATETIME: time, data, and datetime
+- THEATER': theater name. Specially it includes LOCATION + '극장', LOCATION + '상영관', or LOCATION + 'THEATER'.
 - LOCATION': district, place name, landmark, and company name near by theater, and so on. MUST NOT include theater name.
 - COORDINATES: coordinates by longitude and latitude
-- THEATER': theater name
 - ACTOR: well-known actor or actress names
-- MOVIE_GENRE: movie genre, which also includes special circumstance like "date" and "relaxation"
-- MOVIE_TITLE: specific movie title. Generic name like "영화" MUST NOT belong in this element.
+- NOWSHOWING: now showing in theaters
+- CREATING_COUNTRY: creating country of movie
+- SHOWING_COUNTRY: showing country
+- MOVIE_GENRE: movie genre, which also includes special circumstance like "mood", "dating", and "relaxation".
+- MOVIE_SERIES: movie series name, which is not specific movie title but is a group of movies.
+- MOVIE_TITLE: specific movie title.
 - DECISION: acception or rejection in English or Korean
 - RESERVATION: reservation, booking, or cancelation
 '''
 
 __human_template = '''
 - What kinds of elements are contained below message? Choose the element type at first and describe the evidence of decision.
 - MUST exclude elements out of instruction
```

### Comparing `equivalent_llm-0.1.0/PKG-INFO` & `equivalent_llm-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equivalent_llm
-Version: 0.1.0
+Version: 0.2.0
 Summary: Validation tool to compare a generated context by sLLM to reference context
 Author-Email: Sung Gon Yi <skonmeme@sk.com>
 License: BSD-3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/sktaiflow/equivalent_llm
@@ -22,25 +22,51 @@
 Requires-Dist: tqdm>=4.66.2
 Description-Content-Type: text/markdown
 
 # Validation tool to compare a generated context by sLLM to reference context
 
 생성된 문장(Function call 또는 Reservation Board (a.k.a Formatted output))과 기준이 되는 문장을 비교하여 두 문자열이 동일한지 여부를 확인합니다.
 
+## Validataion criteria
+
+### Equivalence test
+
+tests whether the generated sentence is equivalent to the reference sentence or not
+
+### Consistency test
+
+tests whether the generated sentence is consistent with the given information or not
+
+### Grammar test
+
+tests whether the generated sentence is grammatically correct or not
+
+### Elegant test
+
+tests whether the generated sentence is firmly well-structed to human readablity or not
+
+### Etc
+
+-   Function name matching
+-   Arugments matching
+-   Required arguments
+
 ## Input data format
 
+### JSON string
+
 ```json
 {
-    "context": "<s>[INST] <<SYS>>\nYou are a helpful and respectful movie ticketing assistant.\nYou"re actively involved in a three-way conversation with "user", "function" (the function helper other than you), ...",
+    "context": "<s>[INST] <<SYS>>\nYou are a helpful and respectful movie ticketing assistant.\nYou\"re actively involved in a three-way conversation with \"user\", \"function\" (the function helper other than you), ...",
     "answer": "{\"function_call\": {\"name\": \"extract_date_time\", \"arguments\": \"{\\\"query\\\":\\\"현재 시간을 알려주세요~\\\"}\"}, \"role\": \"assistant\", \"content\": null} ",
     "generated": "{\"function_call\": {\"name\": \"extract_date_time\", \"arguments\": \"{\\\"query\\\":\\\"현재 시간을 알려주세요\\\"}\"}, \"role\": \"assistant\", \"content\": null} "
 }
 ```
 
-## Load data from CSV file
+### CSV file
 
 ```csv
 index, context, answer, generated
 0,<s>[INST] <<SYS>>\nYou are a...,{"function_call": {...,{"function_call": {...
 ```
 
 ## Installation
```

