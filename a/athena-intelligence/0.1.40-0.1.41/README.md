# Comparing `tmp/athena_intelligence-0.1.40.tar.gz` & `tmp/athena_intelligence-0.1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athena_intelligence-0.1.40.tar", max compression
+gzip compressed data, was "athena_intelligence-0.1.41.tar", max compression
```

## Comparing `athena_intelligence-0.1.40.tar` & `athena_intelligence-0.1.41.tar`

### file list

```diff
@@ -1,58 +1,60 @@
--rw-r--r--   0        0        0     4235 2024-04-17 21:43:09.635540 athena_intelligence-0.1.40/README.md
--rw-r--r--   0        0        0      435 2024-04-17 21:43:09.635540 athena_intelligence-0.1.40/pyproject.toml
--rw-r--r--   0        0        0     1341 2024-04-17 21:43:09.635540 athena_intelligence-0.1.40/src/athena/__init__.py
--rw-r--r--   0        0        0     5416 2024-04-17 21:43:09.635540 athena_intelligence-0.1.40/src/athena/base_client.py
--rw-r--r--   0        0        0      161 2024-04-17 21:43:09.635540 athena_intelligence-0.1.40/src/athena/chain/__init__.py
--rw-r--r--   0        0        0     7401 2024-04-17 21:43:09.635540 athena_intelligence-0.1.40/src/athena/chain/client.py
--rw-r--r--   0        0        0      190 2024-04-17 21:43:09.635540 athena_intelligence-0.1.40/src/athena/chain/types/__init__.py
--rw-r--r--   0        0        0     2213 2024-04-17 21:43:09.635540 athena_intelligence-0.1.40/src/athena/chain/types/structured_tool_data_parsing_model.py
--rw-r--r--   0        0        0     3576 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/client.py
--rw-r--r--   0        0        0      790 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/core/api_error.py
--rw-r--r--   0        0        0     1198 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/core/file.py
--rw-r--r--   0        0        0     4882 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/core/http_client.py
--rw-r--r--   0        0        0     3799 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/core/request_options.py
--rw-r--r--   0        0        0       65 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/dataset/__init__.py
--rw-r--r--   0        0        0     6087 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/dataset/client.py
--rw-r--r--   0        0        0      165 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/environment.py
--rw-r--r--   0        0        0      170 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0       65 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/message/__init__.py
--rw-r--r--   0        0        0    12185 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/message/client.py
--rw-r--r--   0        0        0     3998 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/polling_message_client.py
--rw-r--r--   0        0        0        0 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/py.typed
--rw-r--r--   0        0        0       65 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/query/__init__.py
--rw-r--r--   0        0        0     6243 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/query/client.py
--rw-r--r--   0        0        0       65 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/report/__init__.py
--rw-r--r--   0        0        0     6528 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/report/client.py
--rw-r--r--   0        0        0       65 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/search/__init__.py
--rw-r--r--   0        0        0    12391 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/search/client.py
--rw-r--r--   0        0        0       65 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/snippet/__init__.py
--rw-r--r--   0        0        0     6087 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/snippet/client.py
--rw-r--r--   0        0        0       65 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/tools/__init__.py
--rw-r--r--   0        0        0     6657 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/tools/client.py
--rw-r--r--   0        0        0     1370 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/__init__.py
--rw-r--r--   0        0        0     1014 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/dataset.py
--rw-r--r--   0        0        0     1021 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py
--rw-r--r--   0        0        0     1128 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/firecrawl_scrape_url_metadata.py
--rw-r--r--   0        0        0      989 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/get_datasets_response.py
--rw-r--r--   0        0        0      989 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/get_snippets_response.py
--rw-r--r--   0        0        0      973 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/http_validation_error.py
--rw-r--r--   0        0        0      865 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/message_out.py
--rw-r--r--   0        0        0     1051 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/message_out_dto.py
--rw-r--r--   0        0        0     2545 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/model.py
--rw-r--r--   0        0        0      946 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/report.py
--rw-r--r--   0        0        0      881 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/scrape_markdown_result.py
--rw-r--r--   0        0        0     1126 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/snippet.py
--rw-r--r--   0        0        0      900 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/sql_results.py
--rw-r--r--   0        0        0      672 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/status_enum.py
--rw-r--r--   0        0        0      905 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/structured_parse_result.py
--rw-r--r--   0        0        0     1422 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/tools.py
--rw-r--r--   0        0        0      893 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/url_result.py
--rw-r--r--   0        0        0      992 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-17 21:43:09.639540 athena_intelligence-0.1.40/src/athena/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.40/PKG-INFO
+-rw-r--r--   0        0        0     4235 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/README.md
+-rw-r--r--   0        0        0      435 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/pyproject.toml
+-rw-r--r--   0        0        0     1455 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/__init__.py
+-rw-r--r--   0        0        0     5416 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/base_client.py
+-rw-r--r--   0        0        0      159 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/chain/__init__.py
+-rw-r--r--   0        0        0     8333 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/chain/client.py
+-rw-r--r--   0        0        0      187 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/chain/types/__init__.py
+-rw-r--r--   0        0        0     2203 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/chain/types/structured_parse_in_parsing_model.py
+-rw-r--r--   0        0        0     3576 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/client.py
+-rw-r--r--   0        0        0      790 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/core/api_error.py
+-rw-r--r--   0        0        0     1198 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/core/file.py
+-rw-r--r--   0        0        0     4882 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/core/http_client.py
+-rw-r--r--   0        0        0     3799 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/core/request_options.py
+-rw-r--r--   0        0        0       65 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/dataset/__init__.py
+-rw-r--r--   0        0        0     6087 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/dataset/client.py
+-rw-r--r--   0        0        0      165 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/environment.py
+-rw-r--r--   0        0        0      170 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0       65 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/message/__init__.py
+-rw-r--r--   0        0        0    12185 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/message/client.py
+-rw-r--r--   0        0        0     3998 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/polling_message_client.py
+-rw-r--r--   0        0        0        0 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/py.typed
+-rw-r--r--   0        0        0       65 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/query/__init__.py
+-rw-r--r--   0        0        0     6243 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/query/client.py
+-rw-r--r--   0        0        0       65 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/report/__init__.py
+-rw-r--r--   0        0        0     6528 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/report/client.py
+-rw-r--r--   0        0        0       65 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/search/__init__.py
+-rw-r--r--   0        0        0     7515 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/search/client.py
+-rw-r--r--   0        0        0       65 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/snippet/__init__.py
+-rw-r--r--   0        0        0     6087 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/snippet/client.py
+-rw-r--r--   0        0        0       65 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/tools/__init__.py
+-rw-r--r--   0        0        0    19332 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/tools/client.py
+-rw-r--r--   0        0        0     1553 2024-04-18 00:32:25.310801 athena_intelligence-0.1.41/src/athena/types/__init__.py
+-rw-r--r--   0        0        0     1014 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/dataset.py
+-rw-r--r--   0        0        0     1081 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/document.py
+-rw-r--r--   0        0        0      895 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/excecute_tool_first_workflow_out.py
+-rw-r--r--   0        0        0     1021 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py
+-rw-r--r--   0        0        0     1128 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/firecrawl_scrape_url_metadata.py
+-rw-r--r--   0        0        0      989 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/get_datasets_response.py
+-rw-r--r--   0        0        0      989 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/get_snippets_response.py
+-rw-r--r--   0        0        0      973 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/http_validation_error.py
+-rw-r--r--   0        0        0      939 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/langchain_documents_request_out.py
+-rw-r--r--   0        0        0      865 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/message_out.py
+-rw-r--r--   0        0        0     1051 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/message_out_dto.py
+-rw-r--r--   0        0        0     2545 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/model.py
+-rw-r--r--   0        0        0      946 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/report.py
+-rw-r--r--   0        0        0     1126 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/snippet.py
+-rw-r--r--   0        0        0      900 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/sql_results.py
+-rw-r--r--   0        0        0      672 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/status_enum.py
+-rw-r--r--   0        0        0      905 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/structured_parse_result.py
+-rw-r--r--   0        0        0     1422 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/tools.py
+-rw-r--r--   0        0        0      893 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/url_result.py
+-rw-r--r--   0        0        0      992 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-18 00:32:25.314801 athena_intelligence-0.1.41/src/athena/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.41/PKG-INFO
```

### Comparing `athena_intelligence-0.1.40/README.md` & `athena_intelligence-0.1.41/README.md`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/base_client.py` & `athena_intelligence-0.1.41/src/athena/base_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/chain/client.py` & `athena_intelligence-0.1.41/src/athena/query/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,71 +7,60 @@
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.http_validation_error import HttpValidationError
-from ..types.structured_parse_result import StructuredParseResult
-from .types.structured_tool_data_parsing_model import StructuredToolDataParsingModel
+from ..types.sql_results import SqlResults
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class ChainClient:
+class QueryClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def structured_parse(
-        self,
-        *,
-        text_input: str,
-        custom_type_dict: typing.Dict[str, typing.Any],
-        parsing_model: typing.Optional[StructuredToolDataParsingModel] = OMIT,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> StructuredParseResult:
+    def execute(
+        self, *, sql_command: str, database_id: int, request_options: typing.Optional[RequestOptions] = None
+    ) -> SqlResults:
         """
         Parameters:
-            - text_input: str. The text input to be parsed.
+            - sql_command: str.
 
-            - custom_type_dict: typing.Dict[str, typing.Any]. A dictionary of field names and their default values.
-
-            - parsing_model: typing.Optional[StructuredToolDataParsingModel]. The model to be used for parsing.
+            - database_id: int.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from athena.client import Athena
 
         client = Athena(
             api_key="YOUR_API_KEY",
         )
-        client.chain.structured_parse(
-            text_input="text_input",
-            custom_type_dict={},
+        client.query.execute(
+            sql_command="sql_command",
+            database_id=1,
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"text_input": text_input, "custom_type_dict": custom_type_dict}
-        if parsing_model is not OMIT:
-            _request["parsing_model"] = parsing_model
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/structured-parse"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/execute-sql"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(_request)
+            json=jsonable_encoder({"sql_command": sql_command, "database_id": database_id})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(_request),
+                **jsonable_encoder({"sql_command": sql_command, "database_id": database_id}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -81,69 +70,59 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else 60,
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(StructuredParseResult, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(SqlResults, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncChainClient:
+class AsyncQueryClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def structured_parse(
-        self,
-        *,
-        text_input: str,
-        custom_type_dict: typing.Dict[str, typing.Any],
-        parsing_model: typing.Optional[StructuredToolDataParsingModel] = OMIT,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> StructuredParseResult:
+    async def execute(
+        self, *, sql_command: str, database_id: int, request_options: typing.Optional[RequestOptions] = None
+    ) -> SqlResults:
         """
         Parameters:
-            - text_input: str. The text input to be parsed.
-
-            - custom_type_dict: typing.Dict[str, typing.Any]. A dictionary of field names and their default values.
+            - sql_command: str.
 
-            - parsing_model: typing.Optional[StructuredToolDataParsingModel]. The model to be used for parsing.
+            - database_id: int.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from athena.client import AsyncAthena
 
         client = AsyncAthena(
             api_key="YOUR_API_KEY",
         )
-        await client.chain.structured_parse(
-            text_input="text_input",
-            custom_type_dict={},
+        await client.query.execute(
+            sql_command="sql_command",
+            database_id=1,
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"text_input": text_input, "custom_type_dict": custom_type_dict}
-        if parsing_model is not OMIT:
-            _request["parsing_model"] = parsing_model
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/structured-parse"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/execute-sql"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(_request)
+            json=jsonable_encoder({"sql_command": sql_command, "database_id": database_id})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(_request),
+                **jsonable_encoder({"sql_command": sql_command, "database_id": database_id}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -153,15 +132,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else 60,
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(StructuredParseResult, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(SqlResults, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `athena_intelligence-0.1.40/src/athena/chain/types/structured_tool_data_parsing_model.py` & `athena_intelligence-0.1.41/src/athena/chain/types/structured_parse_in_parsing_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class StructuredToolDataParsingModel(str, enum.Enum):
+class StructuredParseInParsingModel(str, enum.Enum):
     """
     The model to be used for parsing.
     """
 
     GPT_4_TURBO = "gpt-4-turbo"
     GPT_4_TURBO_PREVIEW = "gpt-4-turbo-preview"
     GPT_4 = "gpt-4"
@@ -29,25 +29,25 @@
         gpt_35_turbo: typing.Callable[[], T_Result],
         mixtral_small_8_x_7_b_0211: typing.Callable[[], T_Result],
         mistral_large_0224: typing.Callable[[], T_Result],
         claude_3_opus_20240229: typing.Callable[[], T_Result],
         claude_3_sonnet_20240229: typing.Callable[[], T_Result],
         claude_3_haiku_20240307: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is StructuredToolDataParsingModel.GPT_4_TURBO:
+        if self is StructuredParseInParsingModel.GPT_4_TURBO:
             return gpt_4_turbo()
-        if self is StructuredToolDataParsingModel.GPT_4_TURBO_PREVIEW:
+        if self is StructuredParseInParsingModel.GPT_4_TURBO_PREVIEW:
             return gpt_4_turbo_preview()
-        if self is StructuredToolDataParsingModel.GPT_4:
+        if self is StructuredParseInParsingModel.GPT_4:
             return gpt_4()
-        if self is StructuredToolDataParsingModel.GPT_35_TURBO:
+        if self is StructuredParseInParsingModel.GPT_35_TURBO:
             return gpt_35_turbo()
-        if self is StructuredToolDataParsingModel.MIXTRAL_SMALL_8_X_7_B_0211:
+        if self is StructuredParseInParsingModel.MIXTRAL_SMALL_8_X_7_B_0211:
             return mixtral_small_8_x_7_b_0211()
-        if self is StructuredToolDataParsingModel.MISTRAL_LARGE_0224:
+        if self is StructuredParseInParsingModel.MISTRAL_LARGE_0224:
             return mistral_large_0224()
-        if self is StructuredToolDataParsingModel.CLAUDE_3_OPUS_20240229:
+        if self is StructuredParseInParsingModel.CLAUDE_3_OPUS_20240229:
             return claude_3_opus_20240229()
-        if self is StructuredToolDataParsingModel.CLAUDE_3_SONNET_20240229:
+        if self is StructuredParseInParsingModel.CLAUDE_3_SONNET_20240229:
             return claude_3_sonnet_20240229()
-        if self is StructuredToolDataParsingModel.CLAUDE_3_HAIKU_20240307:
+        if self is StructuredParseInParsingModel.CLAUDE_3_HAIKU_20240307:
             return claude_3_haiku_20240307()
```

### Comparing `athena_intelligence-0.1.40/src/athena/client.py` & `athena_intelligence-0.1.41/src/athena/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/core/__init__.py` & `athena_intelligence-0.1.41/src/athena/core/__init__.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/core/client_wrapper.py` & `athena_intelligence-0.1.41/src/athena/core/client_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self.api_key = api_key
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "athena-intelligence",
-            "X-Fern-SDK-Version": "0.1.40",
+            "X-Fern-SDK-Version": "0.1.41",
         }
         headers["X-API-KEY"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `athena_intelligence-0.1.40/src/athena/core/datetime_utils.py` & `athena_intelligence-0.1.41/src/athena/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/core/file.py` & `athena_intelligence-0.1.41/src/athena/core/file.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/core/http_client.py` & `athena_intelligence-0.1.41/src/athena/core/http_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/core/jsonable_encoder.py` & `athena_intelligence-0.1.41/src/athena/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/core/request_options.py` & `athena_intelligence-0.1.41/src/athena/core/request_options.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/dataset/client.py` & `athena_intelligence-0.1.41/src/athena/dataset/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/message/client.py` & `athena_intelligence-0.1.41/src/athena/message/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/polling_message_client.py` & `athena_intelligence-0.1.41/src/athena/polling_message_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/query/client.py` & `athena_intelligence-0.1.41/src/athena/snippet/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,63 +6,65 @@
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
+from ..types.get_snippets_response import GetSnippetsResponse
 from ..types.http_validation_error import HttpValidationError
-from ..types.sql_results import SqlResults
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
-# this is used as the default value for optional parameters
-OMIT = typing.cast(typing.Any, ...)
 
-
-class QueryClient:
+class SnippetClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def execute(
-        self, *, sql_command: str, database_id: int, request_options: typing.Optional[RequestOptions] = None
-    ) -> SqlResults:
+    def get(
+        self,
+        *,
+        page: typing.Optional[int] = None,
+        page_size: typing.Optional[int] = None,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> GetSnippetsResponse:
         """
         Parameters:
-            - sql_command: str.
+            - page: typing.Optional[int]. Page number starting from 1
 
-            - database_id: int.
+            - page_size: typing.Optional[int]. Number of items per page
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from athena.client import Athena
 
         client = Athena(
             api_key="YOUR_API_KEY",
         )
-        client.query.execute(
-            sql_command="sql_command",
-            database_id=1,
-        )
+        client.snippet.get()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/execute-sql"),
+            "GET",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/snippets"),
             params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+                remove_none_from_dict(
+                    {
+                        "page": page,
+                        "page_size": page_size,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
             ),
-            json=jsonable_encoder({"sql_command": sql_command, "database_id": database_id})
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder({"sql_command": sql_command, "database_id": database_id}),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -70,61 +72,66 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else 60,
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(SqlResults, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(GetSnippetsResponse, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncQueryClient:
+class AsyncSnippetClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def execute(
-        self, *, sql_command: str, database_id: int, request_options: typing.Optional[RequestOptions] = None
-    ) -> SqlResults:
+    async def get(
+        self,
+        *,
+        page: typing.Optional[int] = None,
+        page_size: typing.Optional[int] = None,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> GetSnippetsResponse:
         """
         Parameters:
-            - sql_command: str.
+            - page: typing.Optional[int]. Page number starting from 1
 
-            - database_id: int.
+            - page_size: typing.Optional[int]. Number of items per page
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from athena.client import AsyncAthena
 
         client = AsyncAthena(
             api_key="YOUR_API_KEY",
         )
-        await client.query.execute(
-            sql_command="sql_command",
-            database_id=1,
-        )
+        await client.snippet.get()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/execute-sql"),
+            "GET",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/snippets"),
             params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+                remove_none_from_dict(
+                    {
+                        "page": page,
+                        "page_size": page_size,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
             ),
-            json=jsonable_encoder({"sql_command": sql_command, "database_id": database_id})
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder({"sql_command": sql_command, "database_id": database_id}),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -132,15 +139,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else 60,
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(SqlResults, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(GetSnippetsResponse, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `athena_intelligence-0.1.40/src/athena/report/client.py` & `athena_intelligence-0.1.41/src/athena/report/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/types/__init__.py` & `athena_intelligence-0.1.41/src/athena/types/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .dataset import Dataset
+from .document import Document
+from .excecute_tool_first_workflow_out import ExcecuteToolFirstWorkflowOut
 from .firecrawl_scrape_url_data_reponse_dto import FirecrawlScrapeUrlDataReponseDto
 from .firecrawl_scrape_url_metadata import FirecrawlScrapeUrlMetadata
 from .get_datasets_response import GetDatasetsResponse
 from .get_snippets_response import GetSnippetsResponse
 from .http_validation_error import HttpValidationError
+from .langchain_documents_request_out import LangchainDocumentsRequestOut
 from .message_out import MessageOut
 from .message_out_dto import MessageOutDto
 from .model import Model
 from .report import Report
-from .scrape_markdown_result import ScrapeMarkdownResult
 from .snippet import Snippet
 from .sql_results import SqlResults
 from .status_enum import StatusEnum
 from .structured_parse_result import StructuredParseResult
 from .tools import Tools
 from .url_result import UrlResult
 from .validation_error import ValidationError
 from .validation_error_loc_item import ValidationErrorLocItem
 
 __all__ = [
     "Dataset",
+    "Document",
+    "ExcecuteToolFirstWorkflowOut",
     "FirecrawlScrapeUrlDataReponseDto",
     "FirecrawlScrapeUrlMetadata",
     "GetDatasetsResponse",
     "GetSnippetsResponse",
     "HttpValidationError",
+    "LangchainDocumentsRequestOut",
     "MessageOut",
     "MessageOutDto",
     "Model",
     "Report",
-    "ScrapeMarkdownResult",
     "Snippet",
     "SqlResults",
     "StatusEnum",
     "StructuredParseResult",
     "Tools",
     "UrlResult",
     "ValidationError",
```

### Comparing `athena_intelligence-0.1.40/src/athena/types/dataset.py` & `athena_intelligence-0.1.41/src/athena/types/dataset.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py` & `athena_intelligence-0.1.41/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/types/firecrawl_scrape_url_metadata.py` & `athena_intelligence-0.1.41/src/athena/types/firecrawl_scrape_url_metadata.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/types/get_datasets_response.py` & `athena_intelligence-0.1.41/src/athena/types/get_datasets_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/types/get_snippets_response.py` & `athena_intelligence-0.1.41/src/athena/types/get_snippets_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/types/http_validation_error.py` & `athena_intelligence-0.1.41/src/athena/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/types/message_out.py` & `athena_intelligence-0.1.41/src/athena/types/message_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/types/message_out_dto.py` & `athena_intelligence-0.1.41/src/athena/types/message_out_dto.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/types/model.py` & `athena_intelligence-0.1.41/src/athena/types/model.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/types/report.py` & `athena_intelligence-0.1.41/src/athena/types/report.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/types/scrape_markdown_result.py` & `athena_intelligence-0.1.41/src/athena/types/structured_parse_result.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ScrapeMarkdownResult(pydantic.BaseModel):
-    markdown: str
+class StructuredParseResult(pydantic.BaseModel):
+    result: typing.Dict[str, typing.Any]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `athena_intelligence-0.1.40/src/athena/types/snippet.py` & `athena_intelligence-0.1.41/src/athena/types/snippet.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/types/sql_results.py` & `athena_intelligence-0.1.41/src/athena/types/sql_results.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/types/status_enum.py` & `athena_intelligence-0.1.41/src/athena/types/status_enum.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/types/structured_parse_result.py` & `athena_intelligence-0.1.41/src/athena/types/document.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,22 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class StructuredParseResult(pydantic.BaseModel):
-    result: typing.Dict[str, typing.Any]
+class Document(pydantic.BaseModel):
+    """
+    Class for storing a piece of text and associated metadata.
+    """
+
+    page_content: str
+    metadata: typing.Optional[typing.Dict[str, typing.Any]] = None
+    type: typing.Optional[typing.Literal["Document"]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `athena_intelligence-0.1.40/src/athena/types/tools.py` & `athena_intelligence-0.1.41/src/athena/types/tools.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/types/url_result.py` & `athena_intelligence-0.1.41/src/athena/types/url_result.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/src/athena/types/validation_error.py` & `athena_intelligence-0.1.41/src/athena/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.40/PKG-INFO` & `athena_intelligence-0.1.41/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athena-intelligence
-Version: 0.1.40
+Version: 0.1.41
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

