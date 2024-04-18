# Comparing `tmp/LLMEasyTools-0.5.tar.gz` & `tmp/LLMEasyTools-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LLMEasyTools-0.5.tar", last modified: Fri Mar 22 17:15:32 2024, max compression
+gzip compressed data, was "LLMEasyTools-0.6.tar", last modified: Thu Apr 18 06:56:55 2024, max compression
```

## Comparing `LLMEasyTools-0.5.tar` & `LLMEasyTools-0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-03-22 17:15:32.938051 LLMEasyTools-0.5/
--rw-rw-r--   0 zby       (1000) zby       (1000)    11357 2024-03-03 11:08:50.000000 LLMEasyTools-0.5/LICENSE
-drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-03-22 17:15:32.938051 LLMEasyTools-0.5/LLMEasyTools.egg-info/
--rw-r--r--   0 zby       (1000) zby       (1000)    16948 2024-03-22 17:15:32.000000 LLMEasyTools-0.5/LLMEasyTools.egg-info/PKG-INFO
--rw-rw-r--   0 zby       (1000) zby       (1000)      407 2024-03-22 17:15:32.000000 LLMEasyTools-0.5/LLMEasyTools.egg-info/SOURCES.txt
--rw-rw-r--   0 zby       (1000) zby       (1000)        1 2024-03-22 17:15:32.000000 LLMEasyTools-0.5/LLMEasyTools.egg-info/dependency_links.txt
--rw-rw-r--   0 zby       (1000) zby       (1000)       54 2024-03-22 17:15:32.000000 LLMEasyTools-0.5/LLMEasyTools.egg-info/requires.txt
--rw-rw-r--   0 zby       (1000) zby       (1000)       15 2024-03-22 17:15:32.000000 LLMEasyTools-0.5/LLMEasyTools.egg-info/top_level.txt
--rw-rw-r--   0 zby       (1000) zby       (1000)       67 2024-03-03 11:08:50.000000 LLMEasyTools-0.5/MANIFEST.in
--rw-r--r--   0 zby       (1000) zby       (1000)    16948 2024-03-22 17:15:32.938051 LLMEasyTools-0.5/PKG-INFO
--rw-rw-r--   0 zby       (1000) zby       (1000)     3202 2024-03-04 13:15:40.000000 LLMEasyTools-0.5/README.md
-drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-03-22 17:15:32.938051 LLMEasyTools-0.5/examples/
--rw-rw-r--   0 zby       (1000) zby       (1000)     1290 2024-03-05 07:21:59.000000 LLMEasyTools-0.5/examples/extract_user_details.py
--rw-rw-r--   0 zby       (1000) zby       (1000)      863 2024-03-05 07:22:09.000000 LLMEasyTools-0.5/examples/extract_user_details_by_function.py
--rw-rw-r--   0 zby       (1000) zby       (1000)     3360 2024-03-05 07:22:24.000000 LLMEasyTools-0.5/examples/stateful_search.py
-drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-03-22 17:15:32.938051 LLMEasyTools-0.5/llm_easy_tools/
--rw-rw-r--   0 zby       (1000) zby       (1000)    14467 2024-03-20 22:48:41.000000 LLMEasyTools-0.5/llm_easy_tools/__init__.py
--rw-rw-r--   0 zby       (1000) zby       (1000)      988 2024-03-22 17:06:17.000000 LLMEasyTools-0.5/pyproject.toml
--rw-rw-r--   0 zby       (1000) zby       (1000)       38 2024-03-22 17:15:32.938051 LLMEasyTools-0.5/setup.cfg
-drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-03-22 17:15:32.938051 LLMEasyTools-0.5/tests/
--rw-rw-r--   0 zby       (1000) zby       (1000)     7838 2024-03-20 22:48:41.000000 LLMEasyTools-0.5/tests/schema_generator_test.py
--rw-rw-r--   0 zby       (1000) zby       (1000)     9179 2024-03-16 20:27:23.000000 LLMEasyTools-0.5/tests/tools_test.py
+drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-04-18 06:56:55.603600 LLMEasyTools-0.6/
+-rw-rw-r--   0 zby       (1000) zby       (1000)    11357 2024-03-03 11:08:50.000000 LLMEasyTools-0.6/LICENSE
+drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-04-18 06:56:55.603600 LLMEasyTools-0.6/LLMEasyTools.egg-info/
+-rw-r--r--   0 zby       (1000) zby       (1000)    16948 2024-04-18 06:56:55.000000 LLMEasyTools-0.6/LLMEasyTools.egg-info/PKG-INFO
+-rw-rw-r--   0 zby       (1000) zby       (1000)      407 2024-04-18 06:56:55.000000 LLMEasyTools-0.6/LLMEasyTools.egg-info/SOURCES.txt
+-rw-rw-r--   0 zby       (1000) zby       (1000)        1 2024-04-18 06:56:55.000000 LLMEasyTools-0.6/LLMEasyTools.egg-info/dependency_links.txt
+-rw-rw-r--   0 zby       (1000) zby       (1000)       54 2024-04-18 06:56:55.000000 LLMEasyTools-0.6/LLMEasyTools.egg-info/requires.txt
+-rw-rw-r--   0 zby       (1000) zby       (1000)       15 2024-04-18 06:56:55.000000 LLMEasyTools-0.6/LLMEasyTools.egg-info/top_level.txt
+-rw-rw-r--   0 zby       (1000) zby       (1000)       67 2024-03-03 11:08:50.000000 LLMEasyTools-0.6/MANIFEST.in
+-rw-r--r--   0 zby       (1000) zby       (1000)    16948 2024-04-18 06:56:55.603600 LLMEasyTools-0.6/PKG-INFO
+-rw-rw-r--   0 zby       (1000) zby       (1000)     3202 2024-03-04 13:15:40.000000 LLMEasyTools-0.6/README.md
+drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-04-18 06:56:55.603600 LLMEasyTools-0.6/examples/
+-rw-rw-r--   0 zby       (1000) zby       (1000)     1290 2024-03-05 07:21:59.000000 LLMEasyTools-0.6/examples/extract_user_details.py
+-rw-rw-r--   0 zby       (1000) zby       (1000)      863 2024-03-05 07:22:09.000000 LLMEasyTools-0.6/examples/extract_user_details_by_function.py
+-rw-rw-r--   0 zby       (1000) zby       (1000)     3360 2024-03-05 07:22:24.000000 LLMEasyTools-0.6/examples/stateful_search.py
+drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-04-18 06:56:55.603600 LLMEasyTools-0.6/llm_easy_tools/
+-rw-rw-r--   0 zby       (1000) zby       (1000)    14944 2024-04-18 06:46:53.000000 LLMEasyTools-0.6/llm_easy_tools/__init__.py
+-rw-rw-r--   0 zby       (1000) zby       (1000)      988 2024-04-18 05:41:21.000000 LLMEasyTools-0.6/pyproject.toml
+-rw-rw-r--   0 zby       (1000) zby       (1000)       38 2024-04-18 06:56:55.603600 LLMEasyTools-0.6/setup.cfg
+drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-04-18 06:56:55.603600 LLMEasyTools-0.6/tests/
+-rw-rw-r--   0 zby       (1000) zby       (1000)     7838 2024-03-20 22:48:41.000000 LLMEasyTools-0.6/tests/schema_generator_test.py
+-rw-rw-r--   0 zby       (1000) zby       (1000)     9872 2024-04-18 06:48:39.000000 LLMEasyTools-0.6/tests/tools_test.py
```

### Comparing `LLMEasyTools-0.5/LICENSE` & `LLMEasyTools-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `LLMEasyTools-0.5/LLMEasyTools.egg-info/PKG-INFO` & `LLMEasyTools-0.6/LLMEasyTools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LLMEasyTools
-Version: 0.5
+Version: 0.6
 Summary: OpenAI tools and functions with no fuss.
 Author-email: Zbigniew Łukasiak <zzbbyy@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `LLMEasyTools-0.5/PKG-INFO` & `LLMEasyTools-0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LLMEasyTools
-Version: 0.5
+Version: 0.6
 Summary: OpenAI tools and functions with no fuss.
 Author-email: Zbigniew Łukasiak <zzbbyy@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `LLMEasyTools-0.5/README.md` & `LLMEasyTools-0.6/README.md`

 * *Files identical despite different names*

### Comparing `LLMEasyTools-0.5/examples/extract_user_details.py` & `LLMEasyTools-0.6/examples/extract_user_details.py`

 * *Files identical despite different names*

### Comparing `LLMEasyTools-0.5/examples/extract_user_details_by_function.py` & `LLMEasyTools-0.6/examples/extract_user_details_by_function.py`

 * *Files identical despite different names*

### Comparing `LLMEasyTools-0.5/examples/stateful_search.py` & `LLMEasyTools-0.6/examples/stateful_search.py`

 * *Files identical despite different names*

### Comparing `LLMEasyTools-0.5/llm_easy_tools/__init__.py` & `LLMEasyTools-0.6/llm_easy_tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,14 +183,15 @@
     Attributes:
     - `name_mappings`: A list of tuples mapping names used in LLM schemas and tool function names used in code.
     - `tool_registry`: A dictionary mapping tool function names to their info
     """
     def __init__(self, strict=True, name_mappings=None, case_insensitive=True,
                  tool_registry=None, generator=None,
                  tool_sets=None,
+                 fix_json_args=True,
                  ):
         self.strict = strict
         self.case_insensitive = case_insensitive
         if tool_registry is None:
             tool_registry = {}
         self.tool_registry = tool_registry
         if name_mappings is None:
@@ -200,14 +201,16 @@
             tool_sets = {}
         self.tool_sets = tool_sets
 
         if generator is None:
             generator = SchemaGenerator(strict=self.strict, case_insensitive=self.case_insensitive, name_mappings=self.name_mappings)
         self.generator = generator
 
+        self.fix_json_args = fix_json_args
+
 
     def tool_schemas(self, prefix_class=None):
         tool_schemas = [self.generator.tool_schema(function_schema) for function_schema in self.function_schemas(prefix_class)]
         return tool_schemas
 
     def get_tool_schema(self, name, prefix_class=None):
         # todo - decide if we want use internal or external name here
@@ -300,28 +303,37 @@
 
     def schema_name_to_func(self, schema_name):
         for fname, sname in self.name_mappings:
             if schema_name == sname:
                 return fname
         return schema_name
 
-    def process_response(self, response, choice_num=0):
+    def process_response(self, response, choice_num=0, prefix_class=None, ignore_prefix=False):
         results = []
         if response.choices[choice_num].message.function_call:
             function_call = response.choices[choice_num].message.function_call
-            result = self.process_function(function_call)
+            result = self.process_function(function_call, prefix_class, ignore_prefix)
             results.append(result)
         if response.choices[choice_num].message.tool_calls:
             for tool_call in response.choices[choice_num].message.tool_calls:
-                result = self.process_function(tool_call.function)
+                result = self.process_function(tool_call.function, prefix_class, ignore_prefix)
                 results.append(result)
         return results
 
     def process_function(self, function_call, prefix_class=None, ignore_prefix=False):
-        tool_args = json.loads(function_call.arguments)
+        args = function_call.arguments
+        if self.fix_json_args:
+            try:
+                tool_args = json.loads(args)
+            except json.decoder.JSONDecodeError as e:
+                args = args.replace(', }', '}').replace(',}', '}')
+                tool_args = json.loads(args)
+        else:
+            tool_args = json.loads(args)
+
         tool_name = function_call.name
         if prefix_class is not None:
             if not ignore_prefix:
                 # todo make better API for returning the prefix
                 self.prefix = self._extract_prefix_unpacked(tool_args, prefix_class)
             prefix_name = prefix_class.__name__
             if self.case_insensitive:
```

### Comparing `LLMEasyTools-0.5/pyproject.toml` & `LLMEasyTools-0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=59.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "LLMEasyTools"
-version = "0.05"
+version = "0.06"
 authors = [{ name = "Zbigniew Łukasiak", email = "zzbbyy@gmail.com" }]
 description = "OpenAI tools and functions with no fuss."
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `LLMEasyTools-0.5/tests/schema_generator_test.py` & `LLMEasyTools-0.6/tests/schema_generator_test.py`

 * *Files identical despite different names*

### Comparing `LLMEasyTools-0.5/tests/tools_test.py` & `LLMEasyTools-0.6/tests/tools_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,20 +115,21 @@
     toolbox.register_model(UserDetail)
     assert "UserDetail" in toolbox.tool_registry
     original_user = UserDetail(name="John", age=21)
     function_call = FunctionCallMock(name="UserDetail", arguments=json.dumps(original_user.model_dump()))
     result = toolbox.process_function(function_call)
     assert result == original_user
 
-def process_response():
+def test_process_response():
+    # too much mocking in this test
     toolbox = ToolBox()
-    toolbox.register_function(UserDetail)
+    toolbox.register_model(UserDetail)
     original_user = UserDetail(name="John", age=21)
     function_call = FunctionCallMock(name="UserDetail", arguments=json.dumps(original_user.model_dump()))
-    response = Mock(choices=[Mock(message=Mock(tool_calls=[Mock(function=function_call)]))])
+    response = Mock(choices=[Mock(message=Mock(function_call=False, tool_calls=[Mock(function=function_call)]))])
     results = toolbox.process_response(response)
     assert len(results) == 1
     assert results[0] == original_user
 
 
 # Define the test cases
 def test_register_tool():
@@ -243,9 +244,24 @@
     args = ToolParam(value=2).model_dump()
     args['relevancy'] = 'very good'
     function_call = FunctionCallMock(name=prefixed_name, arguments=json.dumps(args))
     result = toolbox.process_function(function_call, prefix_class=Reflection)
     assert result == 'executed tool_method with param: value=2'
     assert isinstance(toolbox.prefix, Reflection)
 
+def test_json_fix():
+    toolbox = ToolBox()
+    toolbox.register_model(UserDetail)
+    original_user = UserDetail(name="John", age=21)
+    json_data = json.dumps(original_user.model_dump())
+    json_data = json_data[:-1]
+    json_data = json_data + ',}'
+    function_call = FunctionCallMock(name="UserDetail", arguments=json_data)
+    result = toolbox.process_function(function_call)
+    assert result == original_user
+
+    with pytest.raises(Exception) as exception_info:
+        toolbox.fix_json_args = False
+        toolbox.process_function(function_call)
+    assert isinstance(exception_info.value, json.decoder.JSONDecodeError)
 
 pytest.main()
```

