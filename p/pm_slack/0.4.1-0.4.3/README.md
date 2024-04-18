# Comparing `tmp/pm_slack-0.4.1.tar.gz` & `tmp/pm_slack-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pm_slack-0.4.1.tar", max compression
+gzip compressed data, was "pm_slack-0.4.3.tar", max compression
```

## Comparing `pm_slack-0.4.1.tar` & `pm_slack-0.4.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1078 2023-11-01 13:41:14.761998 pm_slack-0.4.1/LICENSE
--rw-r--r--   0        0        0       45 2023-11-01 13:41:14.761998 pm_slack-0.4.1/README.md
--rw-r--r--   0        0        0       76 2023-11-01 13:41:14.761998 pm_slack-0.4.1/pm_slack/__init__.py
--rw-r--r--   0        0        0       40 2023-11-01 13:41:14.761998 pm_slack-0.4.1/pm_slack/constants.py
--rw-r--r--   0        0        0     2163 2023-11-01 13:41:14.761998 pm_slack-0.4.1/pm_slack/main.py
--rw-r--r--   0        0        0        0 2023-11-01 13:41:14.761998 pm_slack-0.4.1/pm_slack/py.typed
--rw-r--r--   0        0        0     1079 2023-11-01 13:41:14.761998 pm_slack-0.4.1/pm_slack/templates/__init__.py
--rw-r--r--   0        0        0    21356 2023-11-01 13:41:14.761998 pm_slack-0.4.1/pm_slack/templates/_templates.py
--rw-r--r--   0        0        0     1107 2023-11-01 13:41:46.290085 pm_slack-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      674 1970-01-01 00:00:00.000000 pm_slack-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-18 11:34:12.610100 pm_slack-0.4.3/LICENSE
+-rw-r--r--   0        0        0       45 2024-04-18 11:34:12.610100 pm_slack-0.4.3/README.md
+-rw-r--r--   0        0        0       76 2024-04-18 11:34:12.610100 pm_slack-0.4.3/pm_slack/__init__.py
+-rw-r--r--   0        0        0       40 2024-04-18 11:34:12.614100 pm_slack-0.4.3/pm_slack/constants.py
+-rw-r--r--   0        0        0     2612 2024-04-18 11:34:12.614100 pm_slack-0.4.3/pm_slack/main.py
+-rw-r--r--   0        0        0        0 2024-04-18 11:34:12.614100 pm_slack-0.4.3/pm_slack/py.typed
+-rw-r--r--   0        0        0     1079 2024-04-18 11:34:12.614100 pm_slack-0.4.3/pm_slack/templates/__init__.py
+-rw-r--r--   0        0        0    21356 2024-04-18 11:34:12.614100 pm_slack-0.4.3/pm_slack/templates/_templates.py
+-rw-r--r--   0        0        0     1107 2024-04-18 11:34:28.458086 pm_slack-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 pm_slack-0.4.3/PKG-INFO
```

### Comparing `pm_slack-0.4.1/LICENSE` & `pm_slack-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pm_slack-0.4.1/pm_slack/main.py` & `pm_slack-0.4.3/pm_slack/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -71,7 +71,21 @@
             )
 
         self.client.chat_postMessage(
             channel=channel,
             blocks=blocks,
             text="Paket Mutfak",
         )
+
+    def send_file(self, channel:  str = COMMON_SLACK_CHANNEL_ID, file: str = "", title: str = "",
+                  initial_comment: str = "") -> None:
+        if self.send_to_slack is False:
+            if self.logger:
+                self.logger.info(title)
+            return
+
+        self.client.files_upload_v2(
+            channel=channel,
+            file=file,
+            title=title,
+            initial_comment=initial_comment,
+        )
```

### Comparing `pm_slack-0.4.1/pm_slack/templates/__init__.py` & `pm_slack-0.4.3/pm_slack/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pm_slack-0.4.1/pm_slack/templates/_templates.py` & `pm_slack-0.4.3/pm_slack/templates/_templates.py`

 * *Files identical despite different names*

### Comparing `pm_slack-0.4.1/pyproject.toml` & `pm_slack-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pm_slack"
-version = "0.4.1"
+version = "0.4.3"
 description = "A Slack Library for Paket Mutfak"
 authors = ["Paket Mutfak Dev Team <dev@paketmutfak.com.tr>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `pm_slack-0.4.1/PKG-INFO` & `pm_slack-0.4.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pm_slack
-Version: 0.4.1
+Version: 0.4.3
 Summary: A Slack Library for Paket Mutfak
 License: MIT
 Author: Paket Mutfak Dev Team
 Author-email: dev@paketmutfak.com.tr
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ruff (>=0.0.267,<0.0.271)
 Requires-Dist: slack-sdk (>=3.21.3,<4.0.0)
 Description-Content-Type: text/markdown
 
 # pm_slack
 
 A Slack Library for Paket Mutfak
```

