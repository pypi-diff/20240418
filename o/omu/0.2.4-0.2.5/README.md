# Comparing `tmp/omu-0.2.4.tar.gz` & `tmp/omu-0.2.5.tar.gz`

## Comparing `omu-0.2.4.tar` & `omu-0.2.5.tar`

### file list

```diff
@@ -1,65 +1,60 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 omu-0.2.4/.gitattributes
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omu-0.2.4/.prettierrc
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omu-0.2.4/.python-version
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 omu-0.2.4/run_client.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omu-0.2.4/.vscode/settings.json
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/__init__.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/app.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/event_emitter.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/helper.py
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/identifier.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/model.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/plugin.py
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/serializer.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/client/__init__.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/client/client.py
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/client/omuclient.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/extension.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/extension_registry.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/asset/__init__.py
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/asset/asset_extension.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/dashboard/__init__.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/dashboard/dashboard.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/dashboard/dashboard_extension.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/endpoint/__init__.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/endpoint/endpoint.py
--rw-r--r--   0        0        0     6277 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/endpoint/endpoint_extension.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/i18n/__init__.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/i18n/i18n_extension.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/message/__init__.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/message/message.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/message/message_extension.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/permission/__init__.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/permission/permission.py
--rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/permission/permission_extension.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/plugin/__init__.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/plugin/plugin_extension.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/registry/__init__.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/registry/registry.py
--rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/registry/registry_extension.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/server/__init__.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/server/server_extension.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/table/__init__.py
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/table/table.py
--rw-r--r--   0        0        0    15097 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/table/table_extension.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/interface/__init__.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/interface/keyable.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/interface/named.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/localization/__init__.py
--rw-r--r--   0        0        0    33905 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/localization/locale.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/localization/localization.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/network/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/network/address.py
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/network/bytebuffer.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/network/connection.py
--rw-r--r--   0        0        0     5470 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/network/network.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/network/packet_mapper.py
--rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/network/websocket_connection.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/network/packet/__init__.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/network/packet/packet.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/network/packet/packet_types.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 omu-0.2.4/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omu-0.2.4/README.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 omu-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 omu-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/__init__.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/app.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/event_emitter.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/helper.py
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/identifier.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/model.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/plugin.py
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/serializer.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/client/__init__.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/client/client.py
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/client/omuclient.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/__init__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/extension.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/extension_registry.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/asset/__init__.py
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/asset/asset_extension.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/dashboard/__init__.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/dashboard/dashboard.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/dashboard/dashboard_extension.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/endpoint/__init__.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/endpoint/endpoint.py
+-rw-r--r--   0        0        0     6277 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/endpoint/endpoint_extension.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/i18n/__init__.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/i18n/i18n_extension.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/message/__init__.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/message/message.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/message/message_extension.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/permission/__init__.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/permission/permission.py
+-rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/permission/permission_extension.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/plugin/__init__.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/plugin/plugin_extension.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/registry/__init__.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/registry/registry.py
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/registry/registry_extension.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/server/__init__.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/server/server_extension.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/table/__init__.py
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/table/table.py
+-rw-r--r--   0        0        0    15097 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/extension/table/table_extension.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/interface/__init__.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/interface/keyable.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/interface/named.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/localization/__init__.py
+-rw-r--r--   0        0        0    33905 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/localization/locale.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/localization/localization.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/network/__init__.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/network/address.py
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/network/bytebuffer.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/network/connection.py
+-rw-r--r--   0        0        0     5470 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/network/network.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/network/packet_mapper.py
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/network/websocket_connection.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/network/packet/__init__.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/network/packet/packet.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 omu-0.2.5/src/omu/network/packet/packet_types.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omu-0.2.5/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omu-0.2.5/README.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 omu-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 omu-0.2.5/PKG-INFO
```

### Comparing `omu-0.2.4/src/omu/app.py` & `omu-0.2.5/src/omu/app.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,69 @@
 from __future__ import annotations
 
-from typing import Final, NotRequired, TypedDict
+from typing import Final, List, NotRequired, TypedDict
 
 from omu.identifier import Identifier
 from omu.interface import Keyable
 from omu.localization import LocalizedText
 from omu.localization.locale import Locale
 from omu.model import Model
 
 
-class AppLocalization(TypedDict):
+class AppMetadata(TypedDict):
     locale: Locale
     name: NotRequired[LocalizedText]
     description: NotRequired[LocalizedText]
     image: NotRequired[LocalizedText]
     site: NotRequired[LocalizedText]
     repository: NotRequired[LocalizedText]
     authors: NotRequired[LocalizedText]
     license: NotRequired[LocalizedText]
+    tags: NotRequired[List[str]]
 
 
 class AppJson(TypedDict):
     identifier: str
     version: NotRequired[str] | None
     url: NotRequired[str] | None
-    localizations: NotRequired[AppLocalization] | None
+    metadata: NotRequired[AppMetadata] | None
 
 
 class App(Keyable, Model[AppJson]):
     def __init__(
         self,
         identifier: Identifier | str,
         *,
         version: str | None = None,
         url: str | None = None,
-        localizations: AppLocalization | None = None,
+        metadata: AppMetadata | None = None,
     ) -> None:
         if isinstance(identifier, str):
             identifier = Identifier.from_key(identifier)
         self.identifier: Final[Identifier] = identifier
         self.version = version
         self.url = url
-        self.localizations = localizations
+        self.metadata = metadata
 
     @classmethod
     def from_json(cls, json: AppJson) -> App:
         identifier = Identifier.from_key(json["identifier"])
         return cls(
             identifier,
             version=json.get("version"),
             url=json.get("url"),
-            localizations=json.get("localizations"),
+            metadata=json.get("metadata"),
         )
 
     def to_json(self) -> AppJson:
         return AppJson(
             identifier=self.key(),
             version=self.version,
             url=self.url,
-            localizations=self.localizations,
+            metadata=self.metadata,
         )
 
     def key(self) -> str:
         return self.identifier.key()
 
     def __hash__(self) -> int:
         return hash(self.key())
```

### Comparing `omu-0.2.4/src/omu/event_emitter.py` & `omu-0.2.5/src/omu/event_emitter.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/helper.py` & `omu-0.2.5/src/omu/helper.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/identifier.py` & `omu-0.2.5/src/omu/identifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     @classmethod
     def from_json(cls, json: str) -> Identifier:
         return cls.from_key(json)
 
     def key(self) -> str:
         return self.format(self.namespace, *self.path)
 
-    def to_path(self) -> Path:
+    def get_sanitized_path(self) -> Path:
         namespace = (
             f"{sanitize_filename(self.namespace)}-{generate_md5_hash(self.namespace)}"
         )
         return Path(namespace, *self.path)
 
     def is_subpart_of(self, base: Identifier) -> bool:
         return (
```

### Comparing `omu-0.2.4/src/omu/plugin.py` & `omu-0.2.5/src/omu/plugin.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/serializer.py` & `omu-0.2.5/src/omu/serializer.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/client/client.py` & `omu-0.2.5/src/omu/client/client.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/client/omuclient.py` & `omu-0.2.5/src/omu/client/omuclient.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/extension/extension.py` & `omu-0.2.5/src/omu/extension/extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/extension/extension_registry.py` & `omu-0.2.5/src/omu/extension/extension_registry.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/extension/asset/asset_extension.py` & `omu-0.2.5/src/omu/extension/asset/asset_extension.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,115 @@
-from typing import List, Mapping
+from dataclasses import dataclass
+from typing import List
 
 from omu.client import Client
 from omu.extension import Extension, ExtensionType
 from omu.extension.endpoint import EndpointType
 from omu.identifier import Identifier
 from omu.network.bytebuffer import ByteReader, ByteWriter
 from omu.serializer import Serializer
 
 ASSET_EXTENSION_TYPE = ExtensionType(
     "asset",
     lambda client: AssetExtension(client),
     lambda: [],
 )
-type Files = Mapping[Identifier, bytes]
 
 
-class FILES_SERIALIZER:
+@dataclass
+class File:
+    identifier: Identifier
+    buffer: bytes
+
+
+class FileSerializer:
+    @classmethod
+    def serialize(cls, item: File) -> bytes:
+        writer = ByteWriter()
+        writer.write_string(item.identifier.key())
+        writer.write_byte_array(item.buffer)
+        return writer.finish()
+
+    @classmethod
+    def deserialize(cls, item: bytes) -> File:
+        with ByteReader(item) as reader:
+            identifier = Identifier.from_key(reader.read_string())
+            value = reader.read_byte_array()
+        return File(identifier, value)
+
+
+class FileArraySerializer:
     @classmethod
-    def serialize(cls, item: Files) -> bytes:
+    def serialize(cls, item: List[File]) -> bytes:
         writer = ByteWriter()
         writer.write_int(len(item))
-        for identifier, value in item.items():
-            writer.write_string(identifier.key())
-            writer.write_byte_array(value)
+        for file in item:
+            writer.write_string(file.identifier.key())
+            writer.write_byte_array(file.buffer)
         return writer.finish()
 
     @classmethod
-    def deserialize(cls, item: bytes) -> Files:
+    def deserialize(cls, item: bytes) -> List[File]:
         with ByteReader(item) as reader:
             count = reader.read_int()
-            files: Files = {}
+            files: List[File] = []
             for _ in range(count):
                 identifier = Identifier.from_key(reader.read_string())
                 value = reader.read_byte_array()
-                files[identifier] = value
+                files.append(File(identifier, value))
         return files
 
 
-ASSET_UPLOAD_ENDPOINT = EndpointType[Files, List[Identifier]].create_serialized(
+ASSET_UPLOAD_ENDPOINT = EndpointType[File, Identifier].create_serialized(
     ASSET_EXTENSION_TYPE,
     "upload",
-    request_serializer=FILES_SERIALIZER,
+    request_serializer=FileSerializer,
+    response_serializer=Serializer.model(Identifier).to_json(),
+)
+ASSET_UPLOAD_MANY_ENDPOINT = EndpointType[
+    List[File], List[Identifier]
+].create_serialized(
+    ASSET_EXTENSION_TYPE,
+    "upload_many",
+    request_serializer=FileArraySerializer,
     response_serializer=Serializer.model(Identifier).to_array().to_json(),
 )
-ASSET_DOWNLOAD_ENDPOINT = EndpointType[List[Identifier], Files].create_serialized(
+ASSET_DOWNLOAD_ENDPOINT = EndpointType[Identifier, File].create_serialized(
     ASSET_EXTENSION_TYPE,
     "download",
+    request_serializer=Serializer.model(Identifier).to_json(),
+    response_serializer=FileSerializer,
+)
+ASSET_DOWNLOAD_MANY_ENDPOINT = EndpointType[
+    List[Identifier], List[File]
+].create_serialized(
+    ASSET_EXTENSION_TYPE,
+    "download_many",
     request_serializer=Serializer.model(Identifier).to_array().to_json(),
-    response_serializer=FILES_SERIALIZER,
+    response_serializer=FileArraySerializer,
 )
 
 
 class AssetExtension(Extension):
     def __init__(self, client: Client) -> None:
         self.client = client
 
-    async def upload(self, assets: Files) -> List[Identifier]:
-        return await self.client.endpoints.call(ASSET_UPLOAD_ENDPOINT, assets)
+    async def upload(self, file: File) -> Identifier:
+        return await self.client.endpoints.call(ASSET_UPLOAD_ENDPOINT, file)
+
+    async def upload_many(self, files: List[File]) -> List[Identifier]:
+        return await self.client.endpoints.call(ASSET_UPLOAD_MANY_ENDPOINT, files)
+
+    async def download(self, identifier: Identifier) -> File:
+        return await self.client.endpoints.call(ASSET_DOWNLOAD_ENDPOINT, identifier)
 
-    async def download(self, identifiers: List[Identifier]) -> Files:
-        return await self.client.endpoints.call(ASSET_DOWNLOAD_ENDPOINT, identifiers)
+    async def download_many(self, identifiers: List[Identifier]) -> List[File]:
+        return await self.client.endpoints.call(
+            ASSET_DOWNLOAD_MANY_ENDPOINT, identifiers
+        )
 
     def url(self, identifier: Identifier) -> str:
         address = self.client.network.address
         protocol = "https" if address.secure else "http"
         return f"{protocol}://{address.host}:{address.port}/asset?id={identifier.key()}"
 
     def proxy(self, url: str) -> str:
```

### Comparing `omu-0.2.4/src/omu/extension/dashboard/dashboard.py` & `omu-0.2.5/src/omu/extension/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/extension/dashboard/dashboard_extension.py` & `omu-0.2.5/src/omu/extension/dashboard/dashboard_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/extension/endpoint/endpoint.py` & `omu-0.2.5/src/omu/extension/endpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/extension/endpoint/endpoint_extension.py` & `omu-0.2.5/src/omu/extension/endpoint/endpoint_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/extension/i18n/i18n_extension.py` & `omu-0.2.5/src/omu/extension/i18n/i18n_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/extension/message/message.py` & `omu-0.2.5/src/omu/extension/message/message.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/extension/message/message_extension.py` & `omu-0.2.5/src/omu/extension/message/message_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/extension/permission/permission.py` & `omu-0.2.5/src/omu/extension/permission/permission.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/extension/permission/permission_extension.py` & `omu-0.2.5/src/omu/extension/permission/permission_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/extension/plugin/plugin_extension.py` & `omu-0.2.5/src/omu/extension/plugin/plugin_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/extension/registry/registry.py` & `omu-0.2.5/src/omu/extension/registry/registry.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/extension/registry/registry_extension.py` & `omu-0.2.5/src/omu/extension/registry/registry_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/extension/server/server_extension.py` & `omu-0.2.5/src/omu/extension/server/server_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/extension/table/table.py` & `omu-0.2.5/src/omu/extension/table/table.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/extension/table/table_extension.py` & `omu-0.2.5/src/omu/extension/table/table_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/localization/locale.py` & `omu-0.2.5/src/omu/localization/locale.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/network/bytebuffer.py` & `omu-0.2.5/src/omu/network/bytebuffer.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/network/connection.py` & `omu-0.2.5/src/omu/network/connection.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/network/network.py` & `omu-0.2.5/src/omu/network/network.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/network/packet_mapper.py` & `omu-0.2.5/src/omu/network/packet_mapper.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/network/websocket_connection.py` & `omu-0.2.5/src/omu/network/websocket_connection.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/network/packet/packet.py` & `omu-0.2.5/src/omu/network/packet/packet.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/src/omu/network/packet/packet_types.py` & `omu-0.2.5/src/omu/network/packet/packet_types.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.4/pyproject.toml` & `omu-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "omu"
-version = "0.2.4"
+version = "0.2.5"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = ["loguru>=0.7.2"]
 readme = "README.md"
 requires-python = ">= 3.12"
```

