# Comparing `tmp/assemblyline_service_client-4.5.1.dev93-py3-none-any.whl.zip` & `tmp/assemblyline_service_client-4.5.1.dev94-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9660 bytes, number of entries: 8
--rw-r--r--  2.0 unx       12 b- defN 24-Apr-18 15:19 assemblyline_service_client/VERSION
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 15:19 assemblyline_service_client/__init__.py
--rw-r--r--  2.0 unx    22907 b- defN 24-Apr-18 15:19 assemblyline_service_client/task_handler.py
--rw-r--r--  2.0 unx     1396 b- defN 24-Apr-18 15:20 assemblyline_service_client-4.5.1.dev93.dist-info/LICENCE.md
--rw-r--r--  2.0 unx     1577 b- defN 24-Apr-18 15:20 assemblyline_service_client-4.5.1.dev93.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-18 15:20 assemblyline_service_client-4.5.1.dev93.dist-info/WHEEL
--rw-r--r--  2.0 unx       28 b- defN 24-Apr-18 15:20 assemblyline_service_client-4.5.1.dev93.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      803 b- defN 24-Apr-18 15:20 assemblyline_service_client-4.5.1.dev93.dist-info/RECORD
-8 files, 26815 bytes uncompressed, 8212 bytes compressed:  69.4%
+Zip file size: 9727 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       12 b- defN 24-Apr-18 15:57 assemblyline_service_client/VERSION
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 15:57 assemblyline_service_client/__init__.py
+-rw-r--r--  2.0 unx    23233 b- defN 24-Apr-18 15:57 assemblyline_service_client/task_handler.py
+-rw-r--r--  2.0 unx     1396 b- defN 24-Apr-18 15:57 assemblyline_service_client-4.5.1.dev94.dist-info/LICENCE.md
+-rw-r--r--  2.0 unx     1577 b- defN 24-Apr-18 15:57 assemblyline_service_client-4.5.1.dev94.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-18 15:57 assemblyline_service_client-4.5.1.dev94.dist-info/WHEEL
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-18 15:57 assemblyline_service_client-4.5.1.dev94.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      803 b- defN 24-Apr-18 15:57 assemblyline_service_client-4.5.1.dev94.dist-info/RECORD
+8 files, 27141 bytes uncompressed, 8279 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: assemblyline_service_client/__init__.py
 Comment: 
 
 Filename: assemblyline_service_client/task_handler.py
 Comment: 
 
-Filename: assemblyline_service_client-4.5.1.dev93.dist-info/LICENCE.md
+Filename: assemblyline_service_client-4.5.1.dev94.dist-info/LICENCE.md
 Comment: 
 
-Filename: assemblyline_service_client-4.5.1.dev93.dist-info/METADATA
+Filename: assemblyline_service_client-4.5.1.dev94.dist-info/METADATA
 Comment: 
 
-Filename: assemblyline_service_client-4.5.1.dev93.dist-info/WHEEL
+Filename: assemblyline_service_client-4.5.1.dev94.dist-info/WHEEL
 Comment: 
 
-Filename: assemblyline_service_client-4.5.1.dev93.dist-info/top_level.txt
+Filename: assemblyline_service_client-4.5.1.dev94.dist-info/top_level.txt
 Comment: 
 
-Filename: assemblyline_service_client-4.5.1.dev93.dist-info/RECORD
+Filename: assemblyline_service_client-4.5.1.dev94.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## assemblyline_service_client/VERSION

```diff
@@ -1 +1 @@
-4.5.1.dev93
+4.5.1.dev94
```

## assemblyline_service_client/task_handler.py

```diff
@@ -435,16 +435,21 @@
                             ttl=str(task.ttl),
                             is_section_image=str(file_info.get('is_section_image', False))
                         )
 
                         with open(file_info['path'], 'rb') as fh:
                             # Upload the file requested by service server
                             self.log.info(f"[{task.sid}] Uploading file {file_info['path']} [{file_info['sha256']}]")
-                            self.request_with_retries('put', self._path('file'), files=dict(file=fh), headers=headers,
-                                                      timeout=FILE_REQUEST_TIMEOUT)
+                            try:
+                                self.request_with_retries('put', self._path('file'), files=dict(file=fh),
+                                                          headers=headers,timeout=FILE_REQUEST_TIMEOUT)
+                            except ServiceServerException as e:
+                                if "does not match expected file hash" in str(e):
+                                    self.log.warning(f"File upload of '{file_info['path']}' failed.")
+                                raise
 
                     data['freshen'] = False
                     r = self.request_with_retries('post', self._path('task'), json=data, timeout=TASK_REQUEST_TIMEOUT)
         except (ServiceServerException, requests.HTTPError) as e:
             self.handle_task_error(task, message=str(e), error_type='EXCEPTION', status='FAIL_NONRECOVERABLE')
 
     def handle_task_error(self, task: ServiceTask, error_json_path: Optional[str] = None,
```

## Comparing `assemblyline_service_client-4.5.1.dev93.dist-info/LICENCE.md` & `assemblyline_service_client-4.5.1.dev94.dist-info/LICENCE.md`

 * *Files identical despite different names*

## Comparing `assemblyline_service_client-4.5.1.dev93.dist-info/METADATA` & `assemblyline_service_client-4.5.1.dev94.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline-service-client
-Version: 4.5.1.dev93
+Version: 4.5.1.dev94
 Summary: Assemblyline 4 - Service client
 Home-page: https://github.com/CybercentreCanada/assemblyline-service-client/
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `assemblyline_service_client-4.5.1.dev93.dist-info/RECORD` & `assemblyline_service_client-4.5.1.dev94.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-assemblyline_service_client/VERSION,sha256=G9pBMQfRxZ-eeKDX_TxdkLhDvwbvQLuRw3bfiEq6Zo8,12
+assemblyline_service_client/VERSION,sha256=Q8x9DlxKf8FOY8Q5vV_cD68TuE8Yhnvdqry611XBSqY,12
 assemblyline_service_client/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-assemblyline_service_client/task_handler.py,sha256=uJuYbd5tU1DlJXy7f0CjL0912x-Mvw1U4rOB2IiIV48,22907
-assemblyline_service_client-4.5.1.dev93.dist-info/LICENCE.md,sha256=NSkYo9EH8h5oOkzg4VhjAHF4339MqPP2cQ8msTPgl-c,1396
-assemblyline_service_client-4.5.1.dev93.dist-info/METADATA,sha256=ILHXAMHYhKPxUClL6Xl28hWl_9Oll6C5ntyuOCtoXNM,1577
-assemblyline_service_client-4.5.1.dev93.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-assemblyline_service_client-4.5.1.dev93.dist-info/top_level.txt,sha256=clNWHvn8nw0kR15l5TASxWxIQvKGKe5Pso3kVPMiJv0,28
-assemblyline_service_client-4.5.1.dev93.dist-info/RECORD,,
+assemblyline_service_client/task_handler.py,sha256=U6OmqDSbBY9p-JccwdFImZ436McK_PK-A5Pl6d54Kko,23233
+assemblyline_service_client-4.5.1.dev94.dist-info/LICENCE.md,sha256=NSkYo9EH8h5oOkzg4VhjAHF4339MqPP2cQ8msTPgl-c,1396
+assemblyline_service_client-4.5.1.dev94.dist-info/METADATA,sha256=opjQGjjr54fCy60NrNSmkezSsj3N6E06RpVimDIqGHI,1577
+assemblyline_service_client-4.5.1.dev94.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+assemblyline_service_client-4.5.1.dev94.dist-info/top_level.txt,sha256=clNWHvn8nw0kR15l5TASxWxIQvKGKe5Pso3kVPMiJv0,28
+assemblyline_service_client-4.5.1.dev94.dist-info/RECORD,,
```

