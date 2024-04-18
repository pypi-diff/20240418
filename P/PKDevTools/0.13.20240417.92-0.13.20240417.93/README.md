# Comparing `tmp/PKDevTools-0.13.20240417.92.tar.gz` & `tmp/PKDevTools-0.13.20240417.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKDevTools-0.13.20240417.92.tar", last modified: Wed Apr 17 21:42:44 2024, max compression
+gzip compressed data, was "PKDevTools-0.13.20240417.93.tar", last modified: Wed Apr 17 21:55:14 2024, max compression
```

## Comparing `PKDevTools-0.13.20240417.92.tar` & `PKDevTools-0.13.20240417.93.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 21:42:44.883219 PKDevTools-0.13.20240417.92/
--rw-rw-rw-   0        0        0     1086 2024-04-17 21:40:42.000000 PKDevTools-0.13.20240417.92/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-17 21:42:44.867599 PKDevTools-0.13.20240417.92/PKDevTools/
--rw-rw-rw-   0        0        0     1176 2024-04-17 21:40:42.000000 PKDevTools-0.13.20240417.92/PKDevTools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 21:42:44.883219 PKDevTools-0.13.20240417.92/PKDevTools/classes/
--rw-rw-rw-   0        0        0     3402 2024-04-17 21:40:42.000000 PKDevTools-0.13.20240417.92/PKDevTools/classes/Archiver.py
--rw-rw-rw-   0        0        0     4831 2024-04-17 21:40:42.000000 PKDevTools-0.13.20240417.92/PKDevTools/classes/ColorText.py
--rw-rw-rw-   0        0        0     3599 2024-04-17 21:40:42.000000 PKDevTools-0.13.20240417.92/PKDevTools/classes/Committer.py
--rw-rw-rw-   0        0        0     6212 2024-04-17 21:40:42.000000 PKDevTools-0.13.20240417.92/PKDevTools/classes/CookieHelper.py
--rw-rw-rw-   0        0        0     8879 2024-04-17 21:40:42.000000 PKDevTools-0.13.20240417.92/PKDevTools/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11963 2024-04-17 21:40:42.000000 PKDevTools-0.13.20240417.92/PKDevTools/classes/MenuOptions.py
--rw-rw-rw-   0        0        0     2315 2024-04-17 21:40:42.000000 PKDevTools-0.13.20240417.92/PKDevTools/classes/OutputControls.py
--rw-rw-rw-   0        0        0    13778 2024-04-17 21:40:42.000000 PKDevTools-0.13.20240417.92/PKDevTools/classes/PKDateUtilities.py
--rw-rw-rw-   0        0        0     2988 2024-04-17 21:40:42.000000 PKDevTools-0.13.20240417.92/PKDevTools/classes/PKGitFolderDownloader.py
--rw-rw-rw-   0        0        0     8048 2024-04-17 21:40:42.000000 PKDevTools-0.13.20240417.92/PKDevTools/classes/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    14334 2024-04-17 21:40:42.000000 PKDevTools-0.13.20240417.92/PKDevTools/classes/PKPickler.py
--rw-rw-rw-   0        0        0     3433 2024-04-17 21:40:42.000000 PKDevTools-0.13.20240417.92/PKDevTools/classes/PKTimer.py
--rw-rw-rw-   0        0        0     4548 2024-04-17 21:40:42.000000 PKDevTools-0.13.20240417.92/PKDevTools/classes/Singleton.py
--rw-rw-rw-   0        0        0     1916 2024-04-17 21:40:42.000000 PKDevTools-0.13.20240417.92/PKDevTools/classes/SuppressOutput.py
--rw-rw-rw-   0        0        0    11301 2024-04-17 21:40:42.000000 PKDevTools-0.13.20240417.92/PKDevTools/classes/Telegram.py
--rw-rw-rw-   0        0        0    24543 2024-04-17 21:40:42.000000 PKDevTools-0.13.20240417.92/PKDevTools/classes/Utils.py
--rw-rw-rw-   0        0        0     9984 2024-04-17 21:40:42.000000 PKDevTools-0.13.20240417.92/PKDevTools/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       27 2024-04-17 21:42:40.000000 PKDevTools-0.13.20240417.92/PKDevTools/classes/__init__.py
--rw-rw-rw-   0        0        0     3738 2024-04-17 21:40:42.000000 PKDevTools-0.13.20240417.92/PKDevTools/classes/githubutilities.py
--rw-rw-rw-   0        0        0    16118 2024-04-17 21:40:42.000000 PKDevTools-0.13.20240417.92/PKDevTools/classes/log.py
--rw-rw-rw-   0        0        0     5384 2024-04-17 21:40:42.000000 PKDevTools-0.13.20240417.92/PKDevTools/classes/multiprocessing_logging.py
--rw-rw-rw-   0        0        0     2864 2024-04-17 21:40:42.000000 PKDevTools-0.13.20240417.92/PKDevTools/classes/squash.py
--rw-rw-rw-   0        0        0     4846 2024-04-17 21:40:42.000000 PKDevTools-0.13.20240417.92/PKDevTools/classes/updater.py
-drwxrwxrwx   0        0        0        0 2024-04-17 21:42:44.867599 PKDevTools-0.13.20240417.92/PKDevTools.egg-info/
--rw-rw-rw-   0        0        0     5202 2024-04-17 21:42:44.000000 PKDevTools-0.13.20240417.92/PKDevTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1084 2024-04-17 21:42:44.000000 PKDevTools-0.13.20240417.92/PKDevTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 21:42:44.000000 PKDevTools-0.13.20240417.92/PKDevTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      363 2024-04-17 21:42:44.000000 PKDevTools-0.13.20240417.92/PKDevTools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-17 21:42:39.000000 PKDevTools-0.13.20240417.92/PKDevTools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      158 2024-04-17 21:42:44.000000 PKDevTools-0.13.20240417.92/PKDevTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-17 21:42:44.000000 PKDevTools-0.13.20240417.92/PKDevTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5202 2024-04-17 21:42:44.883219 PKDevTools-0.13.20240417.92/PKG-INFO
--rw-rw-rw-   0        0        0     4290 2024-04-17 21:40:42.000000 PKDevTools-0.13.20240417.92/README.md
--rw-rw-rw-   0        0        0       86 2024-04-17 21:42:44.883219 PKDevTools-0.13.20240417.92/setup.cfg
--rw-rw-rw-   0        0        0     4341 2024-04-17 21:40:42.000000 PKDevTools-0.13.20240417.92/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 21:55:14.394192 PKDevTools-0.13.20240417.93/
+-rw-rw-rw-   0        0        0     1086 2024-04-17 21:53:11.000000 PKDevTools-0.13.20240417.93/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-17 21:55:14.378569 PKDevTools-0.13.20240417.93/PKDevTools/
+-rw-rw-rw-   0        0        0     1176 2024-04-17 21:53:11.000000 PKDevTools-0.13.20240417.93/PKDevTools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 21:55:14.394192 PKDevTools-0.13.20240417.93/PKDevTools/classes/
+-rw-rw-rw-   0        0        0     3402 2024-04-17 21:53:11.000000 PKDevTools-0.13.20240417.93/PKDevTools/classes/Archiver.py
+-rw-rw-rw-   0        0        0     4831 2024-04-17 21:53:11.000000 PKDevTools-0.13.20240417.93/PKDevTools/classes/ColorText.py
+-rw-rw-rw-   0        0        0     3599 2024-04-17 21:53:11.000000 PKDevTools-0.13.20240417.93/PKDevTools/classes/Committer.py
+-rw-rw-rw-   0        0        0     6212 2024-04-17 21:53:11.000000 PKDevTools-0.13.20240417.93/PKDevTools/classes/CookieHelper.py
+-rw-rw-rw-   0        0        0     8879 2024-04-17 21:53:11.000000 PKDevTools-0.13.20240417.93/PKDevTools/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11963 2024-04-17 21:53:11.000000 PKDevTools-0.13.20240417.93/PKDevTools/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0     2501 2024-04-17 21:53:11.000000 PKDevTools-0.13.20240417.93/PKDevTools/classes/OutputControls.py
+-rw-rw-rw-   0        0        0    13778 2024-04-17 21:53:11.000000 PKDevTools-0.13.20240417.93/PKDevTools/classes/PKDateUtilities.py
+-rw-rw-rw-   0        0        0     2988 2024-04-17 21:53:11.000000 PKDevTools-0.13.20240417.93/PKDevTools/classes/PKGitFolderDownloader.py
+-rw-rw-rw-   0        0        0     8048 2024-04-17 21:53:11.000000 PKDevTools-0.13.20240417.93/PKDevTools/classes/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    14334 2024-04-17 21:53:11.000000 PKDevTools-0.13.20240417.93/PKDevTools/classes/PKPickler.py
+-rw-rw-rw-   0        0        0     3433 2024-04-17 21:53:11.000000 PKDevTools-0.13.20240417.93/PKDevTools/classes/PKTimer.py
+-rw-rw-rw-   0        0        0     4548 2024-04-17 21:53:11.000000 PKDevTools-0.13.20240417.93/PKDevTools/classes/Singleton.py
+-rw-rw-rw-   0        0        0     1916 2024-04-17 21:53:11.000000 PKDevTools-0.13.20240417.93/PKDevTools/classes/SuppressOutput.py
+-rw-rw-rw-   0        0        0    11301 2024-04-17 21:53:11.000000 PKDevTools-0.13.20240417.93/PKDevTools/classes/Telegram.py
+-rw-rw-rw-   0        0        0    24543 2024-04-17 21:53:11.000000 PKDevTools-0.13.20240417.93/PKDevTools/classes/Utils.py
+-rw-rw-rw-   0        0        0     9984 2024-04-17 21:53:11.000000 PKDevTools-0.13.20240417.93/PKDevTools/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       27 2024-04-17 21:55:09.000000 PKDevTools-0.13.20240417.93/PKDevTools/classes/__init__.py
+-rw-rw-rw-   0        0        0     3738 2024-04-17 21:53:11.000000 PKDevTools-0.13.20240417.93/PKDevTools/classes/githubutilities.py
+-rw-rw-rw-   0        0        0    16118 2024-04-17 21:53:11.000000 PKDevTools-0.13.20240417.93/PKDevTools/classes/log.py
+-rw-rw-rw-   0        0        0     5384 2024-04-17 21:53:11.000000 PKDevTools-0.13.20240417.93/PKDevTools/classes/multiprocessing_logging.py
+-rw-rw-rw-   0        0        0     2864 2024-04-17 21:53:11.000000 PKDevTools-0.13.20240417.93/PKDevTools/classes/squash.py
+-rw-rw-rw-   0        0        0     4846 2024-04-17 21:53:11.000000 PKDevTools-0.13.20240417.93/PKDevTools/classes/updater.py
+drwxrwxrwx   0        0        0        0 2024-04-17 21:55:14.394192 PKDevTools-0.13.20240417.93/PKDevTools.egg-info/
+-rw-rw-rw-   0        0        0     5202 2024-04-17 21:55:14.000000 PKDevTools-0.13.20240417.93/PKDevTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1084 2024-04-17 21:55:14.000000 PKDevTools-0.13.20240417.93/PKDevTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 21:55:14.000000 PKDevTools-0.13.20240417.93/PKDevTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      363 2024-04-17 21:55:14.000000 PKDevTools-0.13.20240417.93/PKDevTools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-17 21:55:08.000000 PKDevTools-0.13.20240417.93/PKDevTools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      158 2024-04-17 21:55:14.000000 PKDevTools-0.13.20240417.93/PKDevTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-17 21:55:14.000000 PKDevTools-0.13.20240417.93/PKDevTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5202 2024-04-17 21:55:14.394192 PKDevTools-0.13.20240417.93/PKG-INFO
+-rw-rw-rw-   0        0        0     4290 2024-04-17 21:53:11.000000 PKDevTools-0.13.20240417.93/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-17 21:55:14.394192 PKDevTools-0.13.20240417.93/setup.cfg
+-rw-rw-rw-   0        0        0     4341 2024-04-17 21:53:11.000000 PKDevTools-0.13.20240417.93/setup.py
```

### Comparing `PKDevTools-0.13.20240417.92/LICENSE` & `PKDevTools-0.13.20240417.93/LICENSE`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.92/PKDevTools/__init__.py` & `PKDevTools-0.13.20240417.93/PKDevTools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.92/PKDevTools/classes/Archiver.py` & `PKDevTools-0.13.20240417.93/PKDevTools/classes/Archiver.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.92/PKDevTools/classes/ColorText.py` & `PKDevTools-0.13.20240417.93/PKDevTools/classes/ColorText.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.92/PKDevTools/classes/Committer.py` & `PKDevTools-0.13.20240417.93/PKDevTools/classes/Committer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.92/PKDevTools/classes/CookieHelper.py` & `PKDevTools-0.13.20240417.93/PKDevTools/classes/CookieHelper.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.92/PKDevTools/classes/Fetcher.py` & `PKDevTools-0.13.20240417.93/PKDevTools/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.92/PKDevTools/classes/MenuOptions.py` & `PKDevTools-0.13.20240417.93/PKDevTools/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.92/PKDevTools/classes/OutputControls.py` & `PKDevTools-0.13.20240417.93/PKDevTools/classes/OutputControls.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,34 +19,36 @@
     AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
     LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
     OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
     SOFTWARE.
 
 """
 import sys
+import os
 from typing_extensions import Literal
 
 from PKDevTools.classes.Singleton import SingletonType, SingletonMixin
 
 class OutputControls(SingletonMixin, metaclass=SingletonType):
     def __init__(self, enableMultipleLineOutput=False):
         super(OutputControls, self).__init__()
-        self.enableMultipleLineOutput = enableMultipleLineOutput
+        self.enableMultipleLineOutput = enableMultipleLineOutput or ('PKDevTools_Default_Log_Level' in os.environ.keys())
 
     def printOutput(
         self,
         *values: object,
         sep: str | None = " ",
         end: str | None = "\n",
         flush: Literal[False]| bool = False,
         enableMultipleLineOutput=False
     ) -> None:
         # end = '\r' if (not enableMultipleLineOutput) else end
         # flush = True if (not enableMultipleLineOutput) else flush
         print(*values, sep=sep, end=end, flush=flush)
+        enableMultipleLineOutput = enableMultipleLineOutput or ('PKDevTools_Default_Log_Level' in os.environ.keys())
         if enableMultipleLineOutput:
             return
         lines = len(str(*values).splitlines())
         if not self.enableMultipleLineOutput and not enableMultipleLineOutput:
             for _ in range(lines):
                 sys.stdout.write("\x1b[1A")  # cursor up one line
                 sys.stdout.write("\x1b[2K")  # delete the last line
```

### Comparing `PKDevTools-0.13.20240417.92/PKDevTools/classes/PKDateUtilities.py` & `PKDevTools-0.13.20240417.93/PKDevTools/classes/PKDateUtilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.92/PKDevTools/classes/PKGitFolderDownloader.py` & `PKDevTools-0.13.20240417.93/PKDevTools/classes/PKGitFolderDownloader.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.92/PKDevTools/classes/PKMultiProcessorClient.py` & `PKDevTools-0.13.20240417.93/PKDevTools/classes/PKMultiProcessorClient.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.92/PKDevTools/classes/PKPickler.py` & `PKDevTools-0.13.20240417.93/PKDevTools/classes/PKPickler.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.92/PKDevTools/classes/PKTimer.py` & `PKDevTools-0.13.20240417.93/PKDevTools/classes/PKTimer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.92/PKDevTools/classes/Singleton.py` & `PKDevTools-0.13.20240417.93/PKDevTools/classes/Singleton.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.92/PKDevTools/classes/SuppressOutput.py` & `PKDevTools-0.13.20240417.93/PKDevTools/classes/SuppressOutput.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.92/PKDevTools/classes/Telegram.py` & `PKDevTools-0.13.20240417.93/PKDevTools/classes/Telegram.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.92/PKDevTools/classes/Utils.py` & `PKDevTools-0.13.20240417.93/PKDevTools/classes/Utils.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.92/PKDevTools/classes/WorkflowManager.py` & `PKDevTools-0.13.20240417.93/PKDevTools/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.92/PKDevTools/classes/githubutilities.py` & `PKDevTools-0.13.20240417.93/PKDevTools/classes/githubutilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.92/PKDevTools/classes/log.py` & `PKDevTools-0.13.20240417.93/PKDevTools/classes/log.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.92/PKDevTools/classes/multiprocessing_logging.py` & `PKDevTools-0.13.20240417.93/PKDevTools/classes/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.92/PKDevTools/classes/squash.py` & `PKDevTools-0.13.20240417.93/PKDevTools/classes/squash.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.92/PKDevTools/classes/updater.py` & `PKDevTools-0.13.20240417.93/PKDevTools/classes/updater.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.92/PKDevTools.egg-info/PKG-INFO` & `PKDevTools-0.13.20240417.93/PKDevTools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240417.92
+Version: 0.13.20240417.93
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240417.92.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240417.93.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240417.92/PKDevTools.egg-info/SOURCES.txt` & `PKDevTools-0.13.20240417.93/PKDevTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.92/PKG-INFO` & `PKDevTools-0.13.20240417.93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240417.92
+Version: 0.13.20240417.93
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240417.92.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240417.93.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240417.92/README.md` & `PKDevTools-0.13.20240417.93/README.md`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.92/setup.py` & `PKDevTools-0.13.20240417.93/setup.py`

 * *Files identical despite different names*

