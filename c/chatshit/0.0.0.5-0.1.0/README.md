# Comparing `tmp/chatshit-0.0.0.5.tar.gz` & `tmp/chatshit-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatshit-0.0.0.5.tar", max compression
+gzip compressed data, was "chatshit-0.1.0.tar", max compression
```

## Comparing `chatshit-0.0.0.5.tar` & `chatshit-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       22 2023-10-15 19:42:51.703549 chatshit-0.0.0.5/README.md
--rw-r--r--   0        0        0        0 2023-10-13 13:59:07.830949 chatshit-0.0.0.5/chatshit/__init__.py
--rw-r--r--   0        0        0      982 2024-04-13 17:36:21.578298 chatshit-0.0.0.5/chatshit/__main__.py
--rw-r--r--   0        0        0     4203 2024-04-13 17:36:21.578298 chatshit-0.0.0.5/chatshit/app.py
--rw-r--r--   0        0        0     5685 2024-04-13 17:36:21.578298 chatshit-0.0.0.5/chatshit/network/chatroom_server.py
--rw-r--r--   0        0        0     1414 2024-04-13 17:36:21.578298 chatshit-0.0.0.5/chatshit/network/client.py
--rw-r--r--   0        0        0     2268 2024-04-13 17:28:56.061402 chatshit-0.0.0.5/chatshit/network/proto.py
--rw-r--r--   0        0        0     2741 2024-04-13 17:36:21.578298 chatshit-0.0.0.5/chatshit/screens/chatroom_screen.py
--rw-r--r--   0        0        0      482 2024-04-13 17:36:21.578298 chatshit-0.0.0.5/chatshit/screens/client_screen.py
--rw-r--r--   0        0        0     1081 2024-04-13 17:36:21.582298 chatshit-0.0.0.5/chatshit/screens/confirmation_screen.py
--rw-r--r--   0        0        0     1391 2024-04-13 17:36:21.582298 chatshit-0.0.0.5/chatshit/screens/create_server_screen.py
--rw-r--r--   0        0        0     1400 2024-04-13 17:36:21.582298 chatshit-0.0.0.5/chatshit/screens/delete_message_screen.py
--rw-r--r--   0        0        0     1713 2024-04-13 17:36:21.582298 chatshit-0.0.0.5/chatshit/screens/home_screen.py
--rw-r--r--   0        0        0     2516 2024-04-13 17:36:21.582298 chatshit-0.0.0.5/chatshit/screens/login_screen.py
--rw-r--r--   0        0        0     4911 2024-04-13 17:36:21.582298 chatshit-0.0.0.5/chatshit/styles.css
--rw-r--r--   0        0        0     1767 2024-04-13 17:36:21.582298 chatshit-0.0.0.5/chatshit/widgets/chat_list.py
--rw-r--r--   0        0        0     1195 2024-04-13 17:36:21.582298 chatshit-0.0.0.5/chatshit/widgets/member_list.py
--rw-r--r--   0        0        0     2088 2024-04-13 17:36:21.582298 chatshit-0.0.0.5/chatshit/widgets/message_list.py
--rw-r--r--   0        0        0     1766 2024-04-13 17:36:21.582298 chatshit-0.0.0.5/chatshit/widgets/server_list.py
--rw-r--r--   0        0        0      448 2024-04-13 17:30:10.794205 chatshit-0.0.0.5/pyproject.toml
--rw-r--r--   0        0        0      809 1970-01-01 00:00:00.000000 chatshit-0.0.0.5/setup.py
--rw-r--r--   0        0        0      373 1970-01-01 00:00:00.000000 chatshit-0.0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      336 2024-04-13 18:02:55.424906 chatshit-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-10-13 13:59:07.830949 chatshit-0.1.0/chatshit/__init__.py
+-rw-r--r--   0        0        0      982 2024-04-13 17:36:21.578298 chatshit-0.1.0/chatshit/__main__.py
+-rw-r--r--   0        0        0     4203 2024-04-13 17:36:21.578298 chatshit-0.1.0/chatshit/app.py
+-rw-r--r--   0        0        0     5685 2024-04-13 17:36:21.578298 chatshit-0.1.0/chatshit/network/chatroom_server.py
+-rw-r--r--   0        0        0     1414 2024-04-13 17:36:21.578298 chatshit-0.1.0/chatshit/network/client.py
+-rw-r--r--   0        0        0     2268 2024-04-13 17:28:56.061402 chatshit-0.1.0/chatshit/network/proto.py
+-rw-r--r--   0        0        0     2741 2024-04-13 17:36:21.578298 chatshit-0.1.0/chatshit/screens/chatroom_screen.py
+-rw-r--r--   0        0        0      482 2024-04-13 17:36:21.578298 chatshit-0.1.0/chatshit/screens/client_screen.py
+-rw-r--r--   0        0        0     1081 2024-04-13 17:36:21.582298 chatshit-0.1.0/chatshit/screens/confirmation_screen.py
+-rw-r--r--   0        0        0     1391 2024-04-13 17:36:21.582298 chatshit-0.1.0/chatshit/screens/create_server_screen.py
+-rw-r--r--   0        0        0     1400 2024-04-13 17:36:21.582298 chatshit-0.1.0/chatshit/screens/delete_message_screen.py
+-rw-r--r--   0        0        0     1774 2024-04-15 15:53:39.222573 chatshit-0.1.0/chatshit/screens/home_screen.py
+-rw-r--r--   0        0        0     2586 2024-04-15 15:48:32.983382 chatshit-0.1.0/chatshit/screens/login_screen.py
+-rw-r--r--   0        0        0     4911 2024-04-13 17:36:21.582298 chatshit-0.1.0/chatshit/styles.css
+-rw-r--r--   0        0        0     1833 2024-04-13 18:04:20.573983 chatshit-0.1.0/chatshit/widgets/chat_list.py
+-rw-r--r--   0        0        0     1195 2024-04-13 17:36:21.582298 chatshit-0.1.0/chatshit/widgets/member_list.py
+-rw-r--r--   0        0        0     2088 2024-04-13 18:04:10.533856 chatshit-0.1.0/chatshit/widgets/message_list.py
+-rw-r--r--   0        0        0     1832 2024-04-13 18:04:12.357879 chatshit-0.1.0/chatshit/widgets/server_list.py
+-rw-r--r--   0        0        0      446 2024-04-18 13:59:00.364634 chatshit-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1137 1970-01-01 00:00:00.000000 chatshit-0.1.0/setup.py
+-rw-r--r--   0        0        0      685 1970-01-01 00:00:00.000000 chatshit-0.1.0/PKG-INFO
```

### Comparing `chatshit-0.0.0.5/chatshit/__main__.py` & `chatshit-0.1.0/chatshit/__main__.py`

 * *Files identical despite different names*

### Comparing `chatshit-0.0.0.5/chatshit/app.py` & `chatshit-0.1.0/chatshit/app.py`

 * *Files identical despite different names*

### Comparing `chatshit-0.0.0.5/chatshit/network/chatroom_server.py` & `chatshit-0.1.0/chatshit/network/chatroom_server.py`

 * *Files identical despite different names*

### Comparing `chatshit-0.0.0.5/chatshit/network/client.py` & `chatshit-0.1.0/chatshit/network/client.py`

 * *Files identical despite different names*

### Comparing `chatshit-0.0.0.5/chatshit/network/proto.py` & `chatshit-0.1.0/chatshit/network/proto.py`

 * *Files identical despite different names*

### Comparing `chatshit-0.0.0.5/chatshit/screens/chatroom_screen.py` & `chatshit-0.1.0/chatshit/screens/chatroom_screen.py`

 * *Files identical despite different names*

### Comparing `chatshit-0.0.0.5/chatshit/screens/confirmation_screen.py` & `chatshit-0.1.0/chatshit/screens/confirmation_screen.py`

 * *Files identical despite different names*

### Comparing `chatshit-0.0.0.5/chatshit/screens/create_server_screen.py` & `chatshit-0.1.0/chatshit/screens/create_server_screen.py`

 * *Files identical despite different names*

### Comparing `chatshit-0.0.0.5/chatshit/screens/delete_message_screen.py` & `chatshit-0.1.0/chatshit/screens/delete_message_screen.py`

 * *Files identical despite different names*

### Comparing `chatshit-0.0.0.5/chatshit/screens/home_screen.py` & `chatshit-0.1.0/chatshit/screens/home_screen.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,8 +34,10 @@
         if event.button == self.create_chatroom_button:
             self.app.push_screen(CreateServerScreen(classes="input-screen"))
         elif event.button == self.connect_to_chatroom_button:
             self.app.push_screen(ChatRoomScreen())
 
     def on_server_list_connect_to(self, message: ServerList.ConnectTo):
         host, port = self.app.get_server_address(message.server_id)
+        if host == "0.0.0.0":
+            host = "127.0.0.1"
         self.app.push_screen(ChatRoomScreen(host=host, port=port))
```

### Comparing `chatshit-0.0.0.5/chatshit/screens/login_screen.py` & `chatshit-0.1.0/chatshit/screens/login_screen.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,9 +67,11 @@
             self.info.update("Wrong address")
         except ConnectionRefusedError:
             self.info.update("No server on this port")
         except OverflowError:
             self.info.update("Port must be 0-65535.")
         except TimeoutError:
             self.info.update("Timeout")
+        except OSError as e:
+            self.info.update(e.strerror)
         else:
             self.dismiss(self.Result(self._client, self.name_field.value))
```

### Comparing `chatshit-0.0.0.5/chatshit/styles.css` & `chatshit-0.1.0/chatshit/styles.css`

 * *Files identical despite different names*

### Comparing `chatshit-0.0.0.5/chatshit/widgets/chat_list.py` & `chatshit-0.1.0/chatshit/widgets/chat_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,16 @@
         if not name:
             name = f"{host}:{port}"
         label = Label(name)
         self.append(ListItem(label, id=f"_{chat_id}"))
 
     def remove_chat(self, chat_id: int):
         self.remove_children(f"#_{chat_id}")
+        self.action_cursor_down()
+        self.action_cursor_up()
 
     def on_key(self, event: events.Key):
         if event.key == "enter":
             chat_id = int(self.highlighted_child.id[1:])
             self.post_message(self.OpenChat(chat_id))
             event.stop()
         elif event.key == "d":
```

### Comparing `chatshit-0.0.0.5/chatshit/widgets/member_list.py` & `chatshit-0.1.0/chatshit/widgets/member_list.py`

 * *Files identical despite different names*

### Comparing `chatshit-0.0.0.5/chatshit/widgets/message_list.py` & `chatshit-0.1.0/chatshit/widgets/message_list.py`

 * *Files identical despite different names*

### Comparing `chatshit-0.0.0.5/chatshit/widgets/server_list.py` & `chatshit-0.1.0/chatshit/widgets/server_list.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     def add_server(self, server_id: int, host: str, port: int):
         name = f"{host}:{port}"
         label = Label(name)
         self.append(ListItem(label, id=f"_{server_id}"))
 
     def remove_server(self, server_id: int):
         self.remove_children(f"#_{server_id}")
+        self.action_cursor_down()
+        self.action_cursor_up()
 
     def on_key(self, event: events.Key):
         if event.key == "enter":
             server_id = int(self.highlighted_child.id[1:])
             self.post_message(self.ConnectTo(server_id))
             event.stop()
         elif event.key == "d":
```

