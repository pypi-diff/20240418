# Comparing `tmp/latch_aws-0.1.7.tar.gz` & `tmp/latch_aws-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_aws-0.1.7.tar", max compression
+gzip compressed data, was "latch_aws-0.1.8.tar", max compression
```

## Comparing `latch_aws-0.1.7.tar` & `latch_aws-0.1.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     7052 2023-05-31 20:53:02.454014 latch_aws-0.1.7/LICENSE
--rw-r--r--   0        0        0       13 2023-05-31 20:53:27.998551 latch_aws-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-05-31 20:53:02.473001 latch_aws-0.1.7/latch_aws/__init__.py
--rw-r--r--   0        0        0     9677 2023-06-09 18:38:21.628052 latch_aws-0.1.7/latch_aws/aws.py
--rw-r--r--   0        0        0     3805 2024-03-05 20:44:13.884663 latch_aws-0.1.7/latch_aws/client_pool.py
--rw-r--r--   0        0        0        0 2023-05-31 20:53:02.473127 latch_aws-0.1.7/latch_aws/py.typed
--rw-r--r--   0        0        0     1264 2024-03-05 20:44:52.239171 latch_aws-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      641 1970-01-01 00:00:00.000000 latch_aws-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     7052 2023-05-31 20:53:02.454014 latch_aws-0.1.8/LICENSE
+-rw-r--r--   0        0        0       13 2023-05-31 20:53:27.998551 latch_aws-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 20:53:02.473001 latch_aws-0.1.8/latch_aws/__init__.py
+-rw-r--r--   0        0        0     9677 2023-06-09 18:38:21.628052 latch_aws-0.1.8/latch_aws/aws.py
+-rw-r--r--   0        0        0     4066 2024-04-17 23:06:41.948054 latch_aws-0.1.8/latch_aws/client_pool.py
+-rw-r--r--   0        0        0        0 2023-05-31 20:53:02.473127 latch_aws-0.1.8/latch_aws/py.typed
+-rw-r--r--   0        0        0     1264 2024-04-17 23:06:50.246277 latch_aws-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      641 1970-01-01 00:00:00.000000 latch_aws-0.1.8/PKG-INFO
```

### Comparing `latch_aws-0.1.7/LICENSE` & `latch_aws-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `latch_aws-0.1.7/latch_aws/aws.py` & `latch_aws-0.1.8/latch_aws/aws.py`

 * *Files identical despite different names*

### Comparing `latch_aws-0.1.7/latch_aws/client_pool.py` & `latch_aws-0.1.8/latch_aws/client_pool.py`

 * *Files 9% similar despite different names*

```diff
@@ -75,19 +75,23 @@
             async with region_client.sema:
                 async with region_client.client_add_sema:
                     if len(region_client.clients) == 0:
                         with tracer.start_as_current_span(
                             "create s3 client",
                             attributes={"region": region},
                         ):
+                            # https://github.com/boto/boto3/issues/421 - use addressing_style=path to support buckets before DNS propagation
                             client = await sess.create_client(
                                 "s3",
                                 region_name=region,
                                 config=AioConfig().merge(
-                                    Config(signature_version="s3v4")
+                                    Config(
+                                        signature_version="s3v4",
+                                        s3={"addressing_style": "path"},
+                                    )
                                 ),
                             ).__aenter__()
                     else:
                         client = region_client.clients.pop()
 
                 try:
                     yield client
@@ -95,10 +99,7 @@
                     region_client.clients.append(client)
                     s.set_attributes(
                         {
                             f"client_count_{region}": len(region_client.clients),
                             "region_count": len(self.region_clients),
                         }
                     )
-
-
-s3_pool = AsyncS3ClientPool()
```

### Comparing `latch_aws-0.1.7/pyproject.toml` & `latch_aws-0.1.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "latch-aws"
-version = "0.1.7"
+version = "0.1.8"
 description = "Traced and managed aws resources"
 authors = ["Max Smolin <max@latch.bio>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "latch_aws"}]
 
 [tool.poetry.dependencies]
```

### Comparing `latch_aws-0.1.7/PKG-INFO` & `latch_aws-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latch-aws
-Version: 0.1.7
+Version: 0.1.8
 Summary: Traced and managed aws resources
 License: CC0 1.0
 Author: Max Smolin
 Author-email: max@latch.bio
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

