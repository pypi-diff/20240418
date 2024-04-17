# Comparing `tmp/pystackql-3.5.7.tar.gz` & `tmp/pystackql-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystackql-3.5.7.tar", last modified: Wed Apr 17 04:54:24 2024, max compression
+gzip compressed data, was "pystackql-3.6.0.tar", last modified: Wed Apr 17 21:43:57 2024, max compression
```

## Comparing `pystackql-3.5.7.tar` & `pystackql-3.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 04:54:24.651374 pystackql-3.5.7/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 pystackql-3.5.7/LICENSE
--rwxrwxrwx   0 javen     (1000) javen     (1000)     7019 2024-04-17 04:54:24.594382 pystackql-3.5.7/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)     5198 2024-04-17 04:54:07.000000 pystackql-3.5.7/README.rst
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 04:54:23.185189 pystackql-3.5.7/pystackql/
--rwxrwxrwx   0 javen     (1000) javen     (1000)      101 2024-04-12 21:02:08.000000 pystackql-3.5.7/pystackql/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     5209 2024-03-15 01:52:38.000000 pystackql-3.5.7/pystackql/_util.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1751 2024-03-15 01:52:38.000000 pystackql-3.5.7/pystackql/base_stackql_magic.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1740 2024-03-15 01:52:38.000000 pystackql-3.5.7/pystackql/magic.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1743 2024-03-15 01:52:38.000000 pystackql-3.5.7/pystackql/magics.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)    26027 2024-04-17 04:52:53.000000 pystackql-3.5.7/pystackql/stackql.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 04:54:24.465778 pystackql-3.5.7/pystackql.egg-info/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     7019 2024-04-17 04:54:21.000000 pystackql-3.5.7/pystackql.egg-info/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)      345 2024-04-17 04:54:22.000000 pystackql-3.5.7/pystackql.egg-info/SOURCES.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-17 04:54:21.000000 pystackql-3.5.7/pystackql.egg-info/dependency_links.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       24 2024-04-17 04:54:21.000000 pystackql-3.5.7/pystackql.egg-info/requires.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       10 2024-04-17 04:54:21.000000 pystackql-3.5.7/pystackql.egg-info/top_level.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-17 04:54:24.655917 pystackql-3.5.7/setup.cfg
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1254 2024-04-17 04:54:07.000000 pystackql-3.5.7/setup.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 04:54:24.219836 pystackql-3.5.7/tests/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     2348 2024-04-07 22:41:05.000000 pystackql-3.5.7/tests/test_params.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 21:43:57.305140 pystackql-3.6.0/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 pystackql-3.6.0/LICENSE
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     7019 2024-04-17 21:43:57.292590 pystackql-3.6.0/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     5198 2024-04-17 21:43:36.000000 pystackql-3.6.0/README.rst
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 21:43:57.061352 pystackql-3.6.0/pystackql/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      101 2024-04-12 21:02:08.000000 pystackql-3.6.0/pystackql/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     5209 2024-03-15 01:52:38.000000 pystackql-3.6.0/pystackql/_util.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1751 2024-03-15 01:52:38.000000 pystackql-3.6.0/pystackql/base_stackql_magic.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1740 2024-03-15 01:52:38.000000 pystackql-3.6.0/pystackql/magic.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1743 2024-03-15 01:52:38.000000 pystackql-3.6.0/pystackql/magics.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)    27094 2024-04-17 21:38:28.000000 pystackql-3.6.0/pystackql/stackql.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 21:43:57.276041 pystackql-3.6.0/pystackql.egg-info/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     7019 2024-04-17 21:43:56.000000 pystackql-3.6.0/pystackql.egg-info/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      345 2024-04-17 21:43:56.000000 pystackql-3.6.0/pystackql.egg-info/SOURCES.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-17 21:43:56.000000 pystackql-3.6.0/pystackql.egg-info/dependency_links.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       24 2024-04-17 21:43:56.000000 pystackql-3.6.0/pystackql.egg-info/requires.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       10 2024-04-17 21:43:56.000000 pystackql-3.6.0/pystackql.egg-info/top_level.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-17 21:43:57.306146 pystackql-3.6.0/setup.cfg
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1254 2024-04-17 21:43:36.000000 pystackql-3.6.0/setup.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 21:43:57.229852 pystackql-3.6.0/tests/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     2348 2024-04-07 22:41:05.000000 pystackql-3.6.0/tests/test_params.py
```

### Comparing `pystackql-3.5.7/LICENSE` & `pystackql-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pystackql-3.5.7/PKG-INFO` & `pystackql-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystackql
-Version: 3.5.7
+Version: 3.6.0
 Summary: A Python interface for StackQL
 Home-page: https://github.com/stackql/pystackql
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT License
         
         Copyright (c) 2022 StackQL Studios
@@ -233,8 +233,8 @@
 Publishing the package
 ~~~~~~~~~~~~~~~~~~~~~~
 
 To publish the package to PyPI, run the following command:
 
 ::
 
-    twine upload --config-file .pypirc dist/pystackql-3.5.7.tar.gz
+    twine upload --config-file .pypirc dist/pystackql-3.6.0.tar.gz
```

### Comparing `pystackql-3.5.7/README.rst` & `pystackql-3.6.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -190,8 +190,8 @@
 Publishing the package
 ~~~~~~~~~~~~~~~~~~~~~~
 
 To publish the package to PyPI, run the following command:
 
 ::
 
-    twine upload --config-file .pypirc dist/pystackql-3.5.7.tar.gz
+    twine upload --config-file .pypirc dist/pystackql-3.6.0.tar.gz
```

### Comparing `pystackql-3.5.7/pystackql/_util.py` & `pystackql-3.6.0/pystackql/_util.py`

 * *Files identical despite different names*

### Comparing `pystackql-3.5.7/pystackql/base_stackql_magic.py` & `pystackql-3.6.0/pystackql/base_stackql_magic.py`

 * *Files identical despite different names*

### Comparing `pystackql-3.5.7/pystackql/magic.py` & `pystackql-3.6.0/pystackql/magic.py`

 * *Files identical despite different names*

### Comparing `pystackql-3.5.7/pystackql/magics.py` & `pystackql-3.6.0/pystackql/magics.py`

 * *Files identical despite different names*

### Comparing `pystackql-3.5.7/pystackql/stackql.py` & `pystackql-3.6.0/pystackql/stackql.py`

 * *Files 3% similar despite different names*

```diff
@@ -172,16 +172,25 @@
 		It waits for the subprocess to complete and captures its stdout as the output. This approach ensures 
 		that resources like pipes are properly cleaned up after the subprocess completes.
 
 		:param query: The StackQL query string to be executed.
 		:type query: str
 
 		:return: The output result of the query, which can either be the actual query result or an error message.
-		:rtype: str
+		:rtype: dict
+
+		Example:
+			::
 
+				{
+					"data": "[{\"machine_type\": \"n1-standard-1\", \"status\": \"RUNNING\", \"num_instances\": 3}, ...]",
+					"error": "stderr message if present",
+					"exception": "ERROR: {\"exception\": \"<exception message>\", \"doc\": \"<exception doc>\", \"params\": \"<params>\", \"stdout\": \"<stdout>\", \"stderr\": \"<stderr>\"}
+				}
+		
 		Possible error messages include:
 		- Indications that the StackQL binary wasn't found.
 		- Generic error messages for other exceptions encountered during the query execution.
 
 		:raises FileNotFoundError: If the StackQL binary isn't found.
 		:raises Exception: For any other exceptions during the execution, providing a generic error message.
 		"""
@@ -215,19 +224,14 @@
 				"doc": e.__doc__,
 				"params": local_params,
 				"stdout": stdout.decode('utf-8') if 'stdout' in locals() and isinstance(stdout, bytes) else "",
 				"stderr": stderr.decode('utf-8') if 'stderr' in locals() and isinstance(stderr, bytes) else ""
 			}
 			output["exception"] = f"ERROR: {json.dumps(error_details)}"
 
-		# output = {'data': <stdout str>, 'error': <stderr str>, 'exception': <exception as a json string> }
-		# for a statement you would expect 'error' to exist
-		# for a query you would expect 'data' to exist
-		# 'exception' in output indicates an error occurred during the execution (statement or query)
-
 		return output
 
 	def __init__(self, 
 				 server_mode=False, 
 				 server_address='127.0.0.1', 
 				 server_port=5466,
 				 backend_storage_mode='memory',
@@ -483,20 +487,28 @@
 				return pd.DataFrame(result)
 			elif self.output == 'csv':
 				# return the string representation of the result
 				return result[0]['message']
 			else:
 				return result
 		else:
+
 			# returns either...
 			# {'error': '<error message>'} if something went wrong; or
 			# {'message': '<message>'} if the statement was executed successfully
+
 			result = self._run_query(query)
 			if "exception" in result:
-				return {"error": result["exception"]}
+				exception_msg = result["exception"]
+				if self.output == 'pandas':
+					return pd.DataFrame({'error': [exception_msg]}) if exception_msg else pd.DataFrame({'error': []})
+				elif self.output == 'csv':		
+					return exception_msg
+				else:		
+					return {"error": exception_msg}
 
 			# message on stderr
 			message = result["error"]
 
 			if self.output == 'pandas':
 				return pd.DataFrame({'message': [message]}) if message else pd.DataFrame({'message': []})
 			elif self.output == 'csv':
@@ -539,43 +551,65 @@
 				return pd.read_json(StringIO(json_str))
 			elif self.output == 'csv':
 				raise ValueError("CSV output is not supported in server_mode.")
 			else:  # Assume 'dict' output
 				return result
 		else:
 			# returns either...
-			# {'error': <error json str>} if something went wrong; or
-			# [{<data>}] if the statement was executed successfully, messages to stderr are ignored
+			# [{'error': <error json str>}] if something went wrong; or
+			# [{<row1>},...] if the statement was executed successfully, messages to stderr are ignored
 
 			output = self._run_query(query)
 			if "exception" in output:
-				return {"error": output["exception"]}
+				exception_msg = output["exception"]
+				if self.output == 'pandas':
+					return pd.DataFrame({'error': [exception_msg]}) if exception_msg else pd.DataFrame({'error': []})
+				elif self.output == 'csv':		
+					return exception_msg
+				else:		
+					return [{"error": exception_msg}]
 
 			if "data" in output:
+				data = output["data"]
 				# theres data, return it
 				if self.output == 'csv':
-					return output["data"]
+					return data
 				elif self.output == 'pandas':
 					try:
-						return pd.read_json(StringIO(output["data"]))
+						return pd.read_json(StringIO(data))
 					except ValueError:
 						return pd.DataFrame([{"error": "Invalid JSON output"}])
 				else:  # Assume 'dict' output
 					try:
-						return json.loads(output["data"])
+						return json.loads(data)
 					except ValueError:
-						return {"error": f"Invalid JSON output : {output['data']}"}            
-			else:
-				if "error" in output:
-					if suppress_errors:
-						return []
-					else:
-						return {"error": output["error"]}
+						return [{"error": f"Invalid JSON output : {data}"}]
+
+			if "error" in output:
+				# theres no data but there is stderr from the request, could be an expected error like a 404
+				if suppress_errors:
+					# we dont care about errors, return an empty list
+					csv_ret = ""
+					pd_ret = pd.DataFrame()
+					dict_ret = []
+				else:
+					# we care about errors, return the error
+					err_msg = output["error"]
+					csv_ret = err_msg
+					pd_ret = pd.DataFrame([{"error": err_msg}])
+					dict_ret = [{"error": err_msg}]
+					  				
+				if self.output == 'csv':
+					return csv_ret
+				elif self.output == 'pandas':
+					return pd_ret
+				else:  # Assume 'dict' output
+					return dict_ret
+				
 
-	#
 	# asnyc query support
 	#
 
 	def _run_server_query_with_new_connection(self, query):
 		"""Run a query against a StackQL postgres wire protocol server with a new connection.
 		"""
 		conn = None
```

### Comparing `pystackql-3.5.7/pystackql.egg-info/PKG-INFO` & `pystackql-3.6.0/pystackql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystackql
-Version: 3.5.7
+Version: 3.6.0
 Summary: A Python interface for StackQL
 Home-page: https://github.com/stackql/pystackql
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT License
         
         Copyright (c) 2022 StackQL Studios
@@ -233,8 +233,8 @@
 Publishing the package
 ~~~~~~~~~~~~~~~~~~~~~~
 
 To publish the package to PyPI, run the following command:
 
 ::
 
-    twine upload --config-file .pypirc dist/pystackql-3.5.7.tar.gz
+    twine upload --config-file .pypirc dist/pystackql-3.6.0.tar.gz
```

### Comparing `pystackql-3.5.7/setup.py` & `pystackql-3.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     readme = f.read()
 
 with open('LICENSE') as f:
     license = f.read()
 
 setup(
     name='pystackql',
-    version='3.5.7',
+    version='3.6.0',
     description='A Python interface for StackQL',
     long_description=readme,
     author='Jeffrey Aven',
     author_email='javen@stackql.io',
     url='https://github.com/stackql/pystackql',
     license=license,
     packages=['pystackql'],
```

### Comparing `pystackql-3.5.7/tests/test_params.py` & `pystackql-3.6.0/tests/test_params.py`

 * *Files identical despite different names*

