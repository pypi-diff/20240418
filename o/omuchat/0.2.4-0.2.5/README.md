# Comparing `tmp/omuchat-0.2.4.tar.gz` & `tmp/omuchat-0.2.5.tar.gz`

## Comparing `omuchat-0.2.4.tar` & `omuchat-0.2.5.tar`

### file list

```diff
@@ -1,23 +1,20 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuchat-0.2.4/.python-version
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omuchat-0.2.4/.vscode/settings.json
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 omuchat-0.2.4/example/chatlogger.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/__init__.py
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/chat.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/client.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/event/__init__.py
--rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/event/event.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/event/event_types.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/model/__init__.py
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/model/author.py
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/model/channel.py
--rw-r--r--   0        0        0     6862 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/model/content.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/model/gift.py
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/model/message.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/model/paid.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/model/provider.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/model/role.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/model/room.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 omuchat-0.2.4/.gitignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 omuchat-0.2.4/README.md
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 omuchat-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 omuchat-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/__init__.py
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/chat.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/client.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/event/__init__.py
+-rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/event/event.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/event/event_types.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/model/__init__.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/model/author.py
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/model/channel.py
+-rw-r--r--   0        0        0     6862 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/model/content.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/model/gift.py
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/model/message.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/model/paid.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/model/provider.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/model/role.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/model/room.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuchat-0.2.5/.gitignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 omuchat-0.2.5/README.md
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 omuchat-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 omuchat-0.2.5/PKG-INFO
```

### Comparing `omuchat-0.2.4/src/omuchat/chat.py` & `omuchat-0.2.5/src/omuchat/chat.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.4/src/omuchat/client.py` & `omuchat-0.2.5/src/omuchat/client.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.4/src/omuchat/event/event.py` & `omuchat-0.2.5/src/omuchat/event/event.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.4/src/omuchat/event/event_types.py` & `omuchat-0.2.5/src/omuchat/event/event_types.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.4/src/omuchat/model/author.py` & `omuchat-0.2.5/src/omuchat/model/author.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,27 +16,27 @@
     description: NotRequired[str | None]
     links: NotRequired[List[str] | None]
 
 
 class AuthorJson(TypedDict):
     provider_id: str
     id: str
-    name: str
+    name: NotRequired[str] | None
     avatar_url: NotRequired[str] | None
     roles: NotRequired[List[RoleJson]] | None
     metadata: NotRequired[AuthorMetadata] | None
 
 
 class Author(Keyable, Model[AuthorJson]):
     def __init__(
         self,
         *,
         provider_id: str,
         id: str,
-        name: str,
+        name: str | None = None,
         avatar_url: str | None = None,
         roles: List[Role] | None = None,
         metadata: AuthorMetadata | None = None,
     ) -> None:
         self.provider_id = provider_id
         self.id = id
         self.name = name
```

### Comparing `omuchat-0.2.4/src/omuchat/model/channel.py` & `omuchat-0.2.5/src/omuchat/model/channel.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.4/src/omuchat/model/content.py` & `omuchat-0.2.5/src/omuchat/model/content.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.4/src/omuchat/model/gift.py` & `omuchat-0.2.5/src/omuchat/model/gift.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.4/src/omuchat/model/message.py` & `omuchat-0.2.5/src/omuchat/model/message.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
+from dataclasses import dataclass
 from datetime import datetime
 from typing import List, NotRequired, TypedDict
 
 from omu.helper import map_optional
+from omu.identifier import Identifier
 from omu.interface import Keyable
 from omu.model import Model
 
 from . import content
 from .gift import Gift, GiftJson
 from .paid import Paid, PaidJson
 
@@ -18,71 +20,56 @@
     author_id: NotRequired[str] | None
     content: NotRequired[content.ComponentJson] | None
     paid: NotRequired[PaidJson] | None
     gifts: NotRequired[List[GiftJson]] | None
     created_at: NotRequired[str] | None  # ISO 8601 date string
 
 
+@dataclass
 class Message(Keyable, Model[MessageJson]):
-    def __init__(
-        self,
-        *,
-        room_id: str,
-        id: str,
-        author_id: str | None = None,
-        content: content.Component | None = None,
-        paid: Paid | None = None,
-        gifts: List[Gift] | None = None,
-        created_at: datetime | None = None,
-    ) -> None:
-        if created_at and not isinstance(created_at, datetime):
-            raise TypeError(f"created_at must be datetime, not {type(created_at)}")
-        self.room_id = room_id
-        self.id = id
-        self.content = content
-        self.author_id = author_id
-        self.paid = paid
-        self.gifts = gifts
-        self.created_at = created_at
+    room_id: str
+    id: Identifier
+    author_id: str | None = None
+    content: content.Component | None = None
+    paid: Paid | None = None
+    gifts: List[Gift] | None = None
+    created_at: datetime | None = None
 
     @classmethod
     def from_json(cls, json: MessageJson) -> Message:
         created_at = None
         if json.get("created_at") and json["created_at"]:
             created_at = datetime.fromisoformat(json["created_at"])
 
         return cls(
             room_id=json["room_id"],
-            id=json["id"],
+            id=Identifier.from_key(json["id"]),
             author_id=json.get("author_id"),
             content=map_optional(json.get("content"), content.deserialize),
             paid=map_optional(json.get("paid"), Paid.from_json),
             gifts=map_optional(
                 json.get("gifts"),
                 lambda gifts: list(map(Gift.from_json, gifts)),
                 [],
             ),
             created_at=created_at,
         )
 
-    @property
-    def text(self) -> str:
-        if not self.content:
-            return ""
-        return str(self.content)
-
-    def key(self) -> str:
-        return f"{self.room_id}#{self.id}"
-
     def to_json(self) -> MessageJson:
         return MessageJson(
             room_id=self.room_id,
-            id=self.id,
+            id=self.id.key(),
             author_id=self.author_id,
             content=content.serialize(self.content) if self.content else None,
             paid=self.paid.to_json() if self.paid else None,
             gifts=[gift.to_json() for gift in self.gifts] if self.gifts else None,
             created_at=self.created_at.isoformat() if self.created_at else None,
         )
 
-    def __str__(self) -> str:
-        return f"Message({self.room_id}, {self.id}, {self.author_id}, {self.content}, {self.paid}, {self.gifts}, {self.created_at})"
+    @property
+    def text(self) -> str:
+        if not self.content:
+            return ""
+        return str(self.content)
+
+    def key(self) -> str:
+        return self.id.key()
```

### Comparing `omuchat-0.2.4/src/omuchat/model/paid.py` & `omuchat-0.2.5/src/omuchat/model/paid.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.4/src/omuchat/model/provider.py` & `omuchat-0.2.5/src/omuchat/model/provider.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,71 +1,64 @@
 from __future__ import annotations
 
 from typing import TypedDict
 
+from omu.identifier import Identifier
 from omu.interface import Keyable
 from omu.model import Model
 
 
 class ProviderJson(TypedDict):
     id: str
     url: str
     name: str
     version: str
     repository_url: str
     image_url: str | None
-    description: str
     regex: str
 
 
 class Provider(Keyable, Model[ProviderJson]):
     def __init__(
         self,
         *,
-        id: str,
+        id: Identifier,
         url: str,
         name: str,
         version: str,
         repository_url: str,
-        description: str,
         regex: str,
         image_url: str | None = None,
     ) -> None:
         self.id = id
         self.url = url
         self.name = name
         self.version = version
         self.repository_url = repository_url
         self.image_url = image_url
-        self.description = description
         self.regex = regex
 
     @classmethod
     def from_json(cls, json: ProviderJson) -> Provider:
         return cls(
-            id=json["id"],
+            id=Identifier.from_key(json["id"]),
             url=json["url"],
             name=json["name"],
             version=json["version"],
             repository_url=json["repository_url"],
             image_url=json["image_url"],
-            description=json["description"],
             regex=json["regex"],
         )
 
     def to_json(self) -> ProviderJson:
         return ProviderJson(
-            id=self.id,
+            id=self.id.key(),
             url=self.url,
             name=self.name,
             version=self.version,
             repository_url=self.repository_url,
             image_url=self.image_url,
-            description=self.description,
             regex=self.regex,
         )
 
     def key(self) -> str:
-        return self.id
-
-    def __repr__(self) -> str:
-        return f"Provider({self.key()})"
+        return self.id.key()
```

### Comparing `omuchat-0.2.4/src/omuchat/model/role.py` & `omuchat-0.2.5/src/omuchat/model/role.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.4/src/omuchat/model/room.py` & `omuchat-0.2.5/src/omuchat/model/room.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from datetime import datetime
 from typing import Hashable, Literal, NotRequired, TypedDict
 
 from omu.helper import map_optional
+from omu.identifier import Identifier
 from omu.interface import Keyable
 from omu.model import Model
 
 
 class RoomMetadata(TypedDict):
     url: NotRequired[str]
     title: NotRequired[str]
@@ -32,16 +33,16 @@
     created_at: NotRequired[str] | None  # ISO 8601 date string
 
 
 class Room(Keyable, Model[RoomJson], Hashable):
     def __init__(
         self,
         *,
-        id: str,
-        provider_id: str,
+        id: Identifier,
+        provider_id: Identifier,
         connected: bool,
         status: Status,
         metadata: RoomMetadata | None = None,
         channel_id: str | None = None,
         created_at: datetime | None = None,
     ) -> None:
         self.id = id
@@ -51,36 +52,36 @@
         self.metadata = metadata
         self.channel_id = channel_id
         self.created_at = created_at
 
     @classmethod
     def from_json(cls, json: RoomJson) -> Room:
         return Room(
-            id=json["id"],
-            provider_id=json["provider_id"],
+            id=Identifier.from_key(json["id"]),
+            provider_id=Identifier.from_key(json["provider_id"]),
             connected=json["connected"],
             status=json["status"],
             metadata=json.get("metadata"),
             channel_id=json.get("channel_id"),
             created_at=map_optional(json.get("created_at"), datetime.fromisoformat),
         )
 
     def to_json(self) -> RoomJson:
         return RoomJson(
-            id=self.id,
-            provider_id=self.provider_id,
+            id=self.id.key(),
+            provider_id=self.provider_id.key(),
             connected=self.connected,
             status=self.status,
             metadata=self.metadata,
             channel_id=self.channel_id,
             created_at=map_optional(self.created_at, datetime.isoformat),
         )
 
     def key(self) -> str:
-        return f"{self.id}@{self.provider_id}"
+        return self.id.key()
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, Room):
             return NotImplemented
         return self.key() == other.key()
 
     def __hash__(self) -> int:
```

