# Comparing `tmp/sesamclient-1.2.4.tar.gz` & `tmp/sesamclient-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sesamclient-1.2.4.tar", last modified: Tue Mar  5 08:23:01 2024, max compression
+gzip compressed data, was "sesamclient-1.2.5.tar", last modified: Thu Apr 18 09:48:28 2024, max compression
```

## Comparing `sesamclient-1.2.4.tar` & `sesamclient-1.2.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 sesam     (1000) sesam     (1000)        0 2024-03-05 08:23:01.247897 sesamclient-1.2.4/
--rw-r--r--   0 sesam     (1000) sesam     (1000)       49 2024-03-05 08:22:57.000000 sesamclient-1.2.4/MANIFEST.in
--rw-r--r--   0 sesam     (1000) sesam     (1000)      277 2024-03-05 08:23:01.247897 sesamclient-1.2.4/PKG-INFO
--rw-r--r--   0 sesam     (1000) sesam     (1000)       33 2024-03-05 08:22:57.000000 sesamclient-1.2.4/README.txt
--rw-r--r--   0 sesam     (1000) sesam     (1000)      427 2024-03-05 08:22:57.000000 sesamclient-1.2.4/requirements.txt
-drwxr-xr-x   0 sesam     (1000) sesam     (1000)        0 2024-03-05 08:23:01.247897 sesamclient-1.2.4/sesamclient/
--rw-r--r--   0 sesam     (1000) sesam     (1000)        5 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/VERSION.txt
--rw-r--r--   0 sesam     (1000) sesam     (1000)      257 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/__init__.py
--rw-r--r--   0 sesam     (1000) sesam     (1000)    56140 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/connection.py
--rw-r--r--   0 sesam     (1000) sesam     (1000)    11949 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/dataset.py
--rw-r--r--   0 sesam     (1000) sesam     (1000)     7002 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/entity_json.py
--rw-r--r--   0 sesam     (1000) sesam     (1000)     3706 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/entitybase.py
--rw-r--r--   0 sesam     (1000) sesam     (1000)     2447 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/exceptions.py
--rw-r--r--   0 sesam     (1000) sesam     (1000)      547 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/log.py
-drwxr-xr-x   0 sesam     (1000) sesam     (1000)        0 2024-03-05 08:23:01.247897 sesamclient-1.2.4/sesamclient/main/
--rw-r--r--   0 sesam     (1000) sesam     (1000)      126 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/main/__init__.py
-drwxr-xr-x   0 sesam     (1000) sesam     (1000)        0 2024-03-05 08:23:01.247897 sesamclient-1.2.4/sesamclient/main/commands/
--rw-r--r--   0 sesam     (1000) sesam     (1000)      126 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/main/commands/__init__.py
--rw-r--r--   0 sesam     (1000) sesam     (1000)     1809 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/main/commands/config.py
--rw-r--r--   0 sesam     (1000) sesam     (1000)     2165 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/main/commands/datasets.py
--rw-r--r--   0 sesam     (1000) sesam     (1000)     1277 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/main/commands/envvarsmanager.py
--rw-r--r--   0 sesam     (1000) sesam     (1000)     5937 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/main/commands/export.py
--rw-r--r--   0 sesam     (1000) sesam     (1000)     8368 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/main/commands/import_cmd.py
--rw-r--r--   0 sesam     (1000) sesam     (1000)      658 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/main/commands/license.py
--rw-r--r--   0 sesam     (1000) sesam     (1000)     1704 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/main/commands/login.py
--rw-r--r--   0 sesam     (1000) sesam     (1000)      615 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/main/commands/logs.py
--rw-r--r--   0 sesam     (1000) sesam     (1000)     1976 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/main/commands/pipes.py
--rw-r--r--   0 sesam     (1000) sesam     (1000)     5414 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/main/commands/pumps.py
--rw-r--r--   0 sesam     (1000) sesam     (1000)     2491 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/main/commands/secretsmanager.py
--rw-r--r--   0 sesam     (1000) sesam     (1000)     1686 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/main/commands/systems.py
--rw-r--r--   0 sesam     (1000) sesam     (1000)    39667 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/main/main.py
--rw-r--r--   0 sesam     (1000) sesam     (1000)     2705 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/main/utils.py
--rw-r--r--   0 sesam     (1000) sesam     (1000)     1045 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/model.py
--rw-r--r--   0 sesam     (1000) sesam     (1000)    11585 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/pipe.py
--rw-r--r--   0 sesam     (1000) sesam     (1000)    16392 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/pump.py
--rw-r--r--   0 sesam     (1000) sesam     (1000)     6052 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/system.py
-drwxr-xr-x   0 sesam     (1000) sesam     (1000)        0 2024-03-05 08:23:01.247897 sesamclient-1.2.4/sesamclient/tests/
--rw-r--r--   0 sesam     (1000) sesam     (1000)      150 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/tests/__init__.py
--rw-r--r--   0 sesam     (1000) sesam     (1000)    11381 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/tests/test_export_command.py
--rw-r--r--   0 sesam     (1000) sesam     (1000)     7947 2024-03-05 08:22:57.000000 sesamclient-1.2.4/sesamclient/utils.py
-drwxr-xr-x   0 sesam     (1000) sesam     (1000)        0 2024-03-05 08:23:01.247897 sesamclient-1.2.4/sesamclient.egg-info/
--rw-r--r--   0 sesam     (1000) sesam     (1000)      277 2024-03-05 08:23:01.000000 sesamclient-1.2.4/sesamclient.egg-info/PKG-INFO
--rw-r--r--   0 sesam     (1000) sesam     (1000)     1233 2024-03-05 08:23:01.000000 sesamclient-1.2.4/sesamclient.egg-info/SOURCES.txt
--rw-r--r--   0 sesam     (1000) sesam     (1000)        1 2024-03-05 08:23:01.000000 sesamclient-1.2.4/sesamclient.egg-info/dependency_links.txt
--rw-r--r--   0 sesam     (1000) sesam     (1000)       54 2024-03-05 08:23:01.000000 sesamclient-1.2.4/sesamclient.egg-info/entry_points.txt
--rw-r--r--   0 sesam     (1000) sesam     (1000)        1 2024-03-05 08:23:01.000000 sesamclient-1.2.4/sesamclient.egg-info/not-zip-safe
--rw-r--r--   0 sesam     (1000) sesam     (1000)       85 2024-03-05 08:23:01.000000 sesamclient-1.2.4/sesamclient.egg-info/requires.txt
--rw-r--r--   0 sesam     (1000) sesam     (1000)       12 2024-03-05 08:23:01.000000 sesamclient-1.2.4/sesamclient.egg-info/top_level.txt
--rw-r--r--   0 sesam     (1000) sesam     (1000)       38 2024-03-05 08:23:01.247897 sesamclient-1.2.4/setup.cfg
--rw-r--r--   0 sesam     (1000) sesam     (1000)     1197 2024-03-05 08:22:57.000000 sesamclient-1.2.4/setup.py
+drwxr-xr-x   0 sesam     (1000) sesam     (1000)        0 2024-04-18 09:48:28.215251 sesamclient-1.2.5/
+-rw-r--r--   0 sesam     (1000) sesam     (1000)       49 2024-04-18 09:15:39.000000 sesamclient-1.2.5/MANIFEST.in
+-rw-r--r--   0 sesam     (1000) sesam     (1000)      277 2024-04-18 09:48:28.215251 sesamclient-1.2.5/PKG-INFO
+-rw-r--r--   0 sesam     (1000) sesam     (1000)       33 2024-04-18 09:15:39.000000 sesamclient-1.2.5/README.txt
+-rw-r--r--   0 sesam     (1000) sesam     (1000)      427 2024-04-18 09:15:39.000000 sesamclient-1.2.5/requirements.txt
+drwxr-xr-x   0 sesam     (1000) sesam     (1000)        0 2024-04-18 09:48:28.211251 sesamclient-1.2.5/sesamclient/
+-rw-r--r--   0 sesam     (1000) sesam     (1000)        5 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/VERSION.txt
+-rw-r--r--   0 sesam     (1000) sesam     (1000)      257 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/__init__.py
+-rw-r--r--   0 sesam     (1000) sesam     (1000)    56499 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/connection.py
+-rw-r--r--   0 sesam     (1000) sesam     (1000)    11949 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/dataset.py
+-rw-r--r--   0 sesam     (1000) sesam     (1000)     7002 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/entity_json.py
+-rw-r--r--   0 sesam     (1000) sesam     (1000)     3706 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/entitybase.py
+-rw-r--r--   0 sesam     (1000) sesam     (1000)     2447 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/exceptions.py
+-rw-r--r--   0 sesam     (1000) sesam     (1000)      547 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/log.py
+drwxr-xr-x   0 sesam     (1000) sesam     (1000)        0 2024-04-18 09:48:28.215251 sesamclient-1.2.5/sesamclient/main/
+-rw-r--r--   0 sesam     (1000) sesam     (1000)      126 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/main/__init__.py
+drwxr-xr-x   0 sesam     (1000) sesam     (1000)        0 2024-04-18 09:48:28.215251 sesamclient-1.2.5/sesamclient/main/commands/
+-rw-r--r--   0 sesam     (1000) sesam     (1000)      126 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/main/commands/__init__.py
+-rw-r--r--   0 sesam     (1000) sesam     (1000)     1809 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/main/commands/config.py
+-rw-r--r--   0 sesam     (1000) sesam     (1000)     2165 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/main/commands/datasets.py
+-rw-r--r--   0 sesam     (1000) sesam     (1000)     1277 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/main/commands/envvarsmanager.py
+-rw-r--r--   0 sesam     (1000) sesam     (1000)     5937 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/main/commands/export.py
+-rw-r--r--   0 sesam     (1000) sesam     (1000)     8368 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/main/commands/import_cmd.py
+-rw-r--r--   0 sesam     (1000) sesam     (1000)      658 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/main/commands/license.py
+-rw-r--r--   0 sesam     (1000) sesam     (1000)     1704 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/main/commands/login.py
+-rw-r--r--   0 sesam     (1000) sesam     (1000)      615 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/main/commands/logs.py
+-rw-r--r--   0 sesam     (1000) sesam     (1000)     1976 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/main/commands/pipes.py
+-rw-r--r--   0 sesam     (1000) sesam     (1000)     5414 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/main/commands/pumps.py
+-rw-r--r--   0 sesam     (1000) sesam     (1000)     2491 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/main/commands/secretsmanager.py
+-rw-r--r--   0 sesam     (1000) sesam     (1000)     1686 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/main/commands/systems.py
+-rw-r--r--   0 sesam     (1000) sesam     (1000)    39667 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/main/main.py
+-rw-r--r--   0 sesam     (1000) sesam     (1000)     2705 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/main/utils.py
+-rw-r--r--   0 sesam     (1000) sesam     (1000)     1045 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/model.py
+-rw-r--r--   0 sesam     (1000) sesam     (1000)    11585 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/pipe.py
+-rw-r--r--   0 sesam     (1000) sesam     (1000)    16392 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/pump.py
+-rw-r--r--   0 sesam     (1000) sesam     (1000)     6052 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/system.py
+drwxr-xr-x   0 sesam     (1000) sesam     (1000)        0 2024-04-18 09:48:28.215251 sesamclient-1.2.5/sesamclient/tests/
+-rw-r--r--   0 sesam     (1000) sesam     (1000)      150 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/tests/__init__.py
+-rw-r--r--   0 sesam     (1000) sesam     (1000)    11381 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/tests/test_export_command.py
+-rw-r--r--   0 sesam     (1000) sesam     (1000)     7947 2024-04-18 09:15:39.000000 sesamclient-1.2.5/sesamclient/utils.py
+drwxr-xr-x   0 sesam     (1000) sesam     (1000)        0 2024-04-18 09:48:28.211251 sesamclient-1.2.5/sesamclient.egg-info/
+-rw-r--r--   0 sesam     (1000) sesam     (1000)      277 2024-04-18 09:48:28.000000 sesamclient-1.2.5/sesamclient.egg-info/PKG-INFO
+-rw-r--r--   0 sesam     (1000) sesam     (1000)     1233 2024-04-18 09:48:28.000000 sesamclient-1.2.5/sesamclient.egg-info/SOURCES.txt
+-rw-r--r--   0 sesam     (1000) sesam     (1000)        1 2024-04-18 09:48:28.000000 sesamclient-1.2.5/sesamclient.egg-info/dependency_links.txt
+-rw-r--r--   0 sesam     (1000) sesam     (1000)       54 2024-04-18 09:48:28.000000 sesamclient-1.2.5/sesamclient.egg-info/entry_points.txt
+-rw-r--r--   0 sesam     (1000) sesam     (1000)        1 2024-04-18 09:15:41.000000 sesamclient-1.2.5/sesamclient.egg-info/not-zip-safe
+-rw-r--r--   0 sesam     (1000) sesam     (1000)       85 2024-04-18 09:48:28.000000 sesamclient-1.2.5/sesamclient.egg-info/requires.txt
+-rw-r--r--   0 sesam     (1000) sesam     (1000)       12 2024-04-18 09:48:28.000000 sesamclient-1.2.5/sesamclient.egg-info/top_level.txt
+-rw-r--r--   0 sesam     (1000) sesam     (1000)       38 2024-04-18 09:48:28.215251 sesamclient-1.2.5/setup.cfg
+-rw-r--r--   0 sesam     (1000) sesam     (1000)     1197 2024-04-18 09:15:39.000000 sesamclient-1.2.5/setup.py
```

### Comparing `sesamclient-1.2.4/sesamclient/connection.py` & `sesamclient-1.2.5/sesamclient/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -783,15 +783,18 @@
 
         # TODO: wrap in a utility-method and add error-detection
         request_params = {}
         if include_internal_pipes:
             request_params["include-internal-pipes"] = "true"
 
         if fields is not None:
-            request_params["fields"] = fields
+            if isinstance(fields, list):
+                request_params["fields"] = ",".join(fields)
+            else:
+                request_params["fields"] = fields
         response = self.do_get_request(self.pipes_url,
                                        allowable_response_status_codes=[200],
                                        params=request_params, **kwargs
                                        )
 
         parsed_response = utils.parse_json_response(response)
 
@@ -802,30 +805,36 @@
     def get_pipes_streaming(self, include_internal_pipes=False, fields=None, **kwargs):
         # TODO: wrap in a utility-method and add error-detection
         request_params = {}
         if include_internal_pipes:
             request_params["include-internal-pipes"] = "true"
 
         if fields is not None:
-            request_params["fields"] = fields
+            if isinstance(fields, list):
+                request_params["fields"] = ",".join(fields)
+            else:
+                request_params["fields"] = fields
         response = self.do_get_request(self.pipes_url,
                                        allowable_response_status_codes=[200],
                                        params=request_params, stream=True, **kwargs
                                        )
 
         for pipe_json in entity_json.parse_json_stream(response.raw, do_transit_decoding=False):
             yield Pipe(self, pipe_json)
 
     def get_pipe(self, pipe_id, fields=None, **kwargs):
         # TODO: wrap in a utility-method and add error-detection
 
         request_params = kwargs.pop("request_params", {})
 
         if fields is not None:
-            request_params["fields"] = ",".join(fields)
+            if isinstance(fields, list):
+                request_params["fields"] = ",".join(fields)
+            else:
+                request_params["fields"] = fields
         response = self.do_get_request(self.get_pipe_url(pipe_id), params=request_params, **kwargs)
         if response.status_code == 404:
             return None
         pipe_json = utils.parse_json_response(response)
         return Pipe(self, pipe_json)
 
     def get_pipe_schema_def(self, pipe_id, sample_size=1000, keys_only=False, **kwargs):
```

### Comparing `sesamclient-1.2.4/sesamclient/dataset.py` & `sesamclient-1.2.5/sesamclient/dataset.py`

 * *Files identical despite different names*

### Comparing `sesamclient-1.2.4/sesamclient/entity_json.py` & `sesamclient-1.2.5/sesamclient/entity_json.py`

 * *Files identical despite different names*

### Comparing `sesamclient-1.2.4/sesamclient/entitybase.py` & `sesamclient-1.2.5/sesamclient/entitybase.py`

 * *Files identical despite different names*

### Comparing `sesamclient-1.2.4/sesamclient/exceptions.py` & `sesamclient-1.2.5/sesamclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `sesamclient-1.2.4/sesamclient/log.py` & `sesamclient-1.2.5/sesamclient/log.py`

 * *Files identical despite different names*

### Comparing `sesamclient-1.2.4/sesamclient/main/commands/config.py` & `sesamclient-1.2.5/sesamclient/main/commands/config.py`

 * *Files identical despite different names*

### Comparing `sesamclient-1.2.4/sesamclient/main/commands/datasets.py` & `sesamclient-1.2.5/sesamclient/main/commands/datasets.py`

 * *Files identical despite different names*

### Comparing `sesamclient-1.2.4/sesamclient/main/commands/envvarsmanager.py` & `sesamclient-1.2.5/sesamclient/main/commands/envvarsmanager.py`

 * *Files identical despite different names*

### Comparing `sesamclient-1.2.4/sesamclient/main/commands/export.py` & `sesamclient-1.2.5/sesamclient/main/commands/export.py`

 * *Files identical despite different names*

### Comparing `sesamclient-1.2.4/sesamclient/main/commands/import_cmd.py` & `sesamclient-1.2.5/sesamclient/main/commands/import_cmd.py`

 * *Files identical despite different names*

### Comparing `sesamclient-1.2.4/sesamclient/main/commands/license.py` & `sesamclient-1.2.5/sesamclient/main/commands/license.py`

 * *Files identical despite different names*

### Comparing `sesamclient-1.2.4/sesamclient/main/commands/login.py` & `sesamclient-1.2.5/sesamclient/main/commands/login.py`

 * *Files identical despite different names*

### Comparing `sesamclient-1.2.4/sesamclient/main/commands/logs.py` & `sesamclient-1.2.5/sesamclient/main/commands/logs.py`

 * *Files identical despite different names*

### Comparing `sesamclient-1.2.4/sesamclient/main/commands/pipes.py` & `sesamclient-1.2.5/sesamclient/main/commands/pipes.py`

 * *Files identical despite different names*

### Comparing `sesamclient-1.2.4/sesamclient/main/commands/pumps.py` & `sesamclient-1.2.5/sesamclient/main/commands/pumps.py`

 * *Files identical despite different names*

### Comparing `sesamclient-1.2.4/sesamclient/main/commands/secretsmanager.py` & `sesamclient-1.2.5/sesamclient/main/commands/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `sesamclient-1.2.4/sesamclient/main/commands/systems.py` & `sesamclient-1.2.5/sesamclient/main/commands/systems.py`

 * *Files identical despite different names*

### Comparing `sesamclient-1.2.4/sesamclient/main/main.py` & `sesamclient-1.2.5/sesamclient/main/main.py`

 * *Files identical despite different names*

### Comparing `sesamclient-1.2.4/sesamclient/main/utils.py` & `sesamclient-1.2.5/sesamclient/main/utils.py`

 * *Files identical despite different names*

### Comparing `sesamclient-1.2.4/sesamclient/model.py` & `sesamclient-1.2.5/sesamclient/model.py`

 * *Files identical despite different names*

### Comparing `sesamclient-1.2.4/sesamclient/pipe.py` & `sesamclient-1.2.5/sesamclient/pipe.py`

 * *Files identical despite different names*

### Comparing `sesamclient-1.2.4/sesamclient/pump.py` & `sesamclient-1.2.5/sesamclient/pump.py`

 * *Files identical despite different names*

### Comparing `sesamclient-1.2.4/sesamclient/system.py` & `sesamclient-1.2.5/sesamclient/system.py`

 * *Files identical despite different names*

### Comparing `sesamclient-1.2.4/sesamclient/tests/test_export_command.py` & `sesamclient-1.2.5/sesamclient/tests/test_export_command.py`

 * *Files identical despite different names*

### Comparing `sesamclient-1.2.4/sesamclient/utils.py` & `sesamclient-1.2.5/sesamclient/utils.py`

 * *Files identical despite different names*

### Comparing `sesamclient-1.2.4/sesamclient.egg-info/SOURCES.txt` & `sesamclient-1.2.5/sesamclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sesamclient-1.2.4/setup.py` & `sesamclient-1.2.5/setup.py`

 * *Files identical despite different names*

