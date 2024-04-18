# Comparing `tmp/composio_core-0.2.7.tar.gz` & `tmp/composio_core-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.2.7.tar", last modified: Wed Apr 17 08:08:52 2024, max compression
+gzip compressed data, was "composio_core-0.2.8.tar", last modified: Thu Apr 18 18:07:27 2024, max compression
```

## Comparing `composio_core-0.2.7.tar` & `composio_core-0.2.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-17 08:08:52.074916 composio_core-0.2.7/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       48 2024-04-15 07:39:40.000000 composio_core-0.2.7/MANIFEST.in
--rw-r--r--   0 karanvaidya   (501) staff       (20)      796 2024-04-17 08:08:52.074680 composio_core-0.2.7/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      102 2024-04-15 07:39:40.000000 composio_core-0.2.7/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-17 08:08:52.072322 composio_core-0.2.7/composio/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      159 2024-04-15 07:39:40.000000 composio_core-0.2.7/composio/__init__.py
--rwxr-xr-x   0 karanvaidya   (501) staff       (20)    22056 2024-04-16 18:39:33.000000 composio_core-0.2.7/composio/composio_cli.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-17 08:08:52.073531 composio_core-0.2.7/composio/sdk/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       85 2024-04-15 07:39:40.000000 composio_core-0.2.7/composio/sdk/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     7018 2024-04-16 18:37:25.000000 composio_core-0.2.7/composio/sdk/core.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)    10226 2024-04-16 18:39:17.000000 composio_core-0.2.7/composio/sdk/enums.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)    21190 2024-04-17 08:08:09.000000 composio_core-0.2.7/composio/sdk/sdk.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)        0 2024-04-15 07:39:40.000000 composio_core-0.2.7/composio/sdk/shared.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     1358 2024-04-16 16:08:42.000000 composio_core-0.2.7/composio/sdk/storage.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3455 2024-04-16 17:03:02.000000 composio_core-0.2.7/composio/sdk/utils.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-17 08:08:52.074461 composio_core-0.2.7/composio_core.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      796 2024-04-17 08:08:52.000000 composio_core-0.2.7/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      489 2024-04-17 08:08:52.000000 composio_core-0.2.7/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-17 08:08:52.000000 composio_core-0.2.7/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       60 2024-04-17 08:08:52.000000 composio_core-0.2.7/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      103 2024-04-17 08:08:52.000000 composio_core-0.2.7/composio_core.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        9 2024-04-17 08:08:52.000000 composio_core-0.2.7/composio_core.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      528 2024-04-15 07:39:40.000000 composio_core-0.2.7/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)      130 2024-04-15 07:39:40.000000 composio_core-0.2.7/requirements.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-17 08:08:52.074961 composio_core-0.2.7/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)     1127 2024-04-17 08:08:46.000000 composio_core-0.2.7/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:07:27.833490 composio_core-0.2.8/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       48 2024-04-15 07:39:40.000000 composio_core-0.2.8/MANIFEST.in
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      796 2024-04-18 18:07:27.833245 composio_core-0.2.8/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      102 2024-04-15 07:39:40.000000 composio_core-0.2.8/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:07:27.827969 composio_core-0.2.8/composio/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      159 2024-04-15 07:39:40.000000 composio_core-0.2.8/composio/__init__.py
+-rwxr-xr-x   0 karanvaidya   (501) staff       (20)    22079 2024-04-18 18:07:01.000000 composio_core-0.2.8/composio/composio_cli.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:07:27.830924 composio_core-0.2.8/composio/sdk/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       85 2024-04-15 07:39:40.000000 composio_core-0.2.8/composio/sdk/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     7018 2024-04-16 18:37:25.000000 composio_core-0.2.8/composio/sdk/core.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)    10226 2024-04-16 18:39:17.000000 composio_core-0.2.8/composio/sdk/enums.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)    21190 2024-04-17 08:08:09.000000 composio_core-0.2.8/composio/sdk/sdk.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        0 2024-04-15 07:39:40.000000 composio_core-0.2.8/composio/sdk/shared.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     1358 2024-04-16 16:08:42.000000 composio_core-0.2.8/composio/sdk/storage.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3455 2024-04-16 17:03:02.000000 composio_core-0.2.8/composio/sdk/utils.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:07:27.832893 composio_core-0.2.8/composio_core.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      796 2024-04-18 18:07:27.000000 composio_core-0.2.8/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      489 2024-04-18 18:07:27.000000 composio_core-0.2.8/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-18 18:07:27.000000 composio_core-0.2.8/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       60 2024-04-18 18:07:27.000000 composio_core-0.2.8/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      103 2024-04-18 18:07:27.000000 composio_core-0.2.8/composio_core.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        9 2024-04-18 18:07:27.000000 composio_core-0.2.8/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      528 2024-04-15 07:39:40.000000 composio_core-0.2.8/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      130 2024-04-15 07:39:40.000000 composio_core-0.2.8/requirements.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-18 18:07:27.833574 composio_core-0.2.8/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     1127 2024-04-18 18:07:01.000000 composio_core-0.2.8/setup.py
```

### Comparing `composio_core-0.2.7/PKG-INFO` & `composio_core-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.2.7
+Version: 0.2.8
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.2.7/composio/composio_cli.py` & `composio_core-0.2.8/composio/composio_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,15 +333,15 @@
             return
 
     console.print(f"\n[green]> Adding integration: {integration_name.capitalize()}...[/green]\n")
     try:
         app = client.sdk.get_app(args.integration_name)
         auth_schemes = app.get('auth_schemes')
         auth_schemes_arr = [auth_scheme.get('auth_mode') for auth_scheme in auth_schemes]
-        if len(auth_schemes_arr) > 1 and auth_schemes_arr[0] == 'API_KEY':
+        if len(auth_schemes_arr) > 1 and auth_schemes_arr[0] in ['API_KEY', 'BASIC', 'SNOWFLAKE']:
             connection = entity.initiate_connection(integration_name.lower())
             fields = auth_schemes[0].get('fields')
             fields_input = {}
             for field in fields:
                 if field.get('expected_from_customer', True):
                     if field.get('required', False):
                         console.print(f"[green]> Enter {field.get('displayName', field.get('name'))}: [/green]", end="")
@@ -349,15 +349,14 @@
                         if not value:  # If a required field is not provided and no default is available
                             console.print(f"[red]Error: {field.get('displayName', field.get('name'))} is required[/red]")
                             sys.exit(1)
                     else:
                         console.print(f"[green]> Enter {field.get('displayName', field.get('name'))} (Optional): [/green]", end="")
                         value = input() or field.get('default')
                     fields_input[field.get('name')] = value
-
             connection.save_user_access_data(fields_input)
         else: 
             # @TODO: add logic to wait and ask for API_KEY
             connection = entity.initiate_connection(integration_name.lower())
             if not should_disable_webbrowser_open:
                 webbrowser.open(connection.redirectUrl)
             print(f"Please authenticate {integration_name} in the browser and come back here. URL: {connection.redirectUrl}")
```

### Comparing `composio_core-0.2.7/composio/sdk/core.py` & `composio_core-0.2.8/composio/sdk/core.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.2.7/composio/sdk/enums.py` & `composio_core-0.2.8/composio/sdk/enums.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.2.7/composio/sdk/sdk.py` & `composio_core-0.2.8/composio/sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.2.7/composio/sdk/storage.py` & `composio_core-0.2.8/composio/sdk/storage.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.2.7/composio/sdk/utils.py` & `composio_core-0.2.8/composio/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.2.7/composio_core.egg-info/PKG-INFO` & `composio_core-0.2.8/composio_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.2.7
+Version: 0.2.8
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.2.7/pyproject.toml` & `composio_core-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `composio_core-0.2.7/setup.py` & `composio_core-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """Customized setuptools install command."""
 
     def run(self):
         install.run(self)
 
 setup(
     name="composio_core",
-    version="0.2.7",
+    version="0.2.8",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

