# Comparing `tmp/PKDevTools-0.13.20240418.95.tar.gz` & `tmp/PKDevTools-0.13.20240418.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKDevTools-0.13.20240418.95.tar", last modified: Thu Apr 18 13:21:54 2024, max compression
+gzip compressed data, was "PKDevTools-0.13.20240418.96.tar", last modified: Thu Apr 18 14:10:37 2024, max compression
```

## Comparing `PKDevTools-0.13.20240418.95.tar` & `PKDevTools-0.13.20240418.96.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 13:21:54.016419 PKDevTools-0.13.20240418.95/
--rw-rw-rw-   0        0        0     1086 2024-04-18 13:19:58.000000 PKDevTools-0.13.20240418.95/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-18 13:21:54.000815 PKDevTools-0.13.20240418.95/PKDevTools/
--rw-rw-rw-   0        0        0     1176 2024-04-18 13:19:58.000000 PKDevTools-0.13.20240418.95/PKDevTools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:21:54.016419 PKDevTools-0.13.20240418.95/PKDevTools/classes/
--rw-rw-rw-   0        0        0     3402 2024-04-18 13:19:58.000000 PKDevTools-0.13.20240418.95/PKDevTools/classes/Archiver.py
--rw-rw-rw-   0        0        0     4831 2024-04-18 13:19:58.000000 PKDevTools-0.13.20240418.95/PKDevTools/classes/ColorText.py
--rw-rw-rw-   0        0        0     3599 2024-04-18 13:19:58.000000 PKDevTools-0.13.20240418.95/PKDevTools/classes/Committer.py
--rw-rw-rw-   0        0        0     6212 2024-04-18 13:19:58.000000 PKDevTools-0.13.20240418.95/PKDevTools/classes/CookieHelper.py
--rw-rw-rw-   0        0        0     8879 2024-04-18 13:19:58.000000 PKDevTools-0.13.20240418.95/PKDevTools/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11963 2024-04-18 13:19:58.000000 PKDevTools-0.13.20240418.95/PKDevTools/classes/MenuOptions.py
--rw-rw-rw-   0        0        0     2534 2024-04-18 13:19:58.000000 PKDevTools-0.13.20240418.95/PKDevTools/classes/OutputControls.py
--rw-rw-rw-   0        0        0    13778 2024-04-18 13:19:58.000000 PKDevTools-0.13.20240418.95/PKDevTools/classes/PKDateUtilities.py
--rw-rw-rw-   0        0        0     2988 2024-04-18 13:19:58.000000 PKDevTools-0.13.20240418.95/PKDevTools/classes/PKGitFolderDownloader.py
--rw-rw-rw-   0        0        0     8048 2024-04-18 13:19:58.000000 PKDevTools-0.13.20240418.95/PKDevTools/classes/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    14334 2024-04-18 13:19:58.000000 PKDevTools-0.13.20240418.95/PKDevTools/classes/PKPickler.py
--rw-rw-rw-   0        0        0     3433 2024-04-18 13:19:58.000000 PKDevTools-0.13.20240418.95/PKDevTools/classes/PKTimer.py
--rw-rw-rw-   0        0        0     4548 2024-04-18 13:19:58.000000 PKDevTools-0.13.20240418.95/PKDevTools/classes/Singleton.py
--rw-rw-rw-   0        0        0     1916 2024-04-18 13:19:58.000000 PKDevTools-0.13.20240418.95/PKDevTools/classes/SuppressOutput.py
--rw-rw-rw-   0        0        0    11301 2024-04-18 13:19:58.000000 PKDevTools-0.13.20240418.95/PKDevTools/classes/Telegram.py
--rw-rw-rw-   0        0        0    24543 2024-04-18 13:19:58.000000 PKDevTools-0.13.20240418.95/PKDevTools/classes/Utils.py
--rw-rw-rw-   0        0        0     9984 2024-04-18 13:19:58.000000 PKDevTools-0.13.20240418.95/PKDevTools/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       27 2024-04-18 13:21:49.000000 PKDevTools-0.13.20240418.95/PKDevTools/classes/__init__.py
--rw-rw-rw-   0        0        0     3738 2024-04-18 13:19:58.000000 PKDevTools-0.13.20240418.95/PKDevTools/classes/githubutilities.py
--rw-rw-rw-   0        0        0    16118 2024-04-18 13:19:58.000000 PKDevTools-0.13.20240418.95/PKDevTools/classes/log.py
--rw-rw-rw-   0        0        0     5384 2024-04-18 13:19:58.000000 PKDevTools-0.13.20240418.95/PKDevTools/classes/multiprocessing_logging.py
--rw-rw-rw-   0        0        0     2864 2024-04-18 13:19:58.000000 PKDevTools-0.13.20240418.95/PKDevTools/classes/squash.py
--rw-rw-rw-   0        0        0     4846 2024-04-18 13:19:58.000000 PKDevTools-0.13.20240418.95/PKDevTools/classes/updater.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:21:54.000815 PKDevTools-0.13.20240418.95/PKDevTools.egg-info/
--rw-rw-rw-   0        0        0     5202 2024-04-18 13:21:53.000000 PKDevTools-0.13.20240418.95/PKDevTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1084 2024-04-18 13:21:53.000000 PKDevTools-0.13.20240418.95/PKDevTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 13:21:53.000000 PKDevTools-0.13.20240418.95/PKDevTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      363 2024-04-18 13:21:53.000000 PKDevTools-0.13.20240418.95/PKDevTools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-18 13:21:48.000000 PKDevTools-0.13.20240418.95/PKDevTools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      176 2024-04-18 13:21:53.000000 PKDevTools-0.13.20240418.95/PKDevTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-18 13:21:53.000000 PKDevTools-0.13.20240418.95/PKDevTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5202 2024-04-18 13:21:54.016419 PKDevTools-0.13.20240418.95/PKG-INFO
--rw-rw-rw-   0        0        0     4290 2024-04-18 13:19:58.000000 PKDevTools-0.13.20240418.95/README.md
--rw-rw-rw-   0        0        0       86 2024-04-18 13:21:54.016419 PKDevTools-0.13.20240418.95/setup.cfg
--rw-rw-rw-   0        0        0     4341 2024-04-18 13:19:58.000000 PKDevTools-0.13.20240418.95/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:10:37.694214 PKDevTools-0.13.20240418.96/
+-rw-rw-rw-   0        0        0     1086 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-18 14:10:37.678598 PKDevTools-0.13.20240418.96/PKDevTools/
+-rw-rw-rw-   0        0        0     1176 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:10:37.694214 PKDevTools-0.13.20240418.96/PKDevTools/classes/
+-rw-rw-rw-   0        0        0     3402 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/Archiver.py
+-rw-rw-rw-   0        0        0     4831 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/ColorText.py
+-rw-rw-rw-   0        0        0     3599 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/Committer.py
+-rw-rw-rw-   0        0        0     6380 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/CookieHelper.py
+-rw-rw-rw-   0        0        0     8879 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11963 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0     2534 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/OutputControls.py
+-rw-rw-rw-   0        0        0    13778 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/PKDateUtilities.py
+-rw-rw-rw-   0        0        0     2988 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/PKGitFolderDownloader.py
+-rw-rw-rw-   0        0        0     8048 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    14334 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/PKPickler.py
+-rw-rw-rw-   0        0        0     3433 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/PKTimer.py
+-rw-rw-rw-   0        0        0     4548 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/Singleton.py
+-rw-rw-rw-   0        0        0     1916 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/SuppressOutput.py
+-rw-rw-rw-   0        0        0    11301 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/Telegram.py
+-rw-rw-rw-   0        0        0    24543 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/Utils.py
+-rw-rw-rw-   0        0        0     9984 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       27 2024-04-18 14:10:33.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/__init__.py
+-rw-rw-rw-   0        0        0     3738 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/githubutilities.py
+-rw-rw-rw-   0        0        0    16118 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/log.py
+-rw-rw-rw-   0        0        0     5384 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/multiprocessing_logging.py
+-rw-rw-rw-   0        0        0     2864 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/squash.py
+-rw-rw-rw-   0        0        0     4846 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/updater.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:10:37.678598 PKDevTools-0.13.20240418.96/PKDevTools.egg-info/
+-rw-rw-rw-   0        0        0     5202 2024-04-18 14:10:37.000000 PKDevTools-0.13.20240418.96/PKDevTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1084 2024-04-18 14:10:37.000000 PKDevTools-0.13.20240418.96/PKDevTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 14:10:37.000000 PKDevTools-0.13.20240418.96/PKDevTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      363 2024-04-18 14:10:37.000000 PKDevTools-0.13.20240418.96/PKDevTools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-18 14:10:32.000000 PKDevTools-0.13.20240418.96/PKDevTools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      176 2024-04-18 14:10:37.000000 PKDevTools-0.13.20240418.96/PKDevTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-18 14:10:37.000000 PKDevTools-0.13.20240418.96/PKDevTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5202 2024-04-18 14:10:37.694214 PKDevTools-0.13.20240418.96/PKG-INFO
+-rw-rw-rw-   0        0        0     4290 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-18 14:10:37.694214 PKDevTools-0.13.20240418.96/setup.cfg
+-rw-rw-rw-   0        0        0     4341 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/setup.py
```

### Comparing `PKDevTools-0.13.20240418.95/LICENSE` & `PKDevTools-0.13.20240418.96/LICENSE`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.95/PKDevTools/__init__.py` & `PKDevTools-0.13.20240418.96/PKDevTools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.95/PKDevTools/classes/Archiver.py` & `PKDevTools-0.13.20240418.96/PKDevTools/classes/Archiver.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.95/PKDevTools/classes/ColorText.py` & `PKDevTools-0.13.20240418.96/PKDevTools/classes/ColorText.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.95/PKDevTools/classes/Committer.py` & `PKDevTools-0.13.20240418.96/PKDevTools/classes/Committer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.95/PKDevTools/classes/CookieHelper.py` & `PKDevTools-0.13.20240418.96/PKDevTools/classes/CookieHelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,37 +76,41 @@
         self.html_path = self.dir / f'{htmlStoreName}_html.pkl'
         self.fetcher = fetcher()
         self.html_metas = self.getMetaDictionary()
         self.cookies = self.getCookies()
 
     def __setCookies(self):
         r = self.__req(self.baseCookieUrl, headers=self.default_headers, timeout=10)
-        cookies = r.cookies
-        self.cookie_path.write_bytes(pickle.dumps(cookies))
+        if r is not None:
+            cookies = r.cookies
+            self.cookie_path.write_bytes(pickle.dumps(cookies))
+        else:
+            cookies = self.getCookies()
         return cookies
 
     def getCookies(self):
         if self.cookie_path.exists():
             cookies = pickle.loads(self.cookie_path.read_bytes())
             if self.__hasCookiesExpired(cookies):
                 cookies = self.__setCookies()
             return cookies
         return self.__setCookies()
 
     def __setMetaDictionary(self):
         r = self.__req(self.baseHtmlUrl, headers=self.default_headers ,timeout=10)
-        html = r.text
-        soup = BeautifulSoup(html,features="lxml")
         metaDict = {}
-        for tag in soup.find_all("meta"):
-            name = tag.get("name", None)
-            content = tag.get("content", None)
-            if name is not None and content is not None:
-                metaDict[name] = content
-        self.html_path.write_bytes(pickle.dumps(metaDict))
+        if r is not None:
+            html = r.text
+            soup = BeautifulSoup(html,features="lxml")
+            for tag in soup.find_all("meta"):
+                name = tag.get("name", None)
+                content = tag.get("content", None)
+                if name is not None and content is not None:
+                    metaDict[name] = content
+            self.html_path.write_bytes(pickle.dumps(metaDict))
         return metaDict
 
     def getMetaDictionary(self):
         if self.html_path.exists():
             metaDict = pickle.loads(self.html_path.read_bytes())
             return metaDict
         return self.__setMetaDictionary()
@@ -144,15 +148,15 @@
     def __req(self, url, params=None, headers=None, timeout=10):
         '''Make a http request'''
         th.check()
         try:
             r = self.fetcher.fetchURL(url=url, params=params, headers=headers, timeout=timeout, raiseError=True)
         except ReadTimeout as e:
             raise TimeoutError(repr(e))
-        if not r.ok:
+        if r is not None and not r.ok:
             raise ConnectionError(f'{url} {r.status_code}: {r.reason}')
         return r
 
 # ch = CookieHelper(download_folder="/Users/praveen.jha1/Downloads/codes/PKScreener-main/results/",
 #                   baseCookieUrl="https://morningstar.in/stocks/0p0000c3nz/nse-hdfc-bank-ltd/overview.aspx",
 #                   baseHtmlUrl="https://morningstar.in/stocks/0p0000c3nz/nse-hdfc-bank-ltd/overview.aspx",
 #                   cookieStoreName="morningstar",
```

### Comparing `PKDevTools-0.13.20240418.95/PKDevTools/classes/Fetcher.py` & `PKDevTools-0.13.20240418.96/PKDevTools/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.95/PKDevTools/classes/MenuOptions.py` & `PKDevTools-0.13.20240418.96/PKDevTools/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.95/PKDevTools/classes/OutputControls.py` & `PKDevTools-0.13.20240418.96/PKDevTools/classes/OutputControls.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.95/PKDevTools/classes/PKDateUtilities.py` & `PKDevTools-0.13.20240418.96/PKDevTools/classes/PKDateUtilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.95/PKDevTools/classes/PKGitFolderDownloader.py` & `PKDevTools-0.13.20240418.96/PKDevTools/classes/PKGitFolderDownloader.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.95/PKDevTools/classes/PKMultiProcessorClient.py` & `PKDevTools-0.13.20240418.96/PKDevTools/classes/PKMultiProcessorClient.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.95/PKDevTools/classes/PKPickler.py` & `PKDevTools-0.13.20240418.96/PKDevTools/classes/PKPickler.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.95/PKDevTools/classes/PKTimer.py` & `PKDevTools-0.13.20240418.96/PKDevTools/classes/PKTimer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.95/PKDevTools/classes/Singleton.py` & `PKDevTools-0.13.20240418.96/PKDevTools/classes/Singleton.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.95/PKDevTools/classes/SuppressOutput.py` & `PKDevTools-0.13.20240418.96/PKDevTools/classes/SuppressOutput.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.95/PKDevTools/classes/Telegram.py` & `PKDevTools-0.13.20240418.96/PKDevTools/classes/Telegram.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.95/PKDevTools/classes/Utils.py` & `PKDevTools-0.13.20240418.96/PKDevTools/classes/Utils.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.95/PKDevTools/classes/WorkflowManager.py` & `PKDevTools-0.13.20240418.96/PKDevTools/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.95/PKDevTools/classes/githubutilities.py` & `PKDevTools-0.13.20240418.96/PKDevTools/classes/githubutilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.95/PKDevTools/classes/log.py` & `PKDevTools-0.13.20240418.96/PKDevTools/classes/log.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.95/PKDevTools/classes/multiprocessing_logging.py` & `PKDevTools-0.13.20240418.96/PKDevTools/classes/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.95/PKDevTools/classes/squash.py` & `PKDevTools-0.13.20240418.96/PKDevTools/classes/squash.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.95/PKDevTools/classes/updater.py` & `PKDevTools-0.13.20240418.96/PKDevTools/classes/updater.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.95/PKDevTools.egg-info/PKG-INFO` & `PKDevTools-0.13.20240418.96/PKDevTools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240418.95
+Version: 0.13.20240418.96
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240418.95.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240418.96.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240418.95/PKDevTools.egg-info/SOURCES.txt` & `PKDevTools-0.13.20240418.96/PKDevTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.95/PKG-INFO` & `PKDevTools-0.13.20240418.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240418.95
+Version: 0.13.20240418.96
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240418.95.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240418.96.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240418.95/README.md` & `PKDevTools-0.13.20240418.96/README.md`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.95/setup.py` & `PKDevTools-0.13.20240418.96/setup.py`

 * *Files identical despite different names*

