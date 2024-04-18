# Comparing `tmp/sentinel_sdk-0.0.2.tar.gz` & `tmp/sentinel_sdk-0.0.3.tar.gz`

## Comparing `sentinel_sdk-0.0.2.tar` & `sentinel_sdk-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/src/sentinel_sdk/__init__.py
--rw-r--r--   0        0        0     7094 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/src/sentinel_sdk/sdk.py
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/src/sentinel_sdk/types.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/src/sentinel_sdk/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/src/sentinel_sdk/modules/__init__.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/src/sentinel_sdk/modules/deposit.py
--rw-r--r--   0        0        0     7689 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/src/sentinel_sdk/modules/node.py
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/src/sentinel_sdk/modules/plan.py
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/src/sentinel_sdk/modules/provider.py
--rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/src/sentinel_sdk/modules/session.py
--rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/src/sentinel_sdk/modules/subscription.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/src/sentinel_sdk/modules/swap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/src/sentinel_sdk/querier/__init__.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/src/sentinel_sdk/querier/multiquerier.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/src/sentinel_sdk/querier/querier.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/src/sentinel_sdk/querier/modules/__init__.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/src/sentinel_sdk/querier/modules/deposit.py
--rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/src/sentinel_sdk/querier/modules/node.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/src/sentinel_sdk/querier/modules/plan.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/src/sentinel_sdk/querier/modules/provider.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/src/sentinel_sdk/querier/modules/session.py
--rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/src/sentinel_sdk/querier/modules/subscription.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/src/sentinel_sdk/querier/modules/swap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/src/sentinel_sdk/transactor/__init__.py
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/src/sentinel_sdk/transactor/transactor.py
--rw-r--r--   0        0        0     8706 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/test/connect.py
--rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/test/connect.sdk.py
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/test/queryall.py
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/LICENSE
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/README.md
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/__init__.py
+-rw-r--r--   0        0        0     7141 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/sdk.py
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/types.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/modules/__init__.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/modules/deposit.py
+-rw-r--r--   0        0        0     7949 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/modules/node.py
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/modules/plan.py
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/modules/provider.py
+-rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/modules/session.py
+-rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/modules/subscription.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/modules/swap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/querier/__init__.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/querier/multiquerier.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/querier/querier.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/__init__.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/deposit.py
+-rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/node.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/plan.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/provider.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/session.py
+-rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/subscription.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/swap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/transactor/__init__.py
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/transactor/transactor.py
+-rw-r--r--   0        0        0     8706 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/test/connect.py
+-rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/test/connect.sdk.py
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/test/queryall.py
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/README.md
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/PKG-INFO
```

### Comparing `sentinel_sdk-0.0.2/.pre-commit-config.yaml` & `sentinel_sdk-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.2/src/sentinel_sdk/sdk.py` & `sentinel_sdk-0.0.3/src/sentinel_sdk/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,16 @@
         try:
             self.__create_and_verify_channel(grpcaddr, grpcport, ssl=ssl)
         except grpc._channel._InactiveRpcError:
             raise ConnectionError("gRPC endpoint is invalid or not responding")
 
         self._client = None
         self._account = None
-
+        self._provider_account = None
+        
         if secret is not None:
             self.__setup_account_and_client(grpcaddr, grpcport, secret, ssl)
 
         self.__load_modules()
 
 
     def __create_and_verify_channel(
```

### Comparing `sentinel_sdk-0.0.2/src/sentinel_sdk/types.py` & `sentinel_sdk-0.0.3/src/sentinel_sdk/types.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.2/src/sentinel_sdk/utils.py` & `sentinel_sdk-0.0.3/src/sentinel_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.2/src/sentinel_sdk/modules/deposit.py` & `sentinel_sdk-0.0.3/src/sentinel_sdk/modules/deposit.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.2/src/sentinel_sdk/modules/node.py` & `sentinel_sdk-0.0.3/src/sentinel_sdk/modules/node.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import ssl
 import threading
 import urllib.parse
 import urllib.request
+import http.client
 from typing import Any
 import json
 import uuid
 import base64
 import hashlib
 import ecdsa
 import grpc
@@ -69,15 +70,18 @@
                 timeout=self.node_timeout,
             ).read()
             contents = contents.decode("utf-8")
         except urllib.error.URLError:
             contents = '{"success":false,"urllib-error":"URLError encountered"}'
         except TimeoutError:
             contents = '{"success":false,"urllib-error":"Data reading timed out"}'
-
+        except http.client.RemoteDisconnected:
+            contents = '{"success":false,"http-error":"Remote endpoint closed connection"}'
+        except:
+            contents = '{"success":false,"error":"Unrecognizable error encountered"}'
         if is_in_thread:
             self.__nodes_status_cache[node.address] = contents
         else:
             return contents
 
     def QueryNodesStatus(self, nodes: list[node_pb2.Node], n_threads: int = 8) -> dict:
         chunks = list(self.__split_into_chunks(nodes, n_threads))
@@ -194,8 +198,8 @@
         payload = {
             "key": key,
             "signature": base64.b64encode(signature).decode("utf-8"),
         }
         return self.__post_session(
             f"{remote_url}/accounts/{self._account.address}/sessions/{session_id}",
             payload,
-        )
+        )
```

### Comparing `sentinel_sdk-0.0.2/src/sentinel_sdk/modules/plan.py` & `sentinel_sdk-0.0.3/src/sentinel_sdk/modules/plan.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.2/src/sentinel_sdk/modules/provider.py` & `sentinel_sdk-0.0.3/src/sentinel_sdk/modules/provider.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.2/src/sentinel_sdk/modules/session.py` & `sentinel_sdk-0.0.3/src/sentinel_sdk/modules/session.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.2/src/sentinel_sdk/modules/subscription.py` & `sentinel_sdk-0.0.3/src/sentinel_sdk/modules/subscription.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.2/src/sentinel_sdk/modules/swap.py` & `sentinel_sdk-0.0.3/src/sentinel_sdk/modules/swap.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.2/src/sentinel_sdk/querier/multiquerier.py` & `sentinel_sdk-0.0.3/src/sentinel_sdk/querier/multiquerier.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.2/src/sentinel_sdk/querier/querier.py` & `sentinel_sdk-0.0.3/src/sentinel_sdk/querier/querier.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.2/src/sentinel_sdk/querier/modules/deposit.py` & `sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/deposit.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.2/src/sentinel_sdk/querier/modules/node.py` & `sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/node.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.2/src/sentinel_sdk/querier/modules/plan.py` & `sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/plan.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.2/src/sentinel_sdk/querier/modules/provider.py` & `sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/provider.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.2/src/sentinel_sdk/querier/modules/session.py` & `sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/session.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.2/src/sentinel_sdk/querier/modules/subscription.py` & `sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/subscription.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.2/src/sentinel_sdk/querier/modules/swap.py` & `sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/swap.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.2/src/sentinel_sdk/transactor/transactor.py` & `sentinel_sdk-0.0.3/src/sentinel_sdk/transactor/transactor.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.2/test/connect.py` & `sentinel_sdk-0.0.3/test/connect.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.2/test/connect.sdk.py` & `sentinel_sdk-0.0.3/test/connect.sdk.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.2/test/queryall.py` & `sentinel_sdk-0.0.3/test/queryall.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.2/.gitignore` & `sentinel_sdk-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.2/LICENSE` & `sentinel_sdk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.2/README.md` & `sentinel_sdk-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -41,10 +41,10 @@
 sdk = SDKInstance("grpc.sentinel.co", 9090)
 nodes = sdk.nodes.QueryNodes(Status.ACTIVE)
 subscriptions = sdk.subscriptions.QuerySubscriptions(pagination=PageRequest(limit=5000, offset=0, reverse=True))
 ```
 
 ## Coded with Love by:
 
-[NAST0R · GitHub](https://github.com/NAST0R) , [Tkd-Alex (Alessandro Maggio) · GitHub](https://github.com/Tkd-Alex), [freQniK]([freQniK · GitHub](https://github.com/freQniK))
+[NAST0R · GitHub](https://github.com/NAST0R) , [Tkd-Alex (Alessandro Maggio) · GitHub](https://github.com/Tkd-Alex), ([freQniK · GitHub](https://github.com/freQniK))
 
 **Commissioned by MathNodes** [MathNodes](https://github.com/MathNodes/sentinel-python-sdk)
```

### Comparing `sentinel_sdk-0.0.2/pyproject.toml` & `sentinel_sdk-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-name = "sentinel-sdk"
-version = "0.0.2"
+name = "sentinel_sdk"
+version = "0.0.3"
 description = "A Sentinel SDK Written in Python"
 authors = [
     { name = "NAST0R" },
-    { name = "Tkd-Alex", email = "dev@ctrl-felix.de" },
+    { name = "Tkd-Alex", email = "alex.tkd.alex@gmail.com" },
     { name = "MathNodes", email = "freQniK@mathnodes.com'" },
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["sentinel_sdk", "mospy", "sentinel", "cosmos", "protobuf", "sentinel_protobuf"]
 license = {text = "GPL-3.0 license"}
 classifiers = [
```

### Comparing `sentinel_sdk-0.0.2/PKG-INFO` & `sentinel_sdk-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.3
-Name: sentinel-sdk
-Version: 0.0.2
+Name: sentinel_sdk
+Version: 0.0.3
 Summary: A Sentinel SDK Written in Python
 Author: NAST0R
-Author-email: Tkd-Alex <dev@ctrl-felix.de>, MathNodes <freQniK@mathnodes.com'>
+Author-email: Tkd-Alex <alex.tkd.alex@gmail.com>, MathNodes <freQniK@mathnodes.com'>
 License: GPL-3.0 license
 License-File: LICENSE
 Keywords: cosmos,mospy,protobuf,sentinel,sentinel_protobuf,sentinel_sdk
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -62,10 +62,10 @@
 sdk = SDKInstance("grpc.sentinel.co", 9090)
 nodes = sdk.nodes.QueryNodes(Status.ACTIVE)
 subscriptions = sdk.subscriptions.QuerySubscriptions(pagination=PageRequest(limit=5000, offset=0, reverse=True))
 ```
 
 ## Coded with Love by:
 
-[NAST0R · GitHub](https://github.com/NAST0R) , [Tkd-Alex (Alessandro Maggio) · GitHub](https://github.com/Tkd-Alex), [freQniK]([freQniK · GitHub](https://github.com/freQniK))
+[NAST0R · GitHub](https://github.com/NAST0R) , [Tkd-Alex (Alessandro Maggio) · GitHub](https://github.com/Tkd-Alex), ([freQniK · GitHub](https://github.com/freQniK))
 
 **Commissioned by MathNodes** [MathNodes](https://github.com/MathNodes/sentinel-python-sdk)
```

