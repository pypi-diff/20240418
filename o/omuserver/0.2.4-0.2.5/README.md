# Comparing `tmp/omuserver-0.2.4.tar.gz` & `tmp/omuserver-0.2.5.tar.gz`

## Comparing `omuserver-0.2.4.tar` & `omuserver-0.2.5.tar`

### file list

```diff
@@ -1,54 +1,52 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuserver-0.2.4/.python-version
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omuserver-0.2.4/.vscode/settings.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/__init__.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/__main__.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/config.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/directories.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/helper.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/__init__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/extension.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/asset/__init__.py
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/asset/asset_extension.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/dashboard/__init__.py
--rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/dashboard/dashboard_extension.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/endpoint/__init__.py
--rw-r--r--   0        0        0     6982 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/endpoint/endpoint_extension.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/message/__init__.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/message/message_extension.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/permission/__init__.py
--rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/permission/permission_extension.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/plugin/__init__.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/plugin/plugin_connection.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/plugin/plugin_extension.py
--rw-r--r--   0        0        0     8546 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/plugin/plugin_loader.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/plugin/plugin_session_connection.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/registry/__init__.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/registry/registry.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/registry/registry_extension.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/server/__init__.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/server/server_extension.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/table/__init__.py
--rw-r--r--   0        0        0     8307 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/table/cached_table.py
--rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/table/serialized_table.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/table/server_table.py
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/table/session_table_handler.py
--rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/table/table_extension.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/table/adapters/__init__.py
--rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/table/adapters/sqlitetable.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/table/adapters/tableadapter.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/network/__init__.py
--rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/network/network.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/network/packet_dispatcher.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/security/__init__.py
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/security/security.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/server/__init__.py
--rw-r--r--   0        0        0     6731 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/server/omuserver.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/server/server.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/session/__init__.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/session/aiohttp_connection.py
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/session/session.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 omuserver-0.2.4/test/helper_test.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuserver-0.2.4/.gitignore
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 omuserver-0.2.4/README.md
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 omuserver-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 omuserver-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/__init__.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/__main__.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/config.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/directories.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/helper.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/extension.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/asset/__init__.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/asset/asset_extension.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/dashboard/__init__.py
+-rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/dashboard/dashboard_extension.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/endpoint/__init__.py
+-rw-r--r--   0        0        0     6982 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/endpoint/endpoint_extension.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/message/__init__.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/message/message_extension.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/permission/__init__.py
+-rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/permission/permission_extension.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/plugin/__init__.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/plugin/plugin_connection.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/plugin/plugin_extension.py
+-rw-r--r--   0        0        0     8603 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/plugin/plugin_loader.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/plugin/plugin_session_connection.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/registry/__init__.py
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/registry/registry.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/registry/registry_extension.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/server/__init__.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/server/server_extension.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/table/__init__.py
+-rw-r--r--   0        0        0     8307 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/table/cached_table.py
+-rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/table/serialized_table.py
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/table/server_table.py
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/table/session_table_handler.py
+-rw-r--r--   0        0        0     6715 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/table/table_extension.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/table/adapters/__init__.py
+-rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/table/adapters/sqlitetable.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/extension/table/adapters/tableadapter.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/network/__init__.py
+-rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/network/network.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/network/packet_dispatcher.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/security/__init__.py
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/security/security.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/server/__init__.py
+-rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/server/omuserver.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/server/server.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/session/__init__.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/session/aiohttp_connection.py
+-rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 omuserver-0.2.5/src/omuserver/session/session.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 omuserver-0.2.5/test/helper_test.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuserver-0.2.5/.gitignore
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 omuserver-0.2.5/README.md
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 omuserver-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 omuserver-0.2.5/PKG-INFO
```

### Comparing `omuserver-0.2.4/src/omuserver/__main__.py` & `omuserver-0.2.5/src/omuserver/__main__.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.4/src/omuserver/directories.py` & `omuserver-0.2.5/src/omuserver/directories.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,27 +3,24 @@
 from typing import LiteralString
 
 
 @dataclass
 class Directories:
     data: pathlib.Path
     assets: pathlib.Path
-    plugins: pathlib.Path
 
     @classmethod
     def default(cls):
         cwd = pathlib.Path.cwd()
         return Directories(
             data=cwd / "data",
             assets=cwd / "assets",
-            plugins=cwd / "plugins",
         )
 
     def mkdir(self):
         self.data.mkdir(parents=True, exist_ok=True)
         self.assets.mkdir(parents=True, exist_ok=True)
-        self.plugins.mkdir(parents=True, exist_ok=True)
 
     def get(self, name: LiteralString):
         path = self.data / name
         path.mkdir(parents=True, exist_ok=True)
         return path
```

### Comparing `omuserver-0.2.4/src/omuserver/helper.py` & `omuserver-0.2.5/src/omuserver/helper.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.4/src/omuserver/extension/dashboard/dashboard_extension.py` & `omuserver-0.2.5/src/omuserver/extension/dashboard/dashboard_extension.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.4/src/omuserver/extension/endpoint/endpoint_extension.py` & `omuserver-0.2.5/src/omuserver/extension/endpoint/endpoint_extension.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.4/src/omuserver/extension/message/message_extension.py` & `omuserver-0.2.5/src/omuserver/extension/message/message_extension.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.4/src/omuserver/extension/permission/permission_extension.py` & `omuserver-0.2.5/src/omuserver/extension/permission/permission_extension.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.4/src/omuserver/extension/plugin/plugin_connection.py` & `omuserver-0.2.5/src/omuserver/extension/plugin/plugin_connection.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.4/src/omuserver/extension/plugin/plugin_extension.py` & `omuserver-0.2.5/src/omuserver/extension/plugin/plugin_extension.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     from omuserver.server import Server
 
 
 class PluginExtension:
     def __init__(self, server: Server) -> None:
         self._server = server
         self.lock = asyncio.Lock()
+        server.listeners.start += self.on_server_start
         self.loader = PluginLoader(server)
         self.dependency_resolver = DependencyResolver()
         server.packet_dispatcher.register(
             PLUGIN_REQUIRE_PACKET,
         )
         server.packet_dispatcher.add_packet_handler(
             PLUGIN_REQUIRE_PACKET,
@@ -39,15 +40,14 @@
         server.endpoints.bind_endpoint(
             PLUGIN_WAIT_ENDPOINT,
             self.handle_wait_endpoint,
         )
         server.permissions.register(
             PLUGIN_PERMISSION,
         )
-        server.listeners.start += self.on_server_start
 
     async def on_server_start(self) -> None:
         await self.loader.load_plugins()
 
     async def handle_require_packet(
         self, session: Session, packages: Dict[str, str | None]
     ) -> None:
```

### Comparing `omuserver-0.2.4/src/omuserver/extension/plugin/plugin_loader.py` & `omuserver-0.2.5/src/omuserver/extension/plugin/plugin_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,15 @@
 
 
 class PluginLoader:
     def __init__(self, server: Server) -> None:
         self._server = server
         self.plugins: Dict[str, Plugin] = {}
         server.listeners.start += self.handle_server_start
+        server.listeners.stop += self.handle_server_stop
 
     async def handle_server_start(self) -> None:
         for plugin in self.plugins.values():
             if plugin.on_start_server is not None:
                 await plugin.on_start_server(self._server)
 
     async def handle_server_stop(self) -> None:
```

### Comparing `omuserver-0.2.4/src/omuserver/extension/plugin/plugin_session_connection.py` & `omuserver-0.2.5/src/omuserver/extension/plugin/plugin_session_connection.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.4/src/omuserver/extension/registry/registry.py` & `omuserver-0.2.5/src/omuserver/extension/registry/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 class ServerRegistry:
     def __init__(self, server: Server, identifier: Identifier) -> None:
         self.identifier = identifier
         self._listeners: Dict[Identifier, Session] = {}
         self._path = server.directories.get(
             "registry"
-        ) / identifier.to_path().with_suffix(".json")
+        ) / identifier.get_sanitized_path().with_suffix(".json")
         self._changed = False
         self.data: bytes | None = None
 
     async def load(self):
         if self._path.exists():
             self.data = self._path.read_bytes()
```

### Comparing `omuserver-0.2.4/src/omuserver/extension/registry/registry_extension.py` & `omuserver-0.2.5/src/omuserver/extension/registry/registry_extension.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.4/src/omuserver/extension/server/server_extension.py` & `omuserver-0.2.5/src/omuserver/extension/server/server_extension.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.4/src/omuserver/extension/table/cached_table.py` & `omuserver-0.2.5/src/omuserver/extension/table/cached_table.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.4/src/omuserver/extension/table/serialized_table.py` & `omuserver-0.2.5/src/omuserver/extension/table/serialized_table.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.4/src/omuserver/extension/table/server_table.py` & `omuserver-0.2.5/src/omuserver/extension/table/server_table.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.4/src/omuserver/extension/table/session_table_handler.py` & `omuserver-0.2.5/src/omuserver/extension/table/session_table_handler.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.4/src/omuserver/extension/table/table_extension.py` & `omuserver-0.2.5/src/omuserver/extension/table/table_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,14 +174,14 @@
         adapter = SqliteTableAdapter.create(self.get_table_path(identifier))
         await adapter.load()
         table.set_adapter(adapter)
         self._tables[identifier] = table
         return table
 
     def get_table_path(self, identifier: Identifier) -> Path:
-        path = self._server.directories.get("tables") / identifier.to_path()
+        path = self._server.directories.get("tables") / identifier.get_sanitized_path()
         path.parent.mkdir(parents=True, exist_ok=True)
         return path
 
     async def on_server_stop(self) -> None:
         for table in self._tables.values():
             await table.store()
```

### Comparing `omuserver-0.2.4/src/omuserver/extension/table/adapters/sqlitetable.py` & `omuserver-0.2.5/src/omuserver/extension/table/adapters/sqlitetable.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.4/src/omuserver/extension/table/adapters/tableadapter.py` & `omuserver-0.2.5/src/omuserver/extension/table/adapters/tableadapter.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.4/src/omuserver/network/network.py` & `omuserver-0.2.5/src/omuserver/network/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             return
         self._sessions.pop(session.app.key())
         await self._listeners.disconnected.emit(session)
 
     async def _handle_start(self, app: web.Application) -> None:
         await self._listeners.start.emit()
 
-    def is_port_available(self) -> bool:
+    def is_port_free(self) -> bool:
         try:
             with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
                 s.bind(
                     (
                         self._server.address.host or "127.0.0.1",
                         self._server.address.port,
                     )
@@ -118,15 +118,15 @@
     def get_process_by_port(self, port: int) -> psutil.Process | None:
         for connection in psutil.net_connections():
             if connection.laddr and connection.laddr.port == port:
                 return psutil.Process(connection.pid)
         return None
 
     async def start(self) -> None:
-        if not self.is_port_available():
+        if not self.is_port_free():
             process = self.get_process_by_port(self._server.address.port)
             if process is None:
                 raise OSError(f"Port {self._server.address.port} already in use")
             port = self._server.address.port
             name = process.name()
             pid = process.pid
             raise OSError(f"Port {port} already in use by {name} ({pid=})")
```

### Comparing `omuserver-0.2.4/src/omuserver/network/packet_dispatcher.py` & `omuserver-0.2.5/src/omuserver/network/packet_dispatcher.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.4/src/omuserver/security/security.py` & `omuserver-0.2.5/src/omuserver/security/security.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.4/src/omuserver/server/omuserver.py` & `omuserver-0.2.5/src/omuserver/server/omuserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             return web.Response(status=500)
 
     async def _handle_assets(self, request: web.Request) -> web.StreamResponse:
         id = request.query.get("id")
         if not id:
             return web.Response(status=400)
         identifier = Identifier.from_key(id)
-        path = identifier.to_path()
+        path = identifier.get_sanitized_path()
         try:
             path = safe_path_join(self._directories.assets, path)
 
             if not path.exists():
                 return web.Response(status=404)
             return web.FileResponse(path)
         except Exception as e:
```

### Comparing `omuserver-0.2.4/src/omuserver/server/server.py` & `omuserver-0.2.5/src/omuserver/server/server.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.4/src/omuserver/session/aiohttp_connection.py` & `omuserver-0.2.5/src/omuserver/session/aiohttp_connection.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.4/src/omuserver/session/session.py` & `omuserver-0.2.5/src/omuserver/session/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import abc
 import asyncio
 from typing import TYPE_CHECKING, Tuple
 
 from omu.event_emitter import EventEmitter
 from omu.network.packet import PACKET_TYPES, Packet, PacketType
 from omu.network.packet.packet_types import ConnectPacket
-from omu.network.packet_mapper import PacketMapper
-
-from omuserver.server.server import Server
 
 if TYPE_CHECKING:
     from omu import App
+    from omu.network.packet_mapper import PacketMapper
+
+    from omuserver.server import Server
 
 
 class SessionConnection(abc.ABC):
     @abc.abstractmethod
     async def send(self, packet: Packet, packet_mapper: PacketMapper) -> None: ...
 
     @abc.abstractmethod
```

### Comparing `omuserver-0.2.4/pyproject.toml` & `omuserver-0.2.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "omuserver"
-version = "0.2.4"
+version = "0.2.5"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = [
     "sqlitedict>=2.1.0",
     "click>=8.1.7",
```

### Comparing `omuserver-0.2.4/PKG-INFO` & `omuserver-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: omuserver
-Version: 0.2.4
+Version: 0.2.5
 Summary: Add your description here
 Author-email: am230 <111672334+am230@users.noreply.github.com>
 Requires-Python: >=3.12
 Requires-Dist: aiohttp>=3.9.3
 Requires-Dist: aiosqlite>=0.19.0
 Requires-Dist: click>=8.1.7
 Requires-Dist: loguru>=0.7.2
```

