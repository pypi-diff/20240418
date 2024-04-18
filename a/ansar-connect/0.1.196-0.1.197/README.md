# Comparing `tmp/ansar_connect-0.1.196.tar.gz` & `tmp/ansar_connect-0.1.197.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.196.tar", last modified: Wed Apr 17 16:53:26 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.197.tar", last modified: Thu Apr 18 00:11:15 2024, max compression
```

## Comparing `ansar_connect-0.1.196.tar` & `ansar_connect-0.1.197.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 16:53:26.331529 ansar_connect-0.1.196/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.196/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-17 16:53:26.331529 ansar_connect-0.1.196/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.196/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.196/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-17 16:53:26.331529 ansar_connect-0.1.196/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.196/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 16:53:26.327528 ansar_connect-0.1.196/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 16:53:26.327528 ansar_connect-0.1.196/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 16:53:26.327528 ansar_connect-0.1.196/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.196/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.196/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.196/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.196/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 16:53:26.331529 ansar_connect-0.1.196/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3063 2024-04-17 16:53:23.000000 ansar_connect-0.1.196/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14167 2024-04-15 03:23:57.000000 ansar_connect-0.1.196/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    77934 2024-04-17 02:33:18.000000 ansar_connect-0.1.196/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.196/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.196/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.196/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.196/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.196/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.196/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.196/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.196/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.196/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.196/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.196/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    41215 2024-04-17 16:52:37.000000 ansar_connect-0.1.196/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.196/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2171 2024-04-17 04:03:15.000000 ansar_connect-0.1.196/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.196/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.196/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 16:53:26.331529 ansar_connect-0.1.196/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-17 16:53:26.000000 ansar_connect-0.1.196/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-04-17 16:53:26.000000 ansar_connect-0.1.196/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-17 16:53:26.000000 ansar_connect-0.1.196/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-17 16:53:26.000000 ansar_connect-0.1.196/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-04-17 16:53:26.000000 ansar_connect-0.1.196/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-17 16:53:26.000000 ansar_connect-0.1.196/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-18 00:11:15.918581 ansar_connect-0.1.197/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.197/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-18 00:11:15.918581 ansar_connect-0.1.197/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.197/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.197/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-18 00:11:15.918581 ansar_connect-0.1.197/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.197/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-18 00:11:15.914581 ansar_connect-0.1.197/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-18 00:11:15.914581 ansar_connect-0.1.197/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-18 00:11:15.914581 ansar_connect-0.1.197/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-17 22:39:03.000000 ansar_connect-0.1.197/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3206 2024-04-18 00:04:05.000000 ansar_connect-0.1.197/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.197/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8819 2024-04-18 00:04:05.000000 ansar_connect-0.1.197/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-18 00:11:15.918581 ansar_connect-0.1.197/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-04-18 00:11:12.000000 ansar_connect-0.1.197/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.197/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    77775 2024-04-18 00:04:05.000000 ansar_connect-0.1.197/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.197/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.197/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.197/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.197/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.197/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.197/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.197/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.197/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.197/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    32848 2024-04-17 22:39:03.000000 ansar_connect-0.1.197/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.197/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    40868 2024-04-18 00:04:05.000000 ansar_connect-0.1.197/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.197/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2101 2024-04-17 21:48:32.000000 ansar_connect-0.1.197/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.197/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6600 2024-04-18 00:04:05.000000 ansar_connect-0.1.197/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-18 00:11:15.918581 ansar_connect-0.1.197/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-18 00:11:15.000000 ansar_connect-0.1.197/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-04-18 00:11:15.000000 ansar_connect-0.1.197/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-18 00:11:15.000000 ansar_connect-0.1.197/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-18 00:11:15.000000 ansar_connect-0.1.197/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-04-18 00:11:15.000000 ansar_connect-0.1.197/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-18 00:11:15.000000 ansar_connect-0.1.197/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.196/LICENSE` & `ansar_connect-0.1.197/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.196/PKG-INFO` & `ansar_connect-0.1.197/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.196
+Version: 0.1.197
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.196/README.md` & `ansar_connect-0.1.197/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.196/pyproject.toml` & `ansar_connect-0.1.197/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.196/setup.py` & `ansar_connect-0.1.197/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.196/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.197/src/ansar/command/ansar_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,31 +328,31 @@
 	(directory, directory_settings),
 )
 
 
 #
 #
 class Settings(object):
-	def __init__(self, force=False, cloud_ip=None, SNI=None, login_token=None):
+	def __init__(self, force=False, cloud_ip=None, encrypted=False, login_token=None):
 		'''
 		* force
 		Override cautionary behaviour, mostly relating to the unintended termination
 		or running processes.
 		* cloud_ip
 		Domain name or dotted IP address.
 		'''
 		self.force = force
 		self.cloud_ip = cloud_ip
-		self.SNI = SNI
+		self.encrypted = encrypted
 		self.login_token = login_token
 
 SETTINGS_SCHEMA = {
 	'force': ar.Boolean(),
 	'cloud_ip': ar.Unicode(),
-	'SNI': ar.Unicode(),
+	'encrypted': ar.Boolean(),
 	'login_token': ar.UUID(),
 }
 
 ar.bind(Settings, object_schema=SETTINGS_SCHEMA)
 
 #
 #
@@ -443,15 +443,15 @@
 		return e.value
 	return output
 
 ar.bind(ansar)
 
 #
 #
-factory_settings = Settings(cloud_ip=FOH_HOST, SNI=FOH_HOST)
+factory_settings = Settings(cloud_ip=FOH_HOST, encrypted=True)
 
 def main():
 	ar.create_object(ansar, factory_settings=factory_settings, parameter_passing=ar.sub_object_passing, parameter_table=table)
 
 # The standard entry point. Needed for IDEs
 # and debugger sessions.
 if __name__ == '__main__':
```

### Comparing `ansar_connect-0.1.196/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.197/src/ansar/command/ansar_directory.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,38 +31,33 @@
 	'main',
 ]
 
 #
 #
 class Settings(object):
 	def __init__(self, directory_scope=None, connect_above=None, accept_below=None,
-			certificate_file=None, key_file=None):
+			encrypted=False):
 		self.directory_scope = directory_scope or ar.ScopeOfService.HOST
 		self.connect_above = connect_above or ar.HostPort()
 		self.accept_below = accept_below or ar.HostPort()
-		self.certificate_file = certificate_file
-		self.key_file = key_file
+		self.encrypted = encrypted
 
 SETTINGS_SCHEMA = {
 	'directory_scope': ar.ScopeOfService,
 	'connect_above': ar.Any(),
 	'accept_below': ar.UserDefined(ar.HostPort),
-	'certificate_file': ar.Unicode(),
-	'key_file': ar.Unicode(),
+	'encrypted': ar.Boolean(),
 }
 
 ar.bind(Settings, object_schema=SETTINGS_SCHEMA)
 
 # Just need an object to stay "on duty" while the 
 # global ServiceDirectory does its work.
 def directory(self, settings):
-	encrypted = None
-	if settings.certificate_file and settings.key_file:
-		encrypted = ar.TlsServer(certificate_file=settings.certificate_file, key_file=settings.key_file)
-
+	encrypted = settings.encrypted
 	a = self.create(ar.ServiceDirectory, settings.directory_scope,
 		settings.connect_above, settings.accept_below,
 		encrypted=encrypted)
 	m = self.select(ar.HostPort, ar.Completed, ar.Stop)
 	if isinstance(m, ar.Completed):
 		return m.value
 	elif isinstance(m, ar.Stop):
```

### Comparing `ansar_connect-0.1.196/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.197/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.196/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.197/src/ansar/command/shared_directory.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,18 +80,15 @@
 	self.store = store
 	self.recover = recover
 
 	# Initial load.
 	self.recover()
 
 	settings = self.settings
-	encrypted = None
-	if settings.certificate_file and settings.key_file:
-		encrypted = ar.TlsServer(certificate_file=settings.certificate_file, key_file=settings.key_file)
-
+	encrypted = settings.encrypted
 	ar.listen(self, self.settings.public_access, encrypted=encrypted)
 	return STARTING
 
 # Verify access
 def ProductDirectory_STARTING_Listening(self, message):
 	self.public_access = message
 	return READY
@@ -275,25 +272,23 @@
 
 ar.bind(ProductDirectory, PRODUCT_DIRECTORY_DISPATCH)
 
 
 # Allow configuration of network details.
 #
 class Settings(object):
-	def __init__(self, directory_scope=None, public_access=None, certificate_file=None, key_file=None):
+	def __init__(self, directory_scope=None, public_access=None, encrypted=False):
 		self.directory_scope = directory_scope
 		self.public_access = public_access or ar.HostPort()
-		self.certificate_file = certificate_file
-		self.key_file = key_file
+		self.encrypted = encrypted
 
 SETTINGS_SCHEMA = {
 	'directory_scope': ar.ScopeOfService,
 	'public_access': ar.UserDefined(ar.HostPort),
-	'certificate_file': ar.Unicode(),
-	'key_file': ar.Unicode(),
+	'encrypted': ar.Boolean(),
 }
 
 ar.bind(Settings, object_schema=SETTINGS_SCHEMA)
 
 #
 #
 factory_settings = Settings(directory_scope=ar.ScopeOfService.HOST,
```

### Comparing `ansar_connect-0.1.196/src/ansar/connect/__init__.py` & `ansar_connect-0.1.197/src/ansar/connect/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,31 +21,30 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: d2a56e772be02e3e22b10a414d361fd9f9cfc5da
-Version: 0.1.195 (2024-04-18@04:53:23+NZST)
+Commit: 3d8a1b9ff207d3e3f2b32173e44ee57f736b99f3
+Version: 0.1.196 (2024-04-18@12:11:12+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
 
 from .socketry import HostPort, LocalPort
 from .socketry import ScopeOfIP, local_private_public
 from .socketry import Blob, CreateFrame
 from .socketry import Listening, NotListening, Accepted, NotAccepted, StopListening
 from .socketry import Connected, NotConnected
 from .socketry import Close, Closed, Abandoned
-from .socketry import TlsServer, TlsClient
-from .transporting import listen, connect, stop_listen, wrench
+from .transporting import listen, connect, stop_listen
 
 from .plumbing import RETRY_LOCAL, RETRY_PRIVATE, RETRY_PUBLIC
 from .plumbing import ip_retry
 
 from .directory_if import ScopeOfService
 from .directory_if import Published, NotPublished, Subscribed
 from .directory_if import Available, NotAvailable, Delivered, NotDelivered
```

### Comparing `ansar_connect-0.1.196/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.197/src/ansar/connect/connect_directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,33 +69,32 @@
 
 		self.closing = None
 		self.intervals = None
 		self.retry = None
 
 	def connect(self):
 		c = self.connect_above
-		encrypted = None
 		if isinstance(c, HostPort):
 			ipp = c
+			encrypted = False
 			next = PENDING
 		elif isinstance(c, ProductAccess):
 			ipp = c.access_ipp
-			if c.SNI:
-				encrypted = TlsClient(SNI=c.SNI)
+			encrypted = c.encrypted
 			next = PRODUCING
 		elif isinstance(c, WideAreaAccess):
 			ipp = c.access_ipp
-			if c.SNI:
-				encrypted = TlsClient(SNI=c.SNI)
+			encrypted = c.encrypted
 			next = CLOUDY
 		else:
 			return DISABLED
 
 		if ipp.host is None:
 			return DISABLED
+
 		connect(self, ipp, session=self.session, encrypted=encrypted)
 		self.start(ar.T1, seconds=8.0)
 		return next
 
 	def reschedule(self):
 		if self.intervals is None:
 			c = self.connect_above
@@ -271,19 +270,16 @@
 	# Connected could be orphaned here.
 	self.complete(ar.Aborted())
 
 def ConnectToDirectory_LOOKING_WideAreaRedirect(self, message):
 	self.redirect = message
 	ipp = message.redirect_ipp
 	self.trace(f'Redirecting from FOH to WAN ({ipp})')
-	if message.SNI:
-		encrypted = TlsClient(message.SNI)
-		connect(self, ipp, encrypted=encrypted)
-	else:
-		connect(self, ipp)
+	encrypted = message.encrypted
+	connect(self, ipp, encrypted=encrypted)
 		
 	self.reply(Close())
 	return REDIRECTING
 
 def ConnectToDirectory_LOOKING_Faulted(self, message):
 	self.trace(f'Access denied - {message}')
 	self.send(Close(message), self.connected.remote_address)
```

### Comparing `ansar_connect-0.1.196/src/ansar/connect/directory.py` & `ansar_connect-0.1.197/src/ansar/connect/directory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1377,19 +1377,16 @@
 		n = len(r[1])
 		self.trace(f'Peer for relay "{key}" already known ({n} routes pending)')
 	except KeyError:
 		r = [None, {key: relay}]
 		self.peered[k] = r
 
 		self.trace(f'Opening peer "{k}" (relay {key})')
-		if message.redirect.SNI:
-			encrypted = ar.TlsClient(SNI=message.redirect.SNI)
-			open = OpenPeer(ipp, key, encrypted=encrypted)
-		else:
-			open = OpenPeer(ipp, key)
+		encrypted = message.redirect.encrypted
+		open = OpenPeer(ipp, key, encrypted=encrypted)
 		self.send(open, pb.house)
 		return READY
 
 	if r[0] is None:
 		return READY
 
 	self.send(relay, r[0])
@@ -1635,19 +1632,16 @@
 		self.start(ar.T2, SECONDS_OF_PEERING)
 
 	def open_relay(self):
 		key = self.route.key
 		ipp = self.route.redirect.redirect_ipp
 		self.peer_ipp = ipp
 		self.trace(f'Requests relay {ipp} for "{key}"')
-		if self.route.redirect.SNI:
-			encrypted = ar.TlsClient(SNI=self.route.redirect.SNI)
-			open = OpenPeer(ipp, key, encrypted=encrypted)
-		else:
-			open = OpenPeer(ipp, key)
+		encrypted = self.route.redirect.encrypted
+		open = OpenPeer(ipp, key, encrypted=encrypted)
 		self.send(open, pb.house)
 		self.start(ar.T2, SECONDS_OF_PEERING)
 
 	def open_latch(self, message):
 		self.remote_loop = self.return_address
 		self.remote_session = message.publisher_session
 		if self.create_session:
```

### Comparing `ansar_connect-0.1.196/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.197/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.196/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.197/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.196/src/ansar/connect/group_if.py` & `ansar_connect-0.1.197/src/ansar/connect/group_if.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,29 +31,29 @@
 
 __all__ = [
 	'GroupSettings',
 ]
 
 class GroupSettings(object):
 	def __init__(self, connect_above=None, roles=None, main_role=None, forwarding=False,
-		show_scopes=None, connect_scope=None, connect_file=None, SNI=None):
+		show_scopes=None, connect_scope=None, connect_file=None, encrypted=None):
 		self.connect_above = connect_above or HostPort()
 		self.roles = roles
 		self.main_role = main_role
 		self.forwarding = forwarding
 		self.show_scopes = show_scopes
 		self.connect_scope = connect_scope
 		self.connect_file = connect_file
-		self.SNI = SNI
+		self.encrypted = encrypted
 
 GROUP_SETTINGS_SCHEMA = {
 	'connect_above': ar.Any(),
 	'roles': ar.Unicode(),
 	'main_role': ar.Unicode(),
 	'forwarding': ar.Boolean(),
 	'show_scopes': ar.Boolean(),
 	'connect_scope': ScopeOfService,
 	'connect_file': ar.Unicode(),
-	'SNI': ar.Unicode(),
+	'encrypted': ar.Boolean(),
 }
 
 ar.bind(GroupSettings, object_schema=GROUP_SETTINGS_SCHEMA)
```

### Comparing `ansar_connect-0.1.196/src/ansar/connect/grouping.py` & `ansar_connect-0.1.197/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.196/src/ansar/connect/moving.py` & `ansar_connect-0.1.197/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.196/src/ansar/connect/networking.py` & `ansar_connect-0.1.197/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.196/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.197/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.196/src/ansar/connect/node.py` & `ansar_connect-0.1.197/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.196/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.197/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.196/src/ansar/connect/procedure.py` & `ansar_connect-0.1.197/src/ansar/connect/procedure.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,27 +59,27 @@
 
 # Per-command arguments as required.
 # e.g. command-line parameters specific to create.
 class NetworkSettings(object):
 	def __init__(self, group_name=None, home_path=None,
 			connect_scope=None, to_scope=None,
 			product_name=None, product_instance=None,
-			SNI=None,
+			encrypted=False,
 			custom_host=None, custom_port=None,
 			reserved=False,
 			connect_file=None, connect_disable=False,
 			published_services=False, subscribed_searches=False, routed_matches=False, accepted_processes=False,
 			host_and_port=False, start_time=False):
 		self.group_name = group_name
 		self.home_path = home_path
 		self.connect_scope = connect_scope
 		self.to_scope = to_scope
 		self.product_name = product_name
 		self.product_instance = product_instance
-		self.SNI = SNI
+		self.encrypted = encrypted
 		self.custom_host = custom_host
 		self.custom_port = custom_port
 		self.reserved = reserved
 		self.connect_file = connect_file
 		self.connect_disable = connect_disable
 		self.published_services = published_services
 		self.subscribed_searches = subscribed_searches
@@ -91,15 +91,15 @@
 NETWORK_SETTINGS_SCHEMA = {
 	'group_name': ar.Unicode(),
 	'home_path': ar.Unicode(),
 	'connect_scope': ScopeOfService,
 	'to_scope': ScopeOfService,
 	'product_name': ar.Unicode(),
 	'product_instance': InstanceOfProduct,
-	'SNI': ar.Unicode(),
+	'encrypted': ar.Boolean(),
 	'custom_host': ar.Unicode(),
 	'custom_port': ar.Integer8(),
 	'reserved': ar.Boolean(),
 	'connect_file': ar.Unicode(),
 	'connect_disable': ar.Boolean(),
 	'published_services': ar.Boolean(),
 	'subscribed_searches': ar.Boolean(),
@@ -227,15 +227,15 @@
 			connect_scope = network.connect_scope
 			to_scope = network.to_scope
 			if network.product_name and network.product_instance:		# ProductAccess
 				shared_host = network.custom_host or scope_host(to_scope)
 				shared_port = network.custom_port or ANSAR_SHARED_PORT
 				access_ipp = ar.HostPort(shared_host, shared_port)
 				connect_above= ProductAccess(access_ipp=access_ipp,
-					SNI=network.SNI,
+					encrypted=network.encrypted,
 					product_name=network.product_name,
 					product_instance=network.product_instance)
 			elif network.product_name or network.product_instance:		# Error
 				e = ar.Faulted('need both product name and product instance')
 				raise ar.Incomplete(e)
 			elif network.reserved:										# Reserved space.
 				reserved_host = network.custom_host or scope_host(to_scope)
@@ -512,18 +512,15 @@
 	settings = ar.object_custom_settings()
 	cloud_ip = settings.cloud_ip
 
 	f = crud_address_and_token(1, cloud_ip, uuid.uuid4())
 	if f:
 		return f
 
-	if settings.SNI:
-		encrypted = ar.TlsClient(SNI=settings.SNI)
-	else:
-		encrypted = None
+	encrypted = settings.encrypted
 	ar.connect(self, ar.HostPort(cloud_ip, FOH_PORT), encrypted=encrypted)
 	m = self.select(ar.Connected, ar.NotConnected, ar.Stop)
 	if isinstance(m, ar.Connected):
 		session = self.return_address
 	elif isinstance(m, ar.NotConnected):
 		return m
 	else:
@@ -541,18 +538,15 @@
 	cloud_ip = settings.cloud_ip
 	login_token = settings.login_token
 
 	f = crud_address_and_token(1, cloud_ip, login_token)
 	if f:
 		return f
 
-	if settings.SNI:
-		encrypted = ar.TlsClient(SNI=settings.SNI)
-	else:
-		encrypted = None
+	encrypted = settings.encrypted
 	ar.connect(self, ar.HostPort(cloud_ip, FOH_PORT), encrypted=encrypted)
 	m = self.select(ar.Connected, ar.NotConnected, ar.Stop)
 	if isinstance(m, ar.Connected):
 		session = self.return_address
 	elif isinstance(m, ar.NotConnected):
 		return m
 	else:
@@ -592,18 +586,15 @@
 
 	crud = sum([account.read, account.update, account.delete, account.add_login, account.add_directory])
 
 	f = crud_address_and_token(crud, cloud_ip, login_token)
 	if f:
 		return f
 
-	if settings.SNI:
-		encrypted = ar.TlsClient(SNI=settings.SNI)
-	else:
-		encrypted = None
+	encrypted = settings.encrypted
 	ar.connect(self, ar.HostPort(cloud_ip, FOH_PORT), encrypted=encrypted)
 	m = self.select(ar.Connected, ar.NotConnected, ar.Stop)
 	if isinstance(m, ar.Connected):
 		session = self.return_address
 	elif isinstance(m, ar.NotConnected):
 		return m
 	else:
@@ -814,18 +805,15 @@
 
 	crud = sum([directory.read, directory.update, directory.export])
 
 	f = crud_address_and_token(crud, cloud_ip, login_token)
 	if f:
 		return f
 
-	if settings.SNI:
-		encrypted = ar.TlsClient(SNI=settings.SNI)
-	else:
-		encrypted = None
+	encrypted = settings.encrypted
 	ar.connect(self, ar.HostPort(cloud_ip, FOH_PORT), encrypted=encrypted)
 	m = self.select(ar.Connected, ar.NotConnected, ar.Stop)
 	if isinstance(m, ar.Connected):
 		session = self.return_address
 	elif isinstance(m, ar.NotConnected):
 		return m
 	else:
@@ -914,16 +902,16 @@
 	if not export.access_name:
 		f = ar.Faulted('access name not specified', 'use --access-name=<uuid>')
 		return f
 	self.send(export, session)
 	m = self.select(DirectoryExported, ar.Faulted, ar.Abandoned, ar.Stop)
 	if isinstance(m, DirectoryExported):
 		cloud_ipp = ar.HostPort(cloud_ip, FOH_PORT)
-		SNI = settings.SNI
-		w = WideAreaAccess(access_ipp=cloud_ipp, SNI=SNI, access_token=m.access_token,
+		encrypted = settings.encrypted
+		w = WideAreaAccess(access_ipp=cloud_ipp, encrypted=encrypted, access_token=m.access_token,
 			account_id=m.account_id, directory_id=m.directory_id,
 			product_name=m.product_name, product_instance=m.product_instance)
 		f = output_access(w, directory.export_file)
 		if f:
 			return f
 		return None
 	elif isinstance(m, ar.Faulted):
```

### Comparing `ansar_connect-0.1.196/src/ansar/connect/product.py` & `ansar_connect-0.1.197/src/ansar/connect/product.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,32 +40,32 @@
 	QA=4, STAGING=5, PRODUCTION=6,
 	DEMONSTRATION=7, TRAINING=8, SALES=9,
 	EVALUATION=10, OTHER=11)
 
 #
 #
 class ProductAccess(object):
-	def __init__(self, access_ipp=None, SNI=None, product_name=None, product_instance=None):
+	def __init__(self, access_ipp=None, encrypted=False, product_name=None, product_instance=None):
 		self.access_ipp = access_ipp or ar.HostPort()
-		self.SNI = SNI
+		self.encrypted = encrypted
 		self.product_name = product_name
 		self.product_instance = product_instance
 
 class ProductLookup(object):
 	def __init__(self, product_name=None, product_instance=None):
 		self.product_name = product_name
 		self.product_instance = product_instance
 
 class YourProduct(object):
 	def __init__(self, address=None):
 		self.address = address
 
 INSTANT_SCHEMA = {
 	"access_ipp": ar.UserDefined(ar.HostPort),
-	"SNI": ar.Unicode(),
+	"encrypted": ar.Boolean(),
 	"product_name": ar.Unicode(),
 	"product_instance": InstanceOfProduct,
 	"address": ar.Address(),
 }
 
 ar.bind(ProductAccess, object_schema=INSTANT_SCHEMA)
 ar.bind(ProductLookup, object_schema=INSTANT_SCHEMA)
```

### Comparing `ansar_connect-0.1.196/src/ansar/connect/socketry.py` & `ansar_connect-0.1.197/src/ansar/connect/socketry.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,14 @@
 	'Connected',
 	'NotListening',
 	'NotAccepted',
 	'NotConnected',
 	'Close',
 	'Closed',
 	'Abandoned',
-	'TlsServer',
-	'TlsClient',
 	'SocketSelect',
 	'SocketChannel',
 ]
 
 #
 #
 LOCAL_HOST = '127.0.0.1'
@@ -133,40 +131,40 @@
 		self.object_type = object_type
 		self.args = args
 		self.kw = kw
 
 # Control messages sent to the sockets thread
 # via the control channel.
 class ListenForStream(object):
-	def __init__(self, requested_ipp=None, create_session=None, tag=None, upgrade=None, encrypted=None):
+	def __init__(self, requested_ipp=None, create_session=None, tag=None, upgrade=None, encrypted=False):
 		self.requested_ipp = requested_ipp or HostPort()
 		self.create_session = create_session
 		self.tag = tag
 		self.upgrade = upgrade
 		self.encrypted = encrypted
 
 class ConnectStream(object):
-	def __init__(self, requested_ipp=None, create_session=None, tag=None, upgrade=None, encrypted=None):
+	def __init__(self, requested_ipp=None, create_session=None, tag=None, upgrade=None, encrypted=False):
 		self.requested_ipp = requested_ipp or HostPort()
 		self.create_session = create_session
 		self.tag = tag
 		self.upgrade = upgrade
 		self.encrypted = encrypted
 
 class StopListening(object):
 	def __init__(self, listening_ipp=None):
 		self.listening_ipp = listening_ipp or HostPort()
 
 # Update messages from sockets thread to app.
 class Listening(object):
-	def __init__(self, requested_ipp=None, listening_ipp=None, tag=None, context=None):
+	def __init__(self, requested_ipp=None, listening_ipp=None, tag=None, encrypted=False):
 		self.requested_ipp = requested_ipp or HostPort()
 		self.listening_ipp = listening_ipp or HostPort()
 		self.tag = tag
-		self.context = context
+		self.encrypted = encrypted
 
 class Accepted(object):
 	def __init__(self, listening_ipp=None, accepted_ipp=None, remote_address=None, opened_at=None, tag=None):
 		self.listening_ipp = listening_ipp or HostPort()
 		self.accepted_ipp = accepted_ipp or HostPort()
 		self.remote_address = remote_address
 		self.opened_at = opened_at
@@ -224,16 +222,15 @@
 	'connected_ipp': ar.UserDefined(HostPort),
 	'listening_ipp': ar.UserDefined(HostPort),
 	'accepted_ipp': ar.UserDefined(HostPort),
 	'condition': ar.Unicode(),
 	'explanation': ar.Unicode(),
 	'error_code': ar.Integer8(),
 	'error_text': ar.Unicode(),
-	'encrypted': ar.Any(),
-	'context': ar.Any(),
+	'encrypted': ar.Boolean(),
 }
 
 ar.bind(ListenForStream, object_schema=CONTROL_SCHEMA)
 ar.bind(ConnectStream, object_schema=CONTROL_SCHEMA)
 ar.bind(StopListening, object_schema=CONTROL_SCHEMA)
 ar.bind(Listening, object_schema=CONTROL_SCHEMA, copy_before_sending=False)
 ar.bind(Accepted, object_schema=CONTROL_SCHEMA)
@@ -280,25 +277,14 @@
 
 ar.bind(Close, object_schema=ENDING_SCHEMA, copy_before_sending=False)
 ar.bind(Closed, object_schema=ENDING_SCHEMA, copy_before_sending=False)
 ar.bind(Abandoned, object_schema=ENDING_SCHEMA, copy_before_sending=False)
 
 #
 #
-class TlsServer(object):
-	def __init__(self, certificate_file=None, key_file=None):
-		self.certificate_file = certificate_file
-		self.key_file = key_file
-
-class TlsClient(object):
-	def __init__(self, SNI=None):
-		self.SNI = SNI
-
-#
-#
 class Shutdown(object):
 	def __init__(self, s=None, value=False):
 		self.s = s
 		self.value = value
 
 class Bump(object):
 	def __init__(self, s=None):
@@ -773,22 +759,24 @@
 		return
 	except OverflowError as e:
 		server.close()
 		self.send(NotListening(requested_ipp, 0, str(e), m.tag), r)
 		return
 
 	hap = server.getsockname()
+	listening_ipp=HostPort(hap[0], hap[1])
 
-	if isinstance(m.encrypted, TlsServer):
-		self.trace(f'Listening (encrypted) as TLS server "{m.encrypted.certificate_file}"')
+	if m.encrypted:
+		self.trace(f'Listening (encrypted) on "{listening_ipp}", requested "{requested_ipp}"')
+	else:
+		self.trace(f'Listening on "{listening_ipp}", requested "{requested_ipp}"')
 
-	self.trace('Listening on "%s"(%d), requested "%s"(%d)' %
-		(hap[0], hap[1],
-		requested_ipp.host, requested_ipp.port))
-	listening = Listening(requested_ipp=requested_ipp, listening_ipp=HostPort(hap[0], hap[1]), tag=m.tag, context=m.encrypted)
+	listening = Listening(requested_ipp=requested_ipp,
+		listening_ipp=listening_ipp,
+		tag=m.tag, encrypted=m.encrypted)
 
 	self.networking[server] = TcpServer(server, m, listening, r, m.upgrade)
 	self.receiving.append(server)
 	self.faulting.append(server)
 
 	self.send(listening, r)
 
@@ -829,17 +817,14 @@
 	try:
 		client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 		client.setblocking(False)
 	except socket.error as e:
 		self.send(NotConnected(requested_ipp, e.errno, str(e), m.tag), r)
 		return
 
-	if isinstance(m.encrypted, TlsClient):
-		self.trace(f'Encrypting connect as TLS client "{m.encrypted.SNI}"')
-
 	def client_not_connected(e):
 		client.close()
 		self.send(NotConnected(requested_ipp, e.errno, str(e), m.tag), r)
 
 	try:
 		e = client.connect_ex(requested_ipp.inet())
 		if e:
@@ -873,42 +858,41 @@
 		return
 	except OverflowError as e:
 		client.close()
 		self.send(NotConnected(requested_ipp, 0, str(e), m.tag), r)
 		return
 
 	hap = client.getsockname()
-
-	self.trace('Connected to "%s"(%d), at local address "%s"(%d)' %
-					(requested_ipp.host, requested_ipp.port,
-					hap[0], hap[1]))
 	connected_ipp = HostPort(hap[0], hap[1])
 
-	connected = Connected(requested_ipp=m.requested_ipp,
+	connected = Connected(requested_ipp=requested_ipp,
 		connected_ipp=connected_ipp,
 		opened_at=ar.world_now(),
 		tag=m.tag)
 
 	parent = TcpClient(client, m, connected, r, m.upgrade, m.encrypted)
 	stream, proxy_address = open_stream(self, parent, client, connected)
 	connected.remote_address = proxy_address
 
 	self.networking[client] = stream
 	self.receiving.append(client)
 	self.sending.append(client)
 	self.faulting.append(client)
 
 	if m.encrypted:
-		self.trace(f'Connected (encrypted) "{connected_ipp}", requested "{m.requested_ipp}"')
+		self.trace(f'Connected (encrypted) to "{requested_ipp}", at local address "{connected_ipp}"')
 		not_connected = NotConnected(requested_ipp, None, None, m.tag)
 		stream.diffie_hellman = (
 			(connected, r, stream.remote_address),
 			(not_connected, r))
+		# Start the exchange. Public key filled out during
+		# streaming.
 		self.send(Diffie(), proxy_address)
 		return
+	self.trace(f'Connected to "{requested_ipp}", at local address ""{connected_ipp}"')
 
 	self.forward(connected, r, stream.remote_address)
 
 def ControlChannel_StopListening(self, control, mr):
 	m, r = mr
 	listening_ipp = m.listening_ipp
 	def server(t):
@@ -1000,23 +984,22 @@
 	accepted_ipp = HostPort(hap[0], hap[1])
 
 	accepted = Accepted(listening_ipp=listening.listening_ipp,
 		accepted_ipp=accepted_ipp, remote_address=stream.remote_address,
 		opened_at=opened_at, tag=listening.tag)
 	stream.opened = accepted
 
-	if listening.context:
+	if listening.encrypted:
 		self.trace(f'Accepted (encrypted) "{accepted_ipp}", requested "{listening.listening_ipp}"')
 		not_accepted = NotAccepted(listening.requested_ipp, None, None, listening.tag)
 		stream.diffie_hellman = (
-			(accepted, stream.controller_address, stream.remote_address),
+			(accepted, server.controller_address, stream.remote_address),
 			(not_accepted, server.controller_address))
 		return
-
-	self.trace(f'Accepted "{accepted_ipp}", listening at "{listening.listening_ipp}"')
+	self.trace(f'Accepted "{accepted_ipp}", requested "{listening.listening_ipp}"')
 
 	self.forward(accepted, server.controller_address, stream.remote_address)
 
 def TcpServer_BrokenTransport(self, server, s):
 	listening = server.listening
 	self.send(NotListening(listening.listening_ipp, 0, "signaled by networking subsystem"), server.controller_address)
 	self.clear(s, TcpServer)
@@ -1025,15 +1008,19 @@
 # A placeholder for the eventual outbound stream.
 def TcpClient_ReceiveBlock(self, selector, s):
 	client = s
 	# NOT NEEDED IN TcpStream_ReceiveBlock SO....
 	#self.sending.remove(client)
 
 	request = selector.request
+
 	hap = client.getsockname()
+	connected_ipp = HostPort(hap[0], hap[1])
+	requested_ipp = request.requested_ipp
+
 	# CANNOT BUILD A STREAM AND IMMEDIATELY TEAR IT DOWN ON AN EXCEPTION.
 	# THIS WILL MAY CREATE A SESSION OBJECT WHEN THERE IS NO REMOTE AND MAY
 	# NEVER BE. DO IT AFTER A SUCCESSFUL RECV().
 	#connected = Connected(requested_ipp=request.requested_ipp,
 	#	connected_ipp=HostPort(hap[0], hap[1]),
 	#	opened_at=ar.world_now(),
 	#	tag=request.tag)
@@ -1042,36 +1029,35 @@
 	#stream, proxy_address = open_stream(self, selector, client, connected.opened_at)
 	#connected.remote_address = proxy_address
 
 	try:
 		scrap = s.recv(TCP_RECV)
 
 		# No exception. New stream.
-		connected_ipp = HostPort(hap[0], hap[1])
-		connected = Connected(requested_ipp=request.requested_ipp,
+		connected = Connected(requested_ipp=requested_ipp,
 			connected_ipp=connected_ipp,
 			opened_at=ar.world_now(),
 			tag=request.tag)
 
 		selector.connected = connected
 		stream, proxy_address = open_stream(self, selector, client, connected)
 		connected.remote_address = proxy_address
 
-		self.trace( 'Connected to "%s"(%d), at local address "%s"(%d)' %
-					   (request.requested_ipp.host, request.requested_ipp.port,
-					   hap[0], hap[1]))
+		self.trace(f'Connected to "{requested_ipp}", at local address "{connected_ipp}"')
 
 		if selector.encrypted:
-			self.trace(f'Connected (encrypted) "{connected_ipp}", requested "{request.requested_ipp}"')
-			not_connected = NotConnected(request.requested_ipp, None, None, request.tag)
+			self.trace(f'Connected (encrypted) to "{requested_ipp}", at local address "{connected_ipp}"')
+			not_connected = NotConnected(requested_ipp, None, None, request.tag)
 			stream.diffie_hellman = (
 				(connected, stream.controller_address, stream.remote_address),
 				(not_connected, selector.controller_address))
 			self.send(Diffie(), proxy_address)
 			return
+		self.trace(f'Connected to "{requested_ipp}", at local address "{connected_ipp}"')
+
 		self.forward(connected, stream.controller_address, stream.remote_address)
 
 		if not scrap:
 			# Immediate shutdown. Need to
 			# generate the full set of messages.
 			#self.clear(s, TcpStream)
 			return
@@ -1093,38 +1079,38 @@
 
 def TcpClient_ReadyToSend(self, selector, s):
 	client = s
 	#self.sending.remove(client)
 
 	request = selector.request
 	hap = client.getsockname()
-	connected_ipp=HostPort(hap[0], hap[1])
-	connected = Connected(requested_ipp=request.requested_ipp,
+	connected_ipp = HostPort(hap[0], hap[1])
+	requested_ipp = request.requested_ipp
+
+	connected = Connected(requested_ipp=requested_ipp,
 		connected_ipp=connected_ipp,
 		opened_at=ar.world_now(),
 		tag=request.tag)
 	selector.connected = connected
 
-	self.trace( 'Connected to "%s"(%d), at local address "%s"(%d)' %
-				   (request.requested_ipp.host, request.requested_ipp.port,
-				   hap[0], hap[1]))
-
 	stream, proxy_address = open_stream(self, selector, client, connected)
 	connected.remote_address = proxy_address
 	#receiving.append( client)
 	#self.faulting.append( client)
 
 	if selector.encrypted:
-		self.trace(f'Connected (encrypted) "{connected_ipp}", requested "{request.requested_ipp}"')
-		not_connected = NotConnected(request.requested_ipp, None, None, request.tag)
+		self.trace(f'Connected (encrypted) to "{requested_ipp}", at local address "{connected_ipp}"')
+		not_connected = NotConnected(requested_ipp, None, None, request.tag)
 		stream.diffie_hellman = (
 			(connected, stream.controller_address, stream.remote_address),
 			(not_connected, selector.controller_address))
+		# Start the exchange of public keys.
 		self.send(Diffie(), proxy_address)
 		return
+	self.trace(f'Connected to "{requested_ipp}", at local address "{connected_ipp}"')
 
 	self.forward(connected, stream.controller_address, stream.remote_address)
 
 def TcpClient_BrokenTransport(self, selector, s):
 	text = 'fault on pending connect, unreachable, no service at that address or blocked'
 	self.send(NotConnected(selector.requested_ipp, 0, text, selector.tag), selector.controller_address)
 	self.clear(s, TcpClient)
```

### Comparing `ansar_connect-0.1.196/src/ansar/connect/standard.py` & `ansar_connect-0.1.197/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.196/src/ansar/connect/transporting.py` & `ansar_connect-0.1.197/src/ansar/connect/transporting.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,24 +40,19 @@
 	ts.channel.send(ar.Stop(), root.address)
 	root.select(ar.Completed)
 
 ar.AddOn(create_sockets, stop_sockets)
 
 #
 #
-def wrench(self, message):
-	ts.channel.send(message, self.address)
-
-#
-#
-def connect(self, requested_ipp, session=None, tag=None, encrypted=None):
+def connect(self, requested_ipp, session=None, tag=None, encrypted=False):
 	ts.channel.send(ConnectStream(requested_ipp=requested_ipp, create_session=session, tag=tag, encrypted=encrypted), self.address)
 
 #
 #
-def listen(self, requested_ipp, session=None, tag=None, encrypted=None):
+def listen(self, requested_ipp, session=None, tag=None, encrypted=False):
 	ts.channel.send(ListenForStream(requested_ipp=requested_ipp, create_session=session, tag=tag, encrypted=encrypted), self.address)
 
 #
 #
 def stop_listen(self, requested_ipp):
 	ts.channel.send(StopListening(requested_ipp), self.address)
```

### Comparing `ansar_connect-0.1.196/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.197/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.196/src/ansar/connect/wan.py` & `ansar_connect-0.1.197/src/ansar/connect/wan.py`

 * *Files 11% similar despite different names*

```diff
@@ -87,18 +87,18 @@
 
 ar.bind(EmailAddress, object_schema=CONTACT_SCHEMA)
 ar.bind(PhoneNumber, object_schema=CONTACT_SCHEMA)
 
 # Protocol between a connecting directory and
 # a cloud directory.
 class WideAreaAccess(object):
-	def __init__(self, access_ipp=None, SNI=None, access_token=None, account_id=None, directory_id=None,
+	def __init__(self, access_ipp=None, encrypted=False, access_token=None, account_id=None, directory_id=None,
 			product_name=None, product_instance=None):
 		self.access_ipp = access_ipp or HostPort()	# Manifestly required.
-		self.SNI = SNI
+		self.encrypted = encrypted
 		self.access_token = access_token
 		self.account_id = account_id				# Speed up processing.
 		self.directory_id = directory_id
 		self.product_name = product_name
 		self.product_instance = product_instance
 
 	def __str__(self):
@@ -112,19 +112,19 @@
 		self.account_id = account_id
 		self.directory_id = directory_id
 		self.access_token = access_token
 		self.product_name = product_name
 		self.product_instance = product_instance
 
 class WideAreaRedirect(object):
-	def __init__(self, redirect_ipp=None, SNI=None, directory_id=None, assignment_token=None):
+	def __init__(self, redirect_ipp=None, directory_id=None, assignment_token=None, encrypted=False):
 		self.redirect_ipp = redirect_ipp or HostPort()
-		self.SNI = SNI
 		self.directory_id = directory_id
 		self.assignment_token = assignment_token
+		self.encrypted = encrypted
 
 class WideAreaAssignment(object):
 	def __init__(self, directory_id=None, assignment_token=None):
 		self.directory_id = directory_id
 		self.assignment_token = assignment_token
 
 class YourWideArea(object):
@@ -137,15 +137,15 @@
 	"account_id": ar.UUID(),
 	"directory_id": ar.UUID(),
 	"redirect_ipp": ar.UserDefined(HostPort),
 	"assignment_token": ar.UUID(),
 	"address": ar.Address(),
 	"product_name": ar.Unicode(),
 	"product_instance": InstanceOfProduct,
-	"SNI": ar.Unicode(),
+	"encrypted": ar.Boolean(),
 }
 
 ar.bind(WideAreaAccess, object_schema=WIDE_AREA_SCHEMA)
 ar.bind(WideAreaLookup, object_schema=WIDE_AREA_SCHEMA)
 ar.bind(WideAreaRedirect, object_schema=WIDE_AREA_SCHEMA)
 ar.bind(WideAreaAssignment, object_schema=WIDE_AREA_SCHEMA)
 ar.bind(YourWideArea, object_schema=WIDE_AREA_SCHEMA)
@@ -154,19 +154,19 @@
 # a publisher.
 class RelayLookup(object):
 	def __init__(self, relay_id=None, directory_id=None):
 		self.relay_id = relay_id
 		self.directory_id = directory_id
 
 class RelayRedirect(object):
-	def __init__(self, redirect_ipp=None, relay_id=None, assignment_token=None, SNI=None):
+	def __init__(self, redirect_ipp=None, relay_id=None, assignment_token=None, encrypted=None):
 		self.redirect_ipp = redirect_ipp or HostPort()
 		self.relay_id = relay_id
 		self.assignment_token = assignment_token
-		self.SNI = SNI
+		self.encrypted = encrypted
 
 class RelayAssignment(object):
 	def __init__(self, relay_id=None, assignment_token=None):
 		self.relay_id = relay_id
 		self.assignment_token = assignment_token
 
 class YourRelay(object):
@@ -180,15 +180,15 @@
 RELAY_SCHEMA = {
 	"relay_id": ar.UUID(),
 	"directory_id": ar.UUID(),
 	"redirect_ipp": ar.UserDefined(HostPort),
 	"assignment_token": ar.UUID(),
 	"address": ar.Address(),
 	"account_id": ar.UUID(),
-	"SNI": ar.Unicode(),
+	"encrypted": ar.Boolean(),
 }
 
 ar.bind(RelayLookup, object_schema=RELAY_SCHEMA)
 ar.bind(RelayRedirect, object_schema=RELAY_SCHEMA)
 ar.bind(RelayAssignment, object_schema=RELAY_SCHEMA)
 ar.bind(YourRelay, object_schema=RELAY_SCHEMA)
```

### Comparing `ansar_connect-0.1.196/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.197/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.196
+Version: 0.1.197
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.196/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.197/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

