# Comparing `tmp/deltachat-rpc-client-1.137.2.tar.gz` & `tmp/deltachat_rpc_client-1.137.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltachat-rpc-client-1.137.2.tar", last modified: Fri Apr  5 14:31:43 2024, max compression
+gzip compressed data, was "deltachat_rpc_client-1.137.3.tar", last modified: Thu Apr 18 03:06:39 2024, max compression
```

## Comparing `deltachat-rpc-client-1.137.2.tar` & `deltachat_rpc_client-1.137.3.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:43.436153 deltachat-rpc-client-1.137.2/
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-05 14:31:43.436153 deltachat-rpc-client-1.137.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:31:43.436153 deltachat-rpc-client-1.137.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:43.432152 deltachat-rpc-client-1.137.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:43.436153 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    10117 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/deltachat.py
--rw-r--r--   0 runner    (1001) docker     (127)     9853 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/message.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/pytestplugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6391 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/rpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:43.436153 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-05 14:31:43.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-05 14:31:43.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:31:43.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-05 14:31:43.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 14:31:43.000000 deltachat-rpc-client-1.137.2/src/deltachat_rpc_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:31:43.436153 deltachat-rpc-client-1.137.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    22608 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/tests/test_securejoin.py
--rw-r--r--   0 runner    (1001) docker     (127)    14930 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/tests/test_something.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-05 14:31:34.000000 deltachat-rpc-client-1.137.2/tests/test_webxdc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:06:39.613222 deltachat_rpc_client-1.137.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-18 03:06:39.613222 deltachat_rpc_client-1.137.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 03:06:39.613222 deltachat_rpc_client-1.137.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:06:39.605222 deltachat_rpc_client-1.137.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:06:39.609222 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13391 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/deltachat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/direct_imap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/pytestplugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:06:39.613222 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-18 03:06:39.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-18 03:06:39.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 03:06:39.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-18 03:06:39.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 03:06:39.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 03:06:39.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:06:39.613222 deltachat_rpc_client-1.137.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/tests/test_chatlist_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24172 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/tests/test_securejoin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21143 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/tests/test_something.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/tests/test_webxdc.py
```

### Comparing `deltachat-rpc-client-1.137.2/LICENSE` & `deltachat_rpc_client-1.137.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.137.2/PKG-INFO` & `deltachat_rpc_client-1.137.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat-rpc-client
-Version: 1.137.2
+Version: 1.137.3
 Summary: Python client for Delta Chat core JSON-RPC interface
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Communications :: Email
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: imap-tools
 
 # Delta Chat RPC python client
 
 RPC client connects to standalone Delta Chat RPC server `deltachat-rpc-server`
 and provides asynchronous interface to it.
 
 ## Getting started
```

### Comparing `deltachat-rpc-client-1.137.2/README.md` & `deltachat_rpc_client-1.137.3/README.md`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.137.2/pyproject.toml` & `deltachat_rpc_client-1.137.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "deltachat-rpc-client"
-version = "1.137.2"
+version = "1.137.3"
 description = "Python client for Delta Chat core JSON-RPC interface"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS :: MacOS X",
@@ -17,14 +17,17 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Communications :: Chat",
     "Topic :: Communications :: Email"
 ]
 readme = "README.md"
+dependencies = [
+    "imap-tools",
+]
 
 [tool.setuptools.package-data]
 deltachat_rpc_client = [
     "py.typed"
 ]
 
 [project.entry-points.pytest11]
```

### Comparing `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/__init__.py` & `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/_utils.py` & `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,19 @@
         account = accounts[0] if accounts else deltachat.add_account()
 
         client = client_type(account, hooks)
         client.logger.debug("Running deltachat core %s", core_version)
         if not client.is_configured():
             assert args.email, "Account is not configured and email must be provided"
             assert args.password, "Account is not configured and password must be provided"
-            configure_thread = Thread(run=client.configure, kwargs={"email": args.email, "password": args.password})
+            configure_thread = Thread(
+                target=client.configure,
+                daemon=True,
+                kwargs={"email": args.email, "password": args.password},
+            )
             configure_thread.start()
         client.run_forever()
 
 
 def extract_addr(text: str) -> str:
     """extract email address from the given text."""
     match = re.match(r".*\((.+@.+)\)", text)
```

### Comparing `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/account.py` & `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/account.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from __future__ import annotations
+
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Optional, Union
 from warnings import warn
 
 from ._utils import AttrDict, futuremethod
 from .chat import Chat
 from .const import ChatlistFlag, ContactFlag, EventType, SpecialContactId
 from .contact import Contact
 from .message import Message
@@ -24,14 +26,18 @@
     def _rpc(self) -> "Rpc":
         return self.manager.rpc
 
     def wait_for_event(self) -> AttrDict:
         """Wait until the next event and return it."""
         return AttrDict(self._rpc.wait_for_event(self.id))
 
+    def clear_all_events(self):
+        """Removes all queued-up events for a given account. Useful for tests."""
+        self._rpc.clear_all_events(self.id)
+
     def remove(self) -> None:
         """Remove the account."""
         self._rpc.remove_account(self.id)
 
     def start_io(self) -> None:
         """Start the account I/O."""
         self._rpc.start_io(self.id)
@@ -72,19 +78,33 @@
         """
         self.set_config("selfavatar", img_path)
 
     def get_avatar(self) -> Optional[str]:
         """Get self avatar."""
         return self.get_config("selfavatar")
 
+    def check_qr(self, qr):
+        return self._rpc.check_qr(self.id, qr)
+
+    def set_config_from_qr(self, qr: str):
+        self._rpc.set_config_from_qr(self.id, qr)
+
     @futuremethod
     def configure(self):
         """Configure an account."""
         yield self._rpc.configure.future(self.id)
 
+    def bring_online(self):
+        """Start I/O and wait until IMAP becomes IDLE."""
+        self.start_io()
+        while True:
+            event = self.wait_for_event()
+            if event.kind == EventType.IMAP_INBOX_IDLE:
+                break
+
     def create_contact(self, obj: Union[int, str, Contact], name: Optional[str] = None) -> Contact:
         """Create a new Contact or return an existing one.
 
         Calling this method will always result in the same
         underlying contact id.  If there already is a Contact
         with that e-mail address, it is unblocked and its display
         name is updated if specified.
@@ -94,24 +114,29 @@
         """
         if isinstance(obj, int):
             obj = Contact(self, obj)
         if isinstance(obj, Contact):
             obj = obj.get_snapshot().address
         return Contact(self, self._rpc.create_contact(self.id, obj, name))
 
+    def create_chat(self, account: "Account") -> Chat:
+        addr = account.get_config("addr")
+        contact = self.create_contact(addr)
+        return contact.create_chat()
+
     def get_contact_by_id(self, contact_id: int) -> Contact:
         """Return Contact instance for the given contact ID."""
         return Contact(self, contact_id)
 
     def get_contact_by_addr(self, address: str) -> Optional[Contact]:
         """Check if an e-mail address belongs to a known and unblocked contact."""
         contact_id = self._rpc.lookup_contact_id_by_addr(self.id, address)
         return contact_id and Contact(self, contact_id)
 
-    def get_blocked_contacts(self) -> List[AttrDict]:
+    def get_blocked_contacts(self) -> list[AttrDict]:
         """Return a list with snapshots of all blocked contacts."""
         contacts = self._rpc.get_blocked_contacts(self.id)
         return [AttrDict(contact=Contact(self, contact["id"]), **contact) for contact in contacts]
 
     def get_chat_by_contact(self, contact: Union[int, Contact]) -> Optional[Chat]:
         """Return 1:1 chat for a contact if it exists."""
         if isinstance(contact, Contact):
@@ -128,15 +153,15 @@
 
     def get_contacts(
         self,
         query: Optional[str] = None,
         with_self: bool = False,
         verified_only: bool = False,
         snapshot: bool = False,
-    ) -> Union[List[Contact], List[AttrDict]]:
+    ) -> Union[list[Contact], list[AttrDict]]:
         """Get a filtered list of contacts.
 
         :param query: if a string is specified, only return contacts
                       whose name or e-mail matches query.
         :param with_self: if True the self-contact is also included if it matches the query.
         :param only_verified: if True only return verified contacts.
         :param snapshot: If True return a list of contact snapshots instead of Contact instances.
@@ -163,15 +188,15 @@
         query: Optional[str] = None,
         contact: Optional[Contact] = None,
         archived_only: bool = False,
         for_forwarding: bool = False,
         no_specials: bool = False,
         alldone_hint: bool = False,
         snapshot: bool = False,
-    ) -> Union[List[Chat], List[AttrDict]]:
+    ) -> Union[list[Chat], list[AttrDict]]:
         """Return list of chats.
 
         :param query: if a string is specified only chats matching this query are returned.
         :param contact: if a contact is specified only chats including this contact are returned.
         :param archived_only: if True only archived chats are returned.
         :param for_forwarding: if True the chat list is sorted with "Saved messages" at the top
                                and without "Device chat" and contact requests.
@@ -221,50 +246,50 @@
         Subsequent calls of `secure_join()` will abort previous, unfinished handshakes.
         See https://securejoin.readthedocs.io/en/latest/new.html for protocol details.
 
         :param qrdata: The text of the scanned QR code.
         """
         return Chat(self, self._rpc.secure_join(self.id, qrdata))
 
-    def get_qr_code(self) -> Tuple[str, str]:
+    def get_qr_code(self) -> tuple[str, str]:
         """Get Setup-Contact QR Code text and SVG data.
 
         this data needs to be transferred to another Delta Chat account
         in a second channel, typically used by mobiles with QRcode-show + scan UX.
         """
         return self._rpc.get_chat_securejoin_qr_code_svg(self.id, None)
 
     def get_message_by_id(self, msg_id: int) -> Message:
         """Return the Message instance with the given ID."""
         return Message(self, msg_id)
 
-    def mark_seen_messages(self, messages: List[Message]) -> None:
+    def mark_seen_messages(self, messages: list[Message]) -> None:
         """Mark the given set of messages as seen."""
         self._rpc.markseen_msgs(self.id, [msg.id for msg in messages])
 
-    def delete_messages(self, messages: List[Message]) -> None:
+    def delete_messages(self, messages: list[Message]) -> None:
         """Delete messages (local and remote)."""
         self._rpc.delete_messages(self.id, [msg.id for msg in messages])
 
-    def get_fresh_messages(self) -> List[Message]:
+    def get_fresh_messages(self) -> list[Message]:
         """Return the list of fresh messages, newest messages first.
 
         This call is intended for displaying notifications.
         If you are writing a bot, use `get_fresh_messages_in_arrival_order()` instead,
         to process oldest messages first.
         """
         fresh_msg_ids = self._rpc.get_fresh_msgs(self.id)
         return [Message(self, msg_id) for msg_id in fresh_msg_ids]
 
-    def get_next_messages(self) -> List[Message]:
+    def get_next_messages(self) -> list[Message]:
         """Return a list of next messages."""
         next_msg_ids = self._rpc.get_next_msgs(self.id)
         return [Message(self, msg_id) for msg_id in next_msg_ids]
 
-    def wait_next_messages(self) -> List[Message]:
+    def wait_next_messages(self) -> list[Message]:
         """Wait for new messages and return a list of them."""
         next_msg_ids = self._rpc.wait_next_msgs(self.id)
         return [Message(self, msg_id) for msg_id in next_msg_ids]
 
     def wait_for_incoming_msg_event(self):
         """Wait for incoming message event and return it."""
         while True:
@@ -280,15 +305,21 @@
 
     def wait_for_securejoin_joiner_success(self):
         while True:
             event = self.wait_for_event()
             if event["kind"] == "SecurejoinJoinerProgress" and event["progress"] == 1000:
                 break
 
-    def get_fresh_messages_in_arrival_order(self) -> List[Message]:
+    def wait_for_reactions_changed(self):
+        while True:
+            event = self.wait_for_event()
+            if event.kind == EventType.REACTIONS_CHANGED:
+                return event
+
+    def get_fresh_messages_in_arrival_order(self) -> list[Message]:
         """Return fresh messages list sorted in the order of their arrival, with ascending IDs."""
         warn(
             "get_fresh_messages_in_arrival_order is deprecated, use get_next_messages instead.",
             DeprecationWarning,
             stacklevel=2,
         )
         fresh_msg_ids = sorted(self._rpc.get_fresh_msgs(self.id))
```

### Comparing `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/chat.py` & `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from __future__ import annotations
+
 import calendar
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Dict, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Optional, Union
 
 from ._utils import AttrDict
 from .const import ChatVisibility, ViewType
 from .contact import Contact
 from .message import Message
 
 if TYPE_CHECKING:
@@ -89,15 +91,15 @@
         0 means the timer is disabled, use 1 for immediate deletion."""
         self._rpc.set_chat_ephemeral_timer(self.account.id, self.id, timer)
 
     def get_encryption_info(self) -> str:
         """Return encryption info for this chat."""
         return self._rpc.get_chat_encryption_info(self.account.id, self.id)
 
-    def get_qr_code(self) -> Tuple[str, str]:
+    def get_qr_code(self) -> tuple[str, str]:
         """Get Join-Group QR code text and SVG data."""
         return self._rpc.get_chat_securejoin_qr_code_svg(self.account.id, self.id)
 
     def get_basic_snapshot(self) -> AttrDict:
         """Get a chat snapshot with basic info about this chat."""
         info = self._rpc.get_basic_chat_info(self.account.id, self.id)
         return AttrDict(chat=self, **info)
@@ -113,15 +115,15 @@
 
     def send_message(
         self,
         text: Optional[str] = None,
         html: Optional[str] = None,
         viewtype: Optional[ViewType] = None,
         file: Optional[str] = None,
-        location: Optional[Tuple[float, float]] = None,
+        location: Optional[tuple[float, float]] = None,
         override_sender_name: Optional[str] = None,
         quoted_msg: Optional[Union[int, Message]] = None,
     ) -> Message:
         """Send a message and return the resulting Message instance."""
         if isinstance(quoted_msg, Message):
             quoted_msg = quoted_msg.id
 
@@ -138,25 +140,29 @@
         return Message(self.account, msg_id)
 
     def send_text(self, text: str) -> Message:
         """Send a text message and return the resulting Message instance."""
         msg_id = self._rpc.misc_send_text_message(self.account.id, self.id, text)
         return Message(self.account, msg_id)
 
+    def send_file(self, path):
+        """Send a file and return the resulting Message instance."""
+        return self.send_message(file=path)
+
     def send_videochat_invitation(self) -> Message:
         """Send a videochat invitation and return the resulting Message instance."""
         msg_id = self._rpc.send_videochat_invitation(self.account.id, self.id)
         return Message(self.account, msg_id)
 
     def send_sticker(self, path: str) -> Message:
         """Send an sticker and return the resulting Message instance."""
         msg_id = self._rpc.send_sticker(self.account.id, self.id, path)
         return Message(self.account, msg_id)
 
-    def forward_messages(self, messages: List[Message]) -> None:
+    def forward_messages(self, messages: list[Message]) -> None:
         """Forward a list of messages to this chat."""
         msg_ids = [msg.id for msg in messages]
         self._rpc.forward_messages(self.account.id, msg_ids, self.id)
 
     def set_draft(
         self,
         text: Optional[str] = None,
@@ -180,15 +186,15 @@
             return None
         snapshot = AttrDict(snapshot)
         snapshot["chat"] = Chat(self.account, snapshot.chat_id)
         snapshot["sender"] = Contact(self.account, snapshot.from_id)
         snapshot["message"] = Message(self.account, snapshot.id)
         return snapshot
 
-    def get_messages(self, info_only: bool = False, add_daymarker: bool = False) -> List[Message]:
+    def get_messages(self, info_only: bool = False, add_daymarker: bool = False) -> list[Message]:
         """get the list of messages in this chat."""
         msgs = self._rpc.get_message_ids(self.account.id, self.id, info_only, add_daymarker)
         return [Message(self.account, msg_id) for msg_id in msgs]
 
     def get_fresh_message_count(self) -> int:
         """Get number of fresh messages in this chat"""
         return self._rpc.get_fresh_msg_cnt(self.account.id, self.id)
@@ -215,15 +221,15 @@
                 contact_id = self.account.create_contact(cnt).id
             elif not isinstance(cnt, int):
                 contact_id = cnt.id
             else:
                 contact_id = cnt
             self._rpc.remove_contact_from_chat(self.account.id, self.id, contact_id)
 
-    def get_contacts(self) -> List[Contact]:
+    def get_contacts(self) -> list[Contact]:
         """Get the contacts belonging to this chat.
 
         For single/direct chats self-address is not included.
         """
         contacts = self._rpc.get_chat_contacts(self.account.id, self.id)
         return [Contact(self.account, contact_id) for contact_id in contacts]
 
@@ -239,23 +245,23 @@
         self._rpc.set_chat_profile_image(self.account.id, self.id, None)
 
     def get_locations(
         self,
         contact: Optional[Contact] = None,
         timestamp_from: Optional["datetime"] = None,
         timestamp_to: Optional["datetime"] = None,
-    ) -> List[AttrDict]:
+    ) -> list[AttrDict]:
         """Get list of location snapshots for the given contact in the given timespan."""
         time_from = calendar.timegm(timestamp_from.utctimetuple()) if timestamp_from else 0
         time_to = calendar.timegm(timestamp_to.utctimetuple()) if timestamp_to else 0
         contact_id = contact.id if contact else 0
 
         result = self._rpc.get_locations(self.account.id, self.id, contact_id, time_from, time_to)
         locations = []
-        contacts: Dict[int, Contact] = {}
+        contacts: dict[int, Contact] = {}
         for loc in result:
             location = AttrDict(loc)
             location["chat"] = self
             location["contact"] = contacts.setdefault(location.contact_id, Contact(self.account, location.contact_id))
             location["message"] = Message(self.account, location.msg_id)
             locations.append(location)
         return locations
```

### Comparing `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/client.py` & `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Event loop implementations offering high level event handling/hooking."""
 
+from __future__ import annotations
+
 import logging
 from typing import (
     TYPE_CHECKING,
     Callable,
-    Dict,
     Iterable,
     Optional,
-    Set,
-    Tuple,
     Type,
     Union,
 )
 
 from ._utils import (
     AttrDict,
     parse_system_add_remove,
@@ -35,24 +34,24 @@
 
 class Client:
     """Simple Delta Chat client that listen to events of a single account."""
 
     def __init__(
         self,
         account: "Account",
-        hooks: Optional[Iterable[Tuple[Callable, Union[type, EventFilter]]]] = None,
+        hooks: Optional[Iterable[tuple[Callable, Union[type, EventFilter]]]] = None,
         logger: Optional[logging.Logger] = None,
     ) -> None:
         self.account = account
         self.logger = logger or logging
-        self._hooks: Dict[type, Set[tuple]] = {}
+        self._hooks: dict[type, set[tuple]] = {}
         self._should_process_messages = 0
         self.add_hooks(hooks or [])
 
-    def add_hooks(self, hooks: Iterable[Tuple[Callable, Union[type, EventFilter]]]) -> None:
+    def add_hooks(self, hooks: Iterable[tuple[Callable, Union[type, EventFilter]]]) -> None:
         for hook, event in hooks:
             self.add_hook(hook, event)
 
     def add_hook(self, hook: Callable, event: Union[type, EventFilter] = RawEvent) -> None:
         """Register hook for the given event filter."""
         if isinstance(event, type):
             event = event()
```

### Comparing `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/const.py` & `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,16 @@
     IMEX_FILE_WRITTEN = "ImexFileWritten"
     SECUREJOIN_INVITER_PROGRESS = "SecurejoinInviterProgress"
     SECUREJOIN_JOINER_PROGRESS = "SecurejoinJoinerProgress"
     CONNECTIVITY_CHANGED = "ConnectivityChanged"
     SELFAVATAR_CHANGED = "SelfavatarChanged"
     WEBXDC_STATUS_UPDATE = "WebxdcStatusUpdate"
     WEBXDC_INSTANCE_DELETED = "WebxdcInstanceDeleted"
+    CHATLIST_CHANGED = "ChatlistChanged"
+    CHATLIST_ITEM_CHANGED = "ChatlistItemChanged"
 
 
 class ChatId(IntEnum):
     """Special chat ids"""
 
     TRASH = 3
     ARCHIVED_LINK = 6
```

### Comparing `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/contact.py` & `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/contact.py`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/deltachat.py` & `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/deltachat.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import TYPE_CHECKING, Dict, List
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
 
 from ._utils import AttrDict
 from .account import Account
 
 if TYPE_CHECKING:
     from .rpc import Rpc
 
@@ -17,15 +19,15 @@
         self.rpc = rpc
 
     def add_account(self) -> Account:
         """Create a new account database."""
         account_id = self.rpc.add_account()
         return Account(self, account_id)
 
-    def get_all_accounts(self) -> List[Account]:
+    def get_all_accounts(self) -> list[Account]:
         """Return a list of all available accounts."""
         account_ids = self.rpc.get_all_account_ids()
         return [Account(self, account_id) for account_id in account_ids]
 
     def start_io(self) -> None:
         """Start the I/O of all accounts."""
         self.rpc.start_io_for_all_accounts()
@@ -40,10 +42,10 @@
         """
         self.rpc.maybe_network()
 
     def get_system_info(self) -> AttrDict:
         """Get information about the Delta Chat core in this system."""
         return AttrDict(self.rpc.get_system_info())
 
-    def set_translations(self, translations: Dict[str, str]) -> None:
+    def set_translations(self, translations: dict[str, str]) -> None:
         """Set stock translation strings."""
         self.rpc.set_stock_strings(translations)
```

### Comparing `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/events.py` & `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """High-level classes for event processing and filtering."""
 
+from __future__ import annotations
+
 import re
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Callable, Iterable, Iterator, Optional, Set, Tuple, Union
+from typing import TYPE_CHECKING, Callable, Iterable, Iterator, Optional, Union
 
 from .const import EventType
 
 if TYPE_CHECKING:
     from ._utils import AttrDict
 
 
@@ -259,17 +261,17 @@
 
 class HookCollection:
     """
     Helper class to collect event hooks that can later be added to a Delta Chat client.
     """
 
     def __init__(self) -> None:
-        self._hooks: Set[Tuple[Callable, Union[type, EventFilter]]] = set()
+        self._hooks: set[tuple[Callable, Union[type, EventFilter]]] = set()
 
-    def __iter__(self) -> Iterator[Tuple[Callable, Union[type, EventFilter]]]:
+    def __iter__(self) -> Iterator[tuple[Callable, Union[type, EventFilter]]]:
         return iter(self._hooks)
 
     def on(self, event: Union[type, EventFilter]) -> Callable:  # noqa
         """Register decorated function as listener for the given event."""
         if isinstance(event, type):
             event = event()
         assert isinstance(event, EventFilter), "Invalid event filter"
```

### Comparing `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/pytestplugin.py` & `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/pytestplugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from __future__ import annotations
+
 import os
 import random
-from typing import AsyncGenerator, List, Optional
+from typing import AsyncGenerator, Optional
 
 import pytest
 
-from . import Account, AttrDict, Bot, Client, DeltaChat, EventType, Message
+from . import Account, AttrDict, Bot, Chat, Client, DeltaChat, EventType, Message
 from ._utils import futuremethod
 from .rpc import Rpc
 
 
 def get_temp_credentials() -> dict:
     domain = os.getenv("CHATMAIL_DOMAIN")
     username = "ci-" + "".join(random.choice("2345789acdefghjkmnpqrstuvwxyz") for i in range(6))
@@ -50,35 +52,35 @@
         bot = self.get_unconfigured_bot()
         bot.configure(credentials["email"], credentials["password"])
         return bot
 
     @futuremethod
     def get_online_account(self):
         account = yield self.new_configured_account.future()
-        account.start_io()
-        while True:
-            event = account.wait_for_event()
-            if event.kind == EventType.IMAP_INBOX_IDLE:
-                break
+        account.bring_online()
         return account
 
-    def get_online_accounts(self, num: int) -> List[Account]:
+    def get_online_accounts(self, num: int) -> list[Account]:
         futures = [self.get_online_account.future() for _ in range(num)]
         return [f() for f in futures]
 
     def resetup_account(self, ac: Account) -> Account:
         """Resetup account from scratch, losing the encryption key."""
         ac.stop_io()
         ac_clone = self.get_unconfigured_account()
         for i in ["addr", "mail_pw"]:
             ac_clone.set_config(i, ac.get_config(i))
         ac.remove()
         ac_clone.configure()
         return ac_clone
 
+    def get_accepted_chat(self, ac1: Account, ac2: Account) -> Chat:
+        ac2.create_chat(ac1)
+        return ac1.create_chat(ac2)
+
     def send_message(
         self,
         to_account: Account,
         from_account: Optional[Account] = None,
         text: Optional[str] = None,
         file: Optional[str] = None,
         group: Optional[str] = None,
```

### Comparing `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client/rpc.py` & `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/rpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+from __future__ import annotations
+
 import itertools
 import json
 import logging
 import os
 import subprocess
 import sys
-from queue import Queue
+from queue import Empty, Queue
 from threading import Event, Thread
-from typing import Any, Dict, Iterator, Optional
+from typing import Any, Iterator, Optional
 
 
 class JsonRpcError(Exception):
     pass
 
 
 class RpcFuture:
@@ -63,19 +65,19 @@
                 **kwargs.get("env", os.environ),
                 "DC_ACCOUNTS_PATH": str(accounts_dir),
             }
 
         self._kwargs = kwargs
         self.process: subprocess.Popen
         self.id_iterator: Iterator[int]
-        self.event_queues: Dict[int, Queue]
+        self.event_queues: dict[int, Queue]
         # Map from request ID to `threading.Event`.
-        self.request_events: Dict[int, Event]
+        self.request_events: dict[int, Event]
         # Map from request ID to the result.
-        self.request_results: Dict[int, Any]
+        self.request_results: dict[int, Any]
         self.request_queue: Queue[Any]
         self.closing: bool
         self.reader_thread: Thread
         self.writer_thread: Thread
         self.events_thread: Thread
 
     def start(self) -> None:
@@ -182,9 +184,18 @@
             logging.exception("Exception in the event loop")
 
     def wait_for_event(self, account_id: int) -> Optional[dict]:
         """Waits for the next event from the given account and returns it."""
         queue = self.get_queue(account_id)
         return queue.get()
 
+    def clear_all_events(self, account_id: int):
+        """Removes all queued-up events for a given account. Useful for tests."""
+        queue = self.get_queue(account_id)
+        try:
+            while True:
+                queue.get_nowait()
+        except Empty:
+            pass
+
     def __getattr__(self, attr: str):
         return RpcMethod(self, attr)
```

### Comparing `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client.egg-info/PKG-INFO` & `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat-rpc-client
-Version: 1.137.2
+Version: 1.137.3
 Summary: Python client for Delta Chat core JSON-RPC interface
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Communications :: Email
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: imap-tools
 
 # Delta Chat RPC python client
 
 RPC client connects to standalone Delta Chat RPC server `deltachat-rpc-server`
 and provides asynchronous interface to it.
 
 ## Getting started
```

### Comparing `deltachat-rpc-client-1.137.2/src/deltachat_rpc_client.egg-info/SOURCES.txt` & `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,20 +5,23 @@
 src/deltachat_rpc_client/_utils.py
 src/deltachat_rpc_client/account.py
 src/deltachat_rpc_client/chat.py
 src/deltachat_rpc_client/client.py
 src/deltachat_rpc_client/const.py
 src/deltachat_rpc_client/contact.py
 src/deltachat_rpc_client/deltachat.py
+src/deltachat_rpc_client/direct_imap.py
 src/deltachat_rpc_client/events.py
 src/deltachat_rpc_client/message.py
 src/deltachat_rpc_client/py.typed
 src/deltachat_rpc_client/pytestplugin.py
 src/deltachat_rpc_client/rpc.py
 src/deltachat_rpc_client.egg-info/PKG-INFO
 src/deltachat_rpc_client.egg-info/SOURCES.txt
 src/deltachat_rpc_client.egg-info/dependency_links.txt
 src/deltachat_rpc_client.egg-info/entry_points.txt
+src/deltachat_rpc_client.egg-info/requires.txt
 src/deltachat_rpc_client.egg-info/top_level.txt
+tests/test_chatlist_events.py
 tests/test_securejoin.py
 tests/test_something.py
 tests/test_webxdc.py
```

### Comparing `deltachat-rpc-client-1.137.2/tests/test_securejoin.py` & `deltachat_rpc_client-1.137.3/tests/test_securejoin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 
 import pytest
-from deltachat_rpc_client import Chat, SpecialContactId
+from deltachat_rpc_client import Chat, EventType, SpecialContactId
 
 
 def test_qr_setup_contact(acfactory, tmp_path) -> None:
     alice, bob = acfactory.get_online_accounts(2)
 
     qr_code, _svg = alice.get_qr_code()
     bob.secure_join(qr_code)
@@ -575,7 +575,44 @@
     assert snapshot.is_info
     ac2_chat = snapshot.chat
     assert ac2_chat.get_basic_snapshot().is_protected
     assert len(ac2_chat.get_contacts()) == 3
 
     # ac1 is still "not verified" for ac2 due to inconsistent state.
     assert not ac2_contact_ac1.get_snapshot().is_verified
+
+
+def test_withdraw_securejoin_qr(acfactory):
+    alice, bob = acfactory.get_online_accounts(2)
+
+    logging.info("Alice creates a verified group")
+    alice_chat = alice.create_group("Verified group", protect=True)
+    assert alice_chat.get_basic_snapshot().is_protected
+    logging.info("Bob joins verified group")
+
+    qr_code, _svg = alice_chat.get_qr_code()
+    bob_chat = bob.secure_join(qr_code)
+    bob.wait_for_securejoin_joiner_success()
+
+    snapshot = bob.get_message_by_id(bob.wait_for_incoming_msg_event().msg_id).get_snapshot()
+    assert snapshot.text == "Member Me ({}) added by {}.".format(bob.get_config("addr"), alice.get_config("addr"))
+    assert snapshot.chat.get_basic_snapshot().is_protected
+    bob_chat.leave()
+
+    snapshot = alice.get_message_by_id(alice.wait_for_incoming_msg_event().msg_id).get_snapshot()
+    assert snapshot.text == "Group left by {}.".format(bob.get_config("addr"))
+
+    logging.info("Alice withdraws QR code.")
+    qr = alice.check_qr(qr_code)
+    assert qr["kind"] == "withdrawVerifyGroup"
+    alice.set_config_from_qr(qr_code)
+
+    logging.info("Bob scans withdrawn QR code.")
+    bob_chat = bob.secure_join(qr_code)
+
+    logging.info("Bob scanned withdrawn QR code")
+    while True:
+        event = alice.wait_for_event()
+        if event.kind == EventType.MSGS_CHANGED and event.chat_id != 0:
+            break
+    snapshot = alice.get_message_by_id(event.msg_id).get_snapshot()
+    assert snapshot.text == "Cannot establish guaranteed end-to-end encryption with {}".format(bob.get_config("addr"))
```

### Comparing `deltachat-rpc-client-1.137.2/tests/test_something.py` & `deltachat_rpc_client-1.137.3/tests/test_something.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import concurrent.futures
 import json
+import logging
+import os
 import subprocess
+import time
 from unittest.mock import MagicMock
 
 import pytest
-from deltachat_rpc_client import EventType, events
+from deltachat_rpc_client import Contact, EventType, Message, events
+from deltachat_rpc_client.const import DownloadState
+from deltachat_rpc_client.direct_imap import DirectImap
 from deltachat_rpc_client.rpc import JsonRpcError
 
 
 def test_system_info(rpc) -> None:
     system_info = rpc.get_system_info()
     assert "arch" in system_info
     assert "deltachat_core_version" in system_info
@@ -435,7 +440,147 @@
     # Bob sends a message to Alice, it should also be encrypted.
     bob_chat_alice.send_text("Hi Alice!")
     event = alice.wait_for_incoming_msg_event()
     msg_id = event.msg_id
     message = alice.get_message_by_id(msg_id)
     snapshot = message.get_snapshot()
     assert snapshot.show_padlock
+
+
+def test_reaction_to_partially_fetched_msg(acfactory, tmp_path):
+    """See https://github.com/deltachat/deltachat-core-rust/issues/3688 "Partially downloaded
+    messages are received out of order".
+
+    If the Inbox contains X small messages followed by Y large messages followed by Z small
+    messages, Delta Chat first downloaded a batch of X+Z messages, and then a batch of Y messages.
+
+    This bug was discovered by @Simon-Laux while testing reactions PR #3644 and can be reproduced
+    with online test as follows:
+    - Bob enables download limit and goes offline.
+    - Alice sends a large message to Bob and reacts to this message with a thumbs-up.
+    - Bob goes online
+    - Bob first processes a reaction message and throws it away because there is no corresponding
+      message, then processes a partially downloaded message.
+    - As a result, Bob does not see a reaction
+    """
+    download_limit = 300000
+    ac1, ac2 = acfactory.get_online_accounts(2)
+    ac1_addr = ac1.get_config("addr")
+    chat = ac1.create_chat(ac2)
+    ac2.set_config("download_limit", str(download_limit))
+    ac2.stop_io()
+
+    logging.info("sending small+large messages from ac1 to ac2")
+    msgs = []
+    msgs.append(chat.send_text("hi"))
+    path = tmp_path / "large"
+    path.write_bytes(os.urandom(download_limit + 1))
+    msgs.append(chat.send_file(str(path)))
+    for m in msgs:
+        m.wait_until_delivered()
+
+    logging.info("sending a reaction to the large message from ac1 to ac2")
+    # TODO: Find the reason of an occasional message reordering on the server (so that the reaction
+    # has a lower UID than the previous message). W/a is to sleep for some time to let the reaction
+    # have a later INTERNALDATE.
+    time.sleep(1.1)
+    react_str = "\N{THUMBS UP SIGN}"
+    msgs.append(msgs[-1].send_reaction(react_str))
+    msgs[-1].wait_until_delivered()
+
+    ac2.start_io()
+
+    logging.info("wait for ac2 to receive a reaction")
+    msg2 = Message(ac2, ac2.wait_for_reactions_changed().msg_id)
+    assert msg2.get_sender_contact().get_snapshot().address == ac1_addr
+    assert msg2.get_snapshot().download_state == DownloadState.AVAILABLE
+    reactions = msg2.get_reactions()
+    contacts = [Contact(ac2, int(i)) for i in reactions.reactions_by_contact]
+    assert len(contacts) == 1
+    assert contacts[0].get_snapshot().address == ac1_addr
+    assert list(reactions.reactions_by_contact.values())[0] == [react_str]
+
+
+def test_reactions_for_a_reordering_move(acfactory):
+    """When a batch of messages is moved from Inbox to DeltaChat folder with a single MOVE command,
+    their UIDs may be reordered (e.g. Gmail is known for that) which led to that messages were
+    processed by receive_imf in the wrong order, and, particularly, reactions were processed before
+    messages they refer to and thus dropped.
+    """
+    (ac1,) = acfactory.get_online_accounts(1)
+    ac2 = acfactory.new_preconfigured_account()
+    ac2.set_config("mvbox_move", "1")
+    ac2.configure()
+    ac2.bring_online()
+    chat1 = acfactory.get_accepted_chat(ac1, ac2)
+    ac2.stop_io()
+
+    logging.info("sending message + reaction from ac1 to ac2")
+    msg1 = chat1.send_text("hi")
+    msg1.wait_until_delivered()
+    # It's is sad, but messages must differ in their INTERNALDATEs to be processed in the correct
+    # order by DC, and most (if not all) mail servers provide only seconds precision.
+    time.sleep(1.1)
+    react_str = "\N{THUMBS UP SIGN}"
+    msg1.send_reaction(react_str).wait_until_delivered()
+
+    logging.info("moving messages to ac2's DeltaChat folder in the reverse order")
+    ac2_direct_imap = DirectImap(ac2)
+    ac2_direct_imap.connect()
+    for uid in sorted([m.uid for m in ac2_direct_imap.get_all_messages()], reverse=True):
+        ac2_direct_imap.conn.move(uid, "DeltaChat")
+
+    logging.info("receiving messages by ac2")
+    ac2.start_io()
+    msg2 = Message(ac2, ac2.wait_for_reactions_changed().msg_id)
+    assert msg2.get_snapshot().text == msg1.get_snapshot().text
+    reactions = msg2.get_reactions()
+    contacts = [Contact(ac2, int(i)) for i in reactions.reactions_by_contact]
+    assert len(contacts) == 1
+    assert contacts[0].get_snapshot().address == ac1.get_config("addr")
+    assert list(reactions.reactions_by_contact.values())[0] == [react_str]
+
+
+@pytest.mark.parametrize("n_accounts", [3, 2])
+def test_download_limit_chat_assignment(acfactory, tmp_path, n_accounts):
+    download_limit = 300000
+
+    alice, *others = acfactory.get_online_accounts(n_accounts)
+    bob = others[0]
+
+    alice_group = alice.create_group("test group")
+    for account in others:
+        chat = account.create_chat(alice)
+        chat.send_text("Hello Alice!")
+        assert alice.get_message_by_id(alice.wait_for_incoming_msg_event().msg_id).get_snapshot().text == "Hello Alice!"
+
+        contact_addr = account.get_config("addr")
+        contact = alice.create_contact(contact_addr, "")
+
+        alice_group.add_contact(contact)
+
+    if n_accounts == 2:
+        bob_chat_alice = bob.create_chat(alice)
+    bob.set_config("download_limit", str(download_limit))
+
+    alice_group.send_text("hi")
+    snapshot = bob.get_message_by_id(bob.wait_for_incoming_msg_event().msg_id).get_snapshot()
+    assert snapshot.text == "hi"
+    bob_group = snapshot.chat
+
+    path = tmp_path / "large"
+    path.write_bytes(os.urandom(download_limit + 1))
+
+    for i in range(10):
+        logging.info("Sending message %s", i)
+        alice_group.send_file(str(path))
+        snapshot = bob.get_message_by_id(bob.wait_for_incoming_msg_event().msg_id).get_snapshot()
+        assert snapshot.download_state == DownloadState.AVAILABLE
+        if n_accounts > 2:
+            assert snapshot.chat == bob_group
+        else:
+            # Group contains only Alice and Bob,
+            # so partially downloaded messages are
+            # hard to distinguish from private replies to group messages.
+            #
+            # Message may be a private reply, so we assign it to 1:1 chat with Alice.
+            assert snapshot.chat == bob_chat_alice
```

### Comparing `deltachat-rpc-client-1.137.2/tests/test_webxdc.py` & `deltachat_rpc_client-1.137.3/tests/test_webxdc.py`

 * *Files identical despite different names*

