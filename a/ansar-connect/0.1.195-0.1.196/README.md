# Comparing `tmp/ansar_connect-0.1.195.tar.gz` & `tmp/ansar_connect-0.1.196.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.195.tar", last modified: Wed Apr 17 16:32:52 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.196.tar", last modified: Wed Apr 17 16:53:26 2024, max compression
```

## Comparing `ansar_connect-0.1.195.tar` & `ansar_connect-0.1.196.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 16:32:52.939198 ansar_connect-0.1.195/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.195/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-17 16:32:52.939198 ansar_connect-0.1.195/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.195/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.195/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-17 16:32:52.939198 ansar_connect-0.1.195/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.195/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 16:32:52.935197 ansar_connect-0.1.195/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 16:32:52.935197 ansar_connect-0.1.195/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 16:32:52.935197 ansar_connect-0.1.195/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.195/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.195/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.195/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.195/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 16:32:52.939198 ansar_connect-0.1.195/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3063 2024-04-17 16:32:49.000000 ansar_connect-0.1.195/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14167 2024-04-15 03:23:57.000000 ansar_connect-0.1.195/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    77934 2024-04-17 02:33:18.000000 ansar_connect-0.1.195/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.195/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.195/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.195/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.195/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.195/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.195/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.195/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.195/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.195/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.195/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.195/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    41146 2024-04-17 16:31:38.000000 ansar_connect-0.1.195/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.195/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2171 2024-04-17 04:03:15.000000 ansar_connect-0.1.195/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.195/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.195/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 16:32:52.939198 ansar_connect-0.1.195/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-17 16:32:52.000000 ansar_connect-0.1.195/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-04-17 16:32:52.000000 ansar_connect-0.1.195/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-17 16:32:52.000000 ansar_connect-0.1.195/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-17 16:32:52.000000 ansar_connect-0.1.195/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-04-17 16:32:52.000000 ansar_connect-0.1.195/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-17 16:32:52.000000 ansar_connect-0.1.195/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 16:53:26.331529 ansar_connect-0.1.196/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.196/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-17 16:53:26.331529 ansar_connect-0.1.196/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.196/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.196/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-17 16:53:26.331529 ansar_connect-0.1.196/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.196/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 16:53:26.327528 ansar_connect-0.1.196/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 16:53:26.327528 ansar_connect-0.1.196/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 16:53:26.327528 ansar_connect-0.1.196/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.196/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.196/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.196/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.196/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 16:53:26.331529 ansar_connect-0.1.196/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3063 2024-04-17 16:53:23.000000 ansar_connect-0.1.196/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14167 2024-04-15 03:23:57.000000 ansar_connect-0.1.196/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    77934 2024-04-17 02:33:18.000000 ansar_connect-0.1.196/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.196/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.196/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.196/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.196/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.196/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.196/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.196/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.196/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.196/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.196/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.196/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    41215 2024-04-17 16:52:37.000000 ansar_connect-0.1.196/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.196/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2171 2024-04-17 04:03:15.000000 ansar_connect-0.1.196/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.196/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.196/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 16:53:26.331529 ansar_connect-0.1.196/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-17 16:53:26.000000 ansar_connect-0.1.196/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-04-17 16:53:26.000000 ansar_connect-0.1.196/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-17 16:53:26.000000 ansar_connect-0.1.196/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-17 16:53:26.000000 ansar_connect-0.1.196/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-04-17 16:53:26.000000 ansar_connect-0.1.196/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-17 16:53:26.000000 ansar_connect-0.1.196/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.195/LICENSE` & `ansar_connect-0.1.196/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.195/PKG-INFO` & `ansar_connect-0.1.196/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.195
+Version: 0.1.196
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.195/README.md` & `ansar_connect-0.1.196/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.195/pyproject.toml` & `ansar_connect-0.1.196/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.195/setup.py` & `ansar_connect-0.1.196/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.195/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.196/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.195/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.196/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.195/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.196/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.195/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.196/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.195/src/ansar/connect/__init__.py` & `ansar_connect-0.1.196/src/ansar/connect/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 93c6328a7a7440ebdb3e36c4f8568379498fdbc3
-Version: 0.1.194 (2024-04-18@04:32:49+NZST)
+Commit: d2a56e772be02e3e22b10a414d361fd9f9cfc5da
+Version: 0.1.195 (2024-04-18@04:53:23+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.195/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.196/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.195/src/ansar/connect/directory.py` & `ansar_connect-0.1.196/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.195/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.196/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.195/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.196/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.195/src/ansar/connect/group_if.py` & `ansar_connect-0.1.196/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.195/src/ansar/connect/grouping.py` & `ansar_connect-0.1.196/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.195/src/ansar/connect/moving.py` & `ansar_connect-0.1.196/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.195/src/ansar/connect/networking.py` & `ansar_connect-0.1.196/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.195/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.196/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.195/src/ansar/connect/node.py` & `ansar_connect-0.1.196/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.195/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.196/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.195/src/ansar/connect/procedure.py` & `ansar_connect-0.1.196/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.195/src/ansar/connect/product.py` & `ansar_connect-0.1.196/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.195/src/ansar/connect/socketry.py` & `ansar_connect-0.1.196/src/ansar/connect/socketry.py`

 * *Files 0% similar despite different names*

```diff
@@ -623,14 +623,16 @@
 			if v is not None:
 				if not self.upgrade:
 					raise ValueError(f'body version "{v}" and no upgrade')
 				body = self.upgrade(body, v)
 
 			if isinstance(body, Diffie):
 				sockets.send(Hellman(body.public_key), self.remote_address)
+				h = self.diffie_hellman[0]
+				sockets.forward(h[0], h[1], h[2])
 			elif isinstance(body, Hellman):
 				public_bytes = bytes(body.public_key)
 				public_key = PublicKey(public_bytes)
 				self.key_box = Box(self.private_key, public_key)
 				h = self.diffie_hellman[0]
 				sockets.forward(h[0], h[1], h[2])
 			else:
```

### Comparing `ansar_connect-0.1.195/src/ansar/connect/standard.py` & `ansar_connect-0.1.196/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.195/src/ansar/connect/transporting.py` & `ansar_connect-0.1.196/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.195/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.196/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.195/src/ansar/connect/wan.py` & `ansar_connect-0.1.196/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.195/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.196/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.195
+Version: 0.1.196
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.195/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.196/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

