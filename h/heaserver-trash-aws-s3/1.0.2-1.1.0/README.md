# Comparing `tmp/heaserver-trash-aws-s3-1.0.2.tar.gz` & `tmp/heaserver_trash_aws_s3-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-trash-aws-s3-1.0.2.tar", last modified: Fri Mar 22 02:56:15 2024, max compression
+gzip compressed data, was "heaserver_trash_aws_s3-1.1.0.tar", last modified: Thu Apr 18 15:25:00 2024, max compression
```

## Comparing `heaserver-trash-aws-s3-1.0.2.tar` & `heaserver_trash_aws_s3-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 02:56:15.618853 heaserver-trash-aws-s3-1.0.2/
--rw-rw-rw-   0        0        0    11625 2023-12-18 21:53:00.000000 heaserver-trash-aws-s3-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       39 2023-12-18 21:53:00.000000 heaserver-trash-aws-s3-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4369 2024-03-22 02:56:15.617853 heaserver-trash-aws-s3-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3000 2024-03-22 02:54:44.000000 heaserver-trash-aws-s3-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-03-22 02:56:15.618853 heaserver-trash-aws-s3-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1947 2024-03-22 02:55:19.000000 heaserver-trash-aws-s3-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-22 02:56:15.548437 heaserver-trash-aws-s3-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-03-22 02:56:15.547416 heaserver-trash-aws-s3-1.0.2/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-22 02:56:15.570990 heaserver-trash-aws-s3-1.0.2/src/heaserver/trashawss3/
--rw-rw-rw-   0        0        0        0 2023-12-18 21:53:00.000000 heaserver-trash-aws-s3-1.0.2/src/heaserver/trashawss3/__init__.py
--rw-rw-rw-   0        0        0    52812 2024-01-04 21:08:31.000000 heaserver-trash-aws-s3-1.0.2/src/heaserver/trashawss3/service.py
-drwxrwxrwx   0        0        0        0 2024-03-22 02:56:15.577927 heaserver-trash-aws-s3-1.0.2/src/heaserver/trashawss3/wstl/
--rw-rw-rw-   0        0        0     7629 2023-12-18 21:53:00.000000 heaserver-trash-aws-s3-1.0.2/src/heaserver/trashawss3/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-03-22 02:56:15.609678 heaserver-trash-aws-s3-1.0.2/src/heaserver_trash_aws_s3.egg-info/
--rw-rw-rw-   0        0        0     4369 2024-03-22 02:56:15.000000 heaserver-trash-aws-s3-1.0.2/src/heaserver_trash_aws_s3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      581 2024-03-22 02:56:15.000000 heaserver-trash-aws-s3-1.0.2/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 02:56:15.000000 heaserver-trash-aws-s3-1.0.2/src/heaserver_trash_aws_s3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2024-03-22 02:56:15.000000 heaserver-trash-aws-s3-1.0.2/src/heaserver_trash_aws_s3.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2024-03-22 02:56:15.000000 heaserver-trash-aws-s3-1.0.2/src/heaserver_trash_aws_s3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-22 02:56:15.000000 heaserver-trash-aws-s3-1.0.2/src/heaserver_trash_aws_s3.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-22 02:56:15.549457 heaserver-trash-aws-s3-1.0.2/tests/
-drwxrwxrwx   0        0        0        0 2024-03-22 02:56:15.549457 heaserver-trash-aws-s3-1.0.2/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-22 02:56:15.609678 heaserver-trash-aws-s3-1.0.2/tests/heaserver/trashawss3test/
--rw-rw-rw-   0        0        0        0 2023-12-18 21:53:00.000000 heaserver-trash-aws-s3-1.0.2/tests/heaserver/trashawss3test/__init__.py
--rw-rw-rw-   0        0        0    69457 2024-03-21 22:53:21.000000 heaserver-trash-aws-s3-1.0.2/tests/heaserver/trashawss3test/test_all.py
--rw-rw-rw-   0        0        0     6372 2023-12-18 21:53:00.000000 heaserver-trash-aws-s3-1.0.2/tests/heaserver/trashawss3test/testcase.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:25:00.276015 heaserver_trash_aws_s3-1.1.0/
+-rw-rw-rw-   0        0        0    11625 2023-12-18 21:53:00.000000 heaserver_trash_aws_s3-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       39 2023-12-18 21:53:00.000000 heaserver_trash_aws_s3-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4561 2024-04-18 15:25:00.275016 heaserver_trash_aws_s3-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3192 2024-04-18 15:20:46.000000 heaserver_trash_aws_s3-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-18 15:25:00.276015 heaserver_trash_aws_s3-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1947 2024-04-18 15:24:23.000000 heaserver_trash_aws_s3-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:25:00.209095 heaserver_trash_aws_s3-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:25:00.209095 heaserver_trash_aws_s3-1.1.0/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:25:00.223994 heaserver_trash_aws_s3-1.1.0/src/heaserver/trashawss3/
+-rw-rw-rw-   0        0        0        0 2023-12-18 21:53:00.000000 heaserver_trash_aws_s3-1.1.0/src/heaserver/trashawss3/__init__.py
+-rw-rw-rw-   0        0        0    54229 2024-04-18 14:59:45.000000 heaserver_trash_aws_s3-1.1.0/src/heaserver/trashawss3/service.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:25:00.231566 heaserver_trash_aws_s3-1.1.0/src/heaserver/trashawss3/wstl/
+-rw-rw-rw-   0        0        0     7918 2024-04-18 04:17:27.000000 heaserver_trash_aws_s3-1.1.0/src/heaserver/trashawss3/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-04-18 15:25:00.274016 heaserver_trash_aws_s3-1.1.0/src/heaserver_trash_aws_s3.egg-info/
+-rw-rw-rw-   0        0        0     4561 2024-04-18 15:25:00.000000 heaserver_trash_aws_s3-1.1.0/src/heaserver_trash_aws_s3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2024-04-18 15:25:00.000000 heaserver_trash_aws_s3-1.1.0/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 15:25:00.000000 heaserver_trash_aws_s3-1.1.0/src/heaserver_trash_aws_s3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2024-04-18 15:25:00.000000 heaserver_trash_aws_s3-1.1.0/src/heaserver_trash_aws_s3.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2024-04-18 15:25:00.000000 heaserver_trash_aws_s3-1.1.0/src/heaserver_trash_aws_s3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-18 15:25:00.000000 heaserver_trash_aws_s3-1.1.0/src/heaserver_trash_aws_s3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 15:25:00.210094 heaserver_trash_aws_s3-1.1.0/tests/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:25:00.210094 heaserver_trash_aws_s3-1.1.0/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:25:00.271779 heaserver_trash_aws_s3-1.1.0/tests/heaserver/trashawss3test/
+-rw-rw-rw-   0        0        0        0 2023-12-18 21:53:00.000000 heaserver_trash_aws_s3-1.1.0/tests/heaserver/trashawss3test/__init__.py
+-rw-rw-rw-   0        0        0    73394 2024-04-18 14:58:21.000000 heaserver_trash_aws_s3-1.1.0/tests/heaserver/trashawss3test/test_all.py
+-rw-rw-rw-   0        0        0     6372 2023-12-18 21:53:00.000000 heaserver_trash_aws_s3-1.1.0/tests/heaserver/trashawss3test/testcase.py
```

### Comparing `heaserver-trash-aws-s3-1.0.2/LICENSE` & `heaserver_trash_aws_s3-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.2/PKG-INFO` & `heaserver_trash_aws_s3-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-trash-aws-s3
-Version: 1.0.2
+Version: 1.1.0
 Summary: Deleted file management
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-trash-aws-s3,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -21,23 +21,28 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.0.8
+Requires-Dist: heaserver~=1.4.1
 Requires-Dist: aiostream~=0.5.1
 
 # HEA Trash Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Trash Microservice is deleted file management.
 
+## Version 1.1.0
+* Added "deleted" date to trash items from their delete marker
+* Return permissions in Collection+JSON objects.
+* Added type_display_name attribute to returned objects.
+
 ## Version 1.0.2
 * Performance improvements.
 
 ## Version 1.0.1
 * Performance improvements.
 
 ## Version 1
```

### Comparing `heaserver-trash-aws-s3-1.0.2/README.md` & `heaserver_trash_aws_s3-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # HEA Trash Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Trash Microservice is deleted file management.
 
+## Version 1.1.0
+* Added "deleted" date to trash items from their delete marker
+* Return permissions in Collection+JSON objects.
+* Added type_display_name attribute to returned objects.
+
 ## Version 1.0.2
 * Performance improvements.
 
 ## Version 1.0.1
 * Performance improvements.
 
 ## Version 1
```

### Comparing `heaserver-trash-aws-s3-1.0.2/setup.py` & `heaserver_trash_aws_s3-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-trash-aws-s3',
-    version='1.0.2',
+    version='1.1.0',
     description="Deleted file management",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
       python_requires='>=3.10',
       package_dir={'': 'src'},
       packages=['heaserver.trashawss3'],
       package_data={'heaserver.trashawss3': ['wstl/*.json']},
       install_requires=[
-          'heaserver~=1.0.8',
+          'heaserver~=1.4.1',
           'aiostream~=0.5.1'
       ],
       classifiers=[
           'Development Status :: 5 - Production/Stable',
           'Environment :: Console',
           'Intended Audience :: Developers',
           'Natural Language :: English',
```

### Comparing `heaserver-trash-aws-s3-1.0.2/src/heaserver/trashawss3/service.py` & `heaserver_trash_aws_s3-1.1.0/src/heaserver/trashawss3/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,20 @@
         - $ref: '#/components/parameters/id'
     responses:
       '200':
         $ref: '#/components/responses/200'
       '404':
         $ref: '#/components/responses/404'
     """
-    return await response.get(request, await _get_deleted_item(request))
+    sub = request.headers.get(SUB, NONE_USER)
+    result = await _get_deleted_item(request)
+    if result is None:
+        return await response.get(request, None)
+    else:
+        return await response.get(request, result.to_dict(), permissions=result.get_permissions(sub))
 
 
 @routes.get('/volumes/{volume_id}/buckets/{bucket_id}/awss3trashfolders/{trash_folder_id}/items/')
 @routes.get('/volumes/{volume_id}/buckets/{bucket_id}/awss3trashfolders/{trash_folder_id}/items')
 @action(name='heaserver-awss3trash-item-get-open-choices',
         rel='hea-opener-choices hea-context-menu',
         path='volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}/opener',
@@ -297,15 +302,19 @@
               value: root
     responses:
       '200':
         $ref: '#/components/responses/200'
       '404':
         $ref: '#/components/responses/404'
     """
-    return await response.get_all(request, [i async for i in _get_deleted_items(request, recursive=False)])
+    sub = request.headers.get(SUB, NONE_USER)
+    result: list[AWSS3FolderFileTrashItem] = []
+    async for i in _get_deleted_items(request, recursive=False):
+        result.append(i)
+    return await response.get_all(request, tuple(r.to_dict() for r in result), permissions=tuple(r.get_permissions(sub) for r in result))
 
 
 @routes.get('/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{folder_id}/awss3trash/')
 @routes.get('/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{folder_id}/awss3trash')
 @action(name='heaserver-awss3trash-item-get-open-choices',
         rel='hea-opener-choices hea-context-menu',
         path='volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}/opener',
@@ -365,15 +374,19 @@
               value: root
     responses:
       '200':
         $ref: '#/components/responses/200'
       '404':
         $ref: '#/components/responses/404'
     """
-    return await response.get_all(request, [i async for i in _get_deleted_items(request, recursive=False)])
+    sub = request.headers.get(SUB, NONE_USER)
+    result: list[AWSS3FolderFileTrashItem] = []
+    async for i in _get_deleted_items(request, recursive=False):
+        result.append(i)
+    return await response.get_all(request, tuple(r.to_dict() for r in result), permissions=tuple(r.get_permissions(sub) for r in result))
 
 
 @routes.get('/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/')
 @routes.get('/volumes/{volume_id}/buckets/{bucket_id}/awss3trash')
 @action(name='heaserver-awss3trash-item-get-open-choices',
         rel='hea-opener-choices hea-context-menu',
         path='volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}/opener',
@@ -427,15 +440,19 @@
         $ref: '#/components/responses/200'
       '404':
         $ref: '#/components/responses/404'
     """
     logger = logging.getLogger(__name__)
     sub = request.headers.get(SUB, NONE_USER)
     async def coro():
-        return await response.get_all(request, [i async for i in _get_deleted_items(request)])
+        result: list[AWSS3FolderFileTrashItem] = []
+        async for i in _get_deleted_items(request):
+            result.append(i)
+        return await response.get_all(request, tuple(r.to_dict() for r in result),
+                                      permissions=tuple(r.get_permissions(sub) for r in result))
     async_requested = PREFERENCE_RESPOND_ASYNC in request.headers.get(PREFER, [])
     if async_requested:
         logger.debug('Asynchronous get all trash')
         global _status_id
         status_location = f'{str(request.url).rstrip("/")}asyncstatus{_status_id}'
         _status_id += 1
         task_name = f'{sub}^{status_location}'
@@ -499,27 +516,28 @@
         volume_id = request.match_info['volume_id']
     except KeyError as e:
         return response.status_bad_request(str(e))
     s3: S3Client = await request.app[HEA_DB].get_client(request, 's3', volume_id)
     loop = asyncio.get_running_loop()
     resp_ = await loop.run_in_executor(None, s3.list_buckets)
 
-    async def coro():
-        asyncgens: list[AsyncGenerator[DesktopObjectDict, None]] = []
+    async def coro() -> web.Response:
+        asyncgens: list[AsyncGenerator[AWSS3FolderFileTrashItem, None]] = []
         try:
             for bucket in resp_.get('Buckets', []):
-                async def asyncgen(volume_id: str, bucket_id: str, sub: str | None) -> AsyncGenerator[DesktopObjectDict, None]:
+                async def asyncgen(volume_id: str, bucket_id: str, sub: str | None) -> AsyncGenerator[AWSS3FolderFileTrashItem, None]:
                     async for item in _get_deleted_items_private(s3, volume_id, bucket_id, None, sub):
                         yield item
                 asyncgens.append(asyncgen(request.match_info['volume_id'], bucket['Name'], request.headers.get(SUB)))
             async with stream.merge(*asyncgens).stream() as streamer:
-                result: list[DesktopObjectDict] = []
+                result: list[AWSS3FolderFileTrashItem] = []
                 async for item in streamer:
                     result.append(item)
-                return await response.get_all(request, result)
+                return await response.get_all(request, tuple(r.to_dict() for r in result),
+                                              permissions=tuple(r.get_permissions(sub) for r in result))
         except ValueError as e:
             return response.status_forbidden(str(e))
     async_requested = PREFERENCE_RESPOND_ASYNC in request.headers.get(PREFER, [])
     if async_requested:
         logger.debug('Asynchronous get all trash')
         global _status_id
         status_location = f'{str(request.url).rstrip("/")}asyncstatus{_status_id}'
@@ -744,15 +762,20 @@
         - $ref: '#/components/parameters/id'
     responses:
       '300':
         $ref: '#/components/responses/300'
       '404':
         $ref: '#/components/responses/404'
     """
-    return await response.get_multiple_choices(request, await _get_deleted_item(request))
+    sub = request.headers.get(SUB, NONE_USER)
+    result = await _get_deleted_item(request)
+    if result is None:
+        return await response.get_multiple_choices(request, None)
+    else:
+        return await response.get_multiple_choices(request, result.to_dict(), permissions=result.get_permissions(sub))
 
 
 def main() -> None:
     config = init_cmd_line(description='Deleted file management',
                            default_port=8080)
     start(package_name='heaserver-trash-aws-s3', db=S3Manager,
           wstl_builder_factory=builder_factory(__package__), config=config)
@@ -772,15 +795,15 @@
         for page in await loop_.run_in_executor(None, paginate_partial):
             yield page
     except ClientError as e:
         raise awsservicelib.handle_client_error(e)
 
 
 
-async def _get_deleted_item(request: web.Request) -> DesktopObjectDict | None:
+async def _get_deleted_item(request: web.Request) -> AWSS3FolderFileTrashItem | None:
     try:
         volume_id = request.match_info['volume_id']
         bucket_id = request.match_info['bucket_id']
     except KeyError as e:
         raise response.status_bad_request(str(e))
     try:
         item = AWSS3FolderFileTrashItem()
@@ -790,15 +813,15 @@
     except ValueError as e:
         return None
     async for deleted_item in _get_deleted_items_private(s3, volume_id, bucket_id, key_, request.headers.get(SUB), version=item.version, recursive=False):
         return deleted_item
     return None
 
 
-async def _get_deleted_items(request: web.Request, recursive=True) -> AsyncIterator[DesktopObjectDict]:
+async def _get_deleted_items(request: web.Request, recursive=True) -> AsyncIterator[AWSS3FolderFileTrashItem]:
     """
     Gets all deleted items (with a delete marker) in a volume and bucket.
     The request's match_info is expected to have volume_id and bucket_id keys
     containing the volume id and bucket name, respectively. It can optionally
     contain a folder_id or trash_folder_id, which will restrict returned items
     to a folder or trash folder, respectively.
 
@@ -833,22 +856,21 @@
         s3 = await request.app[HEA_DB].get_client(request, 's3', volume_id)
     except ValueError:
         raise response.status_not_found()
 
     async for item in _get_deleted_items_private(s3, volume_id, bucket_id, prefix, request.headers.get(SUB), recursive=recursive):
         yield item
 
-
 #count = 0
-def _process_resp(volume_id: str, bucket_id: str, sub_user: str | None, version: str | None, recursive: bool, response_):
+def _process_resp(volume_id: str, bucket_id: str, sub_user: str | None, version: str | None, recursive: bool, response_) -> list[AWSS3FolderFileTrashItem]:
     logger = logging.getLogger(__name__)
     # count += len(response_.get('Versions', []))
     # if count > MAX_VERSIONS_TO_RETRIEVE:
     #     raise ValueError(f'The bucket {bucket_id} has too many objects to display the trash!')
-    result = []
+    result: list[AWSS3FolderFileTrashItem] = []
     def truncate(key: str):
         try:
             return key[:key.index('/') + 1]
         except ValueError:
             return key
     if not recursive:
         truncated_key_dict: dict[str, AWSS3FolderFileTrashItem] = {}
@@ -867,53 +889,55 @@
                     (version is None or version == vers['VersionId']) and
                     vers['Key'] in dms)
     non_null_versions = version_iter(response_, delete_markers)
     for key, versions in itertools.groupby(non_null_versions, itemgetter('Key')):
         if not recursive:
             if key not in truncated_key_dict.keys():
                 for item in truncated_key_dict.values():
-                    result.append(item.to_dict())
+                    result.append(item)
                 truncated_key_dict.clear()
         # Versions are returned by S3 in the order in which they are stored, with the most recently stored returned
         # first.
         version_ = next(v for v in versions if v['LastModified'] < delete_markers[key])
         logger.debug('Version response for key %s and version %s', key, version_)
         if version_:
+            deleted = delete_markers[key]
             key = key if recursive else truncate(key)
             encoded_key = encode_key(key)
             last_modified = version_['LastModified']
             storage_class = version_['StorageClass']
             size = version_['Size']
             if recursive:
                 item = AWSS3FolderFileTrashItem()
             else:
                 item = truncated_key_dict.setdefault(key, AWSS3FolderFileTrashItem())
             item.bucket_id = bucket_id
             item.key = key
             item.version = version_['VersionId']
             item.modified = last_modified if recursive else max(item.modified or timezone_aware_min, last_modified)
             item.created = last_modified if recursive else max(item.modified or timezone_aware_min, last_modified)
+            item.deleted = deleted
             item.owner = (sub_user if sub_user is not None else NONE_USER) if recursive else None
             item.volume_id = volume_id
             item.source = AWS_S3
             item.storage_class = storage_class if recursive else None
             item.size = size if recursive else (item.size or 0) + size
             item.actual_object_type_name = AWSS3Folder.get_type_name() \
                 if is_folder(key) else AWSS3FileObject.get_type_name()
             if is_folder(key):
                 item.actual_object_uri = str(
                     URL('volumes') / volume_id / 'buckets' / bucket_id / 'awss3folders' / encoded_key)
             else:
                 item.actual_object_uri = str(
                     URL('volumes') / volume_id / 'buckets' / bucket_id / 'awss3files' / encoded_key)
             if recursive:
-                result.append(item.to_dict())
+                result.append(item)
     if not recursive:
         for item in truncated_key_dict.values():
-            result.append(item.to_dict())
+            result.append(item)
     return result
 
 
 from collections.abc import Callable
 from typing import TypeVar
 T = TypeVar('T')
 U = TypeVar('U')
@@ -972,25 +996,25 @@
                 for r_ in result_:
                     yield r_
         if exceptions_to_raise:
             raise exceptions_to_raise[0]
 
 
 async def _get_deleted_items_private(s3: S3Client, volume_id: str, bucket_id: str, prefix: str | None = None,
-                                       sub_user: str | None = None, version: str | None = None, recursive=True) -> AsyncGenerator[DesktopObjectDict, None]:
+                                       sub_user: str | None = None, version: str | None = None, recursive=True) -> AsyncGenerator[AWSS3FolderFileTrashItem, None]:
     logger = logging.getLogger(__name__)
     loop_ = asyncio.get_running_loop()
     cpu_count = os.cpu_count()
     max_workers = int((cpu_count if cpu_count else 2) / 2)
     with ProcessPoolExecutor(max_workers=max_workers) as pool:
-        async def producer() -> AsyncGenerator[asyncio.Future[list[DesktopObjectDict]], None]:
+        async def producer() -> AsyncGenerator[asyncio.Future[list[AWSS3FolderFileTrashItem]], None]:
             async for response_ in _get_version_objects(s3, bucket_id, prefix if prefix else '', loop_):
                 yield loop_.run_in_executor(pool, _process_resp, volume_id, bucket_id, sub_user, version, recursive, response_)
 
-        async def consumer(item: asyncio.Future[list[DesktopObjectDict]]) -> AsyncGenerator[DesktopObjectDict, None]:
+        async def consumer(item: asyncio.Future[list[AWSS3FolderFileTrashItem]]) -> AsyncGenerator[AWSS3FolderFileTrashItem, None]:
             await item
             for result in item.result():
                 yield result
 
         async for result in _queued_processing(producer, consumer):
             yield result
```

### Comparing `heaserver-trash-aws-s3-1.0.2/src/heaserver/trashawss3/wstl/all.json` & `heaserver_trash_aws_s3-1.1.0/src/heaserver/trashawss3/wstl/all.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999416433239963%*

 * *Differences: {"'wstl'": "{'actions': {8: {'inputs': {insert: [(13, OrderedDict([('name', 'deleted'), ('prompt', "*

 * *           "'Deleted'), ('readOnly', True), ('hea', OrderedDict([('type', 'datetime')]))]))]}}}}"}*

```diff
@@ -148,14 +148,22 @@
                             "type": "datetime"
                         },
                         "name": "modified",
                         "prompt": "Modified",
                         "readOnly": true
                     },
                     {
+                        "hea": {
+                            "type": "datetime"
+                        },
+                        "name": "deleted",
+                        "prompt": "Deleted",
+                        "readOnly": true
+                    },
+                    {
                         "name": "source",
                         "prompt": "Source",
                         "readOnly": true
                     },
                     {
                         "hea": {
                             "optionsFromUrl": {
```

### Comparing `heaserver-trash-aws-s3-1.0.2/src/heaserver_trash_aws_s3.egg-info/PKG-INFO` & `heaserver_trash_aws_s3-1.1.0/src/heaserver_trash_aws_s3.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-trash-aws-s3
-Version: 1.0.2
+Version: 1.1.0
 Summary: Deleted file management
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-trash-aws-s3,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -21,23 +21,28 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.0.8
+Requires-Dist: heaserver~=1.4.1
 Requires-Dist: aiostream~=0.5.1
 
 # HEA Trash Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Trash Microservice is deleted file management.
 
+## Version 1.1.0
+* Added "deleted" date to trash items from their delete marker
+* Return permissions in Collection+JSON objects.
+* Added type_display_name attribute to returned objects.
+
 ## Version 1.0.2
 * Performance improvements.
 
 ## Version 1.0.1
 * Performance improvements.
 
 ## Version 1
```

### Comparing `heaserver-trash-aws-s3-1.0.2/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt` & `heaserver_trash_aws_s3-1.1.0/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.2/tests/heaserver/trashawss3test/test_all.py` & `heaserver_trash_aws_s3-1.1.0/tests/heaserver/trashawss3test/test_all.py`

 * *Files 12% similar despite different names*

```diff
@@ -70,14 +70,15 @@
         async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}') as resp:
             self.assertEqual(200, resp.status)
 
     async def test_get_deleted_item(self):
         async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA==%2C{self.__version1}') as resp:
             actual = [{'collection': {'version': '1.0',
                                       'href': f'http://127.0.0.1:{resp.url.port}/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA==,{self.__version1}',
+                                      'permissions': [['CHECK_DYNAMIC', 'COOWNER', 'CREATOR', 'DELETER', 'EDITOR', 'SHARER', 'VIEWER']],
                                       'items': [
                                         {'data': [
                                             {'name': 'actual_object_id', 'value': 'VGV4dEZpbGVVVEY4LnR4dA==', 'prompt': 'actual_object_id', 'display': True},
                                             {'name': 'actual_object_type_name', 'value': 'heaobject.data.AWSS3FileObject', 'prompt': 'actual_object_type_name', 'display': True},
                                             {'name': 'actual_object_uri', 'value': 'volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3files/VGV4dEZpbGVVVEY4LnR4dA==', 'prompt': 'actual_object_uri', 'display': True},
                                             {'name': 'bucket_id', 'value': 'arp-scale-2-cloud-bucket-with-tags11', 'prompt': 'bucket_id', 'display': True},
                                             {'name': 'created', 'value': '2022-05-17T00:00:00+00:00', 'prompt': 'created', 'display': True}, {'name': 'derived_by', 'value': None, 'prompt': 'derived_by', 'display': True},
@@ -86,24 +87,26 @@
                                             {'name': 'display_name', 'value': 'TextFileUTF8.txt', 'prompt': 'display_name', 'display': True},
                                             {'name': 'human_readable_original_location', 'value': '/arp-scale-2-cloud-bucket-with-tags11/TextFileUTF8.txt', 'prompt': 'human_readable_original_location', 'display': True},
                                             {'name': 'human_readable_size', 'value': '0 Bytes', 'prompt': 'human_readable_size', 'display': True},
                                             {'name': 'id', 'value': f'VGV4dEZpbGVVVEY4LnR4dA==,{self.__version1}', 'prompt': 'id', 'display': False},
                                             {'name': 'invites', 'value': [], 'prompt': 'invites', 'display': True},
                                             {'name': 'key', 'value': 'TextFileUTF8.txt', 'prompt': 'key', 'display': True},
                                             {'name': 'modified', 'value': '2022-05-17T00:00:00+00:00', 'prompt': 'modified', 'display': True},
+                                            {'name': 'deleted', 'value': '2022-05-18T00:00:00+00:00', 'prompt': 'deleted', 'display': True},
                                             {'name': 'name', 'value': f'VGV4dEZpbGVVVEY4LnR4dA==,{self.__version1}', 'prompt': 'name', 'display': True},
                                             {'name': 'original_location', 'value': '/arp-scale-2-cloud-bucket-with-tags11/TextFileUTF8.txt', 'prompt': 'original_location', 'display': True},
                                             {'name': 'owner', 'value': 'system|none', 'prompt': 'owner', 'display': True},
                                             {'name': 's3_uri', 'value': 's3://arp-scale-2-cloud-bucket-with-tags11/TextFileUTF8.txt', 'prompt': 's3_uri', 'display': True},
                                             {'name': 'shares', 'value': [], 'prompt': 'shares', 'display': True},
                                             {'name': 'size', 'value': 0, 'prompt': 'size', 'display': True},
                                             {'name': 'source', 'value': 'AWS S3', 'prompt': 'source', 'display': True},
                                             {'name': 'source_detail', 'value': None, 'prompt': 'source_detail', 'display': True},
                                             {'name': 'storage_class', 'value': None, 'prompt': 'storage_class', 'display': True},
                                             {'name': 'type', 'value': 'heaobject.trash.AWSS3FolderFileTrashItem', 'prompt': 'type', 'display': True},
+                                            {'name': 'type_display_name', 'value': 'Trash Item', 'prompt': 'type_display_name', 'display': True},
                                             {'name': 'version', 'value': self.__version1, 'prompt': 'version', 'display': True},
                                             {'name': 'volume_id', 'value': '666f6f2d6261722d71757578', 'prompt': 'volume_id', 'display': True}],
                                           'links': [
                                             {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/restorer'},
                                             {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/deleter'},
                                             {'prompt': 'View', 'rel': 'self', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}'},
                                             {'prompt': 'View volume', 'rel': 'hea-volume', 'href': '/volumes/666f6f2d6261722d71757578'},
@@ -119,14 +122,15 @@
                                                         {'name': 'human_readable_size', 'value': '0 Bytes', 'prompt': 'Size', 'required': False, 'readOnly': True, 'pattern': None},
                                                         {'name': 'storage_class', 'value': None, 'prompt': 'Storage class', 'required': False, 'readOnly': True, 'pattern': None},
                                                         {'name': 's3_uri', 'value': 's3://arp-scale-2-cloud-bucket-with-tags11/TextFileUTF8.txt', 'prompt': 'S3 URI', 'required': False, 'readOnly': True, 'pattern': None},
                                                         {'name': 'mime_type', 'value': None, 'prompt': 'MIME Type', 'required': False, 'readOnly': True, 'pattern': None},
                                                         {'name': 'owner', 'value': 'system|none', 'prompt': 'Owner', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': '/people/', 'text': 'display_name', 'value': 'id'}},
                                                         {'name': 'created', 'value': '2022-05-17T00:00:00+00:00', 'prompt': 'Created', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'datetime'},
                                                         {'name': 'modified', 'value': '2022-05-17T00:00:00+00:00', 'prompt': 'Modified', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'datetime'},
+                                                        {'name': 'deleted', 'value': '2022-05-18T00:00:00+00:00', 'prompt': 'Deleted', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'datetime'},
                                                         {'name': 'source', 'value': 'AWS S3', 'prompt': 'Source', 'required': False, 'readOnly': True, 'pattern': None},
                                                         {'section': 'shares', 'index': -1, 'sectionPrompt': 'Shares', 'name': 'user', 'value': None, 'prompt': 'User', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': '/people/', 'text': 'display_name', 'value': 'id'}},
                                                         {'section': 'shares', 'index': -1, 'name': 'permissions', 'value': None, 'prompt': 'Permissions', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'cardinality': 'multiple', 'options': [{'value': 'COOWNER', 'text': 'Co-owner'}, {'value': 'CREATOR', 'text': 'Creator'}, {'value': 'DELETER', 'text': 'Deleter'}, {'value': 'EDITOR', 'text': 'Editor'}, {'value': 'SHARER', 'text': 'Sharer'}, {'value': 'VIEWER', 'text': 'Viewer'}]}]}}}]
             self.assertEqual(_ordered(actual), _ordered(await resp.json()))
 
     async def test_get_deleted_item_nvpjson(self):
         async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA==,{self.__version1}', headers={hdrs.ACCEPT: nvpjson.MIME_TYPE}) as resp:
@@ -142,24 +146,26 @@
                        'display_name': 'TextFileUTF8.txt',
                        'human_readable_original_location': '/arp-scale-2-cloud-bucket-with-tags11/TextFileUTF8.txt',
                        'human_readable_size': '0 Bytes',
                        'id': f'VGV4dEZpbGVVVEY4LnR4dA==,{self.__version1}',
                        'invites': [],
                        'key': 'TextFileUTF8.txt',
                        'modified': '2022-05-17T00:00:00+00:00',
+                       'deleted': '2022-05-18T00:00:00+00:00',
                        'name': f'VGV4dEZpbGVVVEY4LnR4dA==,{self.__version1}',
                        'original_location': '/arp-scale-2-cloud-bucket-with-tags11/TextFileUTF8.txt',
                        'owner': 'system|none',
                        's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TextFileUTF8.txt',
                        'shares': [],
                        'size': 0,
                        'source': 'AWS S3',
                        'source_detail': None,
                        'storage_class': None,
                        'type': 'heaobject.trash.AWSS3FolderFileTrashItem',
+                       'type_display_name': 'Trash Item',
                        'version': self.__version1,
                        'volume_id': '666f6f2d6261722d71757578'}]
             self.assertEqual(actual, await resp.json())
 
     async def test_get_deleted_items_status(self):
         async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash') as resp:
             self.assertEqual(200, resp.status)
@@ -178,24 +184,26 @@
                        'display_name': 'TextFileUTF8.txt',
                        'human_readable_original_location': '/arp-scale-2-cloud-bucket-with-tags11/TextFileUTF8.txt',
                        'human_readable_size': '0 Bytes',
                        'id': f'VGV4dEZpbGVVVEY4LnR4dA==,{self.__version1}',
                        'invites': [],
                        'key': 'TextFileUTF8.txt',
                        'modified': '2022-05-17T00:00:00+00:00',
+                       'deleted': '2022-05-18T00:00:00+00:00',
                        'name': f'VGV4dEZpbGVVVEY4LnR4dA==,{self.__version1}',
                        'original_location': '/arp-scale-2-cloud-bucket-with-tags11/TextFileUTF8.txt',
                        'owner': 'system|none',
                        's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TextFileUTF8.txt',
                        'shares': [],
                        'size': 0,
                        'source': 'AWS S3',
                        'source_detail': None,
                        'storage_class': 'STANDARD',
                        'type': 'heaobject.trash.AWSS3FolderFileTrashItem',
+                       'type_display_name': 'Trash Item',
                        'version': self.__version1,
                        'volume_id': '666f6f2d6261722d71757578'},
                       {'actual_object_id': 'YWZvbGRlci9hbm90aGVyZm9sZGVyL0JpbmFyeUZpbGU=',
                        'actual_object_type_name': 'heaobject.data.AWSS3FileObject',
                        'actual_object_uri': 'volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3files/YWZvbGRlci9hbm90aGVyZm9sZGVyL0JpbmFyeUZpbGU=',
                        'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
                        'created': '2022-05-17T00:00:00+00:00',
@@ -204,32 +212,35 @@
                        'description': None,
                        'display_name': 'BinaryFile',
                        'human_readable_original_location': '/arp-scale-2-cloud-bucket-with-tags11/afolder/anotherfolder/BinaryFile',
                        'human_readable_size': '0 Bytes', 'id': f'YWZvbGRlci9hbm90aGVyZm9sZGVyL0JpbmFyeUZpbGU=,{self.__version2}',
                        'invites': [],
                        'key': 'afolder/anotherfolder/BinaryFile',
                        'modified': '2022-05-17T00:00:00+00:00',
+                       'deleted': '2022-05-18T00:00:00+00:00',
                        'name': f'YWZvbGRlci9hbm90aGVyZm9sZGVyL0JpbmFyeUZpbGU=,{self.__version2}',
                        'original_location': '/arp-scale-2-cloud-bucket-with-tags11/afolder/anotherfolder/BinaryFile',
                        'owner': 'system|none',
                        's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/afolder/anotherfolder/BinaryFile',
                        'shares': [],
                        'size': 0,
                        'source': 'AWS S3',
                        'source_detail': None,
                        'storage_class': 'STANDARD',
                        'type': 'heaobject.trash.AWSS3FolderFileTrashItem',
+                       'type_display_name': 'Trash Item',
                        'version': self.__version2,
                        'volume_id': '666f6f2d6261722d71757578'}]
             self.assertEqual(actual, await resp.json())
 
     async def test_get_deleted_items(self):
         async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash') as resp:
             actual = [{'collection': {'version': '1.0',
                                       'href': f'http://127.0.0.1:{resp.url.port}/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash',
+                                      'permissions': [['CHECK_DYNAMIC', 'COOWNER', 'CREATOR', 'DELETER', 'EDITOR', 'SHARER', 'VIEWER'], ['CHECK_DYNAMIC', 'COOWNER', 'CREATOR', 'DELETER', 'EDITOR', 'SHARER', 'VIEWER']],
                                       'items': [
                                           {'data': [
                                               {'name': 'actual_object_id', 'value': 'VGV4dEZpbGVVVEY4LnR4dA==', 'prompt': 'actual_object_id', 'display': True},
                                               {'name': 'actual_object_type_name', 'value': 'heaobject.data.AWSS3FileObject', 'prompt': 'actual_object_type_name', 'display': True},
                                               {'name': 'actual_object_uri', 'value': 'volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3files/VGV4dEZpbGVVVEY4LnR4dA==', 'prompt': 'actual_object_uri', 'display': True},
                                               {'name': 'bucket_id', 'value': 'arp-scale-2-cloud-bucket-with-tags11', 'prompt': 'bucket_id', 'display': True},
                                               {'name': 'created', 'value': '2022-05-17T00:00:00+00:00', 'prompt': 'created', 'display': True},
@@ -239,24 +250,26 @@
                                               {'name': 'display_name', 'value': 'TextFileUTF8.txt', 'prompt': 'display_name', 'display': True},
                                               {'name': 'human_readable_original_location', 'value': '/arp-scale-2-cloud-bucket-with-tags11/TextFileUTF8.txt', 'prompt': 'human_readable_original_location', 'display': True},
                                               {'name': 'human_readable_size', 'value': '0 Bytes', 'prompt': 'human_readable_size', 'display': True},
                                               {'name': 'id', 'value': f'VGV4dEZpbGVVVEY4LnR4dA==,{self.__version1}', 'prompt': 'id', 'display': False},
                                               {'name': 'invites', 'value': [], 'prompt': 'invites', 'display': True},
                                               {'name': 'key', 'value': 'TextFileUTF8.txt', 'prompt': 'key', 'display': True},
                                               {'name': 'modified', 'value': '2022-05-17T00:00:00+00:00', 'prompt': 'modified', 'display': True},
+                                              {'name': 'deleted', 'value': '2022-05-18T00:00:00+00:00', 'prompt': 'deleted', 'display': True},
                                               {'name': 'name', 'value': f'VGV4dEZpbGVVVEY4LnR4dA==,{self.__version1}', 'prompt': 'name', 'display': True},
                                               {'name': 'original_location', 'value': '/arp-scale-2-cloud-bucket-with-tags11/TextFileUTF8.txt', 'prompt': 'original_location', 'display': True},
                                               {'name': 'owner', 'value': 'system|none', 'prompt': 'owner', 'display': True},
                                               {'name': 's3_uri', 'value': 's3://arp-scale-2-cloud-bucket-with-tags11/TextFileUTF8.txt', 'prompt': 's3_uri', 'display': True},
                                               {'name': 'shares', 'value': [], 'prompt': 'shares', 'display': True},
                                               {'name': 'size', 'value': 0, 'prompt': 'size', 'display': True},
                                               {'name': 'source', 'value': 'AWS S3', 'prompt': 'source', 'display': True},
                                               {'name': 'source_detail', 'value': None, 'prompt': 'source_detail', 'display': True},
                                               {'name': 'storage_class', 'value': 'STANDARD', 'prompt': 'storage_class', 'display': True},
                                               {'name': 'type', 'value': 'heaobject.trash.AWSS3FolderFileTrashItem', 'prompt': 'type', 'display': True},
+                                              {'name': 'type_display_name', 'value': 'Trash Item', 'prompt': 'type_display_name', 'display': True},
                                               {'name': 'version', 'value': self.__version1, 'prompt': 'version', 'display': True},
                                               {'name': 'volume_id', 'value': '666f6f2d6261722d71757578', 'prompt': 'volume_id', 'display': True}],
                                            'links': [
                                               {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/restorer'},
                                               {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/deleter'},
                                               {'prompt': 'View', 'rel': 'self', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}'}]},
                                             {'data': [
@@ -271,23 +284,25 @@
                                               {'name': 'display_name', 'value': 'BinaryFile', 'prompt': 'display_name', 'display': True},
                                               {'name': 'human_readable_original_location', 'value': '/arp-scale-2-cloud-bucket-with-tags11/afolder/anotherfolder/BinaryFile', 'prompt': 'human_readable_original_location', 'display': True},
                                               {'name': 'human_readable_size', 'value': '0 Bytes', 'prompt': 'human_readable_size', 'display': True},
                                               {'name': 'id', 'value': f'YWZvbGRlci9hbm90aGVyZm9sZGVyL0JpbmFyeUZpbGU=,{self.__version2}', 'prompt': 'id', 'display': False},
                                               {'name': 'invites', 'value': [], 'prompt': 'invites', 'display': True},
                                               {'name': 'key', 'value': 'afolder/anotherfolder/BinaryFile', 'prompt': 'key', 'display': True},
                                               {'name': 'modified', 'value': '2022-05-17T00:00:00+00:00', 'prompt': 'modified', 'display': True},
+                                              {'name': 'deleted', 'value': '2022-05-18T00:00:00+00:00', 'prompt': 'deleted', 'display': True},
                                               {'name': 'name', 'value': f'YWZvbGRlci9hbm90aGVyZm9sZGVyL0JpbmFyeUZpbGU=,{self.__version2}', 'prompt': 'name', 'display': True},
                                               {'name': 'original_location', 'value': '/arp-scale-2-cloud-bucket-with-tags11/afolder/anotherfolder/BinaryFile', 'prompt': 'original_location', 'display': True},
                                               {'name': 'owner', 'value': 'system|none', 'prompt': 'owner', 'display': True},
                                               {'name': 's3_uri', 'value': 's3://arp-scale-2-cloud-bucket-with-tags11/afolder/anotherfolder/BinaryFile', 'prompt': 's3_uri', 'display': True},
                                               {'name': 'shares', 'value': [], 'prompt': 'shares', 'display': True}, {'name': 'size', 'value': 0, 'prompt': 'size', 'display': True},
                                               {'name': 'source', 'value': 'AWS S3', 'prompt': 'source', 'display': True},
                                               {'name': 'source_detail', 'value': None, 'prompt': 'source_detail', 'display': True},
                                               {'name': 'storage_class', 'value': 'STANDARD', 'prompt': 'storage_class', 'display': True},
                                               {'name': 'type', 'value': 'heaobject.trash.AWSS3FolderFileTrashItem', 'prompt': 'type', 'display': True},
+                                              {'name': 'type_display_name', 'value': 'Trash Item', 'prompt': 'type_display_name', 'display': True},
                                               {'name': 'version', 'value': self.__version2, 'prompt': 'version', 'display': True},
                                               {'name': 'volume_id', 'value': '666f6f2d6261722d71757578', 'prompt': 'volume_id', 'display': True}],
                                             'links': [
                                               {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci9hbm90aGVyZm9sZGVyL0JpbmFyeUZpbGU%3D%2C{self.__version2}/restorer'},
                                               {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci9hbm90aGVyZm9sZGVyL0JpbmFyeUZpbGU%3D%2C{self.__version2}/deleter'},
                                               {'prompt': 'View', 'rel': 'self', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci9hbm90aGVyZm9sZGVyL0JpbmFyeUZpbGU%3D%2C{self.__version2}'}]}],
                                       'template': {
@@ -303,14 +318,15 @@
                                             {'name': 'human_readable_size', 'value': None, 'prompt': 'Size', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'storage_class', 'value': None, 'prompt': 'Storage class', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 's3_uri', 'value': None, 'prompt': 'S3 URI', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'mime_type', 'value': None, 'prompt': 'MIME Type', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'owner', 'value': None, 'prompt': 'Owner', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': '/people/', 'text': 'display_name', 'value': 'id'}},
                                             {'name': 'created', 'value': None, 'prompt': 'Created', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'datetime'},
                                             {'name': 'modified', 'value': None, 'prompt': 'Modified', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'datetime'},
+                                            {'name': 'deleted', 'value': None, 'prompt': 'Deleted', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'datetime'},
                                             {'name': 'source', 'value': None, 'prompt': 'Source', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'section': 'shares', 'index': -1, 'sectionPrompt': 'Shares', 'name': 'user', 'value': None, 'prompt': 'User', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': '/people/', 'text': 'display_name', 'value': 'id'}},
                                             {'section': 'shares', 'index': -1, 'name': 'permissions', 'value': None, 'prompt': 'Permissions', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'cardinality': 'multiple', 'options': [{'value': 'COOWNER', 'text': 'Co-owner'}, {'value': 'CREATOR', 'text': 'Creator'}, {'value': 'DELETER', 'text': 'Deleter'}, {'value': 'EDITOR', 'text': 'Editor'}, {'value': 'SHARER', 'text': 'Sharer'}, {'value': 'VIEWER', 'text': 'Viewer'}]}]}}}]
             self.assertEqual(_ordered(actual), _ordered(await resp.json()))
 
     async def test_get_deleted_items_invalid_folder_id(self):
         async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/toor/awss3trash') as resp:
@@ -328,14 +344,15 @@
         async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/root/awss3trash') as resp:
             self.assertEqual(200, resp.status)
 
     async def test_get_deleted_items_folder(self):
         async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/root/awss3trash') as resp:
             actual = [{'collection': {'version': '1.0',
                                       'href': f'http://127.0.0.1:{resp.url.port}/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/root/awss3trash',
+                                      'permissions': [['CHECK_DYNAMIC', 'COOWNER', 'CREATOR', 'DELETER', 'EDITOR', 'SHARER', 'VIEWER'], ['CHECK_DYNAMIC', 'COOWNER', 'CREATOR', 'DELETER', 'EDITOR', 'SHARER', 'VIEWER']],
                                       'items': [
                                         {'data': [
                                             {'name': 'actual_object_id', 'value': 'VGV4dEZpbGVVVEY4LnR4dA==', 'prompt': 'actual_object_id', 'display': True},
                                             {'name': 'actual_object_type_name', 'value': 'heaobject.data.AWSS3FileObject', 'prompt': 'actual_object_type_name', 'display': True},
                                             {'name': 'actual_object_uri', 'value': 'volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3files/VGV4dEZpbGVVVEY4LnR4dA==', 'prompt': 'actual_object_uri', 'display': True},
                                             {'name': 'bucket_id', 'value': 'arp-scale-2-cloud-bucket-with-tags11', 'prompt': 'bucket_id', 'display': True},
                                             {'name': 'created', 'value': '2022-05-17T00:00:00+00:00', 'prompt': 'created', 'display': True},
@@ -344,23 +361,25 @@
                                             {'name': 'description', 'value': None, 'prompt': 'description', 'display': True},
                                             {'name': 'display_name', 'value': 'TextFileUTF8.txt', 'prompt': 'display_name', 'display': True},
                                             {'name': 'human_readable_original_location', 'value': '/arp-scale-2-cloud-bucket-with-tags11/TextFileUTF8.txt', 'prompt': 'human_readable_original_location', 'display': True},
                                             {'name': 'human_readable_size', 'value': '0 Bytes', 'prompt': 'human_readable_size', 'display': True},
                                             {'name': 'id', 'value': f'VGV4dEZpbGVVVEY4LnR4dA==,{self.__version1}', 'prompt': 'id', 'display': False},
                                             {'name': 'invites', 'value': [], 'prompt': 'invites', 'display': True}, {'name': 'key', 'value': 'TextFileUTF8.txt', 'prompt': 'key', 'display': True},
                                             {'name': 'modified', 'value': '2022-05-17T00:00:00+00:00', 'prompt': 'modified', 'display': True},
+                                            {'name': 'deleted', 'value': '2022-05-18T00:00:00+00:00', 'prompt': 'deleted', 'display': True},
                                             {'name': 'name', 'value': f'VGV4dEZpbGVVVEY4LnR4dA==,{self.__version1}', 'prompt': 'name', 'display': True},
                                             {'name': 'original_location', 'value': '/arp-scale-2-cloud-bucket-with-tags11/TextFileUTF8.txt', 'prompt': 'original_location', 'display': True},
                                             {'name': 'owner', 'value': 'system|none', 'prompt': 'owner', 'display': True},
                                             {'name': 's3_uri', 'value': 's3://arp-scale-2-cloud-bucket-with-tags11/TextFileUTF8.txt', 'prompt': 's3_uri', 'display': True},
                                             {'name': 'shares', 'value': [], 'prompt': 'shares', 'display': True}, {'name': 'size', 'value': 0, 'prompt': 'size', 'display': True},
                                             {'name': 'source', 'value': 'AWS S3', 'prompt': 'source', 'display': True},
                                             {'name': 'source_detail', 'value': None, 'prompt': 'source_detail', 'display': True},
                                             {'name': 'storage_class', 'value': None, 'prompt': 'storage_class', 'display': True},
                                             {'name': 'type', 'value': 'heaobject.trash.AWSS3FolderFileTrashItem', 'prompt': 'type', 'display': True},
+                                            {'name': 'type_display_name', 'value': 'Trash Item', 'prompt': 'type_display_name', 'display': True},
                                             {'name': 'version', 'value': self.__version1, 'prompt': 'version', 'display': True},
                                             {'name': 'volume_id', 'value': '666f6f2d6261722d71757578', 'prompt': 'volume_id', 'display': True}],
                                           'links': [
                                             {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/restorer'},
                                             {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/deleter'},
                                             {'prompt': 'View', 'rel': 'self', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}'}]},
                                         {'data': [
@@ -375,24 +394,26 @@
                                             {'name': 'display_name', 'value': 'afolder', 'prompt': 'display_name', 'display': True},
                                             {'name': 'human_readable_original_location', 'value': '/arp-scale-2-cloud-bucket-with-tags11/afolder/', 'prompt': 'human_readable_original_location', 'display': True},
                                             {'name': 'human_readable_size', 'value': '0 Bytes', 'prompt': 'human_readable_size', 'display': True},
                                             {'name': 'id', 'value': f'YWZvbGRlci8=,{self.__version2}', 'prompt': 'id', 'display': False},
                                             {'name': 'invites', 'value': [], 'prompt': 'invites', 'display': True},
                                             {'name': 'key', 'value': 'afolder/', 'prompt': 'key', 'display': True},
                                             {'name': 'modified', 'value': '2022-05-17T00:00:00+00:00', 'prompt': 'modified', 'display': True},
+                                            {'name': 'deleted', 'value': '2022-05-18T00:00:00+00:00', 'prompt': 'deleted', 'display': True},
                                             {'name': 'name', 'value': f'YWZvbGRlci8=,{self.__version2}', 'prompt': 'name', 'display': True},
                                             {'name': 'original_location', 'value': '/arp-scale-2-cloud-bucket-with-tags11/afolder/', 'prompt': 'original_location', 'display': True},
                                             {'name': 'owner', 'value': 'system|none', 'prompt': 'owner', 'display': True},
                                             {'name': 's3_uri', 'value': 's3://arp-scale-2-cloud-bucket-with-tags11/afolder/', 'prompt': 's3_uri', 'display': True},
                                             {'name': 'shares', 'value': [], 'prompt': 'shares', 'display': True},
                                             {'name': 'size', 'value': 0, 'prompt': 'size', 'display': True},
                                             {'name': 'source', 'value': 'AWS S3', 'prompt': 'source', 'display': True},
                                             {'name': 'source_detail', 'value': None, 'prompt': 'source_detail', 'display': True},
                                             {'name': 'storage_class', 'value': None, 'prompt': 'storage_class', 'display': True},
                                             {'name': 'type', 'value': 'heaobject.trash.AWSS3FolderFileTrashItem', 'prompt': 'type', 'display': True},
+                                            {'name': 'type_display_name', 'value': 'Trash Item', 'prompt': 'type_display_name', 'display': True},
                                             {'name': 'version', 'value': self.__version2, 'prompt': 'version', 'display': True},
                                             {'name': 'volume_id', 'value': '666f6f2d6261722d71757578', 'prompt': 'volume_id', 'display': True}],
                                           'links': [
                                             {'prompt': 'Open', 'rel': 'hea-opener-choices hea-context-menu', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}/opener'},
                                             {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}/restorer'},
                                             {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}/deleter'},
                                             {'prompt': 'View', 'rel': 'self', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}'}]}],
@@ -407,14 +428,15 @@
                                             {'name': 'human_readable_size', 'value': None, 'prompt': 'Size', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'storage_class', 'value': None, 'prompt': 'Storage class', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 's3_uri', 'value': None, 'prompt': 'S3 URI', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'mime_type', 'value': None, 'prompt': 'MIME Type', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'owner', 'value': None, 'prompt': 'Owner', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': '/people/', 'text': 'display_name', 'value': 'id'}},
                                             {'name': 'created', 'value': None, 'prompt': 'Created', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'datetime'},
                                             {'name': 'modified', 'value': None, 'prompt': 'Modified', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'datetime'},
+                                            {'name': 'deleted', 'value': None, 'prompt': 'Deleted', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'datetime'},
                                             {'name': 'source', 'value': None, 'prompt': 'Source', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'section': 'shares', 'index': -1, 'sectionPrompt': 'Shares', 'name': 'user', 'value': None, 'prompt': 'User', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': '/people/', 'text': 'display_name', 'value': 'id'}},
                                             {'section': 'shares', 'index': -1, 'name': 'permissions', 'value': None, 'prompt': 'Permissions', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'cardinality': 'multiple', 'options': [{'value': 'COOWNER', 'text': 'Co-owner'}, {'value': 'CREATOR', 'text': 'Creator'}, {'value': 'DELETER', 'text': 'Deleter'}, {'value': 'EDITOR', 'text': 'Editor'}, {'value': 'SHARER', 'text': 'Sharer'}, {'value': 'VIEWER', 'text': 'Viewer'}]}]}}}]
             self.assertEqual(_ordered(actual), _ordered(await resp.json()))
 
     async def test_get_deleted_items_invalid_trash_folder(self):
         async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trashfolders/toor/items') as resp:
@@ -428,14 +450,15 @@
         async with self.client.get('/volumes/1/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trashfolders/root/items') as resp:
             self.assertEqual(404, resp.status)
 
     async def test_get_deleted_items_trash_folder(self):
         async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trashfolders/root/items') as resp:
             actual = [{'collection': {'version': '1.0',
                                       'href': f'http://127.0.0.1:{resp.url.port}/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trashfolders/root/items',
+                                      'permissions': [['CHECK_DYNAMIC', 'COOWNER', 'CREATOR', 'DELETER', 'EDITOR', 'SHARER', 'VIEWER'], ['CHECK_DYNAMIC', 'COOWNER', 'CREATOR', 'DELETER', 'EDITOR', 'SHARER', 'VIEWER']],
                                       'items': [
                                         {'data': [
                                             {'name': 'actual_object_id', 'value': 'VGV4dEZpbGVVVEY4LnR4dA==', 'prompt': 'actual_object_id', 'display': True},
                                             {'name': 'actual_object_type_name', 'value': 'heaobject.data.AWSS3FileObject', 'prompt': 'actual_object_type_name', 'display': True},
                                             {'name': 'actual_object_uri', 'value': 'volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3files/VGV4dEZpbGVVVEY4LnR4dA==', 'prompt': 'actual_object_uri', 'display': True},
                                             {'name': 'bucket_id', 'value': 'arp-scale-2-cloud-bucket-with-tags11', 'prompt': 'bucket_id', 'display': True},
                                             {'name': 'created', 'value': '2022-05-17T00:00:00+00:00', 'prompt': 'created', 'display': True},
@@ -444,23 +467,25 @@
                                             {'name': 'description', 'value': None, 'prompt': 'description', 'display': True},
                                             {'name': 'display_name', 'value': 'TextFileUTF8.txt', 'prompt': 'display_name', 'display': True},
                                             {'name': 'human_readable_original_location', 'value': '/arp-scale-2-cloud-bucket-with-tags11/TextFileUTF8.txt', 'prompt': 'human_readable_original_location', 'display': True},
                                             {'name': 'human_readable_size', 'value': '0 Bytes', 'prompt': 'human_readable_size', 'display': True},
                                             {'name': 'id', 'value': f'VGV4dEZpbGVVVEY4LnR4dA==,{self.__version1}', 'prompt': 'id', 'display': False},
                                             {'name': 'invites', 'value': [], 'prompt': 'invites', 'display': True}, {'name': 'key', 'value': 'TextFileUTF8.txt', 'prompt': 'key', 'display': True},
                                             {'name': 'modified', 'value': '2022-05-17T00:00:00+00:00', 'prompt': 'modified', 'display': True},
+                                            {'name': 'deleted', 'value': '2022-05-18T00:00:00+00:00', 'prompt': 'deleted', 'display': True},
                                             {'name': 'name', 'value': f'VGV4dEZpbGVVVEY4LnR4dA==,{self.__version1}', 'prompt': 'name', 'display': True},
                                             {'name': 'original_location', 'value': '/arp-scale-2-cloud-bucket-with-tags11/TextFileUTF8.txt', 'prompt': 'original_location', 'display': True},
                                             {'name': 'owner', 'value': 'system|none', 'prompt': 'owner', 'display': True},
                                             {'name': 's3_uri', 'value': 's3://arp-scale-2-cloud-bucket-with-tags11/TextFileUTF8.txt', 'prompt': 's3_uri', 'display': True},
                                             {'name': 'shares', 'value': [], 'prompt': 'shares', 'display': True}, {'name': 'size', 'value': 0, 'prompt': 'size', 'display': True},
                                             {'name': 'source', 'value': 'AWS S3', 'prompt': 'source', 'display': True},
                                             {'name': 'source_detail', 'value': None, 'prompt': 'source_detail', 'display': True},
                                             {'name': 'storage_class', 'value': None, 'prompt': 'storage_class', 'display': True},
                                             {'name': 'type', 'value': 'heaobject.trash.AWSS3FolderFileTrashItem', 'prompt': 'type', 'display': True},
+                                            {'name': 'type_display_name', 'value': 'Trash Item', 'prompt': 'type_display_name', 'display': True},
                                             {'name': 'version', 'value': self.__version1, 'prompt': 'version', 'display': True},
                                             {'name': 'volume_id', 'value': '666f6f2d6261722d71757578', 'prompt': 'volume_id', 'display': True}],
                                           'links': [
                                             {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/restorer'},
                                             {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/deleter'},
                                             {'prompt': 'View', 'rel': 'self', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}'}]},
                                         {'data': [
@@ -475,24 +500,26 @@
                                             {'name': 'display_name', 'value': 'afolder', 'prompt': 'display_name', 'display': True},
                                             {'name': 'human_readable_original_location', 'value': '/arp-scale-2-cloud-bucket-with-tags11/afolder/', 'prompt': 'human_readable_original_location', 'display': True},
                                             {'name': 'human_readable_size', 'value': '0 Bytes', 'prompt': 'human_readable_size', 'display': True},
                                             {'name': 'id', 'value': f'YWZvbGRlci8=,{self.__version2}', 'prompt': 'id', 'display': False},
                                             {'name': 'invites', 'value': [], 'prompt': 'invites', 'display': True},
                                             {'name': 'key', 'value': 'afolder/', 'prompt': 'key', 'display': True},
                                             {'name': 'modified', 'value': '2022-05-17T00:00:00+00:00', 'prompt': 'modified', 'display': True},
+                                            {'name': 'deleted', 'value': '2022-05-18T00:00:00+00:00', 'prompt': 'deleted', 'display': True},
                                             {'name': 'name', 'value': f'YWZvbGRlci8=,{self.__version2}', 'prompt': 'name', 'display': True},
                                             {'name': 'original_location', 'value': '/arp-scale-2-cloud-bucket-with-tags11/afolder/', 'prompt': 'original_location', 'display': True},
                                             {'name': 'owner', 'value': 'system|none', 'prompt': 'owner', 'display': True},
                                             {'name': 's3_uri', 'value': 's3://arp-scale-2-cloud-bucket-with-tags11/afolder/', 'prompt': 's3_uri', 'display': True},
                                             {'name': 'shares', 'value': [], 'prompt': 'shares', 'display': True},
                                             {'name': 'size', 'value': 0, 'prompt': 'size', 'display': True},
                                             {'name': 'source', 'value': 'AWS S3', 'prompt': 'source', 'display': True},
                                             {'name': 'source_detail', 'value': None, 'prompt': 'source_detail', 'display': True},
                                             {'name': 'storage_class', 'value': None, 'prompt': 'storage_class', 'display': True},
                                             {'name': 'type', 'value': 'heaobject.trash.AWSS3FolderFileTrashItem', 'prompt': 'type', 'display': True},
+                                            {'name': 'type_display_name', 'value': 'Trash Item', 'prompt': 'type_display_name', 'display': True},
                                             {'name': 'version', 'value': self.__version2, 'prompt': 'version', 'display': True},
                                             {'name': 'volume_id', 'value': '666f6f2d6261722d71757578', 'prompt': 'volume_id', 'display': True}],
                                           'links': [
                                             {'prompt': 'Open', 'rel': 'hea-opener-choices hea-context-menu', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}/opener'},
                                             {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}/restorer'},
                                             {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}/deleter'},
                                             {'prompt': 'View', 'rel': 'self', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}'}]}],
@@ -507,14 +534,15 @@
                                             {'name': 'human_readable_size', 'value': None, 'prompt': 'Size', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'storage_class', 'value': None, 'prompt': 'Storage class', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 's3_uri', 'value': None, 'prompt': 'S3 URI', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'mime_type', 'value': None, 'prompt': 'MIME Type', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'owner', 'value': None, 'prompt': 'Owner', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': '/people/', 'text': 'display_name', 'value': 'id'}},
                                             {'name': 'created', 'value': None, 'prompt': 'Created', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'datetime'},
                                             {'name': 'modified', 'value': None, 'prompt': 'Modified', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'datetime'},
+                                            {'name': 'deleted', 'value': None, 'prompt': 'Deleted', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'datetime'},
                                             {'name': 'source', 'value': None, 'prompt': 'Source', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'section': 'shares', 'index': -1, 'sectionPrompt': 'Shares', 'name': 'user', 'value': None, 'prompt': 'User', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': '/people/', 'text': 'display_name', 'value': 'id'}},
                                             {'section': 'shares', 'index': -1, 'name': 'permissions', 'value': None, 'prompt': 'Permissions', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'cardinality': 'multiple', 'options': [{'value': 'COOWNER', 'text': 'Co-owner'}, {'value': 'CREATOR', 'text': 'Creator'}, {'value': 'DELETER', 'text': 'Deleter'}, {'value': 'EDITOR', 'text': 'Editor'}, {'value': 'SHARER', 'text': 'Sharer'}, {'value': 'VIEWER', 'text': 'Viewer'}]}]}}}]
             self.assertEqual(_ordered(actual), _ordered(await resp.json()))
 
     async def test_do_empty_trash_status(self):
         async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trashemptier') as resp:
```

### Comparing `heaserver-trash-aws-s3-1.0.2/tests/heaserver/trashawss3test/testcase.py` & `heaserver_trash_aws_s3-1.1.0/tests/heaserver/trashawss3test/testcase.py`

 * *Files identical despite different names*

