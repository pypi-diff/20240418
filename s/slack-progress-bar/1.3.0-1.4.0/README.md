# Comparing `tmp/slack_progress_bar-1.3.0.tar.gz` & `tmp/slack_progress_bar-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack_progress_bar-1.3.0.tar", last modified: Sun Mar 24 15:23:42 2024, max compression
+gzip compressed data, was "slack_progress_bar-1.4.0.tar", last modified: Thu Apr 18 20:06:56 2024, max compression
```

## Comparing `slack_progress_bar-1.3.0.tar` & `slack_progress_bar-1.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mlizzi     (501) staff       (20)        0 2024-03-24 15:23:42.233882 slack_progress_bar-1.3.0/
--rw-r--r--   0 mlizzi     (501) staff       (20)     1070 2024-03-17 01:58:35.000000 slack_progress_bar-1.3.0/LICENSE
--rw-r--r--   0 mlizzi     (501) staff       (20)     1620 2024-03-24 15:23:42.233423 slack_progress_bar-1.3.0/PKG-INFO
--rw-r--r--   0 mlizzi     (501) staff       (20)     1097 2024-03-23 19:33:11.000000 slack_progress_bar-1.3.0/README.md
--rw-r--r--   0 mlizzi     (501) staff       (20)       38 2024-03-24 15:23:42.234116 slack_progress_bar-1.3.0/setup.cfg
--rw-r--r--   0 mlizzi     (501) staff       (20)      742 2024-03-24 15:12:08.000000 slack_progress_bar-1.3.0/setup.py
-drwxr-xr-x   0 mlizzi     (501) staff       (20)        0 2024-03-24 15:23:42.228751 slack_progress_bar-1.3.0/slack_progress_bar/
--rw-r--r--   0 mlizzi     (501) staff       (20)       49 2024-03-17 20:18:49.000000 slack_progress_bar-1.3.0/slack_progress_bar/__init__.py
--rw-r--r--   0 mlizzi     (501) staff       (20)     2897 2024-03-24 15:09:30.000000 slack_progress_bar-1.3.0/slack_progress_bar/slack_progress_bar.py
-drwxr-xr-x   0 mlizzi     (501) staff       (20)        0 2024-03-24 15:23:42.232454 slack_progress_bar-1.3.0/slack_progress_bar.egg-info/
--rw-r--r--   0 mlizzi     (501) staff       (20)     1620 2024-03-24 15:23:41.000000 slack_progress_bar-1.3.0/slack_progress_bar.egg-info/PKG-INFO
--rw-r--r--   0 mlizzi     (501) staff       (20)      307 2024-03-24 15:23:41.000000 slack_progress_bar-1.3.0/slack_progress_bar.egg-info/SOURCES.txt
--rw-r--r--   0 mlizzi     (501) staff       (20)        1 2024-03-24 15:23:41.000000 slack_progress_bar-1.3.0/slack_progress_bar.egg-info/dependency_links.txt
--rw-r--r--   0 mlizzi     (501) staff       (20)       10 2024-03-24 15:23:41.000000 slack_progress_bar-1.3.0/slack_progress_bar.egg-info/requires.txt
--rw-r--r--   0 mlizzi     (501) staff       (20)       19 2024-03-24 15:23:41.000000 slack_progress_bar-1.3.0/slack_progress_bar.egg-info/top_level.txt
+drwxr-xr-x   0 mlizzi     (501) staff       (20)        0 2024-04-18 20:06:56.737480 slack_progress_bar-1.4.0/
+-rw-r--r--   0 mlizzi     (501) staff       (20)     1070 2024-03-17 01:58:35.000000 slack_progress_bar-1.4.0/LICENSE
+-rw-r--r--   0 mlizzi     (501) staff       (20)     1732 2024-04-18 20:06:56.737103 slack_progress_bar-1.4.0/PKG-INFO
+-rw-r--r--   0 mlizzi     (501) staff       (20)     1209 2024-04-18 17:14:06.000000 slack_progress_bar-1.4.0/README.md
+-rw-r--r--   0 mlizzi     (501) staff       (20)       38 2024-04-18 20:06:56.737738 slack_progress_bar-1.4.0/setup.cfg
+-rw-r--r--   0 mlizzi     (501) staff       (20)      742 2024-04-18 20:06:42.000000 slack_progress_bar-1.4.0/setup.py
+drwxr-xr-x   0 mlizzi     (501) staff       (20)        0 2024-04-18 20:06:56.732402 slack_progress_bar-1.4.0/slack_progress_bar/
+-rw-r--r--   0 mlizzi     (501) staff       (20)       49 2024-03-17 20:18:49.000000 slack_progress_bar-1.4.0/slack_progress_bar/__init__.py
+-rw-r--r--   0 mlizzi     (501) staff       (20)     3666 2024-04-18 20:06:03.000000 slack_progress_bar-1.4.0/slack_progress_bar/slack_progress_bar.py
+drwxr-xr-x   0 mlizzi     (501) staff       (20)        0 2024-04-18 20:06:56.736411 slack_progress_bar-1.4.0/slack_progress_bar.egg-info/
+-rw-r--r--   0 mlizzi     (501) staff       (20)     1732 2024-04-18 20:06:56.000000 slack_progress_bar-1.4.0/slack_progress_bar.egg-info/PKG-INFO
+-rw-r--r--   0 mlizzi     (501) staff       (20)      307 2024-04-18 20:06:56.000000 slack_progress_bar-1.4.0/slack_progress_bar.egg-info/SOURCES.txt
+-rw-r--r--   0 mlizzi     (501) staff       (20)        1 2024-04-18 20:06:56.000000 slack_progress_bar-1.4.0/slack_progress_bar.egg-info/dependency_links.txt
+-rw-r--r--   0 mlizzi     (501) staff       (20)       10 2024-04-18 20:06:56.000000 slack_progress_bar-1.4.0/slack_progress_bar.egg-info/requires.txt
+-rw-r--r--   0 mlizzi     (501) staff       (20)       19 2024-04-18 20:06:56.000000 slack_progress_bar-1.4.0/slack_progress_bar.egg-info/top_level.txt
```

### Comparing `slack_progress_bar-1.3.0/LICENSE` & `slack_progress_bar-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slack_progress_bar-1.3.0/PKG-INFO` & `slack_progress_bar-1.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: slack_progress_bar
-Version: 1.3.0
+Version: 1.4.0
 Summary: A Python package for displaying progress bars in Slack messages.
 Home-page: https://github.com/mlizzi/slack-progress-bar
 Author: Michael Lizzi
 Author-email: michael.lizzi@hotmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# slack-progress-bar
+# slack-progress-bar [![Downloads](https://static.pepy.tech/badge/slack-progress-bar)](https://pepy.tech/project/slack-progress-bar)
 A Python library for adding a progress bar to a Slack Bot, updated for Python 3.9+.
 
 ![animated-gif](https://imgur.com/WkC70eR.gif)
 
 ## Installation
 ```bash
 pip install slack-progress-bar
```

### Comparing `slack_progress_bar-1.3.0/README.md` & `slack_progress_bar-1.4.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# slack-progress-bar
+# slack-progress-bar [![Downloads](https://static.pepy.tech/badge/slack-progress-bar)](https://pepy.tech/project/slack-progress-bar)
 A Python library for adding a progress bar to a Slack Bot, updated for Python 3.9+.
 
 ![animated-gif](https://imgur.com/WkC70eR.gif)
 
 ## Installation
 ```bash
 pip install slack-progress-bar
```

### Comparing `slack_progress_bar-1.3.0/setup.py` & `slack_progress_bar-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="slack_progress_bar",
-    version="1.3.0",
+    version="1.4.0",
     author="Michael Lizzi",
     author_email="michael.lizzi@hotmail.com",
     description="A Python package for displaying progress bars in Slack messages.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mlizzi/slack-progress-bar",
     packages=find_packages(),
```

### Comparing `slack_progress_bar-1.3.0/slack_progress_bar/slack_progress_bar.py` & `slack_progress_bar-1.4.0/slack_progress_bar/slack_progress_bar.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,57 @@
 from slack_sdk import WebClient
 from slack_sdk.errors import SlackApiError
 
 
 class SlackProgressBar:
 
     def __init__(
-        self, token: str, user_id: str, total: int, bar_width: int = 20
+        self,
+        token: str,
+        user_id: str,
+        total: int,
+        value: int = 0,
+        bar_width: int = 20,
+        notify: bool = True,
     ) -> None:
         """A progress bar to use with Slack.
 
         Parameters
         ----------
         token
             The SlackBot token.
         user_id
             The user id of the Slack account to send messages to.
         total
             The total length of the progress bar.
+        value
+            The initial value of the progress bar.
         bar_width
             The width of the progress bar as seen on Slack.
+        notify
+            If the progress bar will send a message on Slack. Can be used
+            to disable or enable message sending.
         """
         self._client = WebClient(token=token)
         self._total = total
         self._bar_width = bar_width
-        self._value = 0
+        self._value = value
+        self._ts = None
+
+        self.notify = notify
 
         # Get channel id of user conversation (for posting and updating)
         try:
             res = self._client.conversations_open(users=user_id)
             self._channel_id = res["channel"]["id"]
         except SlackApiError:
             ValueError("Enter valid user id (Slack Profile -> Copy member ID")
 
-        res = self._client.chat_postMessage(
-            channel=self._channel_id, text=self._as_string()
-        )
-
-        self._ts = res["ts"]
+        if self.notify:
+            self._chat_update()
 
     def update(self, value: int) -> None:
         """Update the current progress bar on Slack.
 
         Parameters
         ----------
         value
@@ -55,29 +66,44 @@
         self._value = value
 
         message = (
             ":white_check_mark: Loading complete!"
             if self._value == self._total
             else ""
         )
-
-        self._client.chat_update(
-            channel=self._channel_id,
-            ts=self._ts,
-            text=self._as_string(message),
-        )
+        self._chat_update(message)
 
     def error(self) -> None:
         """Set the bar to an error state to indicate loading has stopped."""
-        self._client.chat_update(
-            channel=self._channel_id,
-            ts=self._ts,
-            text=self._as_string(message=":warning: ERROR: Loading stopped!"),
+        self._chat_update(
+            self._as_string(message=":warning: ERROR: Loading stopped!")
         )
 
+    def _chat_update(self, message: str = "") -> None:
+        """Sends a message on Slack if the progress bar is not disabled.
+
+        Parameters
+        ----------
+        message
+            A message to include alongside the progress bar.
+        """
+
+        if self.notify:
+            if not self._ts:
+                res = self._client.chat_postMessage(
+                    channel=self._channel_id, text=self._as_string(message)
+                )
+                self._ts = res["ts"]
+            else:
+                self._client.chat_update(
+                    channel=self._channel_id,
+                    ts=self._ts,
+                    text=self._as_string(message),
+                )
+
     def _as_string(self, message: str = "") -> str:
         """Get the progress bar visualized as a string.
 
         Parameters
         ----------
         message
             A message to include alongside the progress bar.
```

### Comparing `slack_progress_bar-1.3.0/slack_progress_bar.egg-info/PKG-INFO` & `slack_progress_bar-1.4.0/slack_progress_bar.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: slack-progress-bar
-Version: 1.3.0
+Version: 1.4.0
 Summary: A Python package for displaying progress bars in Slack messages.
 Home-page: https://github.com/mlizzi/slack-progress-bar
 Author: Michael Lizzi
 Author-email: michael.lizzi@hotmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# slack-progress-bar
+# slack-progress-bar [![Downloads](https://static.pepy.tech/badge/slack-progress-bar)](https://pepy.tech/project/slack-progress-bar)
 A Python library for adding a progress bar to a Slack Bot, updated for Python 3.9+.
 
 ![animated-gif](https://imgur.com/WkC70eR.gif)
 
 ## Installation
 ```bash
 pip install slack-progress-bar
```

