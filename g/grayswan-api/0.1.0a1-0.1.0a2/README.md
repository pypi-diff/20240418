# Comparing `tmp/grayswan_api-0.1.0a1.tar.gz` & `tmp/grayswan_api-0.1.0a2.tar.gz`

## Comparing `grayswan_api-0.1.0a1.tar` & `grayswan_api-0.1.0a2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/__init__.py
--rw-r--r--   0        0        0    64256 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/_base_client.py
--rw-r--r--   0        0        0    15202 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/_compat.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/_constants.py
--rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/_files.py
--rw-r--r--   0        0        0    26079 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/_qs.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/_resource.py
--rw-r--r--   0        0        0    28473 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/_response.py
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/_streaming.py
--rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/_types.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/_utils/__init__.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/_utils/_typing.py
--rw-r--r--   0        0        0    11451 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/lib/.keep
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/resources/__init__.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/resources/chat/__init__.py
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/resources/chat/chat.py
--rw-r--r--   0        0        0     7600 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/resources/chat/completion.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/types/__init__.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/types/chat/__init__.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/types/chat/completion_create_params.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/gray_swan_security/types/chat/completion_create_response.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/src/grayswan/lib/.keep
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/.gitignore
--rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/LICENSE
--rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0    13113 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/__init__.py
+-rw-r--r--   0        0        0    64256 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/_base_client.py
+-rw-r--r--   0        0        0    14852 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/_compat.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/_constants.py
+-rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/_files.py
+-rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/_qs.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/_resource.py
+-rw-r--r--   0        0        0    28473 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/_response.py
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/_streaming.py
+-rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/_types.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/_utils/__init__.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/lib/.keep
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/resources/__init__.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/resources/chat/__init__.py
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/resources/chat/chat.py
+-rw-r--r--   0        0        0     7600 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/resources/chat/completion.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/types/__init__.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/types/chat/__init__.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/types/chat/completion_create_params.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/gray_swan_security/types/chat/completion_create_response.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/src/grayswan/lib/.keep
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/.gitignore
+-rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/LICENSE
+-rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0    12859 2020-02-02 00:00:00.000000 grayswan_api-0.1.0a2/PKG-INFO
```

### Comparing `grayswan_api-0.1.0a1/src/gray_swan_security/__init__.py` & `grayswan_api-0.1.0a2/src/gray_swan_security/__init__.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a1/src/gray_swan_security/_base_client.py` & `grayswan_api-0.1.0a2/src/gray_swan_security/_base_client.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a1/src/gray_swan_security/_client.py` & `grayswan_api-0.1.0a2/src/gray_swan_security/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,21 +74,21 @@
         # If you rely on this feature, please open a GitHub issue
         # outlining your use-case to help us decide if it should be
         # part of our public interface in the future.
         _strict_response_validation: bool = False,
     ) -> None:
         """Construct a new synchronous Gray Swan Security client instance.
 
-        This automatically infers the `api_key` argument from the `GRAYSWAN_BEARER_TOKEN` environment variable if it is not provided.
+        This automatically infers the `api_key` argument from the `GRAYSWAN_API_KEY` environment variable if it is not provided.
         """
         if api_key is None:
-            api_key = os.environ.get("GRAYSWAN_BEARER_TOKEN")
+            api_key = os.environ.get("GRAYSWAN_API_KEY")
         if api_key is None:
             raise GraySwanSecurityError(
-                "The api_key client option must be set either by passing api_key to the client or by setting the GRAYSWAN_BEARER_TOKEN environment variable"
+                "The api_key client option must be set either by passing api_key to the client or by setting the GRAYSWAN_API_KEY environment variable"
             )
         self.api_key = api_key
 
         if base_url is None:
             base_url = os.environ.get("GRAY_SWAN_SECURITY_BASE_URL")
         if base_url is None:
             base_url = f"https://api.grayswan.ai"
@@ -111,20 +111,14 @@
     @property
     @override
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
 
     @property
     @override
-    def auth_headers(self) -> dict[str, str]:
-        api_key = self.api_key
-        return {"Authorization": f"Bearer {api_key}"}
-
-    @property
-    @override
     def default_headers(self) -> dict[str, str | Omit]:
         return {
             **super().default_headers,
             "X-Stainless-Async": "false",
             **self._custom_headers,
         }
 
@@ -242,21 +236,21 @@
         # If you rely on this feature, please open a GitHub issue
         # outlining your use-case to help us decide if it should be
         # part of our public interface in the future.
         _strict_response_validation: bool = False,
     ) -> None:
         """Construct a new async Gray Swan Security client instance.
 
-        This automatically infers the `api_key` argument from the `GRAYSWAN_BEARER_TOKEN` environment variable if it is not provided.
+        This automatically infers the `api_key` argument from the `GRAYSWAN_API_KEY` environment variable if it is not provided.
         """
         if api_key is None:
-            api_key = os.environ.get("GRAYSWAN_BEARER_TOKEN")
+            api_key = os.environ.get("GRAYSWAN_API_KEY")
         if api_key is None:
             raise GraySwanSecurityError(
-                "The api_key client option must be set either by passing api_key to the client or by setting the GRAYSWAN_BEARER_TOKEN environment variable"
+                "The api_key client option must be set either by passing api_key to the client or by setting the GRAYSWAN_API_KEY environment variable"
             )
         self.api_key = api_key
 
         if base_url is None:
             base_url = os.environ.get("GRAY_SWAN_SECURITY_BASE_URL")
         if base_url is None:
             base_url = f"https://api.grayswan.ai"
@@ -279,20 +273,14 @@
     @property
     @override
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
 
     @property
     @override
-    def auth_headers(self) -> dict[str, str]:
-        api_key = self.api_key
-        return {"Authorization": f"Bearer {api_key}"}
-
-    @property
-    @override
     def default_headers(self) -> dict[str, str | Omit]:
         return {
             **super().default_headers,
             "X-Stainless-Async": f"async:{get_async_library()}",
             **self._custom_headers,
         }
```

### Comparing `grayswan_api-0.1.0a1/src/gray_swan_security/_compat.py` & `grayswan_api-0.1.0a2/src/gray_swan_security/_compat.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a1/src/gray_swan_security/_exceptions.py` & `grayswan_api-0.1.0a2/src/gray_swan_security/_exceptions.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a1/src/gray_swan_security/_files.py` & `grayswan_api-0.1.0a2/src/gray_swan_security/_files.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a1/src/gray_swan_security/_models.py` & `grayswan_api-0.1.0a2/src/gray_swan_security/_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,15 +374,15 @@
     """
     # we allow `object` as the input type because otherwise, passing things like
     # `Literal['value']` will be reported as a type error by type checkers
     type_ = cast("type[object]", type_)
 
     # unwrap `Annotated[T, ...]` -> `T`
     if is_annotated_type(type_):
-        meta = get_args(type_)[1:]
+        meta: tuple[Any, ...] = get_args(type_)[1:]
         type_ = extract_type_arg(type_, 0)
     else:
         meta = tuple()
 
     # we need to use the origin class for any types that are subscripted generics
     # e.g. Dict[str, object]
     origin = get_origin(type_) or type_
```

### Comparing `grayswan_api-0.1.0a1/src/gray_swan_security/_qs.py` & `grayswan_api-0.1.0a2/src/gray_swan_security/_qs.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a1/src/gray_swan_security/_resource.py` & `grayswan_api-0.1.0a2/src/gray_swan_security/_resource.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a1/src/gray_swan_security/_response.py` & `grayswan_api-0.1.0a2/src/gray_swan_security/_response.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a1/src/gray_swan_security/_streaming.py` & `grayswan_api-0.1.0a2/src/gray_swan_security/_streaming.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a1/src/gray_swan_security/_types.py` & `grayswan_api-0.1.0a2/src/gray_swan_security/_types.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a1/src/gray_swan_security/_utils/__init__.py` & `grayswan_api-0.1.0a2/src/gray_swan_security/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a1/src/gray_swan_security/_utils/_logs.py` & `grayswan_api-0.1.0a2/src/gray_swan_security/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a1/src/gray_swan_security/_utils/_proxy.py` & `grayswan_api-0.1.0a2/src/gray_swan_security/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a1/src/gray_swan_security/_utils/_sync.py` & `grayswan_api-0.1.0a2/src/gray_swan_security/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a1/src/gray_swan_security/_utils/_transform.py` & `grayswan_api-0.1.0a2/src/gray_swan_security/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a1/src/gray_swan_security/_utils/_typing.py` & `grayswan_api-0.1.0a2/src/gray_swan_security/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a1/src/gray_swan_security/_utils/_utils.py` & `grayswan_api-0.1.0a2/src/gray_swan_security/_utils/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,14 +261,16 @@
             else:  # no break
                 if len(variants) > 1:
                     variations = human_join(
                         ["(" + human_join([quote(arg) for arg in variant], final="and") + ")" for variant in variants]
                     )
                     msg = f"Missing required arguments; Expected either {variations} arguments to be given"
                 else:
+                    assert len(variants) > 0
+
                     # TODO: this error message is not deterministic
                     missing = list(set(variants[0]) - given_params)
                     if len(missing) > 1:
                         msg = f"Missing required arguments: {human_join([quote(arg) for arg in missing])}"
                     else:
                         msg = f"Missing required argument: {quote(missing[0])}"
                 raise TypeError(msg)
```

### Comparing `grayswan_api-0.1.0a1/src/gray_swan_security/resources/chat/__init__.py` & `grayswan_api-0.1.0a2/src/gray_swan_security/resources/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a1/src/gray_swan_security/resources/chat/chat.py` & `grayswan_api-0.1.0a2/src/gray_swan_security/resources/chat/chat.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a1/src/gray_swan_security/resources/chat/completion.py` & `grayswan_api-0.1.0a2/src/gray_swan_security/resources/chat/completion.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a1/src/gray_swan_security/types/chat/completion_create_params.py` & `grayswan_api-0.1.0a2/src/gray_swan_security/types/chat/completion_create_params.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a1/src/gray_swan_security/types/chat/completion_create_response.py` & `grayswan_api-0.1.0a2/src/gray_swan_security/types/chat/completion_create_response.py`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a1/LICENSE` & `grayswan_api-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `grayswan_api-0.1.0a1/pyproject.toml` & `grayswan_api-0.1.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "grayswan-api"
-version = "0.1.0-alpha.1"
+version = "0.1.0-alpha.2"
 description = "The official Python library for the Gray Swan Security API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Gray Swan Security", email = "dev-feedback@grayswan.ai" },
 ]
 dependencies = [
@@ -44,15 +44,15 @@
 
 
 
 [tool.rye]
 managed = true
 # version pins are in requirements-dev.lock
 dev-dependencies = [
-    "pyright",
+    "pyright>=1.1.359",
     "mypy",
     "respx",
     "pytest",
     "pytest-asyncio",
     "ruff",
     "time-machine",
     "nox",
```

### Comparing `grayswan_api-0.1.0a1/PKG-INFO` & `grayswan_api-0.1.0a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: grayswan-api
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: The official Python library for the Gray Swan Security API
 Project-URL: Homepage, https://github.com/grayswansecurity/grayswan-python
 Project-URL: Repository, https://github.com/grayswansecurity/grayswan-python
 Author-email: Gray Swan Security <dev-feedback@grayswan.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -54,45 +54,36 @@
 ```
 
 ## Usage
 
 The full API of this library can be found in [api.md](https://github.com/grayswansecurity/grayswan-python/tree/main/api.md).
 
 ```python
-import os
 from gray_swan_security import GraySwanSecurity
 
 client = GraySwanSecurity(
-    # This is the default and can be omitted
-    api_key=os.environ.get("GRAYSWAN_BEARER_TOKEN"),
+    api_key="My API Key",
 )
 
 completion_create_response = client.chat.completion.create(
     messages=[{"role": "system"}, {"role": "system"}, {"role": "system"}],
     model="cygnet-v0.2",
 )
 ```
 
-While you can provide an `api_key` keyword argument,
-we recommend using [python-dotenv](https://pypi.org/project/python-dotenv/)
-to add `GRAYSWAN_BEARER_TOKEN="My API Key"` to your `.env` file
-so that your API Key is not stored in source control.
-
 ## Async usage
 
 Simply import `AsyncGraySwanSecurity` instead of `GraySwanSecurity` and use `await` with each API call:
 
 ```python
-import os
 import asyncio
 from gray_swan_security import AsyncGraySwanSecurity
 
 client = AsyncGraySwanSecurity(
-    # This is the default and can be omitted
-    api_key=os.environ.get("GRAYSWAN_BEARER_TOKEN"),
+    api_key="My API Key",
 )
 
 
 async def main() -> None:
     completion_create_response = await client.chat.completion.create(
         messages=[{"role": "system"}, {"role": "system"}, {"role": "system"}],
         model="cygnet-v0.2",
@@ -122,15 +113,17 @@
 
 All errors inherit from `gray_swan_security.APIError`.
 
 ```python
 import gray_swan_security
 from gray_swan_security import GraySwanSecurity
 
-client = GraySwanSecurity()
+client = GraySwanSecurity(
+    api_key="My API Key",
+)
 
 try:
     client.chat.completion.create(
         messages=[{"role": "system"}, {"role": "system"}, {"role": "system"}],
         model="cygnet-v0.2",
     )
 except gray_swan_security.APIConnectionError as e:
@@ -168,14 +161,15 @@
 ```python
 from gray_swan_security import GraySwanSecurity
 
 # Configure the default for all requests:
 client = GraySwanSecurity(
     # default is 2
     max_retries=0,
+    api_key="My API Key",
 )
 
 # Or, configure per-request:
 client.with_options(max_retries=5).chat.completion.create(
     messages=[{"role": "system"}, {"role": "system"}, {"role": "system"}],
     model="cygnet-v0.2",
 )
@@ -189,19 +183,21 @@
 ```python
 from gray_swan_security import GraySwanSecurity
 
 # Configure the default for all requests:
 client = GraySwanSecurity(
     # 20 seconds (default is 1 minute)
     timeout=20.0,
+    api_key="My API Key",
 )
 
 # More granular control:
 client = GraySwanSecurity(
     timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),
+    api_key="My API Key",
 )
 
 # Override per-request:
 client.with_options(timeout=5 * 1000).chat.completion.create(
     messages=[{"role": "system"}, {"role": "system"}, {"role": "system"}],
     model="cygnet-v0.2",
 )
@@ -238,15 +234,17 @@
 ### Accessing raw response data (e.g. headers)
 
 The "raw" Response object can be accessed by prefixing `.with_raw_response.` to any HTTP method call, e.g.,
 
 ```py
 from gray_swan_security import GraySwanSecurity
 
-client = GraySwanSecurity()
+client = GraySwanSecurity(
+    api_key="My API Key",
+)
 response = client.chat.completion.with_raw_response.create(
     messages=[{
         "role": "system"
     }, {
         "role": "system"
     }, {
         "role": "system"
@@ -331,14 +329,15 @@
 client = GraySwanSecurity(
     # Or use the `GRAY_SWAN_SECURITY_BASE_URL` env var
     base_url="http://my.test.server.example.com:8083",
     http_client=DefaultHttpxClient(
         proxies="http://my.test.proxy.example.com",
         transport=httpx.HTTPTransport(local_address="0.0.0.0"),
     ),
+    api_key="My API Key",
 )
 ```
 
 ### Managing HTTP resources
 
 By default the library closes underlying HTTP connections whenever the client is [garbage collected](https://docs.python.org/3/reference/datamodel.html#object.__del__). You can manually close the client using the `.close()` method if desired, or with a context manager that closes when exiting.
```

