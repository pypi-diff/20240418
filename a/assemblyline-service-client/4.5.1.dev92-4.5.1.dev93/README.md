# Comparing `tmp/assemblyline_service_client-4.5.1.dev92-py3-none-any.whl.zip` & `tmp/assemblyline_service_client-4.5.1.dev93-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9594 bytes, number of entries: 8
--rw-r--r--  2.0 unx       12 b- defN 24-Apr-17 16:58 assemblyline_service_client/VERSION
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 16:58 assemblyline_service_client/__init__.py
--rw-r--r--  2.0 unx    22546 b- defN 24-Apr-17 16:58 assemblyline_service_client/task_handler.py
--rw-r--r--  2.0 unx     1396 b- defN 24-Apr-17 16:58 assemblyline_service_client-4.5.1.dev92.dist-info/LICENCE.md
--rw-r--r--  2.0 unx     1577 b- defN 24-Apr-17 16:58 assemblyline_service_client-4.5.1.dev92.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 16:58 assemblyline_service_client-4.5.1.dev92.dist-info/WHEEL
--rw-r--r--  2.0 unx       28 b- defN 24-Apr-17 16:58 assemblyline_service_client-4.5.1.dev92.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      803 b- defN 24-Apr-17 16:58 assemblyline_service_client-4.5.1.dev92.dist-info/RECORD
-8 files, 26454 bytes uncompressed, 8146 bytes compressed:  69.2%
+Zip file size: 9660 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       12 b- defN 24-Apr-18 15:19 assemblyline_service_client/VERSION
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 15:19 assemblyline_service_client/__init__.py
+-rw-r--r--  2.0 unx    22907 b- defN 24-Apr-18 15:19 assemblyline_service_client/task_handler.py
+-rw-r--r--  2.0 unx     1396 b- defN 24-Apr-18 15:20 assemblyline_service_client-4.5.1.dev93.dist-info/LICENCE.md
+-rw-r--r--  2.0 unx     1577 b- defN 24-Apr-18 15:20 assemblyline_service_client-4.5.1.dev93.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-18 15:20 assemblyline_service_client-4.5.1.dev93.dist-info/WHEEL
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-18 15:20 assemblyline_service_client-4.5.1.dev93.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      803 b- defN 24-Apr-18 15:20 assemblyline_service_client-4.5.1.dev93.dist-info/RECORD
+8 files, 26815 bytes uncompressed, 8212 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: assemblyline_service_client/__init__.py
 Comment: 
 
 Filename: assemblyline_service_client/task_handler.py
 Comment: 
 
-Filename: assemblyline_service_client-4.5.1.dev92.dist-info/LICENCE.md
+Filename: assemblyline_service_client-4.5.1.dev93.dist-info/LICENCE.md
 Comment: 
 
-Filename: assemblyline_service_client-4.5.1.dev92.dist-info/METADATA
+Filename: assemblyline_service_client-4.5.1.dev93.dist-info/METADATA
 Comment: 
 
-Filename: assemblyline_service_client-4.5.1.dev92.dist-info/WHEEL
+Filename: assemblyline_service_client-4.5.1.dev93.dist-info/WHEEL
 Comment: 
 
-Filename: assemblyline_service_client-4.5.1.dev92.dist-info/top_level.txt
+Filename: assemblyline_service_client-4.5.1.dev93.dist-info/top_level.txt
 Comment: 
 
-Filename: assemblyline_service_client-4.5.1.dev92.dist-info/RECORD
+Filename: assemblyline_service_client-4.5.1.dev93.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## assemblyline_service_client/VERSION

```diff
@@ -1 +1 @@
-4.5.1.dev92
+4.5.1.dev93
```

## assemblyline_service_client/task_handler.py

```diff
@@ -31,14 +31,15 @@
 ])
 
 DEFAULT_API_KEY = 'ThisIsARandomAuthKey...ChangeMe!'
 LOG_LEVEL = logging.getLevelName(os.environ.get("LOG_LEVEL", "INFO"))
 SHUTDOWN_SECONDS_LIMIT = 10
 SUPPORTED_API = 'v1'
 TASK_REQUEST_TIMEOUT = int(os.environ.get('TASK_REQUEST_TIMEOUT', 30))
+FILE_REQUEST_TIMEOUT = int(os.environ.get('FILE_REQUEST_TIMEOUT', 180))
 
 
 # The number of tasks a service will complete before stopping, letting the environment start a new container.
 # By default there is no limit, but this lets the orchestration environment set one
 TASK_COMPLETE_LIMIT = float(os.environ.get('AL_SERVICE_TASK_LIMIT', 'inf'))
 
 
@@ -208,15 +209,16 @@
                     return resp
             except requests.ConnectionError:
                 if not retry:
                     self.log.info("Service server is unreachable...")
                 elif retry % 10 == 0:
                     self.log.warning(f"Service server has been unreachable for the past {retry} attempts. "
                                      "Is there something wrong with it?")
-            except requests.Timeout:  # Handles ConnectTimeout and ReadTimeout
+            except requests.Timeout as e:  # Handles ConnectTimeout and ReadTimeout
+                self.log.warning(f"We've timed out on: {url} ({e}) Retrying..")
                 pass
             except requests.HTTPError as e:
                 self.log.error(str(e))
                 raise
             except requests.exceptions.RequestException as e:  # All other types of exceptions
                 self.log.error(str(e))
                 raise
@@ -363,15 +365,15 @@
 
     def download_file(self, sha256, sid) -> Optional[str]:
         self.status = STATUSES.DOWNLOADING_FILE
         received_file_sha256 = ''
         file_path = None
         self.log.info(f"[{sid}] Downloading file: {sha256}")
         response = self.request_with_retries('get', self._path('file', sha256),
-                                             get_api_response=False, max_retry=3, headers=self.headers)
+                                             get_api_response=False, max_retry=3, headers=self.headers, timeout=FILE_REQUEST_TIMEOUT)
         if response is not None:
             # Check if we got a 'good' response
             if response.status_code == 200:
                 file_path = os.path.join(self.tasking_dir, sha256)
                 with open(file_path, 'wb') as f:
                     for chunk in response.iter_content(chunk_size=1024):
                         if chunk:  # filter out keep-alive new chunks
@@ -417,15 +419,15 @@
         if new_tool_version is not None and self.service_tool_version != new_tool_version:
             self.service_tool_version = new_tool_version
             self.session.headers.update({'service_tool_version': self.service_tool_version})
             self.headers.update({'service_tool_version': self.service_tool_version})
 
         data = dict(task=task.as_primitives(), result=result, freshen=True)
         try:
-            r = self.request_with_retries('post', self._path('task'), json=data)
+            r = self.request_with_retries('post', self._path('task'), json=data, timeout=TASK_REQUEST_TIMEOUT)
 
             if not r['success'] and r['missing_files']:
                 while not r['success'] and r['missing_files']:
                     for f_sha256 in r['missing_files']:
                         file_info = result_files[f_sha256]
                         headers = dict(
                             sha256=file_info['sha256'],
@@ -433,18 +435,19 @@
                             ttl=str(task.ttl),
                             is_section_image=str(file_info.get('is_section_image', False))
                         )
 
                         with open(file_info['path'], 'rb') as fh:
                             # Upload the file requested by service server
                             self.log.info(f"[{task.sid}] Uploading file {file_info['path']} [{file_info['sha256']}]")
-                            self.request_with_retries('put', self._path('file'), files=dict(file=fh), headers=headers)
+                            self.request_with_retries('put', self._path('file'), files=dict(file=fh), headers=headers,
+                                                      timeout=FILE_REQUEST_TIMEOUT)
 
                     data['freshen'] = False
-                    r = self.request_with_retries('post', self._path('task'), json=data)
+                    r = self.request_with_retries('post', self._path('task'), json=data, timeout=TASK_REQUEST_TIMEOUT)
         except (ServiceServerException, requests.HTTPError) as e:
             self.handle_task_error(task, message=str(e), error_type='EXCEPTION', status='FAIL_NONRECOVERABLE')
 
     def handle_task_error(self, task: ServiceTask, error_json_path: Optional[str] = None,
                           message=None, error_type=None, status=None):
         if task is None:
             return
@@ -469,15 +472,15 @@
             try:
                 with open(error_json_path, 'r') as f:
                     error = json.load(f)
             except (IOError, JSONDecodeError, OSError):
                 self.log.exception(f"[{task.sid}] An error occurred while loading service error file.")
 
         data = dict(task=task.as_primitives(), error=error)
-        self.request_with_retries('post', self._path('task'), json=data)
+        self.request_with_retries('post', self._path('task'), json=data, timeout=TASK_REQUEST_TIMEOUT)
 
     def stop(self):
         if self.status == STATUSES.WAITING_FOR_TASK:
             # A task request was sent and a task might be received, so shutdown after giving service time to process it
             self._shutdown_timeout = TASK_REQUEST_TIMEOUT + self.service.timeout
         elif self.status != STATUSES.INITIALIZING:
             # A task is currently running, so wait until service timeout before doing a hard stop
```

## Comparing `assemblyline_service_client-4.5.1.dev92.dist-info/LICENCE.md` & `assemblyline_service_client-4.5.1.dev93.dist-info/LICENCE.md`

 * *Files identical despite different names*

## Comparing `assemblyline_service_client-4.5.1.dev92.dist-info/METADATA` & `assemblyline_service_client-4.5.1.dev93.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline-service-client
-Version: 4.5.1.dev92
+Version: 4.5.1.dev93
 Summary: Assemblyline 4 - Service client
 Home-page: https://github.com/CybercentreCanada/assemblyline-service-client/
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Classifier: Development Status :: 5 - Production/Stable
```

