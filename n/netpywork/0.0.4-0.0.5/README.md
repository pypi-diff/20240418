# Comparing `tmp/netpywork-0.0.4.tar.gz` & `tmp/netpywork-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netpywork-0.0.4.tar", last modified: Wed Apr 10 14:08:19 2024, max compression
+gzip compressed data, was "netpywork-0.0.5.tar", last modified: Thu Apr 18 17:15:04 2024, max compression
```

## Comparing `netpywork-0.0.4.tar` & `netpywork-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 14:08:19.882687 netpywork-0.0.4/
--rw-rw-rw-   0        0        0     1065 2024-04-10 14:08:19.881728 netpywork-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      505 2024-04-10 13:33:55.000000 netpywork-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 14:08:19.865734 netpywork-0.0.4/netpywork/
--rw-rw-rw-   0        0        0      211 2024-04-10 12:49:34.000000 netpywork-0.0.4/netpywork/__init__.py
--rw-rw-rw-   0        0        0     5359 2024-04-10 12:36:43.000000 netpywork-0.0.4/netpywork/client.py
--rw-rw-rw-   0        0        0       84 2024-04-10 14:07:46.000000 netpywork-0.0.4/netpywork/constants.py
--rw-rw-rw-   0        0        0       93 2024-04-08 12:13:40.000000 netpywork-0.0.4/netpywork/protocol.py
--rw-rw-rw-   0        0        0     2284 2024-04-08 14:01:27.000000 netpywork-0.0.4/netpywork/sequence_manager.py
--rw-rw-rw-   0        0        0     7316 2024-04-10 12:41:31.000000 netpywork-0.0.4/netpywork/server.py
--rw-rw-rw-   0        0        0     3799 2024-04-09 14:08:35.000000 netpywork-0.0.4/netpywork/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-10 14:08:19.877735 netpywork-0.0.4/netpywork.egg-info/
--rw-rw-rw-   0        0        0     1065 2024-04-10 14:08:19.000000 netpywork-0.0.4/netpywork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2024-04-10 14:08:19.000000 netpywork-0.0.4/netpywork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 14:08:19.000000 netpywork-0.0.4/netpywork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-10 14:08:19.000000 netpywork-0.0.4/netpywork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 14:08:19.883685 netpywork-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      719 2024-04-08 13:45:44.000000 netpywork-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 17:15:04.760164 netpywork-0.0.5/
+-rw-rw-rw-   0        0        0     1063 2024-04-18 17:15:04.759167 netpywork-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      503 2024-04-10 14:09:29.000000 netpywork-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 17:15:04.744212 netpywork-0.0.5/netpywork/
+-rw-rw-rw-   0        0        0      201 2024-04-14 13:18:43.000000 netpywork-0.0.5/netpywork/__init__.py
+-rw-rw-rw-   0        0        0     5475 2024-04-18 17:12:32.000000 netpywork-0.0.5/netpywork/client.py
+-rw-rw-rw-   0        0        0      153 2024-04-18 17:13:40.000000 netpywork-0.0.5/netpywork/constants.py
+-rw-rw-rw-   0        0        0       93 2024-04-08 12:13:40.000000 netpywork-0.0.5/netpywork/protocol.py
+-rw-rw-rw-   0        0        0     2451 2024-04-14 09:08:08.000000 netpywork-0.0.5/netpywork/sequence_manager.py
+-rw-rw-rw-   0        0        0     7378 2024-04-18 17:13:12.000000 netpywork-0.0.5/netpywork/server.py
+-rw-rw-rw-   0        0        0     3841 2024-04-14 09:09:30.000000 netpywork-0.0.5/netpywork/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-18 17:15:04.756175 netpywork-0.0.5/netpywork.egg-info/
+-rw-rw-rw-   0        0        0     1063 2024-04-18 17:15:04.000000 netpywork-0.0.5/netpywork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2024-04-18 17:15:04.000000 netpywork-0.0.5/netpywork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 17:15:04.000000 netpywork-0.0.5/netpywork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-18 17:15:04.000000 netpywork-0.0.5/netpywork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 17:15:04.761161 netpywork-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      719 2024-04-08 13:45:44.000000 netpywork-0.0.5/setup.py
```

### Comparing `netpywork-0.0.4/PKG-INFO` & `netpywork-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: netpywork
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python library that simplifies UDP and TCP server and client
 Home-page: https://github.com/MurkyYT/netpywork
 Author: Murky
 Author-email: shooterkingof@gmail.com
 License: UNKNOWN
 Description: # netpywork
         **netpywork** is a library that makes using tcp and udp server and client easier
         
         # Features
         - Creating a server and client which uses `TCP` and `UDP`
         - Callbacks for `On Receive`, `On Connect` and `On Disconnect` for server
         - Callbacks for `On Receive` and `On Connect` for client
-        - Sending messages from server to client both with tcp and udp by specifing the address to send to `(see examples [here](https://github.com/MurkyYT/netpywork/tree/main))`
+        - Sending messages from server to client both with tcp and udp by specifing the address to send to (see examples [here](https://github.com/MurkyYT/netpywork/tree/main))
         - Sending *large* `UDP` messages
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `netpywork-0.0.4/netpywork/client.py` & `netpywork-0.0.5/netpywork/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import socket
 from threading import Thread
 from .sequence_manager import sequence_manager
 from .utils import *
 from .utils import _utils
 from .protocol import *
+from .constants import *
 
 class client:
     def __init__(self,ip: str,port: int) -> None:
         self.ip: str = ip
         self.port: int = port
         self.address: tuple = None
         self.auto_receive_udp: bool = True
@@ -34,26 +35,28 @@
         self.__tcp_thread.start()
         self.address = self.__tcp_socket.getsockname()
         server_address = self.__tcp_socket.getpeername()
         self.__seq_manager.add_addr(server_address)
 
         self.__udp_thread = Thread(target=self.__run_udp)
         self.__udp_socket.bind(self.address)
-        self.__udp_socket.settimeout(1)
+        self.__udp_socket.settimeout(UDP_TIMEOUT)
         self.__udp_thread.start()
         if(self.on_connect):
             self.on_connect(server_address,self)
     def close(self):
         self.__is_running = False
         server_address = self.__tcp_socket.getpeername()
+        self.__tcp_socket.shutdown(socket.SHUT_RDWR)
         self.__tcp_socket.close()
         self.__tcp_thread.join()
         self.__seq_manager.delete_addr(server_address)
 
         self.__udp_thread.join()
+        self.__udp_socket.shutdown(socket.SHUT_RDWR)
         self.__udp_socket.close()
 
         self.__seq_manager.stop()
     def has_tcp_messages(self) -> bool:
         return len(self.__tcp_messages) > 0
     def read_tcp_message(self) -> tcp_msg:
         while len(self.__tcp_messages) < 1:
@@ -72,21 +75,21 @@
             self.send_unreliable(msg)
         else:
             raise ValueError(f"Protocol type is unknown")
     def send_reliable(self,msg: bytes):
         _utils.send_tcp(self.__tcp_socket,msg)
     def send_unreliable(self,msg: bytes):
         msg_len = len(msg)
-        if(msg_len <= _utils.MAX_UDP_PACKET_SIZE):
+        if(msg_len <= MAX_UDP_PACKET_SIZE):
             _utils.send_udp(self.__udp_socket,self.address[1],(self.ip,self.port),msg,self.__udp_seq,0,1)
         else:
             parts = []
-            while (len(msg) > _utils.MAX_UDP_PACKET_SIZE):
-                parts.append(msg[0:_utils.MAX_UDP_PACKET_SIZE])
-                msg = msg[_utils.MAX_UDP_PACKET_SIZE:]
+            while (len(msg) > MAX_UDP_PACKET_SIZE):
+                parts.append(msg[0:MAX_UDP_PACKET_SIZE])
+                msg = msg[MAX_UDP_PACKET_SIZE:]
             parts.append(msg)
             for i in range(len(parts)):
                 _utils.send_udp(self.__udp_socket,self.address[1],(self.ip,self.port),parts[i],self.__udp_seq,i,len(parts))
         self.__udp_seq += 1
     def __run_udp(self):
         while self.__is_running:
             try:
```

### Comparing `netpywork-0.0.4/netpywork/sequence_manager.py` & `netpywork-0.0.5/netpywork/sequence_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,18 @@
             del self.__messages[address][seqno]
             del self.__messages_in_process[(address,seqno)]
             return result
         except:
             return None
     def __clear_old(self):
         try:
-            for address in self.__messages.keys():
-                for seqno in self.__messages[address].keys():
-                    timestamp = self.__messages_in_process[(address,seqno)]
-                    if(timestamp + netpywork.udp_storetime < datetime.datetime.now()):
-                        del self.__messages_in_process[(address,seqno)]
-                        del self.__messages[address][seqno]
+            addresses = self.__messages.keys()
+            for address in addresses:
+                seqences = self.__messages[address].keys()
+                for seqno in seqences:
+                    if((address,seqno) in self.__messages_in_process.keys()):
+                        timestamp = self.__messages_in_process[(address,seqno)]
+                        if(timestamp + netpywork.udp_storetime < datetime.datetime.now()):
+                            del self.__messages_in_process[(address,seqno)]
+                            del self.__messages[address][seqno]
         except:
             pass
```

### Comparing `netpywork-0.0.4/netpywork/server.py` & `netpywork-0.0.5/netpywork/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import socket
 import select
 from threading import Thread
 from .protocol import *
 from .sequence_manager import sequence_manager
 from .utils import *
 from .utils import _utils
+from .constants import *
 
 class server:
     def __init__(self,port : int) -> None:
         self.port : int = port
         self.auto_receive_udp: bool = True
         self.auto_receive_tcp: bool = True
         self.on_receive = None
@@ -36,23 +37,24 @@
     def run(self):
         self.__is_running = True
         self.__tcp_thread = Thread(target=self.__run_tcp)
         self.__tcp_socket.listen()
         self.__tcp_thread.start()
 
         self.__udp_thread = Thread(target=self.__run_udp)
-        self.__udp_socket.settimeout(1)
+        self.__udp_socket.settimeout(UDP_TIMEOUT)
         self.__udp_thread.start()
     def close(self):
         self.__is_running = False
         self.__tcp_socket.close()
         self.__tcp_thread.join()
         for client in self.__clients:
             self.__seq_manager.delete_addr(client.getpeername())
         self.__udp_thread.join()
+        self.__udp_socket.shutdown(socket.SHUT_RDWR)
         self.__udp_socket.close()
         self.__seq_manager.stop()
     def has_tcp_messages(self) -> bool:
         return len(self.__tcp_messages) > 0
     def read_tcp_message(self) -> tcp_msg:
         while len(self.__tcp_messages) < 1:
             continue
@@ -77,21 +79,21 @@
             raise ValueError(f"Protocol type is unknown")
     def send_reliable(self,msg: bytes,address:tuple):
         _utils.send_tcp(self.__addr_to_sock[address],msg)
     def __get_actual_address(self,address):
         return self.__addr_to_sock[address].getpeername()
     def send_unreliable(self,msg: bytes,address:tuple):
         msg_len = len(msg)
-        if(msg_len <= _utils.MAX_UDP_PACKET_SIZE):
+        if(msg_len <= MAX_UDP_PACKET_SIZE):
             _utils.send_udp(self.__udp_socket,self.__tcp_socket.getsockname()[1],self.__get_actual_address(address),msg,self.__udp_seq,0,1)
         else:
             parts = []
-            while (len(msg) > _utils.MAX_UDP_PACKET_SIZE):
-                parts.append(msg[0:_utils.MAX_UDP_PACKET_SIZE])
-                msg = msg[_utils.MAX_UDP_PACKET_SIZE:]
+            while (len(msg) > MAX_UDP_PACKET_SIZE):
+                parts.append(msg[0:MAX_UDP_PACKET_SIZE])
+                msg = msg[MAX_UDP_PACKET_SIZE:]
             parts.append(msg)
             for i in range(len(parts)):
                 _utils.send_udp(self.__udp_socket,self.__tcp_socket.getsockname()[1],self.__get_actual_address(address),parts[i],self.__udp_seq,i,len(parts))
         self.__udp_seq += 1
     def __has_client(self,address):
         for client in self.__clients:
             client_address = client.getpeername()
```

### Comparing `netpywork-0.0.4/netpywork/utils.py` & `netpywork-0.0.5/netpywork/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     length:int = -1
     port:int = -1
     address: tuple = ()
     data:bytes = None
     closing:bool = False
 
 class _utils:
-    MAX_UDP_PACKET_SIZE = 65507 - 4 - 2 - 4 - 2 - 2
     def peek_udp(sock: socket.socket,size: int):
             buffer = bytearray(size)
             # Windows workaround as it errors out with errorcode 10040 even though it peeked the msg
             try:
                 sock.recv_into(buffer,size,socket.MSG_PEEK)
             except OSError as ex:
                 if(ex.errno != 10040):
@@ -79,14 +78,15 @@
         udp_message.seq_no = seqno
         udp_message.seq_id = seqid
         return udp_message
     def read_tcp_msg(socket: socket.socket):
         length = socket.recv(4)
         length = int.from_bytes(length,"big")
         buffer = socket.recv(length)
+        # TCP not always reads the entire message, read byte by byte untill length is correct
         while len(buffer) < length:
             buffer += socket.recv(1)
         buffer = bytearray(buffer)
         close_con = int.from_bytes(_utils.read_message(buffer,1),"big") == 1
         result = _utils.read_message(buffer)
         address = socket.getpeername()
         tcp_message = tcp_msg()
```

### Comparing `netpywork-0.0.4/netpywork.egg-info/PKG-INFO` & `netpywork-0.0.5/netpywork.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: netpywork
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python library that simplifies UDP and TCP server and client
 Home-page: https://github.com/MurkyYT/netpywork
 Author: Murky
 Author-email: shooterkingof@gmail.com
 License: UNKNOWN
 Description: # netpywork
         **netpywork** is a library that makes using tcp and udp server and client easier
         
         # Features
         - Creating a server and client which uses `TCP` and `UDP`
         - Callbacks for `On Receive`, `On Connect` and `On Disconnect` for server
         - Callbacks for `On Receive` and `On Connect` for client
-        - Sending messages from server to client both with tcp and udp by specifing the address to send to `(see examples [here](https://github.com/MurkyYT/netpywork/tree/main))`
+        - Sending messages from server to client both with tcp and udp by specifing the address to send to (see examples [here](https://github.com/MurkyYT/netpywork/tree/main))
         - Sending *large* `UDP` messages
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `netpywork-0.0.4/setup.py` & `netpywork-0.0.5/setup.py`

 * *Files identical despite different names*

