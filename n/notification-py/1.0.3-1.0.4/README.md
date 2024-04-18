# Comparing `tmp/notification_py-1.0.3.tar.gz` & `tmp/notification_py-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notification_py-1.0.3.tar", max compression
+gzip compressed data, was "notification_py-1.0.4.tar", max compression
```

## Comparing `notification_py-1.0.3.tar` & `notification_py-1.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2024-03-30 07:03:53.459271 notification_py-1.0.3/LICENSE
--rw-r--r--   0        0        0     5944 2024-04-10 04:18:54.275409 notification_py-1.0.3/README.md
--rw-r--r--   0        0        0      450 2024-04-10 01:05:55.624161 notification_py-1.0.3/notification_py/__init__.py
--rw-r--r--   0        0        0     1084 2024-04-10 03:19:23.410798 notification_py-1.0.3/notification_py/custom_types.py
--rw-r--r--   0        0        0     2409 2024-04-10 04:04:06.737194 notification_py-1.0.3/notification_py/main.py
--rw-r--r--   0        0        0        0 2024-03-30 07:36:24.198672 notification_py-1.0.3/notification_py/services/__init__.py
--rw-r--r--   0        0        0     4636 2024-04-10 03:57:16.042206 notification_py-1.0.3/notification_py/services/discord.py
--rw-r--r--   0        0        0     2300 2024-04-10 03:57:04.290177 notification_py-1.0.3/notification_py/services/email.py
--rw-r--r--   0        0        0     3666 2024-04-10 03:57:23.424224 notification_py-1.0.3/notification_py/services/slack.py
--rw-r--r--   0        0        0      774 2024-04-10 04:26:58.599099 notification_py-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     6868 1970-01-01 00:00:00.000000 notification_py-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-30 07:03:53.459271 notification_py-1.0.4/LICENSE
+-rw-r--r--   0        0        0     6203 2024-04-18 15:11:36.143137 notification_py-1.0.4/README.md
+-rw-r--r--   0        0        0      450 2024-04-10 01:05:55.624161 notification_py-1.0.4/notification_py/__init__.py
+-rw-r--r--   0        0        0     1084 2024-04-10 03:19:23.410798 notification_py-1.0.4/notification_py/custom_types.py
+-rw-r--r--   0        0        0     2409 2024-04-10 04:04:06.737194 notification_py-1.0.4/notification_py/main.py
+-rw-r--r--   0        0        0        0 2024-03-30 07:36:24.198672 notification_py-1.0.4/notification_py/services/__init__.py
+-rw-r--r--   0        0        0     4636 2024-04-10 03:57:16.042206 notification_py-1.0.4/notification_py/services/discord.py
+-rw-r--r--   0        0        0     2300 2024-04-10 03:57:04.290177 notification_py-1.0.4/notification_py/services/email.py
+-rw-r--r--   0        0        0     3886 2024-04-18 15:07:59.399686 notification_py-1.0.4/notification_py/services/slack.py
+-rw-r--r--   0        0        0      774 2024-04-18 15:04:32.857200 notification_py-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     7127 1970-01-01 00:00:00.000000 notification_py-1.0.4/PKG-INFO
```

### Comparing `notification_py-1.0.3/LICENSE` & `notification_py-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `notification_py-1.0.3/README.md` & `notification_py-1.0.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # notification-py
 `notification-py` is a Python package that provides a simple and convenient way to send notifications to Discord, Slack, and Email. You can send notification to either of these using a single command.
 
+- Total Downloads: [![Downloads](https://static.pepy.tech/badge/notification-py)](https://pepy.tech/project/notification-py)
+- Monthly Downloads: [![Downloads](https://static.pepy.tech/badge/notification-py/month)](https://pepy.tech/project/notification-py)
+
 
 ## Motivation
 Lately I noticed several critical errors poping up in my python backend, I thought of a simple way to get notified about these failues (be it Stripe webhooks or anything else). So I came up with this idea to create a simple notification package which can be imported and used when unexpected errors are thrown by code.
 
 > Using this package, developers can receive notifications through various combinations of Discord, Slack, and Email. The package supports sending notifications to all three platforms simultaneously, any two of them, or just one platform, depending on the provided credentials and configuration. This flexibility allows developers to customize their notification setup based on their specific requirements and preferences.
```

### Comparing `notification_py-1.0.3/notification_py/custom_types.py` & `notification_py-1.0.4/notification_py/custom_types.py`

 * *Files identical despite different names*

### Comparing `notification_py-1.0.3/notification_py/main.py` & `notification_py-1.0.4/notification_py/main.py`

 * *Files identical despite different names*

### Comparing `notification_py-1.0.3/notification_py/services/discord.py` & `notification_py-1.0.4/notification_py/services/discord.py`

 * *Files identical despite different names*

### Comparing `notification_py-1.0.3/notification_py/services/email.py` & `notification_py-1.0.4/notification_py/services/email.py`

 * *Files identical despite different names*

### Comparing `notification_py-1.0.3/pyproject.toml` & `notification_py-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "notification_py"
-version = "1.0.3"
+version = "1.0.4"
 description = "A simple package to send notifications on Discord, Slack and Email."
 authors = ["Pranav Soni <pranav.bhawan@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/ps428/notification-py/"
 packages = [{include = "notification_py"}]
```

### Comparing `notification_py-1.0.3/PKG-INFO` & `notification_py-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notification-py
-Version: 1.0.3
+Version: 1.0.4
 Summary: A simple package to send notifications on Discord, Slack and Email.
 Home-page: https://github.com/ps428/notification-py/
 License: Apache-2.0
 Author: Pranav Soni
 Author-email: pranav.bhawan@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -20,14 +20,17 @@
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Project-URL: Repository, https://github.com/ps428/notification-py/
 Description-Content-Type: text/markdown
 
 # notification-py
 `notification-py` is a Python package that provides a simple and convenient way to send notifications to Discord, Slack, and Email. You can send notification to either of these using a single command.
 
+- Total Downloads: [![Downloads](https://static.pepy.tech/badge/notification-py)](https://pepy.tech/project/notification-py)
+- Monthly Downloads: [![Downloads](https://static.pepy.tech/badge/notification-py/month)](https://pepy.tech/project/notification-py)
+
 
 ## Motivation
 Lately I noticed several critical errors poping up in my python backend, I thought of a simple way to get notified about these failues (be it Stripe webhooks or anything else). So I came up with this idea to create a simple notification package which can be imported and used when unexpected errors are thrown by code.
 
 > Using this package, developers can receive notifications through various combinations of Discord, Slack, and Email. The package supports sending notifications to all three platforms simultaneously, any two of them, or just one platform, depending on the provided credentials and configuration. This flexibility allows developers to customize their notification setup based on their specific requirements and preferences.
```

