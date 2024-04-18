# Comparing `tmp/athena_intelligence-0.1.39.tar.gz` & `tmp/athena_intelligence-0.1.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athena_intelligence-0.1.39.tar", max compression
+gzip compressed data, was "athena_intelligence-0.1.40.tar", max compression
```

## Comparing `athena_intelligence-0.1.39.tar` & `athena_intelligence-0.1.40.tar`

### file list

```diff
@@ -1,49 +1,58 @@
--rw-r--r--   0        0        0     4235 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/README.md
--rw-r--r--   0        0        0      435 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/pyproject.toml
--rw-r--r--   0        0        0     1013 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/__init__.py
--rw-r--r--   0        0        0     5014 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/base_client.py
--rw-r--r--   0        0        0     3576 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/client.py
--rw-r--r--   0        0        0      790 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/core/api_error.py
--rw-r--r--   0        0        0     1198 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/core/file.py
--rw-r--r--   0        0        0     4882 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/core/http_client.py
--rw-r--r--   0        0        0     3799 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/core/request_options.py
--rw-r--r--   0        0        0       65 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/dataset/__init__.py
--rw-r--r--   0        0        0     6087 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/dataset/client.py
--rw-r--r--   0        0        0      165 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/environment.py
--rw-r--r--   0        0        0      170 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0       65 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/message/__init__.py
--rw-r--r--   0        0        0    12185 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/message/client.py
--rw-r--r--   0        0        0     3998 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/polling_message_client.py
--rw-r--r--   0        0        0        0 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/py.typed
--rw-r--r--   0        0        0       65 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/query/__init__.py
--rw-r--r--   0        0        0     6243 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/query/client.py
--rw-r--r--   0        0        0       65 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/report/__init__.py
--rw-r--r--   0        0        0     6528 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/report/client.py
--rw-r--r--   0        0        0       65 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/search/__init__.py
--rw-r--r--   0        0        0    12391 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/search/client.py
--rw-r--r--   0        0        0       65 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/snippet/__init__.py
--rw-r--r--   0        0        0     6087 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/snippet/client.py
--rw-r--r--   0        0        0     1054 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/types/__init__.py
--rw-r--r--   0        0        0     1014 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/types/dataset.py
--rw-r--r--   0        0        0      989 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/types/get_datasets_response.py
--rw-r--r--   0        0        0      989 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/types/get_snippets_response.py
--rw-r--r--   0        0        0      973 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/types/http_validation_error.py
--rw-r--r--   0        0        0      865 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/types/message_out.py
--rw-r--r--   0        0        0     1051 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/types/message_out_dto.py
--rw-r--r--   0        0        0     2545 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/types/model.py
--rw-r--r--   0        0        0      946 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/types/report.py
--rw-r--r--   0        0        0      881 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/types/scrape_markdown_result.py
--rw-r--r--   0        0        0     1126 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/types/snippet.py
--rw-r--r--   0        0        0      900 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/types/sql_results.py
--rw-r--r--   0        0        0      672 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/types/status_enum.py
--rw-r--r--   0        0        0     1422 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/types/tools.py
--rw-r--r--   0        0        0      893 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/types/url_result.py
--rw-r--r--   0        0        0      992 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-17 00:50:29.623030 athena_intelligence-0.1.39/src/athena/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.39/PKG-INFO
+-rw-r--r--   0        0        0     4235 2024-04-17 21:43:09.635540 athena_intelligence-0.1.40/README.md
+-rw-r--r--   0        0        0      435 2024-04-17 21:43:09.635540 athena_intelligence-0.1.40/pyproject.toml
+-rw-r--r--   0        0        0     1341 2024-04-17 21:43:09.635540 athena_intelligence-0.1.40/src/athena/__init__.py
+-rw-r--r--   0        0        0     5416 2024-04-17 21:43:09.635540 athena_intelligence-0.1.40/src/athena/base_client.py
+-rw-r--r--   0        0        0      161 2024-04-17 21:43:09.635540 athena_intelligence-0.1.40/src/athena/chain/__init__.py
+-rw-r--r--   0        0        0     7401 2024-04-17 21:43:09.635540 athena_intelligence-0.1.40/src/athena/chain/client.py
+-rw-r--r--   0        0        0      190 2024-04-17 21:43:09.635540 athena_intelligence-0.1.40/src/athena/chain/types/__init__.py
+-rw-r--r--   0        0        0     2213 2024-04-17 21:43:09.635540 athena_intelligence-0.1.40/src/athena/chain/types/structured_tool_data_parsing_model.py
+-rw-r--r--   0        0        0     3576 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/client.py
+-rw-r--r--   0        0        0      790 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/core/api_error.py
+-rw-r--r--   0        0        0     1198 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/core/file.py
+-rw-r--r--   0        0        0     4882 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/core/http_client.py
+-rw-r--r--   0        0        0     3799 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/core/request_options.py
+-rw-r--r--   0        0        0       65 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/dataset/__init__.py
+-rw-r--r--   0        0        0     6087 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/dataset/client.py
+-rw-r--r--   0        0        0      165 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/environment.py
+-rw-r--r--   0        0        0      170 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0       65 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/message/__init__.py
+-rw-r--r--   0        0        0    12185 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/message/client.py
+-rw-r--r--   0        0        0     3998 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/polling_message_client.py
+-rw-r--r--   0        0        0        0 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/py.typed
+-rw-r--r--   0        0        0       65 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/query/__init__.py
+-rw-r--r--   0        0        0     6243 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/query/client.py
+-rw-r--r--   0        0        0       65 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/report/__init__.py
+-rw-r--r--   0        0        0     6528 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/report/client.py
+-rw-r--r--   0        0        0       65 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/search/__init__.py
+-rw-r--r--   0        0        0    12391 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/search/client.py
+-rw-r--r--   0        0        0       65 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/snippet/__init__.py
+-rw-r--r--   0        0        0     6087 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/snippet/client.py
+-rw-r--r--   0        0        0       65 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/tools/__init__.py
+-rw-r--r--   0        0        0     6657 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/tools/client.py
+-rw-r--r--   0        0        0     1370 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/__init__.py
+-rw-r--r--   0        0        0     1014 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/dataset.py
+-rw-r--r--   0        0        0     1021 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py
+-rw-r--r--   0        0        0     1128 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/firecrawl_scrape_url_metadata.py
+-rw-r--r--   0        0        0      989 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/get_datasets_response.py
+-rw-r--r--   0        0        0      989 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/get_snippets_response.py
+-rw-r--r--   0        0        0      973 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/http_validation_error.py
+-rw-r--r--   0        0        0      865 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/message_out.py
+-rw-r--r--   0        0        0     1051 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/message_out_dto.py
+-rw-r--r--   0        0        0     2545 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/model.py
+-rw-r--r--   0        0        0      946 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/report.py
+-rw-r--r--   0        0        0      881 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/scrape_markdown_result.py
+-rw-r--r--   0        0        0     1126 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/snippet.py
+-rw-r--r--   0        0        0      900 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/sql_results.py
+-rw-r--r--   0        0        0      672 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/status_enum.py
+-rw-r--r--   0        0        0      905 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/structured_parse_result.py
+-rw-r--r--   0        0        0     1422 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/tools.py
+-rw-r--r--   0        0        0      893 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/url_result.py
+-rw-r--r--   0        0        0      992 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.40/PKG-INFO
```

### Comparing `athena_intelligence-0.1.39/README.md` & `athena_intelligence-0.1.40/README.md`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/__init__.py` & `athena_intelligence-0.1.40/src/athena/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,60 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .types import (
     Dataset,
+    FirecrawlScrapeUrlDataReponseDto,
+    FirecrawlScrapeUrlMetadata,
     GetDatasetsResponse,
     GetSnippetsResponse,
     HttpValidationError,
     MessageOut,
     MessageOutDto,
     Model,
     Report,
     ScrapeMarkdownResult,
     Snippet,
     SqlResults,
     StatusEnum,
+    StructuredParseResult,
     Tools,
     UrlResult,
     ValidationError,
     ValidationErrorLocItem,
 )
 from .errors import UnprocessableEntityError
-from . import dataset, message, query, report, search, snippet
+from . import chain, dataset, message, query, report, search, snippet, tools
+from .chain import StructuredToolDataParsingModel
 from .environment import AthenaEnvironment
 
 __all__ = [
     "AthenaEnvironment",
     "Dataset",
+    "FirecrawlScrapeUrlDataReponseDto",
+    "FirecrawlScrapeUrlMetadata",
     "GetDatasetsResponse",
     "GetSnippetsResponse",
     "HttpValidationError",
     "MessageOut",
     "MessageOutDto",
     "Model",
     "Report",
     "ScrapeMarkdownResult",
     "Snippet",
     "SqlResults",
     "StatusEnum",
+    "StructuredParseResult",
+    "StructuredToolDataParsingModel",
     "Tools",
     "UnprocessableEntityError",
     "UrlResult",
     "ValidationError",
     "ValidationErrorLocItem",
+    "chain",
     "dataset",
     "message",
     "query",
     "report",
     "search",
     "snippet",
+    "tools",
 ]
```

### Comparing `athena_intelligence-0.1.39/src/athena/client.py` & `athena_intelligence-0.1.40/src/athena/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/core/__init__.py` & `athena_intelligence-0.1.40/src/athena/core/__init__.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/core/client_wrapper.py` & `athena_intelligence-0.1.40/src/athena/core/client_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self.api_key = api_key
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "athena-intelligence",
-            "X-Fern-SDK-Version": "0.1.39",
+            "X-Fern-SDK-Version": "0.1.40",
         }
         headers["X-API-KEY"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `athena_intelligence-0.1.39/src/athena/core/datetime_utils.py` & `athena_intelligence-0.1.40/src/athena/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/core/file.py` & `athena_intelligence-0.1.40/src/athena/core/file.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/core/http_client.py` & `athena_intelligence-0.1.40/src/athena/core/http_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/core/jsonable_encoder.py` & `athena_intelligence-0.1.40/src/athena/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/core/request_options.py` & `athena_intelligence-0.1.40/src/athena/core/request_options.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/dataset/client.py` & `athena_intelligence-0.1.40/src/athena/dataset/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/message/client.py` & `athena_intelligence-0.1.40/src/athena/message/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/polling_message_client.py` & `athena_intelligence-0.1.40/src/athena/polling_message_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/query/client.py` & `athena_intelligence-0.1.40/src/athena/query/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/report/client.py` & `athena_intelligence-0.1.40/src/athena/report/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/search/client.py` & `athena_intelligence-0.1.40/src/athena/search/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/snippet/client.py` & `athena_intelligence-0.1.40/src/athena/snippet/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/types/dataset.py` & `athena_intelligence-0.1.40/src/athena/types/dataset.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/types/get_datasets_response.py` & `athena_intelligence-0.1.40/src/athena/types/get_datasets_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/types/get_snippets_response.py` & `athena_intelligence-0.1.40/src/athena/types/get_snippets_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/types/http_validation_error.py` & `athena_intelligence-0.1.40/src/athena/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/types/message_out.py` & `athena_intelligence-0.1.40/src/athena/types/message_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/types/message_out_dto.py` & `athena_intelligence-0.1.40/src/athena/types/message_out_dto.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/types/model.py` & `athena_intelligence-0.1.40/src/athena/types/model.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/types/report.py` & `athena_intelligence-0.1.40/src/athena/types/report.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/types/scrape_markdown_result.py` & `athena_intelligence-0.1.40/src/athena/types/scrape_markdown_result.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/types/snippet.py` & `athena_intelligence-0.1.40/src/athena/types/snippet.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/types/sql_results.py` & `athena_intelligence-0.1.40/src/athena/types/sql_results.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/types/status_enum.py` & `athena_intelligence-0.1.40/src/athena/types/status_enum.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/types/tools.py` & `athena_intelligence-0.1.40/src/athena/types/tools.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/types/url_result.py` & `athena_intelligence-0.1.40/src/athena/types/url_result.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/src/athena/types/validation_error.py` & `athena_intelligence-0.1.40/src/athena/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.39/PKG-INFO` & `athena_intelligence-0.1.40/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athena-intelligence
-Version: 0.1.39
+Version: 0.1.40
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

