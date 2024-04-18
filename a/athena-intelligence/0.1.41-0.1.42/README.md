# Comparing `tmp/athena_intelligence-0.1.41.tar.gz` & `tmp/athena_intelligence-0.1.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athena_intelligence-0.1.41.tar", max compression
+gzip compressed data, was "athena_intelligence-0.1.42.tar", max compression
```

## Comparing `athena_intelligence-0.1.41.tar` & `athena_intelligence-0.1.42.tar`

### file list

```diff
@@ -1,60 +1,61 @@
--rw-r--r--   0        0        0     4235 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/README.md
--rw-r--r--   0        0        0      435 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/pyproject.toml
--rw-r--r--   0        0        0     1455 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/__init__.py
--rw-r--r--   0        0        0     5416 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/base_client.py
--rw-r--r--   0        0        0      159 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/chain/__init__.py
--rw-r--r--   0        0        0     8333 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/chain/client.py
--rw-r--r--   0        0        0      187 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/chain/types/__init__.py
--rw-r--r--   0        0        0     2203 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/chain/types/structured_parse_in_parsing_model.py
--rw-r--r--   0        0        0     3576 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/client.py
--rw-r--r--   0        0        0      790 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/core/api_error.py
--rw-r--r--   0        0        0     1198 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/core/file.py
--rw-r--r--   0        0        0     4882 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/core/http_client.py
--rw-r--r--   0        0        0     3799 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/core/request_options.py
--rw-r--r--   0        0        0       65 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/dataset/__init__.py
--rw-r--r--   0        0        0     6087 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/dataset/client.py
--rw-r--r--   0        0        0      165 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/environment.py
--rw-r--r--   0        0        0      170 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0       65 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/message/__init__.py
--rw-r--r--   0        0        0    12185 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/message/client.py
--rw-r--r--   0        0        0     3998 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/polling_message_client.py
--rw-r--r--   0        0        0        0 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/py.typed
--rw-r--r--   0        0        0       65 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/query/__init__.py
--rw-r--r--   0        0        0     6243 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/query/client.py
--rw-r--r--   0        0        0       65 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/report/__init__.py
--rw-r--r--   0        0        0     6528 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/report/client.py
--rw-r--r--   0        0        0       65 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/search/__init__.py
--rw-r--r--   0        0        0     7515 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/search/client.py
--rw-r--r--   0        0        0       65 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/snippet/__init__.py
--rw-r--r--   0        0        0     6087 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/snippet/client.py
--rw-r--r--   0        0        0       65 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/tools/__init__.py
--rw-r--r--   0        0        0    19332 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/tools/client.py
--rw-r--r--   0        0        0     1553 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/types/__init__.py
--rw-r--r--   0        0        0     1014 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/dataset.py
--rw-r--r--   0        0        0     1081 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/document.py
--rw-r--r--   0        0        0      895 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/excecute_tool_first_workflow_out.py
--rw-r--r--   0        0        0     1021 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py
--rw-r--r--   0        0        0     1128 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/firecrawl_scrape_url_metadata.py
--rw-r--r--   0        0        0      989 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/get_datasets_response.py
--rw-r--r--   0        0        0      989 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/get_snippets_response.py
--rw-r--r--   0        0        0      973 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/http_validation_error.py
--rw-r--r--   0        0        0      939 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/langchain_documents_request_out.py
--rw-r--r--   0        0        0      865 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/message_out.py
--rw-r--r--   0        0        0     1051 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/message_out_dto.py
--rw-r--r--   0        0        0     2545 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/model.py
--rw-r--r--   0        0        0      946 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/report.py
--rw-r--r--   0        0        0     1126 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/snippet.py
--rw-r--r--   0        0        0      900 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/sql_results.py
--rw-r--r--   0        0        0      672 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/status_enum.py
--rw-r--r--   0        0        0      905 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/structured_parse_result.py
--rw-r--r--   0        0        0     1422 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/tools.py
--rw-r--r--   0        0        0      893 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/url_result.py
--rw-r--r--   0        0        0      992 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.41/PKG-INFO
+-rw-r--r--   0        0        0     4235 2024-04-18 00:54:15.833713 athena_intelligence-0.1.42/README.md
+-rw-r--r--   0        0        0      435 2024-04-18 00:54:15.833713 athena_intelligence-0.1.42/pyproject.toml
+-rw-r--r--   0        0        0     1489 2024-04-18 00:54:15.833713 athena_intelligence-0.1.42/src/athena/__init__.py
+-rw-r--r--   0        0        0     5416 2024-04-18 00:54:15.833713 athena_intelligence-0.1.42/src/athena/base_client.py
+-rw-r--r--   0        0        0      159 2024-04-18 00:54:15.833713 athena_intelligence-0.1.42/src/athena/chain/__init__.py
+-rw-r--r--   0        0        0     8333 2024-04-18 00:54:15.833713 athena_intelligence-0.1.42/src/athena/chain/client.py
+-rw-r--r--   0        0        0      187 2024-04-18 00:54:15.833713 athena_intelligence-0.1.42/src/athena/chain/types/__init__.py
+-rw-r--r--   0        0        0     2203 2024-04-18 00:54:15.833713 athena_intelligence-0.1.42/src/athena/chain/types/structured_parse_in_parsing_model.py
+-rw-r--r--   0        0        0     3576 2024-04-18 00:54:15.833713 athena_intelligence-0.1.42/src/athena/client.py
+-rw-r--r--   0        0        0      790 2024-04-18 00:54:15.833713 athena_intelligence-0.1.42/src/athena/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-18 00:54:15.833713 athena_intelligence-0.1.42/src/athena/core/api_error.py
+-rw-r--r--   0        0        0     1198 2024-04-18 00:54:15.833713 athena_intelligence-0.1.42/src/athena/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-18 00:54:15.833713 athena_intelligence-0.1.42/src/athena/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-18 00:54:15.833713 athena_intelligence-0.1.42/src/athena/core/file.py
+-rw-r--r--   0        0        0     4882 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/core/http_client.py
+-rw-r--r--   0        0        0     3799 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/core/request_options.py
+-rw-r--r--   0        0        0       65 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/dataset/__init__.py
+-rw-r--r--   0        0        0     6087 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/dataset/client.py
+-rw-r--r--   0        0        0      165 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/environment.py
+-rw-r--r--   0        0        0      170 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0       65 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/message/__init__.py
+-rw-r--r--   0        0        0    12185 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/message/client.py
+-rw-r--r--   0        0        0     3998 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/polling_message_client.py
+-rw-r--r--   0        0        0        0 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/py.typed
+-rw-r--r--   0        0        0       65 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/query/__init__.py
+-rw-r--r--   0        0        0     6243 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/query/client.py
+-rw-r--r--   0        0        0       65 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/report/__init__.py
+-rw-r--r--   0        0        0     6528 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/report/client.py
+-rw-r--r--   0        0        0       65 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/search/__init__.py
+-rw-r--r--   0        0        0     7515 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/search/client.py
+-rw-r--r--   0        0        0       65 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/snippet/__init__.py
+-rw-r--r--   0        0        0     6087 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/snippet/client.py
+-rw-r--r--   0        0        0       65 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/tools/__init__.py
+-rw-r--r--   0        0        0    19643 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/tools/client.py
+-rw-r--r--   0        0        0     1607 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/types/__init__.py
+-rw-r--r--   0        0        0     1014 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/types/dataset.py
+-rw-r--r--   0        0        0     1081 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/types/document.py
+-rw-r--r--   0        0        0      895 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/types/excecute_tool_first_workflow_out.py
+-rw-r--r--   0        0        0     1021 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py
+-rw-r--r--   0        0        0     1128 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/types/firecrawl_scrape_url_metadata.py
+-rw-r--r--   0        0        0      989 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/types/get_datasets_response.py
+-rw-r--r--   0        0        0      989 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/types/get_snippets_response.py
+-rw-r--r--   0        0        0      973 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/types/http_validation_error.py
+-rw-r--r--   0        0        0      939 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/types/langchain_documents_request_out.py
+-rw-r--r--   0        0        0      865 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/types/message_out.py
+-rw-r--r--   0        0        0     1051 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/types/message_out_dto.py
+-rw-r--r--   0        0        0     2545 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/types/model.py
+-rw-r--r--   0        0        0      946 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/types/report.py
+-rw-r--r--   0        0        0     1126 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/types/snippet.py
+-rw-r--r--   0        0        0      900 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/types/sql_results.py
+-rw-r--r--   0        0        0      672 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/types/status_enum.py
+-rw-r--r--   0        0        0      905 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/types/structured_parse_result.py
+-rw-r--r--   0        0        0     1829 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/types/tool_models.py
+-rw-r--r--   0        0        0     1422 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/types/tools.py
+-rw-r--r--   0        0        0      893 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/types/url_result.py
+-rw-r--r--   0        0        0      992 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-18 00:54:15.837713 athena_intelligence-0.1.42/src/athena/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.42/PKG-INFO
```

### Comparing `athena_intelligence-0.1.41/README.md` & `athena_intelligence-0.1.42/README.md`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/__init__.py` & `athena_intelligence-0.1.42/src/athena/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     MessageOutDto,
     Model,
     Report,
     Snippet,
     SqlResults,
     StatusEnum,
     StructuredParseResult,
+    ToolModels,
     Tools,
     UrlResult,
     ValidationError,
     ValidationErrorLocItem,
 )
 from .errors import UnprocessableEntityError
 from . import chain, dataset, message, query, report, search, snippet, tools
@@ -44,14 +45,15 @@
     "Model",
     "Report",
     "Snippet",
     "SqlResults",
     "StatusEnum",
     "StructuredParseInParsingModel",
     "StructuredParseResult",
+    "ToolModels",
     "Tools",
     "UnprocessableEntityError",
     "UrlResult",
     "ValidationError",
     "ValidationErrorLocItem",
     "chain",
     "dataset",
```

### Comparing `athena_intelligence-0.1.41/src/athena/base_client.py` & `athena_intelligence-0.1.42/src/athena/base_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/chain/client.py` & `athena_intelligence-0.1.42/src/athena/chain/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/chain/types/structured_parse_in_parsing_model.py` & `athena_intelligence-0.1.42/src/athena/chain/types/structured_parse_in_parsing_model.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/client.py` & `athena_intelligence-0.1.42/src/athena/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/core/__init__.py` & `athena_intelligence-0.1.42/src/athena/core/__init__.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/core/client_wrapper.py` & `athena_intelligence-0.1.42/src/athena/core/client_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self.api_key = api_key
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "athena-intelligence",
-            "X-Fern-SDK-Version": "0.1.41",
+            "X-Fern-SDK-Version": "0.1.42",
         }
         headers["X-API-KEY"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `athena_intelligence-0.1.41/src/athena/core/datetime_utils.py` & `athena_intelligence-0.1.42/src/athena/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/core/file.py` & `athena_intelligence-0.1.42/src/athena/core/file.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/core/http_client.py` & `athena_intelligence-0.1.42/src/athena/core/http_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/core/jsonable_encoder.py` & `athena_intelligence-0.1.42/src/athena/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/core/request_options.py` & `athena_intelligence-0.1.42/src/athena/core/request_options.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/dataset/client.py` & `athena_intelligence-0.1.42/src/athena/dataset/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/message/client.py` & `athena_intelligence-0.1.42/src/athena/message/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/polling_message_client.py` & `athena_intelligence-0.1.42/src/athena/polling_message_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/query/client.py` & `athena_intelligence-0.1.42/src/athena/query/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/report/client.py` & `athena_intelligence-0.1.42/src/athena/report/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/search/client.py` & `athena_intelligence-0.1.42/src/athena/search/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/snippet/client.py` & `athena_intelligence-0.1.42/src/athena/snippet/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/tools/client.py` & `athena_intelligence-0.1.42/src/athena/tools/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.excecute_tool_first_workflow_out import ExcecuteToolFirstWorkflowOut
 from ..types.firecrawl_scrape_url_data_reponse_dto import FirecrawlScrapeUrlDataReponseDto
 from ..types.http_validation_error import HttpValidationError
 from ..types.langchain_documents_request_out import LangchainDocumentsRequestOut
+from ..types.tool_models import ToolModels
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 # this is used as the default value for optional parameters
@@ -160,45 +161,48 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def tool_first_workflow(
         self,
         *,
-        model_name: str,
+        model: typing.Optional[ToolModels] = OMIT,
         tool_name: str,
         content: str,
         tool_kwargs: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ExcecuteToolFirstWorkflowOut:
         """
         Parameters:
-            - model_name: str.
+            - model: typing.Optional[ToolModels].
 
             - tool_name: str.
 
             - content: str.
 
             - tool_kwargs: typing.Optional[typing.Dict[str, typing.Any]].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
+        from athena import ToolModels
         from athena.client import Athena
 
         client = Athena(
             api_key="YOUR_API_KEY",
         )
         client.tools.tool_first_workflow(
-            model_name="gpt-3.5-turbo",
+            model=ToolModels.MISTRAL_LARGE_0224,
             tool_name="tavily_search",
             content="summarize the website in one paragraph",
             tool_kwargs={"query": "website: www.athenaintelligence.ai"},
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"model_name": model_name, "tool_name": tool_name, "content": content}
+        _request: typing.Dict[str, typing.Any] = {"tool_name": tool_name, "content": content}
+        if model is not OMIT:
+            _request["model"] = model
         if tool_kwargs is not OMIT:
             _request["tool_kwargs"] = tool_kwargs
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/tools/first-agent"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
@@ -370,45 +374,48 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def tool_first_workflow(
         self,
         *,
-        model_name: str,
+        model: typing.Optional[ToolModels] = OMIT,
         tool_name: str,
         content: str,
         tool_kwargs: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ExcecuteToolFirstWorkflowOut:
         """
         Parameters:
-            - model_name: str.
+            - model: typing.Optional[ToolModels].
 
             - tool_name: str.
 
             - content: str.
 
             - tool_kwargs: typing.Optional[typing.Dict[str, typing.Any]].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
+        from athena import ToolModels
         from athena.client import AsyncAthena
 
         client = AsyncAthena(
             api_key="YOUR_API_KEY",
         )
         await client.tools.tool_first_workflow(
-            model_name="gpt-3.5-turbo",
+            model=ToolModels.MISTRAL_LARGE_0224,
             tool_name="tavily_search",
             content="summarize the website in one paragraph",
             tool_kwargs={"query": "website: www.athenaintelligence.ai"},
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"model_name": model_name, "tool_name": tool_name, "content": content}
+        _request: typing.Dict[str, typing.Any] = {"tool_name": tool_name, "content": content}
+        if model is not OMIT:
+            _request["model"] = model
         if tool_kwargs is not OMIT:
             _request["tool_kwargs"] = tool_kwargs
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/tools/first-agent"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
```

### Comparing `athena_intelligence-0.1.41/src/athena/types/__init__.py` & `athena_intelligence-0.1.42/src/athena/types/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from .message_out_dto import MessageOutDto
 from .model import Model
 from .report import Report
 from .snippet import Snippet
 from .sql_results import SqlResults
 from .status_enum import StatusEnum
 from .structured_parse_result import StructuredParseResult
+from .tool_models import ToolModels
 from .tools import Tools
 from .url_result import UrlResult
 from .validation_error import ValidationError
 from .validation_error_loc_item import ValidationErrorLocItem
 
 __all__ = [
     "Dataset",
@@ -36,12 +37,13 @@
     "MessageOutDto",
     "Model",
     "Report",
     "Snippet",
     "SqlResults",
     "StatusEnum",
     "StructuredParseResult",
+    "ToolModels",
     "Tools",
     "UrlResult",
     "ValidationError",
     "ValidationErrorLocItem",
 ]
```

### Comparing `athena_intelligence-0.1.41/src/athena/types/dataset.py` & `athena_intelligence-0.1.42/src/athena/types/dataset.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/types/document.py` & `athena_intelligence-0.1.42/src/athena/types/document.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/types/excecute_tool_first_workflow_out.py` & `athena_intelligence-0.1.42/src/athena/types/excecute_tool_first_workflow_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py` & `athena_intelligence-0.1.42/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/types/firecrawl_scrape_url_metadata.py` & `athena_intelligence-0.1.42/src/athena/types/firecrawl_scrape_url_metadata.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/types/get_datasets_response.py` & `athena_intelligence-0.1.42/src/athena/types/get_datasets_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/types/get_snippets_response.py` & `athena_intelligence-0.1.42/src/athena/types/get_snippets_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/types/http_validation_error.py` & `athena_intelligence-0.1.42/src/athena/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/types/langchain_documents_request_out.py` & `athena_intelligence-0.1.42/src/athena/types/langchain_documents_request_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/types/message_out.py` & `athena_intelligence-0.1.42/src/athena/types/message_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/types/message_out_dto.py` & `athena_intelligence-0.1.42/src/athena/types/message_out_dto.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/types/model.py` & `athena_intelligence-0.1.42/src/athena/types/model.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/types/report.py` & `athena_intelligence-0.1.42/src/athena/types/report.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/types/snippet.py` & `athena_intelligence-0.1.42/src/athena/types/snippet.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/types/sql_results.py` & `athena_intelligence-0.1.42/src/athena/types/sql_results.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/types/status_enum.py` & `athena_intelligence-0.1.42/src/athena/types/status_enum.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/types/structured_parse_result.py` & `athena_intelligence-0.1.42/src/athena/types/structured_parse_result.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/types/tools.py` & `athena_intelligence-0.1.42/src/athena/types/tools.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/types/url_result.py` & `athena_intelligence-0.1.42/src/athena/types/url_result.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/src/athena/types/validation_error.py` & `athena_intelligence-0.1.42/src/athena/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.41/PKG-INFO` & `athena_intelligence-0.1.42/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athena-intelligence
-Version: 0.1.41
+Version: 0.1.42
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

