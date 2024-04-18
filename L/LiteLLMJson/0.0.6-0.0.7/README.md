# Comparing `tmp/LiteLLMJson-0.0.6.tar.gz` & `tmp/LiteLLMJson-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LiteLLMJson-0.0.6.tar", last modified: Thu Apr 11 09:15:24 2024, max compression
+gzip compressed data, was "LiteLLMJson-0.0.7.tar", last modified: Thu Apr 18 07:23:54 2024, max compression
```

## Comparing `LiteLLMJson-0.0.6.tar` & `LiteLLMJson-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 09:15:24.867054 LiteLLMJson-0.0.6/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:15:24.852083 LiteLLMJson-0.0.6/LiteLLMJson.egg-info/
--rw-rw-rw-   0        0        0     1726 2024-04-11 09:15:24.000000 LiteLLMJson-0.0.6/LiteLLMJson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2024-04-11 09:15:24.000000 LiteLLMJson-0.0.6/LiteLLMJson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 09:15:24.000000 LiteLLMJson-0.0.6/LiteLLMJson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-11 09:15:24.000000 LiteLLMJson-0.0.6/LiteLLMJson.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-11 09:15:24.000000 LiteLLMJson-0.0.6/LiteLLMJson.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1726 2024-04-11 09:15:24.866053 LiteLLMJson-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1235 2023-12-10 08:02:17.000000 LiteLLMJson-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 09:15:24.864535 LiteLLMJson-0.0.6/lite_llm_json/
--rw-rw-rw-   0        0        0       41 2024-03-23 06:29:14.000000 LiteLLMJson-0.0.6/lite_llm_json/__init__.py
--rw-rw-rw-   0        0        0     2770 2024-04-11 09:14:02.000000 LiteLLMJson-0.0.6/lite_llm_json/lite_llm_json.py
--rw-rw-rw-   0        0        0     4495 2024-04-11 09:13:19.000000 LiteLLMJson-0.0.6/lite_llm_json/test.py
--rw-rw-rw-   0        0        0       42 2024-04-11 09:15:24.867054 LiteLLMJson-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      830 2024-04-11 09:14:30.000000 LiteLLMJson-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 07:23:54.517228 LiteLLMJson-0.0.7/
+drwxrwxrwx   0        0        0        0 2024-04-18 07:23:54.507486 LiteLLMJson-0.0.7/LiteLLMJson.egg-info/
+-rw-rw-rw-   0        0        0     1726 2024-04-18 07:23:54.000000 LiteLLMJson-0.0.7/LiteLLMJson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2024-04-18 07:23:54.000000 LiteLLMJson-0.0.7/LiteLLMJson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 07:23:54.000000 LiteLLMJson-0.0.7/LiteLLMJson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-18 07:23:54.000000 LiteLLMJson-0.0.7/LiteLLMJson.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-18 07:23:54.000000 LiteLLMJson-0.0.7/LiteLLMJson.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1726 2024-04-18 07:23:54.516243 LiteLLMJson-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1235 2023-12-10 08:02:17.000000 LiteLLMJson-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 07:23:54.515003 LiteLLMJson-0.0.7/lite_llm_json/
+-rw-rw-rw-   0        0        0       41 2024-03-23 06:29:14.000000 LiteLLMJson-0.0.7/lite_llm_json/__init__.py
+-rw-rw-rw-   0        0        0     2904 2024-04-18 07:22:45.000000 LiteLLMJson-0.0.7/lite_llm_json/lite_llm_json.py
+-rw-rw-rw-   0        0        0     4735 2024-04-18 07:20:28.000000 LiteLLMJson-0.0.7/lite_llm_json/test.py
+-rw-rw-rw-   0        0        0       42 2024-04-18 07:23:54.517228 LiteLLMJson-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      830 2024-04-18 07:23:17.000000 LiteLLMJson-0.0.7/setup.py
```

### Comparing `LiteLLMJson-0.0.6/LiteLLMJson.egg-info/PKG-INFO` & `LiteLLMJson-0.0.7/LiteLLMJson.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LiteLLMJson
-Version: 0.0.6
+Version: 0.0.7
 Summary: This library offers functionality to cleanly extract JSON from LLM responses and generate prompts for LLM that return JSON. It features a simple implementation while maintaining high versatility.
 Home-page: https://github.com/HawkClaws/lite_llm_json
 Author: HawkClaws
 License: MIT
 Project-URL: Source Code, https://github.com/HawkClaws/lite_llm_json
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `LiteLLMJson-0.0.6/PKG-INFO` & `LiteLLMJson-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LiteLLMJson
-Version: 0.0.6
+Version: 0.0.7
 Summary: This library offers functionality to cleanly extract JSON from LLM responses and generate prompts for LLM that return JSON. It features a simple implementation while maintaining high versatility.
 Home-page: https://github.com/HawkClaws/lite_llm_json
 Author: HawkClaws
 License: MIT
 Project-URL: Source Code, https://github.com/HawkClaws/lite_llm_json
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `LiteLLMJson-0.0.6/README.md` & `LiteLLMJson-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `LiteLLMJson-0.0.6/lite_llm_json/lite_llm_json.py` & `LiteLLMJson-0.0.7/lite_llm_json/lite_llm_json.py`

 * *Files 16% similar despite different names*

```diff
@@ -69,27 +69,26 @@
             Dict: The parsed response as a dictionary.
 
         """
         json_data = self._extract_data_from_response(response)
         jsonschema.validate(json_data, self.json_schema)
         return json_data
 
-    def _extract_data_from_response(self, response_content: str):
-        # Sometimes the response includes the JSON in a code block with ``` pattern
-        pattern = r"```(?:json)?\s*(\[.*?\]|{.*?}|\\[.*?\\]|\\{.*?\\})\s*```"
-        match = re.search(pattern, response_content, re.DOTALL)
-        if match:
-            response_content = match.group(1).strip()
-        else:
-            json_pattern = r"\s*(\[.*?\]|{.*?}|\\[.*?\\]|\\{.*?\\})\s*"
-            match = re.search(json_pattern, response_content, re.DOTALL)
-            if match:
-                response_content = match.group(1)
-            else:
-                return {}
-        try:
-            data = json.loads(response_content, strict=False)
-            return data
-        except Exception as e:
-            print(e)
-            return {}
-
+    def _extract_data_from_response(self, text: str, decoder=json.JSONDecoder(strict=False), symbols=('{', '[')):
+        """Find JSON objects and arrays in text, load the JSON data, and return the loaded data as a list"""
+        pos = 0
+        while True:
+            matches = {symbol: text.find(symbol, pos) for symbol in symbols}
+            matches = {k: v for k, v in matches.items() if v != -1}
+            if not matches:
+                break
+            match_symbol, match_pos = min(matches.items(), key=lambda item: item[1])
+            try:
+                result, index = decoder.raw_decode(text[match_pos:])
+                if match_symbol == '{':
+                    return json.loads(json.dumps(result))
+                elif match_symbol == '[':
+                    return json.loads(json.dumps(result))
+                pos = match_pos + index
+            except ValueError:
+                pos = match_pos + 1
+        return {}
```

### Comparing `LiteLLMJson-0.0.6/lite_llm_json/test.py` & `LiteLLMJson-0.0.7/lite_llm_json/test.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,29 +9,27 @@
             "type": "object",
             "properties": {"name": {"type": "string"}, "age": {"type": "integer"}},
             "required": ["name", "age"],
         }
         llm_json = LiteLLMJson(json_schema)
         query_prompt = "Provide information about a person."
         generated_prompt = llm_json.generate_prompt(query_prompt)
-        print(generated_prompt)
         # Add your assertion here based on the expected output of generate_prompt
         self.assertIn("name", generated_prompt)
         self.assertIn("age", generated_prompt)
 
     def test_parse_response(self):
         json_schema = {
             "type": "object",
             "properties": {"name": {"type": "string"}, "age": {"type": "integer"}},
             "required": ["name", "age"],
         }
         llm_json = LiteLLMJson(json_schema)
         valid_response = '{"name": "John Doe", "age": 30}'
         parsed_response = llm_json.parse_response(valid_response)
-        print(parsed_response)
 
         self.assertIsInstance(parsed_response, dict)
         self.assertEqual(parsed_response["name"], "John Doe")
         self.assertEqual(parsed_response["age"], 30)
 
         invalid_response = '{"name": "John Doe", "age": "thirty"}'
         with self.assertRaises(jsonschema.exceptions.ValidationError):
@@ -55,14 +53,24 @@
 
     def test_extract_data_from_code_block_with_json_prefix(self):
         response_content = '```json\n{"key": "value"}\n```'
         expected_data = {"key": "value"}
         data = self.llm_json._extract_data_from_response(response_content)
         self.assertEqual(data, expected_data)
 
+    def test_extract_data_from_code_block_with_JSON_prefix(self):
+        response_content ="""```JSON
+{
+  "key": "value"
+}
+```"""
+        expected_data = {"key": "value"}
+        data = self.llm_json._extract_data_from_response(response_content)
+        self.assertEqual(data, expected_data)
+
     def test_extract_data_from_json_string(self):
         response_content = '{"key": "value"}'
         expected_data = {"key": "value"}
         data = self.llm_json._extract_data_from_response(response_content)
         self.assertEqual(data, expected_data)
 
     def test_extract_data_from_json_list(self):
@@ -88,15 +96,15 @@
             '{"sentence": "The quick brown fox jumps over the lazy dog."}'
         )
         expected_data = {"sentence": "The quick brown fox jumps over the lazy dog."}
         data = self.llm_json._extract_data_from_response(response_content)
         self.assertEqual(data, expected_data)
 
     def test_extract_data_newline_text(self):
-        response_content = """
+        response_content = """4
         {
             "answer_impossible": false, 
             "text": "# Introduction
 This is a simple example of a markdown-formatted text response."
         }
         """
         expected_data = {
```

### Comparing `LiteLLMJson-0.0.6/setup.py` & `LiteLLMJson-0.0.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fp:
     readme = fp.read()
 
 DESCRIPTION = "This library offers functionality to cleanly extract JSON from LLM responses and generate prompts for LLM that return JSON. It features a simple implementation while maintaining high versatility."
 
 setup(
     name="LiteLLMJson",
-    version="0.0.6",
+    version="0.0.7",
     author="HawkClaws",
     packages=find_packages(),
     install_requires=[
         "jsonschema>=4.19.2"
     ],
     python_requires=">=3.6",
     include_package_data=True,
```

