# Comparing `tmp/zaku-0.0.2-py3-none-any.whl.zip` & `tmp/zaku-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 10063 bytes, number of entries: 12
--rw-r--r--  2.0 unx       60 b- defN 24-Apr-14 19:38 zaku/__init__.py
--rw-r--r--  2.0 unx     3731 b- defN 24-Apr-13 21:49 zaku/base.py
--rw-r--r--  2.0 unx     3216 b- defN 24-Apr-14 19:38 zaku/client.py
--rw-r--r--  2.0 unx     4698 b- defN 24-Apr-14 19:05 zaku/interfaces.py
+Zip file size: 12096 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       59 b- defN 24-Apr-15 02:31 zaku/__init__.py
+-rw-r--r--  2.0 unx     3780 b- defN 24-Apr-17 22:37 zaku/base.py
+-rw-r--r--  2.0 unx     5045 b- defN 24-Apr-17 23:08 zaku/client.py
+-rw-r--r--  2.0 unx     8279 b- defN 24-Apr-17 23:41 zaku/interfaces.py
 -rw-r--r--  2.0 unx     1678 b- defN 24-Apr-14 19:38 zaku/job_queue.py
--rw-r--r--  2.0 unx     4335 b- defN 24-Apr-14 19:38 zaku/server.py
--rw-r--r--  2.0 unx     1064 b- defN 24-Apr-14 19:43 zaku-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3487 b- defN 24-Apr-14 19:43 zaku-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-14 19:43 zaku-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       37 b- defN 24-Apr-14 19:43 zaku-0.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 24-Apr-14 19:43 zaku-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      893 b- defN 24-Apr-14 19:43 zaku-0.0.2.dist-info/RECORD
-12 files, 23296 bytes uncompressed, 8585 bytes compressed:  63.1%
+-rw-r--r--  2.0 unx     5132 b- defN 24-Apr-17 23:55 zaku/server.py
+-rw-r--r--  2.0 unx     1064 b- defN 24-Apr-17 23:57 zaku-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4102 b- defN 24-Apr-17 23:57 zaku-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 23:57 zaku-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 24-Apr-17 23:57 zaku-0.0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-17 23:57 zaku-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      893 b- defN 24-Apr-17 23:57 zaku-0.0.3.dist-info/RECORD
+12 files, 30178 bytes uncompressed, 10618 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: zaku/job_queue.py
 Comment: 
 
 Filename: zaku/server.py
 Comment: 
 
-Filename: zaku-0.0.2.dist-info/LICENSE
+Filename: zaku-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: zaku-0.0.2.dist-info/METADATA
+Filename: zaku-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: zaku-0.0.2.dist-info/WHEEL
+Filename: zaku-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: zaku-0.0.2.dist-info/entry_points.txt
+Filename: zaku-0.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: zaku-0.0.2.dist-info/top_level.txt
+Filename: zaku-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: zaku-0.0.2.dist-info/RECORD
+Filename: zaku-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zaku/__init__.py

```diff
@@ -1,2 +1,2 @@
-# from .server import TaskQServer
+# from .server import TaskServer
 from .client import TaskQ
```

## zaku/base.py

```diff
@@ -46,46 +46,48 @@
         raise web.HTTPNotFound()
 
     return web.FileResponse(filepath)
 
 
 class Server:
     """Base TCP server"""
+
     host: str = "localhost"
     port: int = 8012
     cors: str = "*"
     "Enable CORS"
 
     cert: str = None
     "the path to the SSL certificate"
     key: str = None
     "the path to the SSL key"
     ca_cert: str = None
     "the trusted root CA certificates"
 
-    WEBSOCKET_MAX_SIZE = 2 ** 28
+    WEBSOCKET_MAX_SIZE = 2**28
+    REQUEST_MAX_SIZE = 2**28
 
     def __post_init__(self):
-        self.app = web.Application()
+        self.app = web.Application(client_max_size=self.REQUEST_MAX_SIZE)
 
         default = aiohttp_cors.ResourceOptions(
             allow_credentials=True,
             expose_headers="*",
             allow_headers="*",
             allow_methods="*",
         )
         cors_config = {k: default for k in self.cors.split(",")}
 
         self.cors_context = aiohttp_cors.setup(self.app, defaults=cors_config)
 
     def _route(
-            self,
-            path: str,
-            handler: callable,
-            method: str = "GET",
+        self,
+        path: str,
+        handler: callable,
+        method: str = "GET",
     ):
         route = self.app.router.add_resource(path).add_route(method, handler)
         self.cors_context.add(route)
 
     def _socket(self, path: str, handler: callable):
         ws_handler = partial(
             websocket_handler, handler=handler, max_msg_size=self.WEBSOCKET_MAX_SIZE
```

## zaku/client.py

```diff
@@ -1,99 +1,171 @@
 from contextlib import contextmanager
 from uuid import uuid4
 
 import msgpack
 import requests
-# from requests_futures import sessions
 from params_proto import PrefixProto, Proto, Flag
+from typing import Dict
 
+from zaku.interfaces import Payload
 
-class TaskQ(PrefixProto):
-    host: str = Proto(
+
+class TaskQ(PrefixProto, cli=False):
+    """TaskQ Client
+    ----------------
+
+    This is the client that interacts with the TaskQ server. We do not
+    include the configs in the command line because the TaskServer is
+    the primary entry point from the command line.
+
+    We do provide the option to load environment variables for these
+    configurations.
+
+    Usage
+    +++++
+
+    .. code-block:: shell
+
+        # Put this into an .env file (without the exports)
+        export ZAKU_URI=http://localhost:9000
+        export ZAKU_QUEUE_NAME=jq-debug-1
+
+    Now you can create a queue like this:
+
+    .. code-block:: python
+
+        queue = TaskQ()
+
+    ::
+
+        Out[2]: {
+            "uri": "http://localhost:9000",
+            "name": "jq-debug-1",
+            "ttl": 5.0
+        }
+
+
+    .. automethod:: init_queue
+    .. automethod:: add
+    .. automethod:: take
+    .. automethod:: pop
+    .. automethod:: mark_done
+    .. automethod:: mark_reset
+    """
+
+    uri: str = Proto(
         "http://localhost:9000",
+        env="ZAKU_URI",
         help="host end point, including protocol and port.",
     )
+    """host endpoint uri, including protocol and port.
+    
+    .. code-block:: python
+    
+        uri: str = Proto(
+            "http://localhost:9000",
+            env="ZAKU_URI",
+        )   
+    """
 
-    name = Proto(
+    name: str = Proto(
         f"jq-{uuid4()}",
+        env="ZAKU_QUEUE_NAME",
         help="""This is the name of the queue. It is unique to the client.""",
     )
-    ttl = Proto(5, help="time to live. Defaults to 5.")
-    no_init = Flag("Flag for skipping the queue creation.")
+    """This is the name of the queue. It is unique to the client. Defaults to a random uuid
+    to avoid collision, but you usually want to supply a name so that it is easier to find
+    the queue. Zaku also reads from environment variables to side-load the configurations.
+    
+    .. code-block:: python
+    
+        name: str = Proto(
+            f"jq-{uuid4()}",
+            env="ZAKU_QUEUE_NAME",
+        )
+    """
+
+    ttl: float = Proto(5.0, "time to live in seconds. Defaults to 5.")
+    """time to live in seconds. Defaults to 5."""
+    no_init: bool = Flag("Flag for skipping the queue creation.")
+    """Flag for skipping the queue creation."""
 
     def __post_init__(self):
         if not self.no_init:
             self.init_queue()
 
     def init_queue(self, name=None):
         """Create a new collection.
 
         :param name: (optional) The name of the queue.
         """
         if name:
             self.name = name
 
         print("creating queue:", self.name)
-        res = requests.put(self.host + "/queues", json={"name": self.name})
+        res = requests.put(self.uri + "/queues", json={"name": self.name})
         return res.status_code == 200
 
-    def add(self, value, *, key=None):
+    def add(self, value: Dict, *, key=None):
         """Append a job to the queue."""
         if key is None:
             key = str(uuid4())
 
+        payload = Payload(**value)
+
         json = {
             "queue": self.name,
             "job_id": key,
-            "payload": msgpack.packb(value, use_bin_type=True),
+            "payload": payload.serialize(),
             "ttl": self.ttl,
         }
         # ues msgpack to serialize the data. Bytes are the most efficient.
         res = requests.put(
-            self.host + "/jobs",
+            self.uri + "/tasks",
             msgpack.packb(json, use_bin_type=True),
         )
         if res.status_code == 200:
             return key
-        raise Exception(f"Failed to add job to {self.host}.")
+        raise Exception(f"Failed to add job to {self.uri}.", res.content)
 
     def take(self):
         """Grab a job that has not been grabbed from the queue."""
         response = requests.post(
-            self.host + "/jobs",
+            self.uri + "/tasks",
             json={"queue": self.name},
         )
 
         if response.status_code != 200:
-            raise Exception(f"Failed to grab job from {self.host}.")
+            raise Exception(f"Failed to grab job from {self.uri}.", response.content)
+
         elif response.text == "EMPTY":
             return
 
         data = msgpack.loads(response.content)
         # print("take ==> ", data)
         payload = data.get("payload", None)
-        return data["job_id"], msgpack.unpackb(payload) if payload else None
+        return data["job_id"], Payload.deserialize(payload) if payload else None
 
     def mark_done(self, job_id):
         """Mark a job as done."""
         res = requests.delete(
-            self.host + "/jobs", json={"queue": self.name, "job_id": job_id}
+            self.uri + "/tasks", json={"queue": self.name, "job_id": job_id}
         )
         if res.status_code == 200:
             return True
-        raise Exception(f"Failed to mark job as done on {self.host}.")
+        raise Exception(f"Failed to mark job as done on {self.uri}.", res.content)
 
     def mark_reset(self, job_id):
         res = requests.post(
-            self.host + "/jobs/reset",
-            json={"queue": self.name, "job_id": job_id, "op": "reset"},
+            self.uri + "/tasks/reset",
+            json={"queue": self.name, "job_id": job_id},
         )
         if res.status_code == 200:
             return True
-        raise Exception(f"Failed to reset job on {self.host}.")
+        raise Exception(f"Failed to reset job on {self.uri}.", res.content)
 
     @contextmanager
     def pop(self):
         """Pop a job from the queue."""
         job_tuple = self.take()
         if not job_tuple:
             yield None
```

## zaku/interfaces.py

```diff
@@ -1,43 +1,148 @@
+from io import BytesIO
 from time import time
 from types import SimpleNamespace
-from typing import Literal, Any, Tuple, Coroutine
+from typing import Literal, Any, Tuple, Coroutine, Dict, Union
 
 import msgpack
+import numpy as np
 import redis
 from redis import ResponseError
 from redis.commands.search.query import Query
 from redis.commands.search.result import Result
 
+ZType = Literal["numpy.ndarray", "torch.Tensor", "generic"]
 
-# class Message(NamedTuple):
-#     op: Literal["add", "take", "delete", "reset"]
-#     queue: str
-#     key: str
-#     value: Any = None
+
+class ZData:
+    # data_types = {
+    #     "numpy.ndarray":
+    # }
+
+    @staticmethod
+    def encode(data: Union["torch.Tensor", np.ndarray]):
+        """This converts arrays and tensors to z-format."""
+        import torch
+
+        T = type(data)
+        from PIL.Image import Image
+
+        if isinstance(data, Image):
+            # we always move to CPU
+            with BytesIO() as buffer:
+                # use the format of the Image object, default to PNG.
+                data.save(buffer, format=data.format or "PNG")
+                binary = buffer.getvalue()
+
+            return dict(ztype="image", b=binary)
+        elif T is np.ndarray:
+            # need to support other numpy array types, including mask.
+            binary = data.tobytes()
+            return dict(
+                ztype="numpy.ndarray",
+                b=binary,
+                dtype=str(data.dtype),
+                shape=data.shape,
+            )
+        elif T is torch.Tensor:
+            # we always move to CPU
+            np_v = data.cpu().numpy()
+            binary = np_v.tobytes()
+            return dict(
+                ztype="torch.Tensor",
+                b=binary,
+                dtype=str(np_v.dtype),
+                shape=np_v.shape,
+            )
+        else:
+            return data
+            # return dict(ztype="generic", b=data)
+
+    @staticmethod
+    def get_ztype(data: Dict) -> Union[ZType, None]:
+        """check if it is z-payload"""
+        if type(data) is dict and "ztype" in data:
+            return data["ztype"]
+
+    @staticmethod
+    def decode(zdata):
+        import torch
+
+        T = ZData.get_ztype(zdata)
+        if not T:
+            return zdata
+        elif T == "image":
+            from PIL import Image
+
+            buff = BytesIO(zdata['b'])
+            image = Image.open(buff)
+            return image
+
+        elif T == "numpy.ndarray":
+            # need to support other numpy array types, including mask.
+            array = np.frombuffer(zdata["b"], dtype=zdata["dtype"])
+            array = array.reshape(zdata["shape"])
+            return array
+        elif T == "torch.Tensor":
+            array = np.frombuffer(zdata["b"], dtype=zdata["dtype"])
+            # we copy the array because the buffered version is non-writable.
+            array = array.reshape(zdata["shape"]).copy()
+            torch_array = torch.Tensor(array)
+            return torch_array
+        else:
+            raise TypeError(f"ZData type {T} is not supported")
+
+
+class Payload(SimpleNamespace):
+    # class attributes are not serialized.
+    greedy = True
+    """Set to False to avoid greedy convertion, and make it go faster"""
+
+    def __init__(self, _greedy=None, **payload):
+        if _greedy:
+            self.greedy = _greedy
+
+        super().__init__(**payload)
+
+    def serialize(self):
+        payload = self.__dict__
+        # we serialize components key value pairs
+        if self.greedy:
+            data = {k: ZData.encode(v) for k, v in payload.items()}
+            data["_greedy"] = self.greedy
+            msg = msgpack.packb(data, use_bin_type=True)
+        else:
+            msg = msgpack.packb(payload, use_bin_type=True)
+
+        return msg
+
+    @staticmethod
+    def deserialize(payload) -> Dict:
+        unpacked = msgpack.unpackb(payload, raw=False)
+        is_greedy = unpacked.pop("_greedy", None)
+        if not is_greedy:
+            return unpacked
+        else:
+            data = {}
+
+            for k, v in unpacked.items():
+                data[k] = ZData.decode(v)
+
+            return data
 
 
 class Job(SimpleNamespace):
     created_ts: float
     status: Literal[None, "in_progress", "created"] = "created"
     grab_ts: float = None
     # value: Any = None
     # payload: bytes = None
     # """This is the binary encoding from the msgpack. """
     ttl: float = None
 
-    def serialize(self):
-        msg = msgpack.packb(vars(self), use_bin_type=True)
-        return msg
-
-    @staticmethod
-    async def deserialize(payload) -> "Job":
-        data = msgpack.unpackb(payload, raw=False)
-        return Job(**data)
-
     @staticmethod
     async def create_queue(r: redis.asyncio.Redis, name, *, prefix, smart=True):
         from redis.commands.search.field import TagField, NumericField
         from redis.commands.search.indexDefinition import IndexType, IndexDefinition
 
         index_name = f"{prefix}:{name}"
         index_prefix = f"{prefix}:{name}:"
@@ -54,15 +159,14 @@
         try:
             await r.ft(index_name).create_index(
                 schema,
                 definition=IndexDefinition(
                     prefix=[index_prefix],
                     index_type=IndexType.JSON,
                 ),
-
             )
         except ResponseError:
             if not smart:
                 return
 
             await r.ft(index_name).dropindex()
             await r.ft(index_name).create_index(
@@ -74,15 +178,14 @@
             )
 
     @staticmethod
     async def remove_queue(r: redis.asyncio.Redis, queue, *, prefix):
         index_name = f"{prefix}:{queue}"
         return await r.ft(index_name).dropindex()
 
-
     @staticmethod
     def add(
         r: redis.asyncio.Redis,
         queue: str,
         *,
         prefix: str,
         # value: Any,
@@ -139,15 +242,25 @@
         entry_name = f"{prefix}:{queue}:{job_id}"
 
         p = r.pipeline()
         response = p.json().delete(entry_name).delete(entry_name + ".payload").execute()
         return response
 
     @staticmethod
-    def reset_stale(r: redis.asyncio.Redis, queue, *, prefix, ttl=None):
+    def reset(r: redis.asyncio.Redis, job_id, queue, *, prefix):
+        entry_name = f"{prefix}:{queue}:{job_id}"
+
+        p = r.pipeline()
+        p = p.json().set(entry_name, "$.status", "created")
+        p = p.json().set(entry_name, "$.grab_ts", None)
+
+        return p.execute()
+
+    @staticmethod
+    def timeout(r: redis.asyncio.Redis, queue, *, prefix, ttl=None):
         index_name = f"{prefix}:{queue}"
 
         if ttl:
             result = r.ft(index_name).search(
                 "@status: { in_progress } @grab_ts: < {time() - ttl}"
             )
         else:
```

## zaku/server.py

```diff
@@ -1,52 +1,76 @@
 import msgpack
 import redis
 from aiohttp import web
-from params_proto import Proto, PrefixProto, ParamsProto
+from params_proto import Proto, ParamsProto
 
 from zaku.base import Server
 from zaku.interfaces import Job
 
 DEFAULT_PORT = 9000
 
 
-class Redis(PrefixProto):
-    host = Proto(env="REDIS_HOST", default="localhost")
-    port = Proto(env="REDIS_PORT", default=6379)
-    password = Proto(env="REDIS_PASSWORD")
-    db = Proto(env="REDIS_DB", default=0)
+class Redis(ParamsProto, prefix="redis", cli_parse=False):
+    """Redis Configuration for the TaskServer class.
 
+    .. code-block:: shell
 
-class QServer(ParamsProto, Server):
-    """TaskQ Server
+        # Put this into an .env file
+        REDIS_HOST=localhost
+        REDIS_PORT=6379
+        REDIS_PASSWORD=xxxxxxxxxxxxxxxxxxx
+        REDIS_DB=0
+
+    CLI Options::
+
+        --redis.host      :str 'localhost'
+        --redis.port      :int 6379
+        --redis.password  :any None
+        --redis.db        :any 0
+    """
+
+    host: str = Proto("localhost", env="REDIS_HOST")
+    port: int = Proto(6379, env="REDIS_PORT")
+    password: str = Proto(env="REDIS_PASSWORD")
+    db: int = Proto(0, env="REDIS_DB")
+    """The logical redis database, from 0 - 15. """
+
+
+class TaskServer(ParamsProto, Server):
+    """TaskServer
+
+    This is the server that maintains the Task Queue.
 
-    This is the server for the Vuer client.
+    Usage
 
-    Usage::
+    .. code-block:: python
 
-        app = QServer()
+        app = TaskServer()
         app.run()
 
-    Arguments::
+    CLI Options
 
-        port: int = 8012
-            The port to run the server on.
-        free_port: bool = True
-            If True, kill the port before starting the server.
-        static_root: str = "."
-            The root directory to serve static files from.
-        cors: str = "https://vuer.ai,https://dash.ml,http://localhost:8000,http://
-            The CORS policy to use. Defaults to allow all.
-        cert: str = None
-            The path to the SSL certificate.
+    .. code-block:: shell
 
-    .. automethod:: run
+        python -m zaku.server --help
+
+        -h, --help          show this help message and exit
+        --prefix          :str 'Zaku-task-queues'
+        --queue-len       :int 100
+        --port            :int 9000
+        --free-port       :bool True
+        --static-root     :str '.'
+        --cors            :str 'https://vuer.ai,https://dash.ml,http://lo...
+        --cert            :str None the path to the SSL certificate
+        --key             :str None the path to the SSL key
+        --ca-cert         :str None the trusted root CA certificates
+        --REQUEST-MAX-SIZE  :int 100000000 the maximum packet size
     """
 
-    prefix = "TaskQ-queues"
+    prefix = "Zaku-task-queues"
 
     # Queue Parameters
     queue_len = 100  # use a max length to avoid the memory from blowing up.
 
     # Server Parameters
     port = DEFAULT_PORT
     free_port = True
@@ -56,20 +80,21 @@
     )
 
     # SSL Parameters
     cert = Proto(None, dtype=str, help="the path to the SSL certificate")
     key = Proto(None, dtype=str, help="the path to the SSL key")
     ca_cert = Proto(None, dtype=str, help="the trusted root CA certificates")
 
+    REQUEST_MAX_SIZE = Proto(100_000_000, env="WEBSOCKET_MAX_SIZE", help="the maximum packet size")
+
     def __post_init__(self):
         Server.__post_init__(self)
 
         self.redis = redis.asyncio.Redis(**vars(Redis))
 
-    # @add_route("/", method="POST)
     async def create_queue(self, request: web.Request):
         data = await request.json()
         # print("==>", data)
         try:
             await Job.create_queue(self.redis, **data, prefix=self.prefix)
         except Exception:
             return web.Response(text="index already exists", status=400)
@@ -87,24 +112,26 @@
         data = await request.json()
         # print("==>", data)
         await Job.reset(self.redis, **data, prefix=self.prefix)
         return web.Response(text="OK")
 
     async def remove_handle(self, request: web.Request):
         data = await request.json()
-        print("remove ==>", data)
+        # print("remove ==>", data)
         await Job.remove(self.redis, **data, prefix=self.prefix)
         return web.Response(text="OK")
 
     async def take_handler(self, request):
         data = await request.json()
         # print("take ==> data", data)
         job_id, payload = await Job.take(self.redis, **data, prefix=self.prefix)
         if payload:
-            msg = msgpack.packb({"job_id": job_id, "payload": payload}, use_bin_type=True)
+            msg = msgpack.packb(
+                {"job_id": job_id, "payload": payload}, use_bin_type=True
+            )
             return web.Response(body=msg, status=200)
         else:
             return web.Response(text="EMPTY", status=200)
 
     def run(self, kill=None, *args, **kwargs):
         import os
 
@@ -113,24 +140,27 @@
             from killport import kill_ports
 
             kill_ports(ports=[self.port])
             time.sleep(0.01)
 
         # use the same endpoint for websocket and file serving.
         self._route("/queues", self.create_queue, method="PUT")
-        self._route("/jobs", self.add_job, method="PUT")
-        self._route("/jobs", self.take_handler, method="POST")
-        self._route("/jobs/reset", self.reset_handler, method="POST")
-        self._route("/jobs", self.remove_handle, method="DELETE")
+        self._route("/tasks", self.add_job, method="PUT")
+        self._route("/tasks", self.take_handler, method="POST")
+        self._route("/tasks/reset", self.reset_handler, method="POST")
+        self._route("/tasks", self.remove_handle, method="DELETE")
 
         # serve local files via /static endpoint
         self._static("/static", self.static_root)
         print("Serving file://" + os.path.abspath(self.static_root), "at", "/static")
 
         print("redis server is now connected")
         print(f"serving at http://localhost:{self.port}")
         super().run()
 
 
+def entry_point():
+    TaskServer().run()
+
+
 if __name__ == "__main__":
-    # from zaku.server import QServer
-    QServer().run()
+    entry_point()
```

## Comparing `zaku-0.0.2.dist-info/LICENSE` & `zaku-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zaku-0.0.2.dist-info/METADATA` & `zaku-0.0.3.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: zaku
-Version: 0.0.2
+Version: 0.0.3
+Summary: Zaku Task Queue is for distributed ML-workloads.
 Home-page: https://github.com/geyang/zaku
 Author: Ge Yang<ge.ike.yang@gmail.com>
 Author-email: ge.ike.yang@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
@@ -16,21 +17,25 @@
 Requires-Dist: numpy >=1.21
 Requires-Dist: websockets
 Provides-Extra: all
 Requires-Dist: aiohttp ; extra == 'all'
 Requires-Dist: aiohttp-cors ; extra == 'all'
 Requires-Dist: killport ; extra == 'all'
 Provides-Extra: dev
+Requires-Dist: restructuredtext-lint ; extra == 'dev'
+Requires-Dist: twine ; extra == 'dev'
 Requires-Dist: aiohttp ; extra == 'dev'
 Requires-Dist: aiohttp-cors ; extra == 'dev'
 Requires-Dist: killport ; extra == 'dev'
 Requires-Dist: black ==22.3.0 ; extra == 'dev'
 Requires-Dist: pylint ==2.13.4 ; extra == 'dev'
 Requires-Dist: pytest ==7.1.2 ; extra == 'dev'
 Requires-Dist: sphinx ==7.1.2 ; extra == 'dev'
+Requires-Dist: pytest-asyncio ; extra == 'dev'
+Requires-Dist: pytest-dependency ; extra == 'dev'
 Requires-Dist: furo ; extra == 'dev'
 Requires-Dist: sphinx-copybutton ; extra == 'dev'
 Requires-Dist: myst-parser ; extra == 'dev'
 Requires-Dist: trimesh ; extra == 'dev'
 Requires-Dist: tqdm ; extra == 'dev'
 Provides-Extra: example
 Requires-Dist: aiohttp ; extra == 'example'
@@ -53,33 +58,49 @@
 
 Install zaku --- the latest version is `{VERSION}` on [pypi](https://pypi.org/project/zaku/{VERSION}/).
 
 ```python
 pip install -U 'zaku[all]=={VERSION}'
 ```
 
-Supposed you have a JobServer running at `localhost:9000`.
+**Setting Up Zaku Server**
+
+The server script is installed as the command `zaku`. First, take a look at its options by running
+
+```shell
+zaku -h
+```
+
+This should show you the documents on all of the arguments. Now, to setup a zaku task queue server, run the following: This enables access from other than localhost.
+
+````shell
+zaku --host 0.0.0.0 --port 9000
+````
+
+
 
 **Adding Jobs**:
 
+Supposed you have a TaskServer running at `localhost:9000`.
+
 ```python
 from zaku import TaskQ
 
-queue = TaskQ(name="my-test-queue", host="localhost", port=9000)
+queue = TaskQ(name="my-test-queue", uri="http://localhost:9000")
 
 for i in range(100):
     queue.add_job({"job_id": i, "seed": i * 100})
 ```
 
 **Retrieving Jobs**:
 
 ```python
 from zaku import TaskQ
 
-queue = TaskQ(name="my-test-queue", host="localhost", port=9000)
+queue = TaskQ(name="my-test-queue", uri="http://localhost:9000")
 
 job_id, job = queue.take()
 ```
 
 Now, after you have finished the job, you need to mark the job for completion. The way we do so is by calling
 
 ```python
@@ -93,15 +114,15 @@
 ```
 
 Now, we offer a context manager `TaskQ.pop`, which automatically catches exceptions and resets the job (or marks it complete).
 
 ```python
 from zaku import TaskQ
 
-queue = TaskQ(name="my-test-queue", host="localhost", port=9000)
+queue = TaskQ(name="my-test-queue", uri="http://localhost:9000")
 
 with queue.pop() as job:
   if job is None:
     print("No job available")
   
   print("Retrieved job:", job)
 ```
@@ -109,15 +130,15 @@
 ## Developing Zaku (Optional)
 
 If you want to develop zaku, you can install it in editable mode plus dependencies
 relevant for building the documentations:
 
 ```shell
 cd zaku
-pip install -e '.[all]'
+pip install -e '.[dev]'
 ```
 
 To build the documentations, run
 
 ```shell
 make docs
 ```
```

