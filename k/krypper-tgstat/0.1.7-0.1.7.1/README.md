# Comparing `tmp/krypper_tgstat-0.1.7.tar.gz` & `tmp/krypper_tgstat-0.1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krypper_tgstat-0.1.7.tar", last modified: Mon Apr 15 06:49:21 2024, max compression
+gzip compressed data, was "krypper_tgstat-0.1.7.1.tar", last modified: Thu Apr 18 13:27:28 2024, max compression
```

## Comparing `krypper_tgstat-0.1.7.tar` & `krypper_tgstat-0.1.7.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-15 06:49:21.517125 krypper_tgstat-0.1.7/
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)     1063 2024-04-15 06:40:20.000000 krypper_tgstat-0.1.7/LICENSE
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      955 2024-04-15 06:49:21.517125 krypper_tgstat-0.1.7/PKG-INFO
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      103 2024-04-15 06:40:20.000000 krypper_tgstat-0.1.7/README.md
-drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-15 06:49:21.515125 krypper_tgstat-0.1.7/krypper_tgstat/
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      242 2024-04-15 06:49:13.000000 krypper_tgstat-0.1.7/krypper_tgstat/__init__.py
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)     9194 2024-04-15 06:40:20.000000 krypper_tgstat-0.1.7/krypper_tgstat/classes.py
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)     2906 2024-04-15 06:40:20.000000 krypper_tgstat-0.1.7/krypper_tgstat/enums.py
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      666 2024-04-15 06:45:39.000000 krypper_tgstat-0.1.7/krypper_tgstat/exceptions.py
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)     8210 2024-04-15 06:47:48.000000 krypper_tgstat-0.1.7/krypper_tgstat/tg_stat.py
-drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-15 06:49:21.517125 krypper_tgstat-0.1.7/krypper_tgstat.egg-info/
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      955 2024-04-15 06:49:21.000000 krypper_tgstat-0.1.7/krypper_tgstat.egg-info/PKG-INFO
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      382 2024-04-15 06:49:21.000000 krypper_tgstat-0.1.7/krypper_tgstat.egg-info/SOURCES.txt
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)        1 2024-04-15 06:49:21.000000 krypper_tgstat-0.1.7/krypper_tgstat.egg-info/dependency_links.txt
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)       17 2024-04-15 06:49:21.000000 krypper_tgstat-0.1.7/krypper_tgstat.egg-info/requires.txt
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)       15 2024-04-15 06:49:21.000000 krypper_tgstat-0.1.7/krypper_tgstat.egg-info/top_level.txt
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)       38 2024-04-15 06:49:21.517125 krypper_tgstat-0.1.7/setup.cfg
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)     1287 2024-04-15 06:49:17.000000 krypper_tgstat-0.1.7/setup.py
-drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-15 06:49:21.516125 krypper_tgstat-0.1.7/tests/
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)    37040 2024-04-15 06:44:32.000000 krypper_tgstat-0.1.7/tests/test_TGStatSync.py
+drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-18 13:27:28.328367 krypper_tgstat-0.1.7.1/
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)     1063 2024-04-15 06:40:20.000000 krypper_tgstat-0.1.7.1/LICENSE
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      957 2024-04-18 13:27:28.328367 krypper_tgstat-0.1.7.1/PKG-INFO
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      103 2024-04-15 06:40:20.000000 krypper_tgstat-0.1.7.1/README.md
+drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-18 13:27:28.327367 krypper_tgstat-0.1.7.1/krypper_tgstat/
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      244 2024-04-18 13:26:52.000000 krypper_tgstat-0.1.7.1/krypper_tgstat/__init__.py
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)    10375 2024-04-18 13:25:29.000000 krypper_tgstat-0.1.7.1/krypper_tgstat/classes.py
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)     2906 2024-04-18 13:20:59.000000 krypper_tgstat-0.1.7.1/krypper_tgstat/enums.py
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      666 2024-04-15 06:45:39.000000 krypper_tgstat-0.1.7.1/krypper_tgstat/exceptions.py
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)     8210 2024-04-15 06:47:48.000000 krypper_tgstat-0.1.7.1/krypper_tgstat/tg_stat.py
+drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-18 13:27:28.328367 krypper_tgstat-0.1.7.1/krypper_tgstat.egg-info/
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      957 2024-04-18 13:27:28.000000 krypper_tgstat-0.1.7.1/krypper_tgstat.egg-info/PKG-INFO
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      382 2024-04-18 13:27:28.000000 krypper_tgstat-0.1.7.1/krypper_tgstat.egg-info/SOURCES.txt
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)        1 2024-04-18 13:27:28.000000 krypper_tgstat-0.1.7.1/krypper_tgstat.egg-info/dependency_links.txt
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)       17 2024-04-18 13:27:28.000000 krypper_tgstat-0.1.7.1/krypper_tgstat.egg-info/requires.txt
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)       15 2024-04-18 13:27:28.000000 krypper_tgstat-0.1.7.1/krypper_tgstat.egg-info/top_level.txt
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)       38 2024-04-18 13:27:28.329367 krypper_tgstat-0.1.7.1/setup.cfg
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)     1289 2024-04-18 13:26:59.000000 krypper_tgstat-0.1.7.1/setup.py
+drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-18 13:27:28.328367 krypper_tgstat-0.1.7.1/tests/
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)    37040 2024-04-15 07:20:55.000000 krypper_tgstat-0.1.7.1/tests/test_TGStatSync.py
```

### Comparing `krypper_tgstat-0.1.7/LICENSE` & `krypper_tgstat-0.1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `krypper_tgstat-0.1.7/PKG-INFO` & `krypper_tgstat-0.1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krypper_tgstat
-Version: 0.1.7
+Version: 0.1.7.1
 Summary: Wrapper for TG Stat API writing on Python
 Home-page: https://github.com/KrymmyEM/krypper_tgstat
 Download-URL: https://github.com/KrymmyEM/krypper_tgstat/archive/main.zip
 Author: Evgeny Momotov (KrymmyEM)
 Author-email: evgeny.momotov@gmail.com
 License: MIT License. See LICENSE file
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `krypper_tgstat-0.1.7/krypper_tgstat/classes.py` & `krypper_tgstat-0.1.7.1/krypper_tgstat/classes.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 class Channel:
     def __init__(
             self, id, link, username,
             title, about, image100, image640, participants_count, peer_type=None, 
             active_usernames=None, tgstat_restrictions = None, tg_id = None,
-            category = None, country = None, language = None
+            category = None, country = None, language = None, **kwargs
         ):
         self.id = id
         self.tg_id = tg_id
         self.link = link
         self.peer_type = peer_type
         self.username = username
         self.active_usernames = active_usernames
@@ -19,25 +19,27 @@
         self.image100 = image100
         self.image640 = image640
         self.participants_count = participants_count
         self.tgstat_restrictions = tgstat_restrictions
         self.category = None
         self.country = None
         self.language = None
+        for key, value in kwargs.items():
+            setattr(self, key, value)
 
 
 
 class ChannelStatistic:
     def __init__(self, id, title, username, peer_type, participants_count,
                  avg_post_reach=None, adv_post_reach_12h=None, adv_post_reach_24h=None, adv_post_reach_48h=None,
                  err_percent=None, err24_percent=None, er_percent=None, daily_reach=None, ci_index=None,
                  mentions_count=None, forwards_count=None, mentioning_channels_count=None, posts_count=None,
                  dau=None, wau=None, mau=None, online_count_day_time=None, online_count_night_time=None,
                  messages_count_yesterday=None, messages_count_last_week=None, messages_count_last_month=None,
-                 messages_count_total=None):
+                 messages_count_total=None, **kwargs):
         self.id = id
         self.title = title
         self.username = username
         self.peer_type = peer_type
         self.participants_count = participants_count
         self.avg_post_reach = avg_post_reach
         self.adv_post_reach_12h = adv_post_reach_12h
@@ -57,87 +59,100 @@
         self.mau = mau
         self.online_count_day_time = online_count_day_time
         self.online_count_night_time = online_count_night_time
         self.messages_count_yesterday = messages_count_yesterday
         self.messages_count_last_week = messages_count_last_week
         self.messages_count_last_month = messages_count_last_month
         self.messages_count_total = messages_count_total
+        for key, value in kwargs.items():
+            setattr(self, key, value)
 
 
 class Media:
     def __init__(self, **kwargs):
         # kwargs содержит дополнительные аргументы, которые могут быть переданы
         for key, value in kwargs.items():
             setattr(self, key, value)
 
 
 class Story:
     def __init__(
         self, id, date, views, link,
         channel_id, is_expired, expire_at,
-        caption, media
+        caption, media, **kwargs
         ):
         self.id = id
         self.date = date
         self.views = views
         self.link = link
         self.channel_id = channel_id
         self.is_expired = is_expired
         self.expire_at = expire_at
         self.caption = caption
         self.media = None
         if media:
             self.media = Media(**media)
 
+        for key, value in kwargs.items():
+            setattr(self, key, value)
+
 
 class User:
     def __init__(
         self, id, tg_id, username, 
-        firstname, lastname
+        firstname, lastname, **kwargs
         ):
         self.id = id
         self.tg_id = tg_id
         self.username = username
         self.firstname = firstname
         self.lastname = lastname
+        for key, value in kwargs.items():
+            setattr(self, key, value)
 
 
 class Mention:
-    def __init__(self, mentionId, mentionType, postId, postLink, postDate, channelId = None):
+    def __init__(self, mentionId, mentionType, postId, postLink, postDate, channelId = None, **kwargs):
         self.mentionId = mentionId
         self.mentionType = mentionType
         self.postId = postId
         self.postLink = postLink
         self.postDate = postDate
         self.channelId = channelId
+        for key, value in kwargs.items():
+            setattr(self, key, value)
+
 
 
 class Forward:
-    def __init__(self, postId, postLink, channelId, peerType=None, postDate=None, forwardId=0, sourcePostId=0):
+    def __init__(self, postId, postLink, channelId, peerType=None, postDate=None, forwardId=0, sourcePostId=0, **kwargs):
         if forwardId:
             self.forwardId = forwardId
         
         if sourcePostId:
             self.sourcePostId = sourcePostId
 
         self.postId = postId
         self.postLink = postLink
         self.channelId = channelId
         self.peerType = peerType
         self.postDate = postDate
+        for key, value in kwargs.items():
+            setattr(self, key, value)
+
 
 
 class Post:
     def __init__(
             self, id = None, date = None, views = None, link = "",
             channel_id = None, forwarded_from = [], 
             user_id = None, is_deleted = False, deleted_at="", 
             group_id=None, text="", snippet="", media = [], shares_count= None,
             comments_count = None, reactions_count = None
-        ):
+        , **kwargs):
         self.id = id
         self.date = date
         self.views = views
         self.link = link
         self.channel_id = channel_id
         self.forwarded_from = None
         if forwarded_from:
@@ -151,57 +166,73 @@
         self.snippet = snippet
         self.media = None
         if media:
             self.media = Media(**media)
 
         self.shares_count = shares_count
         self.comments_count = comments_count
+        for key, value in kwargs.items():
+            setattr(self, key, value)
+
 
 
 class MentionChannel:
-    def __init__(self, channel_id, mentions_count, views_count, last_mention_date):
+    def __init__(self, channel_id, mentions_count, views_count, last_mention_date, **kwargs):
         self.channel_id = channel_id
         self.mentions_count = mentions_count
         self.views_count = views_count
         self.last_mention_date = last_mention_date
+        for key, value in kwargs.items():
+            setattr(self, key, value)
+
 
 
 class UnionStatistic:
-    def __init__(self, viewsCount, sharesCount, reactionsCount, commentsCount=0, postId=0, storyId=0):
+    def __init__(self, viewsCount, sharesCount, reactionsCount, commentsCount=0, postId=0, storyId=0, **kwargs):
         if postId:
             self.postId = postId
         if storyId:
             self.storyId = storyId
         self.viewsCount = viewsCount
         self.sharesCount = sharesCount
         self.commentsCount = commentsCount
         self.reactionsCount = reactionsCount
+        for key, value in kwargs.items():
+            setattr(self, key, value)
+
 
 
 class View:
-    def __init__(self, date, viewsGrowth):
+    def __init__(self, date, viewsGrowth, **kwargs):
         self.date = date
         self.viewsGrowth = viewsGrowth
+        for key, value in kwargs.items():
+            setattr(self, key, value)
+
 
 
 class GroupStatistic:
-    def __init__(self, viewsCount=None, sharesCount=None, commentsCount=None, reactionsCount=None, forwardsCount=None, mentionsCount=None, forwards=[], mentions=[], views=[]):
+    def __init__(self, viewsCount=None, sharesCount=None, commentsCount=None, reactionsCount=None, forwardsCount=None, mentionsCount=None, forwards=[], mentions=[], views=[], **kwargs):
         self.viewsCount = viewsCount
         self.sharesCount = sharesCount
         self.commentsCount = commentsCount
         self.reactionsCount = reactionsCount
         self.forwardsCount = forwardsCount
         self.mentionsCount = mentionsCount
         if forwards:
             self.forwards = [Forward(**fwd) for fwd in forwards]
         if mentions:
             self.mentions = [Mention(**mention) for mention in mentions]
         if views:
             self.views = [View(**view) for view in views]
 
+        for key, value in kwargs.items():
+            setattr(self, key, value)
+
+
 
 class CallbackNotify:
     def __init__(
         self, subscription_id,
         subscription_type, event_id,
         event_type, **kwargs
         ):
@@ -211,22 +242,25 @@
         self.event_type = event_type
         # kwargs содержит дополнительные аргументы, которые могут быть переданы
         for key, value in kwargs.items():
             setattr(self, key, value)
 
 
 class DatabaseEntity:
-    def __init__(self, database_type: DatabaseTypes, code=None, name=None):
+    def __init__(self, database_type: DatabaseTypes, code=None, name=None, **kwargs):
         self.database_type = database_type
         self.code = code
         self.name = name
+        for key, value in kwargs.items():
+            setattr(self, key, value)
+
 
 
 class MassiveResult:
-    def __init__(self, result_type: ResultsType, count = None, total_count = None, channel = None, items = None, channels = None):
+    def __init__(self, result_type: ResultsType, count = None, total_count = None, channel = None, items = None, channels = None, **kwargs):
         self.result_type = result_type
         if count:
             self.count = count
         if total_count:
             self.total_count = total_count
         if channel:
             self.channel = Channel(**channel)
@@ -248,14 +282,17 @@
                 self.items = [Forward(**fr) for fr in items]
             
             elif result_type == ResultsType.CHANNELS:
                 self.items = [Channel(**chan) for chan in items]
 
         if channels:
             self.channels = [Channel(**chan) for chan in channels]
+        for key, value in kwargs.items():
+            setattr(self, key, value)
+
 
 
 class DynamicData:
     def __init__(self, dynamic_type, period, **kwargs):
         self.dynamic_type = dynamic_type
         self.period = period
```

### Comparing `krypper_tgstat-0.1.7/krypper_tgstat/enums.py` & `krypper_tgstat-0.1.7.1/krypper_tgstat/enums.py`

 * *Files identical despite different names*

### Comparing `krypper_tgstat-0.1.7/krypper_tgstat/exceptions.py` & `krypper_tgstat-0.1.7.1/krypper_tgstat/exceptions.py`

 * *Files identical despite different names*

### Comparing `krypper_tgstat-0.1.7/krypper_tgstat/tg_stat.py` & `krypper_tgstat-0.1.7.1/krypper_tgstat/tg_stat.py`

 * *Files identical despite different names*

### Comparing `krypper_tgstat-0.1.7/krypper_tgstat.egg-info/PKG-INFO` & `krypper_tgstat-0.1.7.1/krypper_tgstat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krypper_tgstat
-Version: 0.1.7
+Version: 0.1.7.1
 Summary: Wrapper for TG Stat API writing on Python
 Home-page: https://github.com/KrymmyEM/krypper_tgstat
 Download-URL: https://github.com/KrymmyEM/krypper_tgstat/archive/main.zip
 Author: Evgeny Momotov (KrymmyEM)
 Author-email: evgeny.momotov@gmail.com
 License: MIT License. See LICENSE file
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `krypper_tgstat-0.1.7/setup.py` & `krypper_tgstat-0.1.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """
 :authors: Evgeny Momotov (KrymmyEM)
 :license: MIT License
 Copyright: (c) 2024 Evgeny
 """
 
-version = "0.1.7"
+version = "0.1.7.1"
 
 long_description = ""
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
```

### Comparing `krypper_tgstat-0.1.7/tests/test_TGStatSync.py` & `krypper_tgstat-0.1.7.1/tests/test_TGStatSync.py`

 * *Files identical despite different names*

