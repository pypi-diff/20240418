# Comparing `tmp/pysharek-0.10.0.tar.gz` & `tmp/pysharek-0.10.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysharek-0.10.0.tar", last modified: Wed Apr 17 13:00:10 2024, max compression
+gzip compressed data, was "pysharek-0.10.3.tar", last modified: Thu Apr 18 18:15:31 2024, max compression
```

## Comparing `pysharek-0.10.0.tar` & `pysharek-0.10.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-04-17 13:00:10.073189 pysharek-0.10.0/
--rw-r--r--   0 the220th  (1000) the220th  (1000)     1066 2023-11-16 09:09:35.000000 pysharek-0.10.0/LICENSE
--rw-r--r--   0 the220th  (1000) the220th  (1000)      693 2024-04-17 13:00:10.073189 pysharek-0.10.0/PKG-INFO
--rw-r--r--   0 the220th  (1000) the220th  (1000)      103 2023-11-16 08:55:11.000000 pysharek-0.10.0/README.md
--rw-r--r--   0 the220th  (1000) the220th  (1000)      853 2024-04-17 12:59:36.000000 pysharek-0.10.0/pyproject.toml
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-04-17 13:00:10.072189 pysharek-0.10.0/pysharek/
--rw-r--r--   0 the220th  (1000) the220th  (1000)       24 2023-11-16 09:11:39.000000 pysharek-0.10.0/pysharek/__init__.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)      390 2024-04-17 12:54:50.000000 pysharek-0.10.0/pysharek/__main__.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     2194 2023-11-18 17:28:54.000000 pysharek-0.10.0/pysharek/args.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     6799 2023-11-18 13:15:55.000000 pysharek-0.10.0/pysharek/crypto.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     1512 2024-04-17 11:49:02.000000 pysharek-0.10.0/pysharek/hashes_work.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     1150 2024-04-17 12:56:59.000000 pysharek-0.10.0/pysharek/main.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     5646 2023-11-18 16:47:34.000000 pysharek-0.10.0/pysharek/net.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     4018 2024-04-17 11:49:02.000000 pysharek-0.10.0/pysharek/sup.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)    13273 2024-04-17 12:52:20.000000 pysharek-0.10.0/pysharek/work.py
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-04-17 13:00:10.073189 pysharek-0.10.0/pysharek.egg-info/
--rw-r--r--   0 the220th  (1000) the220th  (1000)      693 2024-04-17 13:00:10.000000 pysharek-0.10.0/pysharek.egg-info/PKG-INFO
--rw-r--r--   0 the220th  (1000) the220th  (1000)      394 2024-04-17 13:00:10.000000 pysharek-0.10.0/pysharek.egg-info/SOURCES.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)        1 2024-04-17 13:00:10.000000 pysharek-0.10.0/pysharek.egg-info/dependency_links.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)       48 2024-04-17 13:00:10.000000 pysharek-0.10.0/pysharek.egg-info/entry_points.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)       37 2024-04-17 13:00:10.000000 pysharek-0.10.0/pysharek.egg-info/requires.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)        9 2024-04-17 13:00:10.000000 pysharek-0.10.0/pysharek.egg-info/top_level.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)       38 2024-04-17 13:00:10.073189 pysharek-0.10.0/setup.cfg
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-04-18 18:15:31.112906 pysharek-0.10.3/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     1066 2024-04-18 18:14:26.000000 pysharek-0.10.3/LICENSE
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      693 2024-04-18 18:15:31.111906 pysharek-0.10.3/PKG-INFO
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      103 2024-04-18 18:14:26.000000 pysharek-0.10.3/README.md
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     1011 2024-04-18 18:14:26.000000 pysharek-0.10.3/pyproject.toml
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-04-18 18:15:31.111906 pysharek-0.10.3/pysharek/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       63 2024-04-18 18:14:26.000000 pysharek-0.10.3/pysharek/__init__.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      390 2024-04-18 18:14:26.000000 pysharek-0.10.3/pysharek/__main__.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       48 2024-04-18 18:14:26.000000 pysharek-0.10.3/pysharek/__version__.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     2378 2024-04-18 18:14:26.000000 pysharek-0.10.3/pysharek/args.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     6799 2024-04-18 18:14:26.000000 pysharek-0.10.3/pysharek/crypto.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     1512 2024-04-18 18:14:26.000000 pysharek-0.10.3/pysharek/hashes_work.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      969 2024-04-18 18:14:26.000000 pysharek-0.10.3/pysharek/main.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     5646 2024-04-18 18:14:26.000000 pysharek-0.10.3/pysharek/net.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     4065 2024-04-18 18:14:26.000000 pysharek-0.10.3/pysharek/sup.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)    14359 2024-04-18 18:14:26.000000 pysharek-0.10.3/pysharek/work.py
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-04-18 18:15:31.111906 pysharek-0.10.3/pysharek.egg-info/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      693 2024-04-18 18:15:31.000000 pysharek-0.10.3/pysharek.egg-info/PKG-INFO
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      418 2024-04-18 18:15:31.000000 pysharek-0.10.3/pysharek.egg-info/SOURCES.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)        1 2024-04-18 18:15:31.000000 pysharek-0.10.3/pysharek.egg-info/dependency_links.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       48 2024-04-18 18:15:31.000000 pysharek-0.10.3/pysharek.egg-info/entry_points.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       37 2024-04-18 18:15:31.000000 pysharek-0.10.3/pysharek.egg-info/requires.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)        9 2024-04-18 18:15:31.000000 pysharek-0.10.3/pysharek.egg-info/top_level.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       38 2024-04-18 18:15:31.112906 pysharek-0.10.3/setup.cfg
```

### Comparing `pysharek-0.10.0/LICENSE` & `pysharek-0.10.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pysharek-0.10.0/PKG-INFO` & `pysharek-0.10.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysharek
-Version: 0.10.0
+Version: 0.10.3
 Summary: Share file with encryption and hash checking
 Author-email: The220th <author@example.com>
 Project-URL: Homepage, https://github.com/The220th/pysharek
 Project-URL: Issues, https://github.com/The220th/pysharek/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pysharek-0.10.0/pyproject.toml` & `pysharek-0.10.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysharek"
-version = "0.10.0"
+dynamic = ["version"]
 authors = [
   { name="The220th", email="author@example.com" },
 ]
 description = "Share file with encryption and hash checking"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -18,14 +18,19 @@
 ]
 dependencies = [
     "cryptography",
     "argparse",
     "alive_progress"
 ]
 
+# [metadata]
+[tool.setuptools.dynamic]
+version = {attr = "pysharek.__version__"}
+# https://github.com/pypa/setuptools/issues/2530#issuecomment-1135391647
+
 # [console_scripts]
 [project.scripts]
 pysharek = "pysharek.main:main"
 # my_script = "my_package.my_module:main"
 # https://packaging.python.org/en/latest/specifications/entry-points/#use-for-scripts
 
 [project.urls]
```

### Comparing `pysharek-0.10.0/pysharek/crypto.py` & `pysharek-0.10.3/pysharek/crypto.py`

 * *Files identical despite different names*

### Comparing `pysharek-0.10.0/pysharek/hashes_work.py` & `pysharek-0.10.3/pysharek/hashes_work.py`

 * *Files identical despite different names*

### Comparing `pysharek-0.10.0/pysharek/net.py` & `pysharek-0.10.3/pysharek/net.py`

 * *Files identical despite different names*

### Comparing `pysharek-0.10.0/pysharek/sup.py` & `pysharek-0.10.3/pysharek/sup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,20 @@
 
 
 class Global:
     version = None
     outfile = None
     logfile = None
     log_debug = None
+    yes_always = None
     file_dir = None
     sock: "socket" = None
     cipher: "PycaAES256CBC or PycaFernet" = None
     file_size_4_message = 262144  # 256 KB  # 1048576  # 1 MB
+    hash_4_thread = None
 
 
 def pout(msg: str, endl=True):
     if not endl:
         pout_low(msg)
     else:
         pout_low(msg + "\n")
```

### Comparing `pysharek-0.10.0/pysharek/work.py` & `pysharek-0.10.3/pysharek/work.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 
 import sys
 import os
 import io
 import json
 import argparse
 import hashlib
+import threading
+import time
 
 from .sup import *
 from .net import *
-from .crypto import PycaAES256CBC
 from .hashes_work import calc_hash_file
 from .hashes_work import calc_hash_dir
 from .sup import get_dirs_needed_for_files
 
 
 def work_as_sender(args: "argparse.Namespace"):
     # python -m pysharek --mode send --connect server --port 1337
@@ -32,14 +33,22 @@
         exit()
     else:
         pout(f"Failed successfully (what is file \"{file}\")")
         Global.sock.close()
         exit()
 
 
+def calc_hash_4_thread(path: str, dir_file: bool):
+    if dir_file == False:
+        calculated_hash = calc_hash_dir(path, True)
+    else:
+        calculated_hash = calc_hash_file(path)
+    Global.hash_4_thread = calculated_hash
+
+
 def send_file(file_name: str):
     file = os.path.abspath(file_name)
     plog(f"File (not dir) \"{file}\" will be sended", 1)
     sock = Global.sock
     meta = build_file_meta(file)
     plog(f"meta={meta}", 4)
     plog("Sending meta...", 1)
@@ -88,29 +97,29 @@
     files = sorted(meta["files"].keys())
     sock = Global.sock
     plog(f"meta={meta}", 4)
     plog("Sending meta...", 1)
     send_crypto_msg(sock, meta, b"")
     plog("Meta sended!", 1)
     with alive_bar(meta["dir_size"]) as bar:
-        for file_i in files:
+        for file_i_num, file_i in enumerate(files):
             # print(file_i)
             # input()
             file = os.path.join(dir_name, file_i)
             with open(file, "rb") as fd:
                 file_size = meta["files"][file_i]["size"]
                 plog(f"File size {file_size} bytes", 4)
                 readed = 0
                 block_size = Global.file_size_4_message
                 file_buffer = fd.read(block_size)
                 bar(len(file_buffer)-1)  # I do not know why need -1?!
                 readed += len(file_buffer)
                 while len(file_buffer) > 0:
                     while True:
-                        js_send = {"type": "sending", "file_count": 1, "slice": readed}
+                        js_send = {"type": "sending", "file_num": file_i_num, "slice": readed}
                         plog(f"Sendeding: {js_send} + data", 4)
                         send_crypto_msg(sock, js_send, file_buffer)
                         plog(f"Sended", 4)
                         js, bs = recv_crypto_msg(sock)
                         plog(f"Received js={js}", 4)
                         if "type" not in js or js["type"] != "received":
                             pout("Cannot send block. Trying again.")
@@ -199,32 +208,45 @@
                     send_crypto_msg(sock, answer, b"")
                     plog(f"Sended", 4)
                     fd.write(file_buffer)
                     fd.flush()
                     bar(len(file_buffer))
                     break
     pout(f"Receiving and calculating hash...")
+
+    x = threading.Thread(target=calc_hash_4_thread, args=(file, True))
+    x.start()
+
     js, trash = recv_crypto_msg(sock)
     if "type" not in js or js["type"] != "hash":
         pout(f"Cannot receive hash. Exiting")
         Global.sock.close()
         exit()
     recv_hash = js["hash"]
     pout(f"\"{recv_hash}\" is received hash")
-    file_hash = calc_hash_file(file)
+    # file_hash = calc_hash_file(file)
+    while Global.hash_4_thread is None:
+        time.sleep(1.0)  # Dude, what is join?
+    file_hash = Global.hash_4_thread
     pout(f"\"{file_hash}\" is hash of file=\"{file}\"")
+    pout(f"Comparing hashes: \"{recv_hash}\" (recieved) vs \"{file_hash}\" (calculating)")
     if recv_hash != file_hash:
         pout(f"{'='*15} HASHES DOES NOT MATCH!!! {'='*15}")
     else:
         pout(f"Hashes matched. All is OK!")
 
 
 def receive_dir(dir_name: str, meta: dict):
-    # TODO: check if dir exists and if this not empty
     dir_name = os.path.abspath(dir_name)
+    if Global.yes_always == False:
+        if len(get_files_list(dir_name)) != 0:
+            user_in = input(f"Directory \"{dir_name}\" is not empty!!! Continue? (Y): ")
+            if user_in.strip().lower() not in ["", "y", "1", "yes", "yep"]:
+                exit()
+
     plog(f"Dir will be received", 1)
     sock = Global.sock
     files = sorted(meta["files"].keys())
     files_4_dirs = [os.path.join(dir_name, file_i) for file_i in files]
     needed_dirs = get_dirs_needed_for_files(files_4_dirs)
     for needed_dir_i in needed_dirs:
         mkdir_with_p(needed_dir_i)
@@ -256,23 +278,31 @@
                         send_crypto_msg(sock, answer, b"")
                         plog(f"Sended", 4)
                         fd.write(file_buffer)
                         fd.flush()
                         bar(len(file_buffer))
                         break
     pout(f"Receiving and calculating hash...")
+
+    x = threading.Thread(target=calc_hash_4_thread, args=(dir_name, False))
+    x.start()
+
     js, trash = recv_crypto_msg(sock)
     if "type" not in js or js["type"] != "hash":
         pout(f"Cannot receive hash. Exiting")
         Global.sock.close()
         exit()
     recv_hash = js["hash"]
-    pout(f"\"{recv_hash}\" is received hash")
-    dir_hash = calc_hash_dir(dir_name, True)
+    pout(f"\n\"{recv_hash}\" is received hash")
+    # dir_hash = calc_hash_dir(dir_name, True)
+    while Global.hash_4_thread is None:
+        time.sleep(1.0)  # Dude, what is join?
+    dir_hash = Global.hash_4_thread
     pout(f"\"{dir_hash}\" is hash of dir=\"{dir_name}\"")
+    pout(f"Comparing hashes: \"{recv_hash}\" (recieved) vs \"{dir_hash}\" (calculating)")
     if recv_hash != dir_hash:
         pout(f"{'='*15} HASHES DOES NOT MATCH!!! {'='*15}")
     else:
         pout(f"Hashes matched. All is OK!")
 
 
 def common_block_of_sender_and_receiver(args: "argparse.Namespace"):
```

### Comparing `pysharek-0.10.0/pysharek.egg-info/PKG-INFO` & `pysharek-0.10.3/pysharek.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysharek
-Version: 0.10.0
+Version: 0.10.3
 Summary: Share file with encryption and hash checking
 Author-email: The220th <author@example.com>
 Project-URL: Homepage, https://github.com/The220th/pysharek
 Project-URL: Issues, https://github.com/The220th/pysharek/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

