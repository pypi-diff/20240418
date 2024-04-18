# Comparing `tmp/robotframework_openapitools-0.2.0.tar.gz` & `tmp/robotframework_openapitools-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_openapitools-0.2.0.tar", max compression
+gzip compressed data, was "robotframework_openapitools-0.2.1.tar", max compression
```

## Comparing `robotframework_openapitools-0.2.0.tar` & `robotframework_openapitools-0.2.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rwxr-xr-x   0        0        0    11558 2024-02-12 15:55:24.206229 robotframework_openapitools-0.2.0/LICENSE
--rwxr-xr-x   0        0        0      185 2024-03-08 15:13:37.215159 robotframework_openapitools-0.2.0/docs/README.md
--rwxr-xr-x   0        0        0     3371 2024-04-12 13:00:01.288060 robotframework_openapitools-0.2.0/pyproject.toml
--rwxr-xr-x   0        0        0     1331 2024-03-06 16:35:05.537954 robotframework_openapitools-0.2.0/src/OpenApiDriver/__init__.py
--rw-r--r--   0        0        0    32851 2024-04-12 12:59:35.488243 robotframework_openapitools-0.2.0/src/OpenApiDriver/openapi_executors.py
--rwxr-xr-x   0        0        0     4652 2024-03-15 20:22:54.832269 robotframework_openapitools-0.2.0/src/OpenApiDriver/openapi_reader.py
--rw-r--r--   0        0        0    28323 2024-04-12 13:08:13.742460 robotframework_openapitools-0.2.0/src/OpenApiDriver/openapidriver.libspec
--rw-r--r--   0        0        0    15214 2024-04-12 12:59:35.504855 robotframework_openapitools-0.2.0/src/OpenApiDriver/openapidriver.py
--rwxr-xr-x   0        0        0        0 2024-01-31 08:42:12.630853 robotframework_openapitools-0.2.0/src/OpenApiDriver/py.typed
--rwxr-xr-x   0        0        0     1591 2024-02-12 14:16:27.194996 robotframework_openapitools-0.2.0/src/OpenApiLibCore/__init__.py
--rw-r--r--   0        0        0    11764 2024-04-12 12:59:35.521702 robotframework_openapitools-0.2.0/src/OpenApiLibCore/dto_base.py
--rwxr-xr-x   0        0        0     2903 2024-02-12 14:16:27.196984 robotframework_openapitools-0.2.0/src/OpenApiLibCore/dto_utils.py
--rwxr-xr-x   0        0        0      112 2024-03-06 08:33:13.925424 robotframework_openapitools-0.2.0/src/OpenApiLibCore/oas_cache.py
--rw-r--r--   0        0        0    33102 2024-04-12 13:08:13.149393 robotframework_openapitools-0.2.0/src/OpenApiLibCore/openapi_libcore.libspec
--rw-r--r--   0        0        0    63998 2024-04-12 12:59:35.521702 robotframework_openapitools-0.2.0/src/OpenApiLibCore/openapi_libcore.py
--rwxr-xr-x   0        0        0        0 2024-01-31 08:43:45.640076 robotframework_openapitools-0.2.0/src/OpenApiLibCore/py.typed
--rwxr-xr-x   0        0        0    18145 2024-01-31 08:43:45.640833 robotframework_openapitools-0.2.0/src/OpenApiLibCore/value_utils.py
--rwxr-xr-x   0        0        0      223 2024-03-06 16:35:05.808004 robotframework_openapitools-0.2.0/src/roboswag/__init__.py
--rwxr-xr-x   0        0        0       35 2024-02-12 15:55:24.208754 robotframework_openapitools-0.2.0/src/roboswag/__main__.py
--rwxr-xr-x   0        0        0     1323 2024-03-06 16:35:03.918414 robotframework_openapitools-0.2.0/src/roboswag/auth.py
--rwxr-xr-x   0        0        0     2216 2024-03-06 16:35:05.748050 robotframework_openapitools-0.2.0/src/roboswag/cli.py
--rwxr-xr-x   0        0        0     2870 2024-03-06 16:35:03.983780 robotframework_openapitools-0.2.0/src/roboswag/core.py
--rwxr-xr-x   0        0        0       59 2024-02-12 15:55:24.222947 robotframework_openapitools-0.2.0/src/roboswag/generate/__init__.py
--rwxr-xr-x   0        0        0     4706 2024-03-06 16:35:04.067930 robotframework_openapitools-0.2.0/src/roboswag/generate/generate.py
--rwxr-xr-x   0        0        0        0 2024-02-12 15:55:24.223963 robotframework_openapitools-0.2.0/src/roboswag/generate/models/__init__.py
--rwxr-xr-x   0        0        0     8528 2024-03-06 16:35:04.137359 robotframework_openapitools-0.2.0/src/roboswag/generate/models/api.py
--rwxr-xr-x   0        0        0      841 2024-03-06 16:35:03.958474 robotframework_openapitools-0.2.0/src/roboswag/generate/models/definition.py
--rwxr-xr-x   0        0        0     2304 2024-03-06 16:35:04.024928 robotframework_openapitools-0.2.0/src/roboswag/generate/models/endpoint.py
--rwxr-xr-x   0        0        0      682 2024-03-06 16:35:03.991681 robotframework_openapitools-0.2.0/src/roboswag/generate/models/parameter.py
--rwxr-xr-x   0        0        0      257 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.0/src/roboswag/generate/models/response.py
--rwxr-xr-x   0        0        0      561 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.0/src/roboswag/generate/models/tag.py
--rwxr-xr-x   0        0        0     1550 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.0/src/roboswag/generate/models/utils.py
--rwxr-xr-x   0        0        0      621 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.0/src/roboswag/generate/templates/api_init.jinja
--rwxr-xr-x   0        0        0      357 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.0/src/roboswag/generate/templates/models.jinja
--rwxr-xr-x   0        0        0     3191 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.0/src/roboswag/generate/templates/paths.jinja
--rwxr-xr-x   0        0        0     1025 2024-03-06 16:35:04.038806 robotframework_openapitools-0.2.0/src/roboswag/logger.py
--rwxr-xr-x   0        0        0      188 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.0/src/roboswag/validate/__init__.py
--rwxr-xr-x   0        0        0       84 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.0/src/roboswag/validate/core.py
--rwxr-xr-x   0        0        0      711 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.0/src/roboswag/validate/schema.py
--rwxr-xr-x   0        0        0      527 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.0/src/roboswag/validate/text_response.py
--rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 robotframework_openapitools-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0    11558 2024-02-12 15:55:24.206229 robotframework_openapitools-0.2.1/LICENSE
+-rwxr-xr-x   0        0        0      185 2024-03-08 15:13:37.215159 robotframework_openapitools-0.2.1/docs/README.md
+-rwxr-xr-x   0        0        0     3371 2024-04-18 10:12:45.018662 robotframework_openapitools-0.2.1/pyproject.toml
+-rwxr-xr-x   0        0        0     1331 2024-03-06 16:35:05.537954 robotframework_openapitools-0.2.1/src/OpenApiDriver/__init__.py
+-rw-r--r--   0        0        0    32851 2024-04-12 12:59:35.488243 robotframework_openapitools-0.2.1/src/OpenApiDriver/openapi_executors.py
+-rwxr-xr-x   0        0        0     4652 2024-03-15 20:22:54.832269 robotframework_openapitools-0.2.1/src/OpenApiDriver/openapi_reader.py
+-rw-r--r--   0        0        0    28323 2024-04-18 10:17:56.759029 robotframework_openapitools-0.2.1/src/OpenApiDriver/openapidriver.libspec
+-rw-r--r--   0        0        0    15214 2024-04-12 12:59:35.504855 robotframework_openapitools-0.2.1/src/OpenApiDriver/openapidriver.py
+-rwxr-xr-x   0        0        0        0 2024-01-31 08:42:12.630853 robotframework_openapitools-0.2.1/src/OpenApiDriver/py.typed
+-rwxr-xr-x   0        0        0     1591 2024-02-12 14:16:27.194996 robotframework_openapitools-0.2.1/src/OpenApiLibCore/__init__.py
+-rw-r--r--   0        0        0    11794 2024-04-18 09:40:15.299767 robotframework_openapitools-0.2.1/src/OpenApiLibCore/dto_base.py
+-rwxr-xr-x   0        0        0     2903 2024-02-12 14:16:27.196984 robotframework_openapitools-0.2.1/src/OpenApiLibCore/dto_utils.py
+-rwxr-xr-x   0        0        0      379 2024-04-18 10:15:55.247807 robotframework_openapitools-0.2.1/src/OpenApiLibCore/oas_cache.py
+-rw-r--r--   0        0        0    33102 2024-04-18 10:17:56.170803 robotframework_openapitools-0.2.1/src/OpenApiLibCore/openapi_libcore.libspec
+-rwxr-xr-x   0        0        0    65826 2024-04-18 10:15:55.249816 robotframework_openapitools-0.2.1/src/OpenApiLibCore/openapi_libcore.py
+-rwxr-xr-x   0        0        0        0 2024-01-31 08:43:45.640076 robotframework_openapitools-0.2.1/src/OpenApiLibCore/py.typed
+-rwxr-xr-x   0        0        0    18145 2024-01-31 08:43:45.640833 robotframework_openapitools-0.2.1/src/OpenApiLibCore/value_utils.py
+-rwxr-xr-x   0        0        0      223 2024-03-06 16:35:05.808004 robotframework_openapitools-0.2.1/src/roboswag/__init__.py
+-rwxr-xr-x   0        0        0       35 2024-02-12 15:55:24.208754 robotframework_openapitools-0.2.1/src/roboswag/__main__.py
+-rwxr-xr-x   0        0        0     1323 2024-03-06 16:35:03.918414 robotframework_openapitools-0.2.1/src/roboswag/auth.py
+-rwxr-xr-x   0        0        0     2216 2024-03-06 16:35:05.748050 robotframework_openapitools-0.2.1/src/roboswag/cli.py
+-rwxr-xr-x   0        0        0     2870 2024-03-06 16:35:03.983780 robotframework_openapitools-0.2.1/src/roboswag/core.py
+-rwxr-xr-x   0        0        0       59 2024-02-12 15:55:24.222947 robotframework_openapitools-0.2.1/src/roboswag/generate/__init__.py
+-rwxr-xr-x   0        0        0     4706 2024-03-06 16:35:04.067930 robotframework_openapitools-0.2.1/src/roboswag/generate/generate.py
+-rwxr-xr-x   0        0        0        0 2024-02-12 15:55:24.223963 robotframework_openapitools-0.2.1/src/roboswag/generate/models/__init__.py
+-rwxr-xr-x   0        0        0     8528 2024-03-06 16:35:04.137359 robotframework_openapitools-0.2.1/src/roboswag/generate/models/api.py
+-rwxr-xr-x   0        0        0      841 2024-03-06 16:35:03.958474 robotframework_openapitools-0.2.1/src/roboswag/generate/models/definition.py
+-rwxr-xr-x   0        0        0     2304 2024-03-06 16:35:04.024928 robotframework_openapitools-0.2.1/src/roboswag/generate/models/endpoint.py
+-rwxr-xr-x   0        0        0      682 2024-03-06 16:35:03.991681 robotframework_openapitools-0.2.1/src/roboswag/generate/models/parameter.py
+-rwxr-xr-x   0        0        0      257 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.1/src/roboswag/generate/models/response.py
+-rwxr-xr-x   0        0        0      561 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.1/src/roboswag/generate/models/tag.py
+-rwxr-xr-x   0        0        0     1550 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.1/src/roboswag/generate/models/utils.py
+-rwxr-xr-x   0        0        0      621 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.1/src/roboswag/generate/templates/api_init.jinja
+-rwxr-xr-x   0        0        0      357 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.1/src/roboswag/generate/templates/models.jinja
+-rwxr-xr-x   0        0        0     3191 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.1/src/roboswag/generate/templates/paths.jinja
+-rwxr-xr-x   0        0        0     1025 2024-03-06 16:35:04.038806 robotframework_openapitools-0.2.1/src/roboswag/logger.py
+-rwxr-xr-x   0        0        0      188 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.1/src/roboswag/validate/__init__.py
+-rwxr-xr-x   0        0        0       84 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.1/src/roboswag/validate/core.py
+-rwxr-xr-x   0        0        0      711 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.1/src/roboswag/validate/schema.py
+-rwxr-xr-x   0        0        0      527 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.1/src/roboswag/validate/text_response.py
+-rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 robotframework_openapitools-0.2.1/PKG-INFO
```

### Comparing `robotframework_openapitools-0.2.0/LICENSE` & `robotframework_openapitools-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.0/pyproject.toml` & `robotframework_openapitools-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name="robotframework-openapitools"
-version = "0.2.0"
+version = "0.2.1"
 description = "A set of Robot Framework libraries to test APIs for which the OAS is available."
 license = "Apache-2.0"
 authors = [
     "Bartlomiej Hirsz <bartek.hirsz@gmail.com>",
     "Mateusz Nojek <matnojek@gmail.com>",
     "Robin Mackaij <r.a.mackaij@gmail.com>"
 ]
```

### Comparing `robotframework_openapitools-0.2.0/src/OpenApiDriver/__init__.py` & `robotframework_openapitools-0.2.1/src/OpenApiDriver/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.0/src/OpenApiDriver/openapi_executors.py` & `robotframework_openapitools-0.2.1/src/OpenApiDriver/openapi_executors.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.0/src/OpenApiDriver/openapi_reader.py` & `robotframework_openapitools-0.2.1/src/OpenApiDriver/openapi_reader.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.0/src/OpenApiDriver/openapidriver.libspec` & `robotframework_openapitools-0.2.1/src/OpenApiDriver/openapidriver.libspec`

 * *Files 0% similar despite different names*

#### Comparing `robotframework_openapitools-0.2.0/src/OpenApiDriver/openapidriver.libspec` & `robotframework_openapitools-0.2.1/src/OpenApiDriver/openapidriver.libspec`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
-<keywordspec name="OpenApiDriver" type="LIBRARY" format="HTML" scope="SUITE" generated="2024-04-12T13:08:14+00:00" specversion="5" source="/workspaces/robotframework-openapitools/src/OpenApiDriver/openapidriver.py" lineno="352">
-  <version>0.2.0</version>
+<keywordspec name="OpenApiDriver" type="LIBRARY" format="HTML" scope="SUITE" generated="2024-04-18T10:17:57+00:00" specversion="5" source="/workspaces/robotframework-openapitools/src/OpenApiDriver/openapidriver.py" lineno="352">
+  <version>0.2.1</version>
   <doc>&lt;p&gt;Visit the &lt;a href=&quot;https://github.com/MarketSquare/robotframework-openapidriver&quot;&gt;library page&lt;/a&gt; for an introduction and examples.&lt;/p&gt;</doc>
   <tags/>
   <inits>
     <init name="__init__" lineno="144">
       <arguments repr="source: str, origin: str = , base_path: str = , included_paths: Iterable[str] | None = None, ignored_paths: Iterable[str] | None = None, ignored_responses: Iterable[int] | None = None, ignored_testcases: Iterable[Tuple[str, str, int]] | None = None, response_validation: ValidationLevel = WARN, disable_server_validation: bool = True, mappings_path: str | Path = , invalid_property_default_response: int = 422, default_id_property_name: str = id, faker_locale: str | List[str] | None = None, require_body_for_invalid_url: bool = False, recursion_limit: int = 1, recursion_default: Any = {}, username: str = , password: str = , security_token: str = , auth: AuthBase | None = None, cert: str | Tuple[str, str] | None = None, verify_tls: bool | str | None = True, extra_headers: Dict[str, str] | None = None, cookies: Dict[str, str] | RequestsCookieJar | None = None, proxies: Dict[str, str] | None = None">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="source: str">
           <name>source</name>
```

### Comparing `robotframework_openapitools-0.2.0/src/OpenApiDriver/openapidriver.py` & `robotframework_openapitools-0.2.1/src/OpenApiDriver/openapidriver.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.0/src/OpenApiLibCore/__init__.py` & `robotframework_openapitools-0.2.1/src/OpenApiLibCore/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.0/src/OpenApiLibCore/dto_base.py` & `robotframework_openapitools-0.2.1/src/OpenApiLibCore/dto_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,16 +72,16 @@
         if key in merged_schema.keys():
             if isinstance(value, dict):
                 # if the key holds a dict, merge the values (e.g. 'properties')
                 merged_schema[key].update(value)
             elif isinstance(value, list):
                 # if the key holds a list, extend the values (e.g. 'required')
                 merged_schema[key].extend(value)
-            else:
-                logger.debug(
+            elif value != merged_schema[key]:
+                logger.warning(
                     f"key '{key}' with value '{merged_schema[key]}' not "
                     f"updated to '{value}'"
                 )
         else:
             merged_schema[key] = value
     return merged_schema
```

### Comparing `robotframework_openapitools-0.2.0/src/OpenApiLibCore/dto_utils.py` & `robotframework_openapitools-0.2.1/src/OpenApiLibCore/dto_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.0/src/OpenApiLibCore/openapi_libcore.libspec` & `robotframework_openapitools-0.2.1/src/OpenApiLibCore/openapi_libcore.libspec`

 * *Files 0% similar despite different names*

#### Comparing `robotframework_openapitools-0.2.0/src/OpenApiLibCore/openapi_libcore.libspec` & `robotframework_openapitools-0.2.1/src/OpenApiLibCore/openapi_libcore.libspec`

```diff
@@ -1,15 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
-<keywordspec name="OpenApiLibCore" type="LIBRARY" format="HTML" scope="SUITE" generated="2024-04-12T13:08:13+00:00" specversion="5" source="/workspaces/robotframework-openapitools/src/OpenApiLibCore/openapi_libcore.py" lineno="404">
-  <version>0.2.0</version>
+<keywordspec name="OpenApiLibCore" type="LIBRARY" format="HTML" scope="SUITE" generated="2024-04-18T10:17:56+00:00" specversion="5" source="/workspaces/robotframework-openapitools/src/OpenApiLibCore/openapi_libcore.py" lineno="415">
+  <version>0.2.1</version>
   <doc>&lt;p&gt;Main class providing the keywords and core logic to interact with an OpenAPI server.&lt;/p&gt;
 &lt;p&gt;Visit the &lt;a href=&quot;https://github.com/MarketSquare/robotframework-openapi-libcore&quot;&gt;library page&lt;/a&gt; for an introduction.&lt;/p&gt;</doc>
   <tags/>
   <inits>
-    <init name="__init__" lineno="412">
+    <init name="__init__" lineno="423">
       <arguments repr="source: str, origin: str = , base_path: str = , mappings_path: str | Path = , invalid_property_default_response: int = 422, default_id_property_name: str = id, faker_locale: str | List[str] | None = None, recursion_limit: int = 1, recursion_default: Any = {}, username: str = , password: str = , security_token: str = , auth: AuthBase | None = None, cert: str | Tuple[str, str] | None = None, verify_tls: bool | str | None = True, extra_headers: Dict[str, str] | None = None, cookies: Dict[str, str] | RequestsCookieJar | None = None, proxies: Dict[str, str] | None = None">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="source: str">
           <name>source</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="origin: str = ">
           <name>origin</name>
@@ -194,15 +194,15 @@
 &lt;p&gt;A dictionary or &lt;a href=&quot;https://docs.python.org/3/library/http.cookiejar.html#http.cookiejar.CookieJar&quot;&gt;CookieJar object&lt;/a&gt; to send with all requests.&lt;/p&gt;
 &lt;h4&gt;proxies&lt;/h4&gt;
 &lt;p&gt;A dictionary of 'protocol': 'proxy url' to use for all requests.&lt;/p&gt;</doc>
       <shortdoc>== Base parameters ==</shortdoc>
     </init>
   </inits>
   <keywords>
-    <kw name="Authorized Request" lineno="1535">
+    <kw name="Authorized Request" lineno="1591">
       <arguments repr="url: str, method: str, params: Dict[str, Any] | None = None, headers: Dict[str, str] | None = None, json_data: Dict[str, Dict[str, ForwardRef('JSON')] | List[ForwardRef('JSON')] | str | int | float | bool | None] | List[Dict[str, ForwardRef('JSON')] | List[ForwardRef('JSON')] | str | int | float | bool | None] | str | int | float | bool | None = None">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -288,39 +288,39 @@
           <default>None</default>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Perform a request using the security token or authentication set in the library.&lt;/p&gt;
 &lt;p&gt;&amp;gt; Note: provided username / password or auth objects take precedence over token based security&lt;/p&gt;</doc>
       <shortdoc>Perform a request using the security token or authentication set in the library.</shortdoc>
     </kw>
-    <kw name="Ensure In Use" lineno="1439">
+    <kw name="Ensure In Use" lineno="1495">
       <arguments repr="url: str, resource_relation: IdReference">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="resource_relation: IdReference">
           <name>resource_relation</name>
           <type name="IdReference">IdReference</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Ensure that the (right-most) &lt;span class=&quot;name&quot;&gt;id&lt;/span&gt; of the resource referenced by the &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt; is used by the resource defined by the &lt;span class=&quot;name&quot;&gt;resource_relation&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Ensure that the (right-most) `id` of the resource referenced by the `url` is used by the resource defined by the `resource_relation`.</shortdoc>
     </kw>
-    <kw name="Get Ids From Url" lineno="810">
+    <kw name="Get Ids From Url" lineno="866">
       <arguments repr="url: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Perform a GET request on the &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt; and return the list of resource &lt;span class=&quot;name&quot;&gt;ids&lt;/span&gt; from the response.&lt;/p&gt;</doc>
       <shortdoc>Perform a GET request on the `url` and return the list of resource `ids` from the response.</shortdoc>
     </kw>
-    <kw name="Get Invalid Json Data" lineno="1216">
+    <kw name="Get Invalid Json Data" lineno="1272">
       <arguments repr="url: str, method: str, status_code: int, request_data: RequestData">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -335,40 +335,40 @@
           <type name="RequestData">RequestData</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return &lt;span class=&quot;name&quot;&gt;json_data&lt;/span&gt; based on the &lt;span class=&quot;name&quot;&gt;dto&lt;/span&gt; on the &lt;span class=&quot;name&quot;&gt;request_data&lt;/span&gt; that will cause the provided &lt;span class=&quot;name&quot;&gt;status_code&lt;/span&gt; for the &lt;span class=&quot;name&quot;&gt;method&lt;/span&gt; operation on the &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt;.&lt;/p&gt;
 &lt;p&gt;&amp;gt; Note: applicable UniquePropertyValueConstraint and IdReference Relations are considered before changes to &lt;span class=&quot;name&quot;&gt;json_data&lt;/span&gt; are made.&lt;/p&gt;</doc>
       <shortdoc>Return `json_data` based on the `dto` on the `request_data` that will cause the provided `status_code` for the `method` operation on the `url`.</shortdoc>
     </kw>
-    <kw name="Get Invalidated Parameters" lineno="1264">
+    <kw name="Get Invalidated Parameters" lineno="1320">
       <arguments repr="status_code: int, request_data: RequestData">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="status_code: int">
           <name>status_code</name>
           <type name="int" typedoc="integer">int</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="request_data: RequestData">
           <name>request_data</name>
           <type name="RequestData">RequestData</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Returns a version of &lt;span class=&quot;name&quot;&gt;params, headers&lt;/span&gt; as present on &lt;span class=&quot;name&quot;&gt;request_data&lt;/span&gt; that has been modified to cause the provided &lt;span class=&quot;name&quot;&gt;status_code&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Returns a version of `params, headers` as present on `request_data` that has been modified to cause the provided `status_code`.</shortdoc>
     </kw>
-    <kw name="Get Invalidated Url" lineno="1182">
+    <kw name="Get Invalidated Url" lineno="1238">
       <arguments repr="valid_url: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="valid_url: str">
           <name>valid_url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return an url with all the path parameters in the &lt;span class=&quot;name&quot;&gt;valid_url&lt;/span&gt; replaced by a random UUID.&lt;/p&gt;
 &lt;p&gt;Raises ValueError if the valid_url cannot be invalidated.&lt;/p&gt;</doc>
       <shortdoc>Return an url with all the path parameters in the `valid_url` replaced by a random UUID.</shortdoc>
     </kw>
-    <kw name="Get Json Data For Dto Class" lineno="1058">
+    <kw name="Get Json Data For Dto Class" lineno="1114">
       <arguments repr="schema: Dict[str, Any], dto_class: Dto | Type[Dto], operation_id: str = ">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="schema: Dict[str, Any]">
           <name>schema</name>
           <type name="Dict" typedoc="dictionary">
             Dict[str, Any]
             <type name="str" typedoc="string">str</type>
             <type name="Any" typedoc="Any">Any</type>
@@ -390,15 +390,15 @@
           <type name="str" typedoc="string">str</type>
           <default/>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Generate a valid (json-compatible) dict for all the &lt;span class=&quot;name&quot;&gt;dto_class&lt;/span&gt; properties.&lt;/p&gt;</doc>
       <shortdoc>Generate a valid (json-compatible) dict for all the `dto_class` properties.</shortdoc>
     </kw>
-    <kw name="Get Json Data With Conflict" lineno="1483">
+    <kw name="Get Json Data With Conflict" lineno="1539">
       <arguments repr="url: str, method: str, dto: Dto, conflict_status_code: int">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -412,54 +412,54 @@
           <name>conflict_status_code</name>
           <type name="int" typedoc="integer">int</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return &lt;span class=&quot;name&quot;&gt;json_data&lt;/span&gt; based on the &lt;span class=&quot;name&quot;&gt;UniquePropertyValueConstraint&lt;/span&gt; that must be returned by the &lt;span class=&quot;name&quot;&gt;get_relations&lt;/span&gt; implementation on the &lt;span class=&quot;name&quot;&gt;dto&lt;/span&gt; for the given &lt;span class=&quot;name&quot;&gt;conflict_status_code&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Return `json_data` based on the `UniquePropertyValueConstraint` that must be returned by the `get_relations` implementation on the `dto` for the given `conflict_status_code`.</shortdoc>
     </kw>
-    <kw name="Get Parameterized Endpoint From Url" lineno="1204">
+    <kw name="Get Parameterized Endpoint From Url" lineno="1260">
       <arguments repr="url: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return the endpoint as found in the &lt;span class=&quot;name&quot;&gt;paths&lt;/span&gt; section based on the given &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Return the endpoint as found in the `paths` section based on the given `url`.</shortdoc>
     </kw>
-    <kw name="Get Request Data" lineno="850">
+    <kw name="Get Request Data" lineno="906">
       <arguments repr="endpoint: str, method: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="endpoint: str">
           <name>endpoint</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
           <type name="str" typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return an object with valid request data for body, headers and query params.&lt;/p&gt;</doc>
       <shortdoc>Return an object with valid request data for body, headers and query params.</shortdoc>
     </kw>
-    <kw name="Get Valid Id For Endpoint" lineno="714">
+    <kw name="Get Valid Id For Endpoint" lineno="770">
       <arguments repr="endpoint: str, method: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="endpoint: str">
           <name>endpoint</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
           <type name="str" typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Support keyword that returns the &lt;span class=&quot;name&quot;&gt;id&lt;/span&gt; for an existing resource at &lt;span class=&quot;name&quot;&gt;endpoint&lt;/span&gt;.&lt;/p&gt;
 &lt;p&gt;To prevent resource conflicts with other test cases, a new resource is created (POST) if possible.&lt;/p&gt;</doc>
       <shortdoc>Support keyword that returns the `id` for an existing resource at `endpoint`.</shortdoc>
     </kw>
-    <kw name="Get Valid Url" lineno="674">
+    <kw name="Get Valid Url" lineno="730">
       <arguments repr="endpoint: str, method: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="endpoint: str">
           <name>endpoint</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -467,15 +467,15 @@
         </arg>
       </arguments>
       <doc>&lt;p&gt;This keyword returns a valid url for the given &lt;span class=&quot;name&quot;&gt;endpoint&lt;/span&gt; and &lt;span class=&quot;name&quot;&gt;method&lt;/span&gt;.&lt;/p&gt;
 &lt;p&gt;If the &lt;span class=&quot;name&quot;&gt;endpoint&lt;/span&gt; contains path parameters the Get Valid Id For Endpoint keyword will be executed to retrieve valid ids for the path parameters.&lt;/p&gt;
 &lt;p&gt;&amp;gt; Note: if valid ids cannot be retrieved within the scope of the API, the &lt;span class=&quot;name&quot;&gt;PathPropertiesConstraint&lt;/span&gt; Relation can be used. More information can be found &lt;a href=&quot;https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html&quot;&gt;here&lt;/a&gt;.&lt;/p&gt;</doc>
       <shortdoc>This keyword returns a valid url for the given `endpoint` and `method`.</shortdoc>
     </kw>
-    <kw name="Set Origin" lineno="581">
+    <kw name="Set Origin" lineno="592">
       <arguments repr="origin: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="origin: str">
           <name>origin</name>
           <type name="str" typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Update the &lt;span class=&quot;name&quot;&gt;origin&lt;/span&gt; after the library is imported.&lt;/p&gt;
```

### Comparing `robotframework_openapitools-0.2.0/src/OpenApiLibCore/openapi_libcore.py` & `robotframework_openapitools-0.2.1/src/OpenApiLibCore/openapi_libcore.py`

 * *Files 7% similar despite different names*

```diff
@@ -124,15 +124,26 @@
 from copy import deepcopy
 from dataclasses import Field, dataclass, field, make_dataclass
 from functools import cached_property
 from itertools import zip_longest
 from logging import getLogger
 from pathlib import Path
 from random import choice, sample
-from typing import Any, Dict, List, Optional, Set, Tuple, Type, Union
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Generator,
+    List,
+    Optional,
+    Set,
+    Tuple,
+    Type,
+    Union,
+)
 from uuid import uuid4
 
 from openapi_core import Config, OpenAPI, Spec
 from openapi_core.contrib.requests import (
     RequestsOpenAPIRequest,
     RequestsOpenAPIResponse,
 )
@@ -593,60 +604,110 @@
 
     @property
     def base_url(self) -> str:
         return f"{self.origin}{self._base_path}"
 
     @cached_property
     def validation_spec(self) -> Spec:
-        return Spec.from_dict(self.openapi_spec)
+        _, validation_spec, _ = self._load_specs_and_validator()
+        return validation_spec
 
     @property
     def openapi_spec(self) -> Dict[str, Any]:
         """Return a deepcopy of the parsed openapi document."""
         # protect the parsed openapi spec from being mutated by reference
         return deepcopy(self._openapi_spec)
 
     @cached_property
     def _openapi_spec(self) -> Dict[str, Any]:
-        parser = self._load_parser()
+        parser, _, _ = self._load_specs_and_validator()
         return parser.specification
 
-    def read_paths(self) -> Dict[str, Any]:
-        return self.openapi_spec["paths"]
+    @cached_property
+    def response_validator(
+        self,
+    ) -> Callable[[RequestsOpenAPIRequest, RequestsOpenAPIResponse], None]:
+        _, _, response_validator = self._load_specs_and_validator()
+        return response_validator
+
+    def _get_json_types_from_spec(self, spec: Dict[str, Any]) -> Set[str]:
+        json_types: Set[str] = set(self._get_json_types(spec))
+        return {json_type for json_type in json_types if json_type is not None}
+
+    def _get_json_types(self, item: Any) -> Generator[str, None, None]:
+        if isinstance(item, dict):
+            content_dict = item.get("content")
+            if content_dict is None:
+                for value in item.values():
+                    yield from self._get_json_types(value)
 
-    def _load_parser(self) -> ResolvingParser:
+            else:
+                for content_type in content_dict:
+                    if "json" in content_type:
+                        yield content_type
+
+        if isinstance(item, list):
+            for list_item in item:
+                yield from self._get_json_types(list_item)
+
+    def _load_specs_and_validator(
+        self,
+    ) -> Tuple[
+        ResolvingParser,
+        Spec,
+        Callable[[RequestsOpenAPIRequest, RequestsOpenAPIResponse], None],
+    ]:
         try:
 
             def recursion_limit_handler(
                 limit: int, refstring: str, recursions: Any
             ) -> Any:
                 return self._recursion_default
 
             # Since parsing of the OAS and creating the Spec can take a long time,
             # they are cached. This is done by storing them in an imported module that
             # will have a global scope due to how the Python import system works. This
             # ensures that in a Suite of Suites where multiple Suites use the same
             # `source`, that OAS is only parsed / loaded once.
-            parser = PARSER_CACHE.get(self._source, None)
+            parser, validation_spec, response_validator = PARSER_CACHE.get(
+                self._source, (None, None, None)
+            )
+
             if parser is None:
                 parser = ResolvingParser(
                     self._source,
                     backend="openapi-spec-validator",
                     recursion_limit=self._recursion_limit,
                     recursion_limit_handler=recursion_limit_handler,
                 )
 
                 if parser.specification is None:  # pragma: no cover
                     BuiltIn().fatal_error(
                         "Source was loaded, but no specification was present after parsing."
                     )
 
-                PARSER_CACHE[self._source] = parser
+                validation_spec = Spec.from_dict(parser.specification)
+
+                json_types_from_spec: Set[str] = self._get_json_types_from_spec(
+                    parser.specification
+                )
+                extra_deserializers = {
+                    json_type: _json.loads for json_type in json_types_from_spec
+                }
+                config = Config(extra_media_type_deserializers=extra_deserializers)
+                openapi = OpenAPI(spec=validation_spec, config=config)
+                response_validator = openapi.validate_response
+
+                PARSER_CACHE[self._source] = (
+                    parser,
+                    validation_spec,
+                    response_validator,
+                )
 
-            return parser
+            return parser, validation_spec, response_validator
 
         except ResolutionError as exception:
             BuiltIn().fatal_error(
                 f"ResolutionError while trying to load openapi spec: {exception}"
             )
         except ValidationError as exception:
             BuiltIn().fatal_error(
@@ -656,23 +717,18 @@
     def validate_response_vs_spec(
         self, request: RequestsOpenAPIRequest, response: RequestsOpenAPIResponse
     ) -> None:
         """
         Validate the reponse for a given request against the OpenAPI Spec that is
         loaded during library initialization.
         """
-        if response.content_type == "application/json":
-            config = None
-        else:
-            extra_deserializer = {response.content_type: _json.loads}
-            config = Config(extra_media_type_deserializers=extra_deserializer)
+        self.response_validator(request=request, response=response)
 
-        OpenAPI(spec=self.validation_spec, config=config).validate_response(
-            request, response
-        )
+    def read_paths(self) -> Dict[str, Any]:
+        return self.openapi_spec["paths"]
 
     @keyword
     def get_valid_url(self, endpoint: str, method: str) -> str:
         """
         This keyword returns a valid url for the given `endpoint` and `method`.
 
         If the `endpoint` contains path parameters the Get Valid Id For Endpoint
```

### Comparing `robotframework_openapitools-0.2.0/src/OpenApiLibCore/value_utils.py` & `robotframework_openapitools-0.2.1/src/OpenApiLibCore/value_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.0/src/roboswag/auth.py` & `robotframework_openapitools-0.2.1/src/roboswag/auth.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.0/src/roboswag/cli.py` & `robotframework_openapitools-0.2.1/src/roboswag/cli.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.0/src/roboswag/core.py` & `robotframework_openapitools-0.2.1/src/roboswag/core.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.0/src/roboswag/generate/generate.py` & `robotframework_openapitools-0.2.1/src/roboswag/generate/generate.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.0/src/roboswag/generate/models/api.py` & `robotframework_openapitools-0.2.1/src/roboswag/generate/models/api.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.0/src/roboswag/generate/models/definition.py` & `robotframework_openapitools-0.2.1/src/roboswag/generate/models/definition.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.0/src/roboswag/generate/models/endpoint.py` & `robotframework_openapitools-0.2.1/src/roboswag/generate/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.0/src/roboswag/generate/models/parameter.py` & `robotframework_openapitools-0.2.1/src/roboswag/generate/models/parameter.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.0/src/roboswag/generate/models/tag.py` & `robotframework_openapitools-0.2.1/src/roboswag/generate/models/tag.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.0/src/roboswag/generate/models/utils.py` & `robotframework_openapitools-0.2.1/src/roboswag/generate/models/utils.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.0/src/roboswag/generate/templates/api_init.jinja` & `robotframework_openapitools-0.2.1/src/roboswag/generate/templates/api_init.jinja`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.0/src/roboswag/generate/templates/paths.jinja` & `robotframework_openapitools-0.2.1/src/roboswag/generate/templates/paths.jinja`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.0/src/roboswag/logger.py` & `robotframework_openapitools-0.2.1/src/roboswag/logger.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.0/src/roboswag/validate/schema.py` & `robotframework_openapitools-0.2.1/src/roboswag/validate/schema.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.0/src/roboswag/validate/text_response.py` & `robotframework_openapitools-0.2.1/src/roboswag/validate/text_response.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.0/PKG-INFO` & `robotframework_openapitools-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-openapitools
-Version: 0.2.0
+Version: 0.2.1
 Summary: A set of Robot Framework libraries to test APIs for which the OAS is available.
 Home-page: https://github.com/MarketSquare/robotframework-openapitools
 License: Apache-2.0
 Author: Bartlomiej Hirsz
 Author-email: bartek.hirsz@gmail.com
 Maintainer: Robin Mackaij
 Maintainer-email: r.a.mackaij@gmail.com
```

