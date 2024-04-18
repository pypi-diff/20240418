# Comparing `tmp/rizaio-0.1.0a2.tar.gz` & `tmp/rizaio-0.1.0a3.tar.gz`

## Comparing `rizaio-0.1.0a2.tar` & `rizaio-0.1.0a3.tar`

### file list

```diff
@@ -1,33 +1,62 @@
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/__init__.py
--rw-r--r--   0        0        0    64250 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/_base_client.py
--rw-r--r--   0        0        0    14864 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/_constants.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/_files.py
--rw-r--r--   0        0        0    26079 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/_qs.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/_resource.py
--rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/_response.py
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/_streaming.py
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/_types.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/_utils/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/_utils/_typing.py
--rw-r--r--   0        0        0    11451 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/lib/.keep
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/resources/__init__.py
--rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/resources/v1.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/types/__init__.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/types/v1_execute_params.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/src/riza/types/v1_execute_response.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/.gitignore
--rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/LICENSE
--rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0    11643 2020-02-02 00:00:00.000000 rizaio-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/__init__.py
+-rw-r--r--   0        0        0    64250 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_base_client.py
+-rw-r--r--   0        0        0    14864 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_constants.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_files.py
+-rw-r--r--   0        0        0    26079 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_qs.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_resource.py
+-rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_response.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_streaming.py
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_types.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_utils/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_utils/_typing.py
+-rw-r--r--   0        0        0    11451 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/lib/.keep
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/resources/__init__.py
+-rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/resources/v1.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/types/__init__.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/types/v1_execute_params.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/riza/types/v1_execute_response.py
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/__init__.py
+-rw-r--r--   0        0        0    64250 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_base_client.py
+-rw-r--r--   0        0        0    14784 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_constants.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_files.py
+-rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_qs.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_resource.py
+-rw-r--r--   0        0        0    28371 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_response.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_streaming.py
+-rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_types.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_utils/__init__.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/lib/.keep
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/resources/__init__.py
+-rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/resources/code.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/types/__init__.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/types/code_execute_params.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/src/rizaio/types/code_execute_response.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/.gitignore
+-rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/LICENSE
+-rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0    11680 2020-02-02 00:00:00.000000 rizaio-0.1.0a3/PKG-INFO
```

### Comparing `rizaio-0.1.0a2/src/riza/__init__.py` & `rizaio-0.1.0a3/src/riza/__init__.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a2/src/riza/_base_client.py` & `rizaio-0.1.0a3/src/riza/_base_client.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a2/src/riza/_client.py` & `rizaio-0.1.0a3/src/riza/_client.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a2/src/riza/_compat.py` & `rizaio-0.1.0a3/src/riza/_compat.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a2/src/riza/_exceptions.py` & `rizaio-0.1.0a3/src/riza/_exceptions.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a2/src/riza/_files.py` & `rizaio-0.1.0a3/src/riza/_files.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a2/src/riza/_models.py` & `rizaio-0.1.0a3/src/riza/_models.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a2/src/riza/_qs.py` & `rizaio-0.1.0a3/src/riza/_qs.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a2/src/riza/_resource.py` & `rizaio-0.1.0a3/src/riza/_resource.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a2/src/riza/_response.py` & `rizaio-0.1.0a3/src/riza/_response.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a2/src/riza/_streaming.py` & `rizaio-0.1.0a3/src/riza/_streaming.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a2/src/riza/_types.py` & `rizaio-0.1.0a3/src/riza/_types.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a2/src/riza/_utils/__init__.py` & `rizaio-0.1.0a3/src/riza/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a2/src/riza/_utils/_logs.py` & `rizaio-0.1.0a3/src/riza/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a2/src/riza/_utils/_proxy.py` & `rizaio-0.1.0a3/src/riza/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a2/src/riza/_utils/_sync.py` & `rizaio-0.1.0a3/src/riza/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a2/src/riza/_utils/_transform.py` & `rizaio-0.1.0a3/src/riza/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a2/src/riza/_utils/_typing.py` & `rizaio-0.1.0a3/src/riza/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a2/src/riza/_utils/_utils.py` & `rizaio-0.1.0a3/src/riza/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a2/src/riza/resources/v1.py` & `rizaio-0.1.0a3/src/riza/resources/v1.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a2/LICENSE` & `rizaio-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a2/pyproject.toml` & `rizaio-0.1.0a3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rizaio"
-version = "0.1.0-alpha.2"
+version = "0.1.0-alpha.3"
 description = "The official Python library for the riza API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Riza", email = "hello@riza.io" },
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
@@ -80,28 +80,28 @@
 "fix:ruff" = "ruff --fix ."
 
 typecheck = { chain = [
   "typecheck:pyright",
   "typecheck:mypy"
 ]}
 "typecheck:pyright" = "pyright"
-"typecheck:verify-types" = "pyright --verifytypes riza --ignoreexternal"
+"typecheck:verify-types" = "pyright --verifytypes rizaio --ignoreexternal"
 "typecheck:mypy" = "mypy ."
 
 [build-system]
 requires = ["hatchling", "hatch-fancy-pypi-readme"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 include = [
   "src/*"
 ]
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/riza"]
+packages = ["src/rizaio"]
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 path = "README.md"
 
@@ -183,13 +183,13 @@
 "functools.lru_cache".msg = "This function does not retain type information for the wrapped function's arguments; The `lru_cache` function from `_utils` should be used instead"
 
 [tool.ruff.lint.isort]
 length-sort = true
 length-sort-straight = true
 combine-as-imports = true
 extra-standard-library = ["typing_extensions"]
-known-first-party = ["riza", "tests"]
+known-first-party = ["rizaio", "tests"]
 
 [tool.ruff.per-file-ignores]
 "bin/**.py" = ["T201", "T203"]
 "tests/**.py" = ["T201", "T203"]
 "examples/**.py" = ["T201", "T203"]
```

### Comparing `rizaio-0.1.0a2/PKG-INFO` & `rizaio-0.1.0a3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rizaio
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: The official Python library for the riza API
 Project-URL: Homepage, https://github.com/riza-io/riza-api-python
 Project-URL: Repository, https://github.com/riza-io/riza-api-python
 Author-email: Riza <hello@riza.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -55,48 +55,48 @@
 
 ## Usage
 
 The full API of this library can be found in [api.md](https://github.com/riza-io/riza-api-python/tree/main/api.md).
 
 ```python
 import os
-from riza import Riza
+from rizaio import Riza
 
 client = Riza(
     # This is the default and can be omitted
-    auth_token=os.environ.get("RIZA_AUTH_TOKEN"),
+    api_key=os.environ.get("RIZA_API_KEY"),
 )
 
-v1_execute_response = client.v1.execute()
-print(v1_execute_response.exit_code)
+code_execute_response = client.code.execute()
+print(code_execute_response.exit_code)
 ```
 
-While you can provide a `auth_token` keyword argument,
+While you can provide an `api_key` keyword argument,
 we recommend using [python-dotenv](https://pypi.org/project/python-dotenv/)
-to add `RIZA_AUTH_TOKEN="My Auth Token"` to your `.env` file
-so that your Auth Token is not stored in source control.
+to add `RIZA_API_KEY="My API Key"` to your `.env` file
+so that your API Key is not stored in source control.
 
 ## Async usage
 
 Simply import `AsyncRiza` instead of `Riza` and use `await` with each API call:
 
 ```python
 import os
 import asyncio
-from riza import AsyncRiza
+from rizaio import AsyncRiza
 
 client = AsyncRiza(
     # This is the default and can be omitted
-    auth_token=os.environ.get("RIZA_AUTH_TOKEN"),
+    api_key=os.environ.get("RIZA_API_KEY"),
 )
 
 
 async def main() -> None:
-    v1_execute_response = await client.v1.execute()
-    print(v1_execute_response.exit_code)
+    code_execute_response = await client.code.execute()
+    print(code_execute_response.exit_code)
 
 
 asyncio.run(main())
 ```
 
 Functionality between the synchronous and asynchronous clients is otherwise identical.
 
@@ -107,35 +107,35 @@
 - Serializing back into JSON, `model.to_json()`
 - Converting to a dictionary, `model.to_dict()`
 
 Typed requests and responses provide autocomplete and documentation within your editor. If you would like to see type errors in VS Code to help catch bugs earlier, set `python.analysis.typeCheckingMode` to `basic`.
 
 ## Handling errors
 
-When the library is unable to connect to the API (for example, due to network connection problems or a timeout), a subclass of `riza.APIConnectionError` is raised.
+When the library is unable to connect to the API (for example, due to network connection problems or a timeout), a subclass of `rizaio.APIConnectionError` is raised.
 
 When the API returns a non-success status code (that is, 4xx or 5xx
-response), a subclass of `riza.APIStatusError` is raised, containing `status_code` and `response` properties.
+response), a subclass of `rizaio.APIStatusError` is raised, containing `status_code` and `response` properties.
 
-All errors inherit from `riza.APIError`.
+All errors inherit from `rizaio.APIError`.
 
 ```python
-import riza
-from riza import Riza
+import rizaio
+from rizaio import Riza
 
 client = Riza()
 
 try:
-    client.v1.execute()
-except riza.APIConnectionError as e:
+    client.code.execute()
+except rizaio.APIConnectionError as e:
     print("The server could not be reached")
     print(e.__cause__)  # an underlying Exception, likely raised within httpx.
-except riza.RateLimitError as e:
+except rizaio.RateLimitError as e:
     print("A 429 status code was received; we should back off a bit.")
-except riza.APIStatusError as e:
+except rizaio.APIStatusError as e:
     print("Another non-200-range status code was received")
     print(e.status_code)
     print(e.response)
 ```
 
 Error codes are as followed:
 
@@ -155,47 +155,47 @@
 Certain errors are automatically retried 2 times by default, with a short exponential backoff.
 Connection errors (for example, due to a network connectivity problem), 408 Request Timeout, 409 Conflict,
 429 Rate Limit, and >=500 Internal errors are all retried by default.
 
 You can use the `max_retries` option to configure or disable retry settings:
 
 ```python
-from riza import Riza
+from rizaio import Riza
 
 # Configure the default for all requests:
 client = Riza(
     # default is 2
     max_retries=0,
 )
 
 # Or, configure per-request:
-client.with_options(max_retries=5).v1.execute()
+client.with_options(max_retries=5).code.execute()
 ```
 
 ### Timeouts
 
 By default requests time out after 1 minute. You can configure this with a `timeout` option,
 which accepts a float or an [`httpx.Timeout`](https://www.python-httpx.org/advanced/#fine-tuning-the-configuration) object:
 
 ```python
-from riza import Riza
+from rizaio import Riza
 
 # Configure the default for all requests:
 client = Riza(
     # 20 seconds (default is 1 minute)
     timeout=20.0,
 )
 
 # More granular control:
 client = Riza(
     timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),
 )
 
 # Override per-request:
-client.with_options(timeout=5 * 1000).v1.execute()
+client.with_options(timeout=5 * 1000).code.execute()
 ```
 
 On timeout, an `APITimeoutError` is thrown.
 
 Note that requests that time out are [retried twice by default](https://github.com/riza-io/riza-api-python/tree/main/#retries).
 
 ## Advanced
@@ -223,36 +223,36 @@
 ```
 
 ### Accessing raw response data (e.g. headers)
 
 The "raw" Response object can be accessed by prefixing `.with_raw_response.` to any HTTP method call, e.g.,
 
 ```py
-from riza import Riza
+from rizaio import Riza
 
 client = Riza()
-response = client.v1.with_raw_response.execute()
+response = client.code.with_raw_response.execute()
 print(response.headers.get('X-My-Header'))
 
-v1 = response.parse()  # get the object that `v1.execute()` would have returned
-print(v1.exit_code)
+code = response.parse()  # get the object that `code.execute()` would have returned
+print(code.exit_code)
 ```
 
-These methods return an [`APIResponse`](https://github.com/riza-io/riza-api-python/tree/main/src/riza/_response.py) object.
+These methods return an [`APIResponse`](https://github.com/riza-io/riza-api-python/tree/main/src/rizaio/_response.py) object.
 
-The async client returns an [`AsyncAPIResponse`](https://github.com/riza-io/riza-api-python/tree/main/src/riza/_response.py) with the same structure, the only difference being `await`able methods for reading the response content.
+The async client returns an [`AsyncAPIResponse`](https://github.com/riza-io/riza-api-python/tree/main/src/rizaio/_response.py) with the same structure, the only difference being `await`able methods for reading the response content.
 
 #### `.with_streaming_response`
 
 The above interface eagerly reads the full response body when you make the request, which may not always be what you want.
 
 To stream the response body, use `.with_streaming_response` instead, which requires a context manager and only reads the response body once you call `.read()`, `.text()`, `.json()`, `.iter_bytes()`, `.iter_text()`, `.iter_lines()` or `.parse()`. In the async client, these are async methods.
 
 ```python
-with client.v1.with_streaming_response.execute() as response:
+with client.code.with_streaming_response.execute() as response:
     print(response.headers.get("X-My-Header"))
 
     for line in response.iter_lines():
         print(line)
 ```
 
 The context manager is required so that the response will reliably be closed.
@@ -297,15 +297,15 @@
 You can directly override the [httpx client](https://www.python-httpx.org/api/#client) to customize it for your use case, including:
 
 - Support for proxies
 - Custom transports
 - Additional [advanced](https://www.python-httpx.org/advanced/#client-instances) functionality
 
 ```python
-from riza import Riza, DefaultHttpxClient
+from rizaio import Riza, DefaultHttpxClient
 
 client = Riza(
     # Or use the `RIZA_BASE_URL` env var
     base_url="http://my.test.server.example.com:8083",
     http_client=DefaultHttpxClient(
         proxies="http://my.test.proxy.example.com",
         transport=httpx.HTTPTransport(local_address="0.0.0.0"),
```

