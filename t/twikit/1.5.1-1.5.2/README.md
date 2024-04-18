# Comparing `tmp/twikit-1.5.1.tar.gz` & `tmp/twikit-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twikit-1.5.1.tar", last modified: Tue Apr 16 15:19:30 2024, max compression
+gzip compressed data, was "twikit-1.5.2.tar", last modified: Thu Apr 18 10:35:52 2024, max compression
```

## Comparing `twikit-1.5.1.tar` & `twikit-1.5.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 15:19:30.407811 twikit-1.5.1/
--rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:36.000000 twikit-1.5.1/LICENSE
--rw-rw-rw-   0        0        0     3863 2024-04-16 15:19:30.404823 twikit-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     3590 2024-04-13 12:42:36.000000 twikit-1.5.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-16 15:19:30.407811 twikit-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0      694 2024-04-13 12:42:36.000000 twikit-1.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 15:19:30.293120 twikit-1.5.1/twikit/
--rw-rw-rw-   0        0        0      620 2024-04-16 15:17:55.000000 twikit-1.5.1/twikit/__init__.py
--rw-rw-rw-   0        0        0   132489 2024-04-16 15:17:16.000000 twikit-1.5.1/twikit/client.py
--rw-rw-rw-   0        0        0     8639 2024-04-15 14:41:30.000000 twikit-1.5.1/twikit/community.py
--rw-rw-rw-   0        0        0     2626 2024-04-14 11:15:08.000000 twikit-1.5.1/twikit/errors.py
--rw-rw-rw-   0        0        0     7305 2024-04-13 12:42:36.000000 twikit-1.5.1/twikit/group.py
--rw-rw-rw-   0        0        0     2095 2024-04-14 11:11:34.000000 twikit-1.5.1/twikit/http.py
--rw-rw-rw-   0        0        0     7617 2024-04-13 12:42:37.000000 twikit-1.5.1/twikit/list.py
--rw-rw-rw-   0        0        0     3908 2024-04-13 12:42:37.000000 twikit-1.5.1/twikit/message.py
--rw-rw-rw-   0        0        0     1439 2024-04-13 14:30:38.000000 twikit-1.5.1/twikit/notification.py
--rw-rw-rw-   0        0        0     1070 2024-04-13 12:42:37.000000 twikit-1.5.1/twikit/trend.py
--rw-rw-rw-   0        0        0    20836 2024-04-16 15:06:59.000000 twikit-1.5.1/twikit/tweet.py
-drwxrwxrwx   0        0        0        0 2024-04-16 15:19:30.401828 twikit-1.5.1/twikit/twikit_async/
--rw-rw-rw-   0        0        0      572 2024-04-15 14:48:54.000000 twikit-1.5.1/twikit/twikit_async/__init__.py
--rw-rw-rw-   0        0        0   134756 2024-04-16 15:17:50.000000 twikit-1.5.1/twikit/twikit_async/client.py
--rw-rw-rw-   0        0        0     8767 2024-04-15 14:48:23.000000 twikit-1.5.1/twikit/twikit_async/community.py
--rw-rw-rw-   0        0        0      875 2024-04-13 12:42:37.000000 twikit-1.5.1/twikit/twikit_async/errors.py
--rw-rw-rw-   0        0        0     7509 2024-04-13 12:42:37.000000 twikit-1.5.1/twikit/twikit_async/group.py
--rw-rw-rw-   0        0        0     2137 2024-04-14 11:11:58.000000 twikit-1.5.1/twikit/twikit_async/http.py
--rw-rw-rw-   0        0        0     7780 2024-04-13 12:42:37.000000 twikit-1.5.1/twikit/twikit_async/list.py
--rw-rw-rw-   0        0        0     3974 2024-04-13 12:42:37.000000 twikit-1.5.1/twikit/twikit_async/message.py
--rw-rw-rw-   0        0        0     1439 2024-04-13 12:42:37.000000 twikit-1.5.1/twikit/twikit_async/notification.py
--rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:37.000000 twikit-1.5.1/twikit/twikit_async/trend.py
--rw-rw-rw-   0        0        0    20701 2024-04-15 15:04:49.000000 twikit-1.5.1/twikit/twikit_async/tweet.py
--rw-rw-rw-   0        0        0    14740 2024-04-14 04:11:42.000000 twikit-1.5.1/twikit/twikit_async/user.py
--rw-rw-rw-   0        0        0     3390 2024-04-13 12:42:37.000000 twikit-1.5.1/twikit/twikit_async/utils.py
--rw-rw-rw-   0        0        0    14517 2024-04-14 04:11:03.000000 twikit-1.5.1/twikit/user.py
--rw-rw-rw-   0        0        0    24789 2024-04-15 12:37:05.000000 twikit-1.5.1/twikit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-16 15:19:30.313065 twikit-1.5.1/twikit.egg-info/
--rw-rw-rw-   0        0        0     3863 2024-04-16 15:19:29.000000 twikit-1.5.1/twikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      790 2024-04-16 15:19:30.000000 twikit-1.5.1/twikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 15:19:29.000000 twikit-1.5.1/twikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-16 15:19:29.000000 twikit-1.5.1/twikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-16 15:19:29.000000 twikit-1.5.1/twikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 10:35:52.650138 twikit-1.5.2/
+-rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:36.000000 twikit-1.5.2/LICENSE
+-rw-rw-rw-   0        0        0     3863 2024-04-18 10:35:52.645151 twikit-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3590 2024-04-13 12:42:36.000000 twikit-1.5.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-18 10:35:52.651135 twikit-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      694 2024-04-13 12:42:36.000000 twikit-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 10:35:52.452666 twikit-1.5.2/twikit/
+-rw-rw-rw-   0        0        0      620 2024-04-18 10:33:50.000000 twikit-1.5.2/twikit/__init__.py
+-rw-rw-rw-   0        0        0   132500 2024-04-18 10:32:01.000000 twikit-1.5.2/twikit/client.py
+-rw-rw-rw-   0        0        0     8639 2024-04-15 14:41:30.000000 twikit-1.5.2/twikit/community.py
+-rw-rw-rw-   0        0        0     2626 2024-04-14 11:15:08.000000 twikit-1.5.2/twikit/errors.py
+-rw-rw-rw-   0        0        0     7305 2024-04-13 12:42:36.000000 twikit-1.5.2/twikit/group.py
+-rw-rw-rw-   0        0        0     2095 2024-04-14 11:11:34.000000 twikit-1.5.2/twikit/http.py
+-rw-rw-rw-   0        0        0     7617 2024-04-13 12:42:37.000000 twikit-1.5.2/twikit/list.py
+-rw-rw-rw-   0        0        0     3908 2024-04-13 12:42:37.000000 twikit-1.5.2/twikit/message.py
+-rw-rw-rw-   0        0        0     1439 2024-04-13 14:30:38.000000 twikit-1.5.2/twikit/notification.py
+-rw-rw-rw-   0        0        0     1070 2024-04-13 12:42:37.000000 twikit-1.5.2/twikit/trend.py
+-rw-rw-rw-   0        0        0    20836 2024-04-16 15:06:59.000000 twikit-1.5.2/twikit/tweet.py
+drwxrwxrwx   0        0        0        0 2024-04-18 10:35:52.637173 twikit-1.5.2/twikit/twikit_async/
+-rw-rw-rw-   0        0        0      572 2024-04-15 14:48:54.000000 twikit-1.5.2/twikit/twikit_async/__init__.py
+-rw-rw-rw-   0        0        0   134767 2024-04-17 07:31:13.000000 twikit-1.5.2/twikit/twikit_async/client.py
+-rw-rw-rw-   0        0        0     8767 2024-04-15 14:48:23.000000 twikit-1.5.2/twikit/twikit_async/community.py
+-rw-rw-rw-   0        0        0      875 2024-04-13 12:42:37.000000 twikit-1.5.2/twikit/twikit_async/errors.py
+-rw-rw-rw-   0        0        0     7509 2024-04-13 12:42:37.000000 twikit-1.5.2/twikit/twikit_async/group.py
+-rw-rw-rw-   0        0        0     2137 2024-04-14 11:11:58.000000 twikit-1.5.2/twikit/twikit_async/http.py
+-rw-rw-rw-   0        0        0     7780 2024-04-13 12:42:37.000000 twikit-1.5.2/twikit/twikit_async/list.py
+-rw-rw-rw-   0        0        0     3974 2024-04-13 12:42:37.000000 twikit-1.5.2/twikit/twikit_async/message.py
+-rw-rw-rw-   0        0        0     1439 2024-04-13 12:42:37.000000 twikit-1.5.2/twikit/twikit_async/notification.py
+-rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:37.000000 twikit-1.5.2/twikit/twikit_async/trend.py
+-rw-rw-rw-   0        0        0    20705 2024-04-18 10:33:30.000000 twikit-1.5.2/twikit/twikit_async/tweet.py
+-rw-rw-rw-   0        0        0    14740 2024-04-16 15:30:17.000000 twikit-1.5.2/twikit/twikit_async/user.py
+-rw-rw-rw-   0        0        0     3390 2024-04-13 12:42:37.000000 twikit-1.5.2/twikit/twikit_async/utils.py
+-rw-rw-rw-   0        0        0    14517 2024-04-16 15:30:25.000000 twikit-1.5.2/twikit/user.py
+-rw-rw-rw-   0        0        0    24789 2024-04-15 12:37:05.000000 twikit-1.5.2/twikit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-18 10:35:52.480591 twikit-1.5.2/twikit.egg-info/
+-rw-rw-rw-   0        0        0     3863 2024-04-18 10:35:51.000000 twikit-1.5.2/twikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      790 2024-04-18 10:35:52.000000 twikit-1.5.2/twikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 10:35:51.000000 twikit-1.5.2/twikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-18 10:35:51.000000 twikit-1.5.2/twikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-18 10:35:51.000000 twikit-1.5.2/twikit.egg-info/top_level.txt
```

### Comparing `twikit-1.5.1/LICENSE` & `twikit-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twikit-1.5.1/PKG-INFO` & `twikit-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.5.1
+Version: 1.5.2
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.5.1/README.md` & `twikit-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `twikit-1.5.1/setup.py` & `twikit-1.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.1/twikit/__init__.py` & `twikit-1.5.2/twikit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ==========================
 Twikit Twitter API Wrapper
 ==========================
 
 A Python library for interacting with the Twitter API.
 """
 
-__version__ = '1.5.1'
+__version__ = '1.5.2'
 
 from .client import Client
 from .community import (Community, CommunityCreator, CommunityMember,
                         CommunityRule)
 from .errors import *
 from .group import Group, GroupMessage
 from .list import List
```

### Comparing `twikit-1.5.1/twikit/client.py` & `twikit-1.5.2/twikit/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1246,15 +1246,15 @@
 
     def _get_more_replies(self, tweet_id: str, cursor: str) -> Result[Tweet]:
         response = self._get_tweet_detail(tweet_id, cursor)
         entries = find_dict(response, 'entries')[0]
 
         results = []
         for entry in entries:
-            if entry['entryId'].startswith('cursor'):
+            if entry['entryId'].startswith(('cursor', 'label')):
                 continue
             tweet_info = find_dict(entry, 'result')[0]
             if tweet_info['__typename'] == 'TweetTombstone':
                 continue
             if tweet_info['__typename'] == 'TweetWithVisibilityResults':
                 tweet_info = tweet_info['tweet']
             user_info = tweet_info['core']['user_results']['result']
```

### Comparing `twikit-1.5.1/twikit/community.py` & `twikit-1.5.2/twikit/community.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.1/twikit/errors.py` & `twikit-1.5.2/twikit/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.1/twikit/group.py` & `twikit-1.5.2/twikit/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.1/twikit/http.py` & `twikit-1.5.2/twikit/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.1/twikit/list.py` & `twikit-1.5.2/twikit/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.1/twikit/message.py` & `twikit-1.5.2/twikit/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.1/twikit/notification.py` & `twikit-1.5.2/twikit/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.1/twikit/trend.py` & `twikit-1.5.2/twikit/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.1/twikit/tweet.py` & `twikit-1.5.2/twikit/tweet.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.1/twikit/twikit_async/__init__.py` & `twikit-1.5.2/twikit/twikit_async/__init__.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.1/twikit/twikit_async/client.py` & `twikit-1.5.2/twikit/twikit_async/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1262,15 +1262,15 @@
         self, tweet_id: str, cursor: str
     ) -> Result[Tweet]:
         response = await self._get_tweet_detail(tweet_id, cursor)
         entries = find_dict(response, 'entries')[0]
 
         results = []
         for entry in entries:
-            if entry['entryId'].startswith('cursor'):
+            if entry['entryId'].startswith(('cursor', 'label')):
                 continue
             tweet_info = find_dict(entry, 'result')[0]
             if tweet_info['__typename'] == 'TweetTombstone':
                 continue
             if tweet_info['__typename'] == 'TweetWithVisibilityResults':
                 tweet_info = tweet_info['tweet']
             user_info = tweet_info['core']['user_results']['result']
```

### Comparing `twikit-1.5.1/twikit/twikit_async/community.py` & `twikit-1.5.2/twikit/twikit_async/community.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.1/twikit/twikit_async/errors.py` & `twikit-1.5.2/twikit/twikit_async/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.1/twikit/twikit_async/group.py` & `twikit-1.5.2/twikit/twikit_async/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.1/twikit/twikit_async/http.py` & `twikit-1.5.2/twikit/twikit_async/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.1/twikit/twikit_async/list.py` & `twikit-1.5.2/twikit/twikit_async/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.1/twikit/twikit_async/message.py` & `twikit-1.5.2/twikit/twikit_async/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.1/twikit/twikit_async/notification.py` & `twikit-1.5.2/twikit/twikit_async/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.1/twikit/twikit_async/trend.py` & `twikit-1.5.2/twikit/twikit_async/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.1/twikit/twikit_async/tweet.py` & `twikit-1.5.2/twikit/twikit_async/tweet.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,20 +166,20 @@
                 hashtags = []
         else:
             hashtags = legacy['entities'].get('hashtags', [])
         self.hashtags: list[str] = [
             i['text'] for i in hashtags
         ]
 
-        if all([
-            'card' in data,
-            'legacy' in data['card'],
-            'name' in data['card']['legacy'],
+        if (
+            'card' in data and
+            'legacy' in data['card'] and
+            'name' in data['card']['legacy'] and
             data['card']['legacy']['name'].startswith('poll')
-        ]):
+        ):
             self._poll_data = data['card']
         else:
             self._poll_data = None
 
     @property
     def created_at_datetime(self) -> datetime:
         return timestamp_to_datetime(self.created_at)
```

### Comparing `twikit-1.5.1/twikit/twikit_async/user.py` & `twikit-1.5.2/twikit/twikit_async/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.1/twikit/twikit_async/utils.py` & `twikit-1.5.2/twikit/twikit_async/utils.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.1/twikit/user.py` & `twikit-1.5.2/twikit/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.1/twikit/utils.py` & `twikit-1.5.2/twikit/utils.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.1/twikit.egg-info/PKG-INFO` & `twikit-1.5.2/twikit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.5.1
+Version: 1.5.2
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.5.1/twikit.egg-info/SOURCES.txt` & `twikit-1.5.2/twikit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

