# Comparing `tmp/zaku-0.0.3-py3-none-any.whl.zip` & `tmp/zaku-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 12096 bytes, number of entries: 12
+Zip file size: 12265 bytes, number of entries: 12
 -rw-r--r--  2.0 unx       59 b- defN 24-Apr-15 02:31 zaku/__init__.py
 -rw-r--r--  2.0 unx     3780 b- defN 24-Apr-17 22:37 zaku/base.py
 -rw-r--r--  2.0 unx     5045 b- defN 24-Apr-17 23:08 zaku/client.py
 -rw-r--r--  2.0 unx     8279 b- defN 24-Apr-17 23:41 zaku/interfaces.py
 -rw-r--r--  2.0 unx     1678 b- defN 24-Apr-14 19:38 zaku/job_queue.py
--rw-r--r--  2.0 unx     5132 b- defN 24-Apr-17 23:55 zaku/server.py
--rw-r--r--  2.0 unx     1064 b- defN 24-Apr-17 23:57 zaku-0.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     4102 b- defN 24-Apr-17 23:57 zaku-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 23:57 zaku-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 24-Apr-17 23:57 zaku-0.0.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 24-Apr-17 23:57 zaku-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      893 b- defN 24-Apr-17 23:57 zaku-0.0.3.dist-info/RECORD
-12 files, 30178 bytes uncompressed, 10618 bytes compressed:  64.8%
+-rw-r--r--  2.0 unx     5879 b- defN 24-Apr-18 03:36 zaku/server.py
+-rw-r--r--  2.0 unx     1064 b- defN 24-Apr-18 03:37 zaku-0.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4102 b- defN 24-Apr-18 03:37 zaku-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-18 03:37 zaku-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 24-Apr-18 03:37 zaku-0.0.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-18 03:37 zaku-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      893 b- defN 24-Apr-18 03:37 zaku-0.0.5.dist-info/RECORD
+12 files, 30925 bytes uncompressed, 10787 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: zaku/job_queue.py
 Comment: 
 
 Filename: zaku/server.py
 Comment: 
 
-Filename: zaku-0.0.3.dist-info/LICENSE
+Filename: zaku-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: zaku-0.0.3.dist-info/METADATA
+Filename: zaku-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: zaku-0.0.3.dist-info/WHEEL
+Filename: zaku-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: zaku-0.0.3.dist-info/entry_points.txt
+Filename: zaku-0.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: zaku-0.0.3.dist-info/top_level.txt
+Filename: zaku-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: zaku-0.0.3.dist-info/RECORD
+Filename: zaku-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zaku/server.py

```diff
@@ -1,17 +1,15 @@
 import msgpack
 import redis
 from aiohttp import web
-from params_proto import Proto, ParamsProto
+from params_proto import Proto, ParamsProto, Flag
 
 from zaku.base import Server
 from zaku.interfaces import Job
 
-DEFAULT_PORT = 9000
-
 
 class Redis(ParamsProto, prefix="redis", cli_parse=False):
     """Redis Configuration for the TaskServer class.
 
     .. code-block:: shell
 
         # Put this into an .env file
@@ -49,50 +47,68 @@
 
     CLI Options
 
     .. code-block:: shell
 
         python -m zaku.server --help
 
-        -h, --help          show this help message and exit
-        --prefix          :str 'Zaku-task-queues'
-        --queue-len       :int 100
-        --port            :int 9000
-        --free-port       :bool True
-        --static-root     :str '.'
-        --cors            :str 'https://vuer.ai,https://dash.ml,http://lo...
-        --cert            :str None the path to the SSL certificate
-        --key             :str None the path to the SSL key
-        --ca-cert         :str None the trusted root CA certificates
+        -h, --help            show this help message and exit
+        --prefix            :str 'Zaku-task-queues'
+        --queue-len         :int 100
+        --host              :str 'localhost'
+                              set to 0.0.0.0 to enable remote (not localhost) connections.
+        --port              :int 9000
+        --cors              :str 'https://vuer.ai,https://dash.ml,http://lo...
+        --cert              :str None the path to the SSL certificate
+        --key               :str None the path to the SSL key
+        --ca-cert           :str None the trusted root CA certificates
         --REQUEST-MAX-SIZE  :int 100000000 the maximum packet size
+        --free-port         :bool False
+                              kill process squatting target port if True.
+        --static-root       :str '.'
+        --verbose           :bool False
+                              show the list of configurations during launch if True.
+
     """
 
     prefix = "Zaku-task-queues"
 
     # Queue Parameters
     queue_len = 100  # use a max length to avoid the memory from blowing up.
 
     # Server Parameters
-    port = DEFAULT_PORT
-    free_port = True
-    static_root = "."
-    cors = (
+    host: str = Proto(
+        "localhost",
+        help="set to 0.0.0.0 to enable remote (not localhost) connections.",
+    )
+    port: int = 9000
+    cors: str = (
         "https://vuer.ai,https://dash.ml,http://localhost:8000,http://127.0.0.1:8000,*"
     )
 
     # SSL Parameters
-    cert = Proto(None, dtype=str, help="the path to the SSL certificate")
-    key = Proto(None, dtype=str, help="the path to the SSL key")
-    ca_cert = Proto(None, dtype=str, help="the trusted root CA certificates")
+    cert: str = Proto(None, dtype=str, help="the path to the SSL certificate")
+    key: str = Proto(None, dtype=str, help="the path to the SSL key")
+    ca_cert: str = Proto(None, dtype=str, help="the trusted root CA certificates")
 
-    REQUEST_MAX_SIZE = Proto(100_000_000, env="WEBSOCKET_MAX_SIZE", help="the maximum packet size")
+    REQUEST_MAX_SIZE: int = Proto(
+        100_000_000, env="WEBSOCKET_MAX_SIZE", help="the maximum packet size"
+    )
+
+    free_port: bool = Flag("kill process squatting target port if True.")
+    static_root: str = "."
+    verbose = Flag("show the list of configurations during launch if True.")
 
     def __post_init__(self):
         Server.__post_init__(self)
 
+        if self.verbose:
+            for k, v in vars(self).items():
+                print(f"{k}: {v},")
+
         self.redis = redis.asyncio.Redis(**vars(Redis))
 
     async def create_queue(self, request: web.Request):
         data = await request.json()
         # print("==>", data)
         try:
             await Job.create_queue(self.redis, **data, prefix=self.prefix)
```

## Comparing `zaku-0.0.3.dist-info/LICENSE` & `zaku-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zaku-0.0.3.dist-info/METADATA` & `zaku-0.0.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zaku
-Version: 0.0.3
+Version: 0.0.5
 Summary: Zaku Task Queue is for distributed ML-workloads.
 Home-page: https://github.com/geyang/zaku
 Author: Ge Yang<ge.ike.yang@gmail.com>
 Author-email: ge.ike.yang@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
```

## Comparing `zaku-0.0.3.dist-info/RECORD` & `zaku-0.0.5.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 zaku/__init__.py,sha256=dVBFG2RyfsJ9Yf3OgSN49X6Tpk7RgfdFHyFYgs1vvjs,59
 zaku/base.py,sha256=7jgQ1Rcz6eDLNjkryDXLC9QrDWcct9fdixwHPjXd59g,3780
 zaku/client.py,sha256=u0GhknUONMzwGjY7mcS3A8HCrDZAxWx-vCdn0cheOo8,5045
 zaku/interfaces.py,sha256=Ak6jU-O7GMXxHW9ZF_5WiMyzNDj9xaIy5wHUy9pqAAI,8279
 zaku/job_queue.py,sha256=rClaiGYU6ZDSi-ehPtKbZfJcYxZaOr3DHMPfRq9jl4o,1678
-zaku/server.py,sha256=8ylbWScYJ556v84o1nYHaFsmBTODY1B-S0c-v0eugtI,5132
-zaku-0.0.3.dist-info/LICENSE,sha256=ViVJUWot4p3kmGwzBBRu6vqoBFQuLFKyGIR3jzh4X_A,1064
-zaku-0.0.3.dist-info/METADATA,sha256=PfFRBaz1uIVm29JWXRNJiH4c9azDHa5skNHso_90fos,4102
-zaku-0.0.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-zaku-0.0.3.dist-info/entry_points.txt,sha256=OQmjyBNrqRKNAK7zutZ83SXuKvH6EURf28dG8-nPtdE,49
-zaku-0.0.3.dist-info/top_level.txt,sha256=NOH9JyYZg-VCpceLmApF5Rx3njTGe8RjuRaQsTc5k4o,5
-zaku-0.0.3.dist-info/RECORD,,
+zaku/server.py,sha256=EiCWvox4LGtdNVcAkTcSlSCbOj7yQ6YRq9iPmppyTok,5879
+zaku-0.0.5.dist-info/LICENSE,sha256=ViVJUWot4p3kmGwzBBRu6vqoBFQuLFKyGIR3jzh4X_A,1064
+zaku-0.0.5.dist-info/METADATA,sha256=3YM2xv7zKiUvThsw_JUgGraeQOOJbeeRasHI82VDtzI,4102
+zaku-0.0.5.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+zaku-0.0.5.dist-info/entry_points.txt,sha256=OQmjyBNrqRKNAK7zutZ83SXuKvH6EURf28dG8-nPtdE,49
+zaku-0.0.5.dist-info/top_level.txt,sha256=NOH9JyYZg-VCpceLmApF5Rx3njTGe8RjuRaQsTc5k4o,5
+zaku-0.0.5.dist-info/RECORD,,
```

