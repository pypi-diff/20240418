# Comparing `tmp/pytorrentdl-0.2.2.tar.gz` & `tmp/pytorrentdl-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorrentdl-0.2.2.tar", last modified: Thu Apr 18 11:18:49 2024, max compression
+gzip compressed data, was "pytorrentdl-1.0.0.tar", last modified: Thu Apr 18 11:54:25 2024, max compression
```

## Comparing `pytorrentdl-0.2.2.tar` & `pytorrentdl-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 11:18:49.029758 pytorrentdl-0.2.2/
--rw-rw-rw-   0        0        0    12179 2024-04-18 14:36:08.000000 pytorrentdl-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     5121 2024-04-18 11:18:49.026758 pytorrentdl-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3982 2024-04-18 14:36:08.000000 pytorrentdl-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 11:18:48.952754 pytorrentdl-0.2.2/pytorrentdl/
--rw-rw-rw-   0        0        0      578 2024-04-18 11:17:35.000000 pytorrentdl-0.2.2/pytorrentdl/__init__.py
--rw-rw-rw-   0        0        0     1812 2024-04-18 14:36:08.000000 pytorrentdl-0.2.2/pytorrentdl/cli.py
--rw-rw-rw-   0        0        0     3493 2024-04-18 11:09:16.000000 pytorrentdl-0.2.2/pytorrentdl/downloader.py
--rw-rw-rw-   0        0        0     1204 2024-04-18 14:36:08.000000 pytorrentdl-0.2.2/pytorrentdl/session.py
--rw-rw-rw-   0        0        0     2020 2024-04-18 11:14:34.000000 pytorrentdl-0.2.2/pytorrentdl/torrent_downloader.py
--rw-rw-rw-   0        0        0      470 2024-04-18 14:36:08.000000 pytorrentdl-0.2.2/pytorrentdl/torrent_info.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:18:49.019758 pytorrentdl-0.2.2/pytorrentdl.egg-info/
--rw-rw-rw-   0        0        0     5121 2024-04-18 11:18:46.000000 pytorrentdl-0.2.2/pytorrentdl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2024-04-18 11:18:47.000000 pytorrentdl-0.2.2/pytorrentdl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 11:18:46.000000 pytorrentdl-0.2.2/pytorrentdl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-04-18 11:18:46.000000 pytorrentdl-0.2.2/pytorrentdl.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       38 2024-04-18 11:18:46.000000 pytorrentdl-0.2.2/pytorrentdl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-18 11:18:46.000000 pytorrentdl-0.2.2/pytorrentdl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 11:18:49.050759 pytorrentdl-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1733 2024-04-18 11:17:10.000000 pytorrentdl-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:54:25.854742 pytorrentdl-1.0.0/
+-rw-rw-rw-   0        0        0    12179 2024-04-18 14:36:08.000000 pytorrentdl-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     5121 2024-04-18 11:54:25.851742 pytorrentdl-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3982 2024-04-18 14:36:08.000000 pytorrentdl-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 11:54:25.809739 pytorrentdl-1.0.0/pytorrentdl/
+-rw-rw-rw-   0        0        0      578 2024-04-18 11:53:46.000000 pytorrentdl-1.0.0/pytorrentdl/__init__.py
+-rw-rw-rw-   0        0        0     1812 2024-04-18 14:36:08.000000 pytorrentdl-1.0.0/pytorrentdl/cli.py
+-rw-rw-rw-   0        0        0     3827 2024-04-18 11:53:36.000000 pytorrentdl-1.0.0/pytorrentdl/downloader.py
+-rw-rw-rw-   0        0        0     1204 2024-04-18 14:36:08.000000 pytorrentdl-1.0.0/pytorrentdl/session.py
+-rw-rw-rw-   0        0        0     1972 2024-04-18 11:53:32.000000 pytorrentdl-1.0.0/pytorrentdl/torrent_downloader.py
+-rw-rw-rw-   0        0        0      470 2024-04-18 14:36:08.000000 pytorrentdl-1.0.0/pytorrentdl/torrent_info.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:54:25.844741 pytorrentdl-1.0.0/pytorrentdl.egg-info/
+-rw-rw-rw-   0        0        0     5121 2024-04-18 11:54:24.000000 pytorrentdl-1.0.0/pytorrentdl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2024-04-18 11:54:25.000000 pytorrentdl-1.0.0/pytorrentdl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 11:54:24.000000 pytorrentdl-1.0.0/pytorrentdl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-18 11:54:24.000000 pytorrentdl-1.0.0/pytorrentdl.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       38 2024-04-18 11:54:24.000000 pytorrentdl-1.0.0/pytorrentdl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-18 11:54:24.000000 pytorrentdl-1.0.0/pytorrentdl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 11:54:25.855742 pytorrentdl-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1733 2024-04-18 11:17:10.000000 pytorrentdl-1.0.0/setup.py
```

### Comparing `pytorrentdl-0.2.2/LICENSE` & `pytorrentdl-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorrentdl-0.2.2/PKG-INFO` & `pytorrentdl-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorrentdl
-Version: 0.2.2
+Version: 1.0.0
 Summary: Download from torrent with magnet link or .torrent file
 Home-page: https://github.com/iw4p/torrentp
 Author: Nima Akbarzade
 Author-email: iw4p@protonmail.com
 License: BSD 2-clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pytorrentdl-0.2.2/README.md` & `pytorrentdl-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pytorrentdl-0.2.2/pytorrentdl/__init__.py` & `pytorrentdl-1.0.0/pytorrentdl/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 A great wrapped library for downloading from torrent.
 """
 from .torrent_downloader import TorrentDownloader
 from .torrent_info import TorrentInfo
 from .downloader import Downloader
 from .session import Session
 
-__version__ = "0.2.2"
+__version__ = "1.0.0"
 __author__ = 'Nima Akbarzade'
 __author_email__ = "iw4p@protonmail.com"
 __license__ = "BSD 2-clause"
 __url__ = "https://github.com/iw4p/torrentp"
 
 PYPI_SIMPLE_ENDPOINT: str = "https://pypi.org/project/torrentp"
```

### Comparing `pytorrentdl-0.2.2/pytorrentdl/cli.py` & `pytorrentdl-1.0.0/pytorrentdl/cli.py`

 * *Files identical despite different names*

### Comparing `pytorrentdl-0.2.2/pytorrentdl/downloader.py` & `pytorrentdl-1.0.0/pytorrentdl/downloader.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
         self._status = None
         self._name = ''
         self._state = ''
         self._lt = libtorrent
         self._add_torrent_params = None
         self._is_magnet = is_magnet
         self._paused = False
+        self._callback = None
 
     def status(self):
         if not self._is_magnet:
             self._file = self._session.add_torrent({'ti': self._torrent_info, 'save_path': f'{self._save_path}'})
             self._status = self._file.status()
         else:
             self._add_torrent_params = self._torrent_info
@@ -31,22 +32,27 @@
         return self._status
 
     @property
     def name(self):
         self._name = self.status().name
         return self._name
 
-    async def download(self):
+    async def download(self,callback=None):
+        self._callback = callback
         self.get_size_info(self.status().total_wanted)
 
         while not self._status.is_seeding:
             if not self._paused:
-                return self.status()
+                self._get_status_progress(self.status())
+                if self._callback:
+                    self._callback(torrent_info, save_path,self.status(),self.name, self._status.progress, self._status.download_rate,finalizado=False)
+                #sys.stdout.flush()
+
             await asyncio.sleep(1)
-        return "Downloaded"
+        self._callback(finalizado=True)
 
     def _get_status_progress(self, s):
         _percentage = s.progress * 100
         _download_speed = s.download_rate / 1000
         _upload_speed = s.upload_rate / 1000
 
         counting = math.ceil(_percentage / 5)
```

### Comparing `pytorrentdl-0.2.2/pytorrentdl/session.py` & `pytorrentdl-1.0.0/pytorrentdl/session.py`

 * *Files identical despite different names*

### Comparing `pytorrentdl-0.2.2/pytorrentdl/torrent_downloader.py` & `pytorrentdl-1.0.0/pytorrentdl/torrent_downloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from .session import Session
 from .torrent_info import TorrentInfo
 from .downloader import Downloader
 import libtorrent as lt
 
 
 class TorrentDownloader:
-    def __init__(self, file_path, save_path, port=6881):
+    def __init__(self, file_path, save_path, callback=None,port=6881):
         self._file_path = file_path
         self._save_path = save_path
         self._port = port  # Default port is 6881
         self._downloader = None
         self._torrent_info = None
         self._lt = lt
         self._file = None
         self._add_torrent_params = None
         self._session = Session(self._lt, port=self._port)  # Pass port to Session
 
-    async def start_download(self, download_speed=0, upload_speed=0, callback_func=None):
+    async def start_download(self, download_speed=0, upload_speed=0, callback=None):
         if self._file_path.startswith('magnet:'):
             self._add_torrent_params = self._lt.parse_magnet_uri(self._file_path)
             self._add_torrent_params.save_path = self._save_path
             self._downloader = Downloader(
                 session=self._session(), torrent_info=self._add_torrent_params, 
                 save_path=self._save_path, libtorrent=lt, is_magnet=True
             )
@@ -32,17 +32,15 @@
                 save_path=self._save_path, libtorrent=None, is_magnet=False
             )
 
         self._session.set_download_limit(download_speed)
         self._session.set_upload_limit(upload_speed)
 
         self._file = self._downloader
-        data = await self._file.download()
-        if callback_func:
-            callback_func(data)
+        await self._file.download(callback)
 
     def pause_download(self):
         if self._downloader:
             self._downloader.pause()
 
     def resume_download(self):
         if self._downloader:
```

### Comparing `pytorrentdl-0.2.2/pytorrentdl.egg-info/PKG-INFO` & `pytorrentdl-1.0.0/pytorrentdl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorrentdl
-Version: 0.2.2
+Version: 1.0.0
 Summary: Download from torrent with magnet link or .torrent file
 Home-page: https://github.com/iw4p/torrentp
 Author: Nima Akbarzade
 Author-email: iw4p@protonmail.com
 License: BSD 2-clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pytorrentdl-0.2.2/setup.py` & `pytorrentdl-1.0.0/setup.py`

 * *Files identical despite different names*

