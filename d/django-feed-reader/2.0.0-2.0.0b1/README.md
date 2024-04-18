# Comparing `tmp/django_feed_reader-2.0.0.tar.gz` & `tmp/django-feed-reader-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_feed_reader-2.0.0.tar", last modified: Thu Apr 18 18:16:00 2024, max compression
+gzip compressed data, was "django-feed-reader-2.0.0b1.tar", last modified: Wed Feb 28 13:40:26 2024, max compression
```

## Comparing `django_feed_reader-2.0.0.tar` & `django-feed-reader-2.0.0b1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 g          (501) staff       (20)        0 2024-04-18 18:16:00.153053 django_feed_reader-2.0.0/
--rw-r--r--   0 g          (501) staff       (20)     1071 2023-01-28 17:47:47.000000 django_feed_reader-2.0.0/LICENSE
--rw-r--r--   0 g          (501) staff       (20)       87 2023-01-28 17:47:47.000000 django_feed_reader-2.0.0/MANIFEST.in
--rw-r--r--   0 g          (501) staff       (20)     5565 2024-04-18 18:16:00.152993 django_feed_reader-2.0.0/PKG-INFO
-drwxr-xr-x   0 g          (501) staff       (20)        0 2024-04-18 18:16:00.152617 django_feed_reader-2.0.0/django_feed_reader.egg-info/
--rw-r--r--   0 g          (501) staff       (20)     5565 2024-04-18 18:16:00.000000 django_feed_reader-2.0.0/django_feed_reader.egg-info/PKG-INFO
--rw-r--r--   0 g          (501) staff       (20)     1236 2024-04-18 18:16:00.000000 django_feed_reader-2.0.0/django_feed_reader.egg-info/SOURCES.txt
--rw-r--r--   0 g          (501) staff       (20)        1 2024-04-18 18:16:00.000000 django_feed_reader-2.0.0/django_feed_reader.egg-info/dependency_links.txt
--rw-r--r--   0 g          (501) staff       (20)       90 2024-04-18 18:16:00.000000 django_feed_reader-2.0.0/django_feed_reader.egg-info/requires.txt
--rw-r--r--   0 g          (501) staff       (20)        6 2024-04-18 18:16:00.000000 django_feed_reader-2.0.0/django_feed_reader.egg-info/top_level.txt
-drwxr-xr-x   0 g          (501) staff       (20)        0 2024-04-18 18:16:00.148610 django_feed_reader-2.0.0/feeds/
--rw-r--r--   0 g          (501) staff       (20)      442 2024-04-01 18:29:16.000000 django_feed_reader-2.0.0/feeds/__init__.py
--rw-r--r--   0 g          (501) staff       (20)     1528 2024-04-06 12:46:13.000000 django_feed_reader-2.0.0/feeds/admin.py
--rw-r--r--   0 g          (501) staff       (20)      139 2024-04-01 18:29:16.000000 django_feed_reader-2.0.0/feeds/apps.py
-drwxr-xr-x   0 g          (501) staff       (20)        0 2024-04-18 18:16:00.148829 django_feed_reader-2.0.0/feeds/management/
--rw-r--r--   0 g          (501) staff       (20)        1 2024-04-01 18:29:16.000000 django_feed_reader-2.0.0/feeds/management/__init__.py
-drwxr-xr-x   0 g          (501) staff       (20)        0 2024-04-18 18:16:00.149250 django_feed_reader-2.0.0/feeds/management/commands/
--rw-r--r--   0 g          (501) staff       (20)        1 2024-04-01 18:29:16.000000 django_feed_reader-2.0.0/feeds/management/commands/__init__.py
--rw-r--r--   0 g          (501) staff       (20)      415 2024-04-18 14:38:51.000000 django_feed_reader-2.0.0/feeds/management/commands/refreshfeeds.py
-drwxr-xr-x   0 g          (501) staff       (20)        0 2024-04-18 18:16:00.152485 django_feed_reader-2.0.0/feeds/migrations/
--rw-r--r--   0 g          (501) staff       (20)     3384 2024-04-05 14:54:09.000000 django_feed_reader-2.0.0/feeds/migrations/0001_initial.py
--rw-r--r--   0 g          (501) staff       (20)      395 2024-04-01 18:29:16.000000 django_feed_reader-2.0.0/feeds/migrations/0002_auto_20190604_0845.py
--rw-r--r--   0 g          (501) staff       (20)      407 2024-04-01 18:29:16.000000 django_feed_reader-2.0.0/feeds/migrations/0003_post_image_url.py
--rw-r--r--   0 g          (501) staff       (20)      513 2024-04-01 18:29:16.000000 django_feed_reader-2.0.0/feeds/migrations/0004_webproxy.py
--rw-r--r--   0 g          (501) staff       (20)      385 2024-04-01 18:29:16.000000 django_feed_reader-2.0.0/feeds/migrations/0005_source_description.py
--rw-r--r--   0 g          (501) staff       (20)      921 2024-04-05 14:50:09.000000 django_feed_reader-2.0.0/feeds/migrations/0006_auto_20190901_1644.py
--rw-r--r--   0 g          (501) staff       (20)     1098 2024-04-01 18:29:16.000000 django_feed_reader-2.0.0/feeds/migrations/0007_auto_20210502_0716.py
--rw-r--r--   0 g          (501) staff       (20)      419 2024-04-01 18:29:16.000000 django_feed_reader-2.0.0/feeds/migrations/0008_allow_longer_post_guid.py
--rw-r--r--   0 g          (501) staff       (20)      576 2024-04-01 18:29:16.000000 django_feed_reader-2.0.0/feeds/migrations/0009_allow_source_last_change_and_last_success_to_be_blank.py
--rw-r--r--   0 g          (501) staff       (20)      626 2024-04-01 18:29:16.000000 django_feed_reader-2.0.0/feeds/migrations/0010_enclosure_description_enclosure_medium.py
--rw-r--r--   0 g          (501) staff       (20)      439 2024-04-01 18:29:16.000000 django_feed_reader-2.0.0/feeds/migrations/0011_alter_post_guid.py
--rw-r--r--   0 g          (501) staff       (20)     1383 2024-04-01 18:29:16.000000 django_feed_reader-2.0.0/feeds/migrations/0012_source_last_read_subscription.py
--rw-r--r--   0 g          (501) staff       (20)      474 2024-02-24 22:48:14.000000 django_feed_reader-2.0.0/feeds/migrations/0013_delete_webproxy_enclosure_is_current.py
--rw-r--r--   0 g          (501) staff       (20)      561 2024-02-25 01:08:43.000000 django_feed_reader-2.0.0/feeds/migrations/0014_post_json_source_json.py
--rw-r--r--   0 g          (501) staff       (20)      393 2024-04-04 06:54:09.000000 django_feed_reader-2.0.0/feeds/migrations/0015_source_alt_url.py
--rw-r--r--   0 g          (501) staff       (20)        0 2024-04-01 18:29:16.000000 django_feed_reader-2.0.0/feeds/migrations/__init__.py
--rw-r--r--   0 g          (501) staff       (20)    17419 2024-04-18 14:31:54.000000 django_feed_reader-2.0.0/feeds/models.py
--rw-r--r--   0 g          (501) staff       (20)    34044 2024-04-18 14:24:50.000000 django_feed_reader-2.0.0/feeds/tests.py
--rw-r--r--   0 g          (501) staff       (20)    13919 2024-04-13 19:20:22.000000 django_feed_reader-2.0.0/feeds/utils.py
--rw-r--r--   0 g          (501) staff       (20)    20969 2024-04-13 19:20:22.000000 django_feed_reader-2.0.0/feeds/utils_internal.py
--rw-r--r--   0 g          (501) staff       (20)       63 2024-04-01 18:29:16.000000 django_feed_reader-2.0.0/feeds/views.py
--rw-r--r--   0 g          (501) staff       (20)       38 2024-04-18 18:16:00.153223 django_feed_reader-2.0.0/setup.cfg
--rw-r--r--   0 g          (501) staff       (20)      896 2024-04-18 18:15:56.000000 django_feed_reader-2.0.0/setup.py
+drwxr-xr-x   0 g          (501) staff       (20)        0 2024-02-28 13:40:26.605566 django-feed-reader-2.0.0b1/
+-rw-r--r--   0 g          (501) staff       (20)     1071 2023-01-28 17:47:47.000000 django-feed-reader-2.0.0b1/LICENSE
+-rw-r--r--   0 g          (501) staff       (20)       87 2023-01-28 17:47:47.000000 django-feed-reader-2.0.0b1/MANIFEST.in
+-rw-r--r--   0 g          (501) staff       (20)     4757 2024-02-28 13:40:26.605505 django-feed-reader-2.0.0b1/PKG-INFO
+-rw-r--r--   0 g          (501) staff       (20)     4152 2024-02-25 20:00:43.000000 django-feed-reader-2.0.0b1/README.md
+drwxr-xr-x   0 g          (501) staff       (20)        0 2024-02-28 13:40:26.605263 django-feed-reader-2.0.0b1/django_feed_reader.egg-info/
+-rw-r--r--   0 g          (501) staff       (20)     4757 2024-02-28 13:40:26.000000 django-feed-reader-2.0.0b1/django_feed_reader.egg-info/PKG-INFO
+-rw-r--r--   0 g          (501) staff       (20)     1202 2024-02-28 13:40:26.000000 django-feed-reader-2.0.0b1/django_feed_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 g          (501) staff       (20)        1 2024-02-28 13:40:26.000000 django-feed-reader-2.0.0b1/django_feed_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 g          (501) staff       (20)       74 2024-02-28 13:40:26.000000 django-feed-reader-2.0.0b1/django_feed_reader.egg-info/requires.txt
+-rw-r--r--   0 g          (501) staff       (20)        6 2024-02-28 13:40:26.000000 django-feed-reader-2.0.0b1/django_feed_reader.egg-info/top_level.txt
+drwxr-xr-x   0 g          (501) staff       (20)        0 2024-02-28 13:40:26.601413 django-feed-reader-2.0.0b1/feeds/
+-rw-r--r--   0 g          (501) staff       (20)      442 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/__init__.py
+-rw-r--r--   0 g          (501) staff       (20)     1528 2024-02-24 14:36:21.000000 django-feed-reader-2.0.0b1/feeds/admin.py
+-rw-r--r--   0 g          (501) staff       (20)      139 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/apps.py
+-rw-r--r--   0 g          (501) staff       (20)       17 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/cloudflare.py
+drwxr-xr-x   0 g          (501) staff       (20)        0 2024-02-28 13:40:26.601559 django-feed-reader-2.0.0b1/feeds/management/
+-rw-r--r--   0 g          (501) staff       (20)        1 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/management/__init__.py
+drwxr-xr-x   0 g          (501) staff       (20)        0 2024-02-28 13:40:26.601837 django-feed-reader-2.0.0b1/feeds/management/commands/
+-rw-r--r--   0 g          (501) staff       (20)        1 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/management/commands/__init__.py
+-rw-r--r--   0 g          (501) staff       (20)      298 2024-02-24 14:37:34.000000 django-feed-reader-2.0.0b1/feeds/management/commands/refreshfeeds.py
+drwxr-xr-x   0 g          (501) staff       (20)        0 2024-02-28 13:40:26.605117 django-feed-reader-2.0.0b1/feeds/migrations/
+-rw-r--r--   0 g          (501) staff       (20)     3384 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/migrations/0001_initial.py
+-rw-r--r--   0 g          (501) staff       (20)      395 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/migrations/0002_auto_20190604_0845.py
+-rw-r--r--   0 g          (501) staff       (20)      407 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/migrations/0003_post_image_url.py
+-rw-r--r--   0 g          (501) staff       (20)      513 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/migrations/0004_webproxy.py
+-rw-r--r--   0 g          (501) staff       (20)      385 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/migrations/0005_source_description.py
+-rw-r--r--   0 g          (501) staff       (20)      921 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/migrations/0006_auto_20190901_1644.py
+-rw-r--r--   0 g          (501) staff       (20)     1098 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/migrations/0007_auto_20210502_0716.py
+-rw-r--r--   0 g          (501) staff       (20)      419 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/migrations/0008_allow_longer_post_guid.py
+-rw-r--r--   0 g          (501) staff       (20)      576 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/migrations/0009_allow_source_last_change_and_last_success_to_be_blank.py
+-rw-r--r--   0 g          (501) staff       (20)      626 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/migrations/0010_enclosure_description_enclosure_medium.py
+-rw-r--r--   0 g          (501) staff       (20)      439 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/migrations/0011_alter_post_guid.py
+-rw-r--r--   0 g          (501) staff       (20)     1383 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/migrations/0012_source_last_read_subscription.py
+-rw-r--r--   0 g          (501) staff       (20)      474 2024-02-24 22:48:14.000000 django-feed-reader-2.0.0b1/feeds/migrations/0013_delete_webproxy_enclosure_is_current.py
+-rw-r--r--   0 g          (501) staff       (20)      561 2024-02-25 01:08:43.000000 django-feed-reader-2.0.0b1/feeds/migrations/0014_post_json_source_json.py
+-rw-r--r--   0 g          (501) staff       (20)        0 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/migrations/__init__.py
+-rw-r--r--   0 g          (501) staff       (20)     8560 2024-02-25 01:43:17.000000 django-feed-reader-2.0.0b1/feeds/models.py
+-rw-r--r--   0 g          (501) staff       (20)    27558 2024-02-25 01:41:59.000000 django-feed-reader-2.0.0b1/feeds/tests.py
+-rw-r--r--   0 g          (501) staff       (20)    32167 2024-02-25 01:12:25.000000 django-feed-reader-2.0.0b1/feeds/utils.py
+-rw-r--r--   0 g          (501) staff       (20)       63 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/views.py
+-rw-r--r--   0 g          (501) staff       (20)       38 2024-02-28 13:40:26.605732 django-feed-reader-2.0.0b1/setup.cfg
+-rw-r--r--   0 g          (501) staff       (20)      875 2024-02-28 13:34:16.000000 django-feed-reader-2.0.0b1/setup.py
```

### Comparing `django_feed_reader-2.0.0/LICENSE` & `django-feed-reader-2.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_feed_reader-2.0.0/PKG-INFO` & `django-feed-reader-2.0.0b1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,150 +1,116 @@
 Metadata-Version: 2.1
 Name: django-feed-reader
-Version: 2.0.0
+Version: 2.0.0b1
 Summary: An RSS feed reading library for Django.
 Home-page: https://github.com/xurble/django-feed-reader
 Author: Gareth Simpson
 Author-email: g@xurble.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dripfeed-client
 Requires-Dist: sgmllib3k
 Requires-Dist: requests
 Requires-Dist: feedparser>=6.0.0
 Requires-Dist: beautifulsoup4
 Requires-Dist: pyrfc3339
 Requires-Dist: Django>=2.2
 
-Django Feed Reader
-==================
+
+# Django Feed Reader
 
 This is a simple Django module to allow you subscribe to RSS (and other) feeds.
 
 This app has no UI, it just reads and stores the feeds for you to use as you see fit.
 
 This app builds on top of the FeedParser library to provide feed management, storage, scheduling etc.
 
-Features
---------
+## Features
 
 * Consumes RSS, Atom and JSONFeed feeds.
 * Parses feeds liberally to try and accomodate simple errors.
 * Will attempt to bypass Cloudflare protection of feeds
 * Supports enclosure (podcast) discovery
 * Automatic feed scheduling based on frequency of updates
 
 
-Installation
-------------
+## Installation
+
+`django-feed-reader` is written in Python 3 and supports Django 2.2+
 
-``django-feed-reader`` is written in Python 3 and supports Django 2.2+
+1. `pip install django-feed-reader`
+2. Add `feeds` to your `INSTALLED_APPS`
+3. Setup some values in `settings.py` so that your feed reader politely announces itself to servers:
+   * Set `FEEDS_USER_AGENT` to the name and (optionally version) of your service e.g. `"ExampleFeeder/1.2"`
+   * Set `FEEDS_SERVER` to preferred web address of your service so that feed hosts can locate you if required e.g. `https://example.com`
+4. Setup a mechanism to periodically refresh the feeds (see below)
 
-- ``pip install django-feed-reader``
-- Add ``feeds`` to your ``INSTALLED_APPS``
-- Setup some values in ``settings.py`` so that your feed reader politely announces itself to servers
-   - Set ``FEEDS_USER_AGENT`` to the name and (optionally version) of your service e.g. ``"ExampleFeeder/1.2"``
-   - Set ``FEEDS_SERVER`` to preferred web address of your service so that feed hosts can locate you if required e.g. ``https://example.com``
-- Setup a mechanism to periodically refresh the feeds (see below)
+## Basic Models
 
-Basic Models
-------------
+A feed is represented by a `Source` object which has (among other things) a `feed_url`.
 
-A feed is represented by a ``Source`` object which has (among other things) a ``feed_url``.
+`Source`s have `Posts` which contain the content.
 
-To start reading a feed, simply create a new ``Source`` with the desired ``feed_url``
+`Posts` may have `Enclosure`s which is what podcasts use to send their audio.  The app does not download enclosures, if you want to do that you will need to it in your project using the url provided.
 
-``Source`` objects have ``Post`` children  which contain the content.
+If your system supports multiple users, each user will have a `Subscription` to a `Source`.
 
-A ``Post`` may have ``Enclosure`` (or more) which is what podcasts use to send their audio.
-The app does not download enclosures, if you want to do that you will need to do that in your project
-using the url provided.
+A full description of the models and their fields is coming soon (probably).  In the mean  time, why not read `models.py`, it's all obvious stuff.
 
 
-Refreshing feeds
-----------------
+## Refreshing feeds
 
-To conserve resources with large feed lists, the module will adjust how often it polls feeds
-based on how often they are updated.  The fastest it will poll a feed is every hour. The
-slowest it will poll is every 24 hours.
+To conserve resources with large feed lists, the app will adjust how often it polls feeds based on how often they are updated.  The fastest it will poll a feed is every hour. The slowest it will poll is every 24 hours.
 
-Sources that don't get updated are polled progressively more slowly until the 24 hour limit is
-reached.  When a feed changes, its polling frequency increases.
+Feeds that don't get updated are polled progressively more slowly until the 24 hour limit is reached.  When a feed changes, its polling frequency increases.
 
-You will need to decided how and when to run the poller.  When the poller runs, it checks all
-feeds that are currently due.  The ideal frequency to run it is every 5 - 10 minutes.
+You will need to decided how and when to run the poller.  When the poller runs, it checks all feeds that are currently due.  The ideal frequency to run it is every 5 - 10 minutes.
 
-Polling with cron
------------------
+### Polling with cron.
 
-Set up a job that calls ``python manage.py refreshfeeds`` on your desired schedule.
+Set up a job that calls `python manage.py refreshfeeds` on your desired schedule.
 
 Be careful to ensure you're running out of the correct directory and with the correct python environment.
 
-Polling with celery
--------------------
+### Polling with celery
 
-Create a new celery task and schedule in your app (see the celery documentation for details).  Your ``tasks.py`` should look something like this:
+Create a new celery task and schedule in your app (see the celery documentation for details).  Your `tasks.py` should look something like this:
 
-::
+```python
 
-  from celery import shared_task
-  from feeds.utils import update_feeds
+from celery import shared_task
+from feeds.utils import update_feeds
 
-  @shared_task
-  def get_those_feeds():
+@shared_task
+def get_those_feeds():
 
     # the number is the max number of feeds to poll in one go
     update_feeds(30)
 
+```
 
-Tracking read/unread state of feeds
------------------------------------
-
-There are two ways to track the read/unread state of feeds depending on your needs.
-
+## Tracking subscribers and read/unread state of feeds
 
-Single User Installations
-^^^^^^^^^^^^^^^^^^^^^^^^^
+The app does not (currently) track the read/unread state of posts within a feed.  That will need doing in your project according to your needs.
 
-If your usage is just for a single user, then there are helper methods on a Source
-to track your read state.
+The app assumes that each feed only has one subscriber that is the project itself.  If your project can allow personal subscriptions for individual users, you can let the app know on per feed basis how many subscribers it has by settings `num_subs` on a `Source` object.
+The app will then report this via the user agent to the feed source for analytics purposes.
 
-All posts come in unread.  You can get the current number of unread posts from
-``Source.unread_count``.
 
-To get a ResultSet of all the unread posts from a feed call ``Source.get_unread_posts``
+### Dealing with Cloudflare
 
-To mark all posts on a fed as read call ``Source.mark_read``
+Depending on where you run your server, you may run into problems with Cloudflare's web captcha.  Plenty of sites out there set up their Cloudflare to have default security on their RSS feed and this can block server-side RSS readers.
 
-To get all of the posts in a feed regardless of read status, a page at a time call
-``Source.get_paginated_posts`` which returns a tuple of (Posts, Paginator)
+It's a huge pain and affects lots of self-hosted RSS readers. Seriously, Google it.
 
-Multi-User Installations
-^^^^^^^^^^^^^^^^^^^^^^^^
-To allow multiple users to follow the same feed with individual read/unread status,
-create a new ``Subscription`` for that Source and User.
+`django-feed-reader` will do it's utmost to get these feeds anyway through the judicious use of public proxy servers, but is haphazard and you cannot rely on the scheduling of such feeds.
 
-Subscription has the same helper methods for retrieving posts and marking read as
-Source.
+Feeds blocked by Cloudflare will have the `is_cloudflare` flag set on their `Source` and will update on a best-efforts basis.
 
-You can also arrange feeds into a folder-like hierarchy using Subscriptions.
-Every Subscription has an optional ``parent``.  Subscriptions with a ``None`` parent
-are considered at the root level.  By convention, Subscriptions that are acting as parent
-folders should have a ``None`` ``source``
 
-Subscriptions have a ``name`` field which by convention should be a display name if it is
-a folder or the name of the Source it is tracking.  However this can be set to any
-value if you want to give a personally-meaningful name to a feed who's name is cryptic.
 
-There are two helper methods in the ``utils`` module to help manage subscriptions as folders.
-``get_subscription_list_for_user`` will return all Subscriptions for a User where the
-parent is None.  ``get_unread_subscription_list_for_user`` will do the same but only returns
-Subscriptions that are unread or that have unread children if they are a folder.
 
 
 
-For more details see the `full documentation <https//django-feed-reader.readthedocs.io>`_.
```

### Comparing `django_feed_reader-2.0.0/django_feed_reader.egg-info/PKG-INFO` & `django-feed-reader-2.0.0b1/django_feed_reader.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,150 +1,116 @@
 Metadata-Version: 2.1
 Name: django-feed-reader
-Version: 2.0.0
+Version: 2.0.0b1
 Summary: An RSS feed reading library for Django.
 Home-page: https://github.com/xurble/django-feed-reader
 Author: Gareth Simpson
 Author-email: g@xurble.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dripfeed-client
 Requires-Dist: sgmllib3k
 Requires-Dist: requests
 Requires-Dist: feedparser>=6.0.0
 Requires-Dist: beautifulsoup4
 Requires-Dist: pyrfc3339
 Requires-Dist: Django>=2.2
 
-Django Feed Reader
-==================
+
+# Django Feed Reader
 
 This is a simple Django module to allow you subscribe to RSS (and other) feeds.
 
 This app has no UI, it just reads and stores the feeds for you to use as you see fit.
 
 This app builds on top of the FeedParser library to provide feed management, storage, scheduling etc.
 
-Features
---------
+## Features
 
 * Consumes RSS, Atom and JSONFeed feeds.
 * Parses feeds liberally to try and accomodate simple errors.
 * Will attempt to bypass Cloudflare protection of feeds
 * Supports enclosure (podcast) discovery
 * Automatic feed scheduling based on frequency of updates
 
 
-Installation
-------------
+## Installation
+
+`django-feed-reader` is written in Python 3 and supports Django 2.2+
 
-``django-feed-reader`` is written in Python 3 and supports Django 2.2+
+1. `pip install django-feed-reader`
+2. Add `feeds` to your `INSTALLED_APPS`
+3. Setup some values in `settings.py` so that your feed reader politely announces itself to servers:
+   * Set `FEEDS_USER_AGENT` to the name and (optionally version) of your service e.g. `"ExampleFeeder/1.2"`
+   * Set `FEEDS_SERVER` to preferred web address of your service so that feed hosts can locate you if required e.g. `https://example.com`
+4. Setup a mechanism to periodically refresh the feeds (see below)
 
-- ``pip install django-feed-reader``
-- Add ``feeds`` to your ``INSTALLED_APPS``
-- Setup some values in ``settings.py`` so that your feed reader politely announces itself to servers
-   - Set ``FEEDS_USER_AGENT`` to the name and (optionally version) of your service e.g. ``"ExampleFeeder/1.2"``
-   - Set ``FEEDS_SERVER`` to preferred web address of your service so that feed hosts can locate you if required e.g. ``https://example.com``
-- Setup a mechanism to periodically refresh the feeds (see below)
+## Basic Models
 
-Basic Models
-------------
+A feed is represented by a `Source` object which has (among other things) a `feed_url`.
 
-A feed is represented by a ``Source`` object which has (among other things) a ``feed_url``.
+`Source`s have `Posts` which contain the content.
 
-To start reading a feed, simply create a new ``Source`` with the desired ``feed_url``
+`Posts` may have `Enclosure`s which is what podcasts use to send their audio.  The app does not download enclosures, if you want to do that you will need to it in your project using the url provided.
 
-``Source`` objects have ``Post`` children  which contain the content.
+If your system supports multiple users, each user will have a `Subscription` to a `Source`.
 
-A ``Post`` may have ``Enclosure`` (or more) which is what podcasts use to send their audio.
-The app does not download enclosures, if you want to do that you will need to do that in your project
-using the url provided.
+A full description of the models and their fields is coming soon (probably).  In the mean  time, why not read `models.py`, it's all obvious stuff.
 
 
-Refreshing feeds
-----------------
+## Refreshing feeds
 
-To conserve resources with large feed lists, the module will adjust how often it polls feeds
-based on how often they are updated.  The fastest it will poll a feed is every hour. The
-slowest it will poll is every 24 hours.
+To conserve resources with large feed lists, the app will adjust how often it polls feeds based on how often they are updated.  The fastest it will poll a feed is every hour. The slowest it will poll is every 24 hours.
 
-Sources that don't get updated are polled progressively more slowly until the 24 hour limit is
-reached.  When a feed changes, its polling frequency increases.
+Feeds that don't get updated are polled progressively more slowly until the 24 hour limit is reached.  When a feed changes, its polling frequency increases.
 
-You will need to decided how and when to run the poller.  When the poller runs, it checks all
-feeds that are currently due.  The ideal frequency to run it is every 5 - 10 minutes.
+You will need to decided how and when to run the poller.  When the poller runs, it checks all feeds that are currently due.  The ideal frequency to run it is every 5 - 10 minutes.
 
-Polling with cron
------------------
+### Polling with cron.
 
-Set up a job that calls ``python manage.py refreshfeeds`` on your desired schedule.
+Set up a job that calls `python manage.py refreshfeeds` on your desired schedule.
 
 Be careful to ensure you're running out of the correct directory and with the correct python environment.
 
-Polling with celery
--------------------
+### Polling with celery
 
-Create a new celery task and schedule in your app (see the celery documentation for details).  Your ``tasks.py`` should look something like this:
+Create a new celery task and schedule in your app (see the celery documentation for details).  Your `tasks.py` should look something like this:
 
-::
+```python
 
-  from celery import shared_task
-  from feeds.utils import update_feeds
+from celery import shared_task
+from feeds.utils import update_feeds
 
-  @shared_task
-  def get_those_feeds():
+@shared_task
+def get_those_feeds():
 
     # the number is the max number of feeds to poll in one go
     update_feeds(30)
 
+```
 
-Tracking read/unread state of feeds
------------------------------------
-
-There are two ways to track the read/unread state of feeds depending on your needs.
-
+## Tracking subscribers and read/unread state of feeds
 
-Single User Installations
-^^^^^^^^^^^^^^^^^^^^^^^^^
+The app does not (currently) track the read/unread state of posts within a feed.  That will need doing in your project according to your needs.
 
-If your usage is just for a single user, then there are helper methods on a Source
-to track your read state.
+The app assumes that each feed only has one subscriber that is the project itself.  If your project can allow personal subscriptions for individual users, you can let the app know on per feed basis how many subscribers it has by settings `num_subs` on a `Source` object.
+The app will then report this via the user agent to the feed source for analytics purposes.
 
-All posts come in unread.  You can get the current number of unread posts from
-``Source.unread_count``.
 
-To get a ResultSet of all the unread posts from a feed call ``Source.get_unread_posts``
+### Dealing with Cloudflare
 
-To mark all posts on a fed as read call ``Source.mark_read``
+Depending on where you run your server, you may run into problems with Cloudflare's web captcha.  Plenty of sites out there set up their Cloudflare to have default security on their RSS feed and this can block server-side RSS readers.
 
-To get all of the posts in a feed regardless of read status, a page at a time call
-``Source.get_paginated_posts`` which returns a tuple of (Posts, Paginator)
+It's a huge pain and affects lots of self-hosted RSS readers. Seriously, Google it.
 
-Multi-User Installations
-^^^^^^^^^^^^^^^^^^^^^^^^
-To allow multiple users to follow the same feed with individual read/unread status,
-create a new ``Subscription`` for that Source and User.
+`django-feed-reader` will do it's utmost to get these feeds anyway through the judicious use of public proxy servers, but is haphazard and you cannot rely on the scheduling of such feeds.
 
-Subscription has the same helper methods for retrieving posts and marking read as
-Source.
+Feeds blocked by Cloudflare will have the `is_cloudflare` flag set on their `Source` and will update on a best-efforts basis.
 
-You can also arrange feeds into a folder-like hierarchy using Subscriptions.
-Every Subscription has an optional ``parent``.  Subscriptions with a ``None`` parent
-are considered at the root level.  By convention, Subscriptions that are acting as parent
-folders should have a ``None`` ``source``
 
-Subscriptions have a ``name`` field which by convention should be a display name if it is
-a folder or the name of the Source it is tracking.  However this can be set to any
-value if you want to give a personally-meaningful name to a feed who's name is cryptic.
 
-There are two helper methods in the ``utils`` module to help manage subscriptions as folders.
-``get_subscription_list_for_user`` will return all Subscriptions for a User where the
-parent is None.  ``get_unread_subscription_list_for_user`` will do the same but only returns
-Subscriptions that are unread or that have unread children if they are a folder.
 
 
 
-For more details see the `full documentation <https//django-feed-reader.readthedocs.io>`_.
```

### Comparing `django_feed_reader-2.0.0/django_feed_reader.egg-info/SOURCES.txt` & `django-feed-reader-2.0.0b1/django_feed_reader.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 LICENSE
 MANIFEST.in
+README.md
 setup.cfg
 setup.py
 django_feed_reader.egg-info/PKG-INFO
 django_feed_reader.egg-info/SOURCES.txt
 django_feed_reader.egg-info/dependency_links.txt
 django_feed_reader.egg-info/requires.txt
 django_feed_reader.egg-info/top_level.txt
 feeds/__init__.py
 feeds/admin.py
 feeds/apps.py
+feeds/cloudflare.py
 feeds/models.py
 feeds/tests.py
 feeds/utils.py
-feeds/utils_internal.py
 feeds/views.py
 feeds/management/__init__.py
 feeds/management/commands/__init__.py
 feeds/management/commands/refreshfeeds.py
 feeds/migrations/0001_initial.py
 feeds/migrations/0002_auto_20190604_0845.py
 feeds/migrations/0003_post_image_url.py
@@ -28,9 +29,8 @@
 feeds/migrations/0008_allow_longer_post_guid.py
 feeds/migrations/0009_allow_source_last_change_and_last_success_to_be_blank.py
 feeds/migrations/0010_enclosure_description_enclosure_medium.py
 feeds/migrations/0011_alter_post_guid.py
 feeds/migrations/0012_source_last_read_subscription.py
 feeds/migrations/0013_delete_webproxy_enclosure_is_current.py
 feeds/migrations/0014_post_json_source_json.py
-feeds/migrations/0015_source_alt_url.py
 feeds/migrations/__init__.py
```

### Comparing `django_feed_reader-2.0.0/feeds/admin.py` & `django-feed-reader-2.0.0b1/feeds/admin.py`

 * *Files identical despite different names*

### Comparing `django_feed_reader-2.0.0/feeds/migrations/0001_initial.py` & `django-feed-reader-2.0.0b1/feeds/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_feed_reader-2.0.0/feeds/migrations/0004_webproxy.py` & `django-feed-reader-2.0.0b1/feeds/migrations/0004_webproxy.py`

 * *Files identical despite different names*

### Comparing `django_feed_reader-2.0.0/feeds/migrations/0006_auto_20190901_1644.py` & `django-feed-reader-2.0.0b1/feeds/migrations/0006_auto_20190901_1644.py`

 * *Files identical despite different names*

### Comparing `django_feed_reader-2.0.0/feeds/migrations/0007_auto_20210502_0716.py` & `django-feed-reader-2.0.0b1/feeds/migrations/0007_auto_20210502_0716.py`

 * *Files identical despite different names*

### Comparing `django_feed_reader-2.0.0/feeds/migrations/0009_allow_source_last_change_and_last_success_to_be_blank.py` & `django-feed-reader-2.0.0b1/feeds/migrations/0009_allow_source_last_change_and_last_success_to_be_blank.py`

 * *Files identical despite different names*

### Comparing `django_feed_reader-2.0.0/feeds/migrations/0010_enclosure_description_enclosure_medium.py` & `django-feed-reader-2.0.0b1/feeds/migrations/0010_enclosure_description_enclosure_medium.py`

 * *Files identical despite different names*

### Comparing `django_feed_reader-2.0.0/feeds/migrations/0012_source_last_read_subscription.py` & `django-feed-reader-2.0.0b1/feeds/migrations/0012_source_last_read_subscription.py`

 * *Files identical despite different names*

### Comparing `django_feed_reader-2.0.0/feeds/migrations/0014_post_json_source_json.py` & `django-feed-reader-2.0.0b1/feeds/migrations/0014_post_json_source_json.py`

 * *Files identical despite different names*

### Comparing `django_feed_reader-2.0.0/feeds/tests.py` & `django-feed-reader-2.0.0b1/feeds/tests.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,36 @@
-
-from datetime import timedelta
-from importlib import reload
-import os
-
-from django.conf import settings
-from django.contrib.auth import get_user_model
 from django.test import TestCase, TransactionTestCase
-from django.utils import timezone
-import requests_mock
-
+from django.conf import settings
 
 # Create your tests here.
-from feeds.models import Source, Subscription, Post
-from feeds.utils_internal import (
-    fix_relative,
-    hash_body,
-)
+from feeds.models import Source, Subscription
 from feeds.utils import (
     read_feed,
+    fix_relative,
+    hash_body,
     get_subscription_list_for_user,
     get_unread_subscription_list_for_user
 )
 
 from feeds import utils
-from feeds import utils_internal
+from importlib import reload
 
+from django.contrib.auth import get_user_model
+from django.utils import timezone
 
-User = get_user_model()
+from datetime import timedelta
 
-TEST_FILES_FOLDER = os.path.join(os.path.dirname(os.path.abspath(__file__)), "testdata")
-BASE_URL = 'http://feed.com/'
+import os
 
+import requests_mock
 
-class NullOutput(object):
+User = get_user_model()
 
-    # little class to stop the tests filling the console window
-    def write(self, strin: str):
-        pass
+TEST_FILES_FOLDER = os.path.join(os.path.dirname(os.path.abspath(__file__)), "testdata")
+BASE_URL = 'http://feed.com/'
 
 
 class UtilsTest(TestCase):
 
     def test_fix_relative(self):
 
         url = "https://example.com/rss.xml"
@@ -58,16 +48,17 @@
         content = open(os.path.join(TEST_FILES_FOLDER, test_file), "rb").read()
 
         ret_headers = {"Content-Type": content_type, "etag": "an-etag"}
         if headers is not None:
             ret_headers = {**ret_headers, **headers}
 
         if is_cloudflare:
-            ret_headers["Server"] = "Some cloudflare thing"
-            mock.register_uri('GET', url, status_code=status, content=content, headers=ret_headers)
+            agent = "{user_agent} (+{server}; Updater; {subs} subscribers)".format(user_agent=settings.FEEDS_USER_AGENT, server=settings.FEEDS_SERVER, subs=1)
+
+            mock.register_uri('GET', url, request_headers={"User-Agent": agent}, status_code=status, content=content, headers=ret_headers)
         else:
             if etag is None:
                 mock.register_uri('GET', url, status_code=status, content=content, headers=ret_headers)
             else:
                 mock.register_uri('GET', url, request_headers={'If-None-Match': etag}, status_code=status, content=content, headers=ret_headers)
 
 
@@ -79,29 +70,25 @@
         self._populate_mock(mock, status=200, test_file="rss_xhtml_body.xml", content_type="application/rss+xml")
 
         ls = timezone.now()
         src = Source(name="test1", feed_url=BASE_URL, interval=0, last_success=ls, last_change=ls)
         src.save()
 
         # Read the feed once to get the 1 post  and the etag
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
         self.assertEqual(src.unread_count, 1)
 
-        self.assertEqual(len(src.get_unread_posts()), 1)
-
         src.mark_read()
 
         src.refresh_from_db()
 
         self.assertEqual(src.unread_count, 0)
 
-        self.assertEqual(len(src.get_unread_posts()), 0)
-
     def test_subscriber_count(self, mock):
 
         ls = timezone.now()
         src = Source(name="test1", feed_url=BASE_URL, interval=0, last_success=ls, last_change=ls)
         src.save()
         src.refresh_from_db()
         # If we don't use Subscriptions then the default is 1
@@ -140,15 +127,15 @@
         ls = timezone.now()
         src = Source(name="test1", feed_url=BASE_URL, interval=0, last_success=ls, last_change=ls)
         src.save()
 
         user = User(email='x@example.com')
         user.save()
 
-        read_feed(src, output=NullOutput())
+        read_feed(src)
 
         sub = Subscription(user=user, source=src)
         sub.save()
         sub.refresh_from_db()
 
         self.assertEqual(src.unread_count, 1)
 
@@ -205,157 +192,116 @@
         all_subs_and_folder = Subscription.objects.filter(user=user).count()
 
         sub_list = get_subscription_list_for_user(user)
 
         self.assertEqual(all_subs_and_folder, 11)
         self.assertEqual(len(sub_list), 6)
 
-    def test_basic_subscription_read(self, mock):
+    def test_basic_subscription_unread_counts(self, mock):
 
         user = User(email='x@example.com')
         user.save()
 
         for i in range(5):
             ls = timezone.now()
             src = Source(name="test{i}".format(i=i), feed_url=BASE_URL, interval=0, last_success=ls, last_change=ls)
             src.max_index = 1
-            src.last_read
             src.save()
 
             sub = Subscription(user=user, source=src)
             sub.save()
 
         folder = Subscription(user=user, source=None, name="Folder")
         folder.save()
 
         for i in range(5):
             ls = timezone.now()
             src = Source(name="folder_test{i}".format(i=i), feed_url=BASE_URL, interval=0, last_success=ls, last_change=ls)
             src.max_index = 1
             src.save()
 
-            # make the posts get created earlier as they increase in index to check the ordering below
-            p = Post(source=src, title=f"post{i}", created=timezone.now() - timedelta(days=i), index=1, guid=f"src-{src.id}-post-{i}")
-            p.save()
-
             sub = Subscription(user=user, source=src, parent=folder)
-            src.last_read = 0
             sub.save()
 
         all_subs_and_folder = Subscription.objects.filter(user=user).count()
 
         sub_list = get_unread_subscription_list_for_user(user)
 
         self.assertEqual(all_subs_and_folder, 11)
         self.assertEqual(len(sub_list), 6)
 
         for s in sub_list:
             if s.source is None:
                 self.assertEqual(s.unread_count, 5)
 
-                self.assertEqual(len(s.get_unread_posts()), 5)
-
-                i = 5
-                for p in s.get_unread_posts():
-                    i -= 1
-                    self.assertEqual(p.title, f"post{i}")
-
-    def test_nested_subscription_read(self, mock):
+    def test_nested_subscription_unread_counts(self, mock):
 
         user = User(email='x@example.com')
         user.save()
 
-        pcount = 0
-
         for i in range(3):
             ls = timezone.now()
             src = Source(name="test{i}".format(i=i), feed_url=BASE_URL, interval=0, last_success=ls, last_change=ls)
+            src.max_index = 1
             src.save()
 
-            for j in range(3):
-                p = Post(source=src, title="post", created=timezone.now())
-                p.save()
-
             sub = Subscription(user=user, source=src)
             sub.save()
 
         folder = Subscription(user=user, source=None, name="Folder")
         folder.save()
 
         for i in range(3):
             ls = timezone.now()
             src = Source(name="folder1_test{i}".format(i=i), feed_url=BASE_URL, interval=0, last_success=ls, last_change=ls)
+            src.max_index = 1
             src.save()
 
-            for j in range(3):
-                p = Post(source=src, title=f"post-{pcount}", created=timezone.now()-timedelta(days=pcount))
-                p.save()
-                pcount += 1
-
             sub = Subscription(user=user, source=src, parent=folder)
-            sub.name = f"Sub-1-{i}"
             sub.save()
 
         folder2 = Subscription(user=user, source=None, name="AFolder2", parent=folder)
         folder2.save()
 
         for i in range(3):
             ls = timezone.now()
             src = Source(name="folder2_test{i}".format(i=i), feed_url=BASE_URL, interval=0, last_success=ls, last_change=ls)
+            src.max_index = 1
             src.save()
 
-            for j in range(3):
-                p = Post(source=src, title=f"post-{pcount}", created=timezone.now()-timedelta(days=pcount))
-                p.save()
-                pcount += 1
-
             sub = Subscription(user=user, source=src, parent=folder2)
             sub.save()
 
         all_subs_and_folder = Subscription.objects.filter(user=user).count()
 
         sub_list = get_unread_subscription_list_for_user(user)
 
         self.assertEqual(all_subs_and_folder, 11)
         self.assertEqual(len(sub_list), 4)
 
         for s in sub_list:
             if s.source is None:
-                self.assertEqual(s.unread_count, 18)
-                self.assertEqual(len(s.get_unread_posts()), 18)
-                last = None
-                for p in s.get_unread_posts():
-                    if last:
-                        self.assertGreater(p.created, last.created)
-                    last = p
-
-        (posts, paginator) = folder.get_paginated_posts(1, posts_per_page=10)
-        self.assertEqual(len(posts), 10)
-        self.assertEqual(paginator.num_pages, 2)
-        self.assertEqual(posts[0].subscription.name, "Sub-1-0")
-
-        (posts, paginator) = folder.get_paginated_posts(2, posts_per_page=10)
-        self.assertEqual(len(posts), 8)
+                self.assertEqual(s.unread_count, 6)
 
     def test_get_unread(self, mock):
 
         self._populate_mock(mock, status=200, test_file="rss_xhtml_body.xml", content_type="application/rss+xml")
 
         ls = timezone.now()
         src = Source(name="test1", feed_url=BASE_URL, interval=0, last_success=ls, last_change=ls)
         src.save()
 
         # Read the feed once to get the 1 post  and the etag
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
-        self.assertEqual(len(src.get_unread_posts()), 1)
+        self.assertEqual(src.unread_posts.count(), 1)
         src.mark_read()
         src.refresh_from_db()
-        self.assertEqual(len(src.get_unread_posts()), 0)
+        self.assertEqual(src.unread_posts.count(), 0)
 
     def test_get_unread_count_for_single_folder(self, mock):
 
         user = User(email='x@example.com')
         user.save()
 
         for i in range(3):
@@ -406,15 +352,15 @@
         self._populate_mock(mock, status=200, test_file="rss_xhtml_body.xml", content_type="application/rss+xml")
 
         ls = timezone.now()
         src = Source(name="test1", feed_url=BASE_URL, interval=0, last_success=ls, last_change=ls)
         src.save()
 
         # Read the feed once to get the 1 post  and the etag
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)
         self.assertEqual(src.posts.count(), 1)  # got the one post
         self.assertEqual(src.interval, 60)
         self.assertEqual(src.etag, "an-etag")
         self.assertNotEqual(src.last_success, ls)
@@ -424,15 +370,15 @@
 
         self._populate_mock(mock, status=200, test_file="podcast.xml", content_type="application/rss+xml")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
         # Read the feed once to get the 1 post  and the etag
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
         self.assertEqual(src.description, 'SU: Three nerds discussing tech, Apple, programming, and loosely related matters.')
 
         self.assertEqual(src.posts.all()[0].enclosures.count(), 1)
 
         enc = src.posts.all()[0].enclosures.all()[0]
@@ -442,29 +388,29 @@
     def test_mastodon(self, mock):
 
         self._populate_mock(mock, status=200, test_file="mastodon.xml", content_type="application/rss+xml")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
         self.assertEqual(src.description, 'Public posts from @xurble@toot.community')
 
         self.assertEqual(src.posts.all()[0].enclosures.count(), 1)
 
     def test_media_content(self, mock):
 
         self._populate_mock(mock, status=200, test_file="media_content.xml", content_type="application/rss+xml")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
         post = src.posts.all()[0]
         self.assertEqual(post.enclosures.count(), 1)
 
         self.assertEqual(post.body, "<p>New job, new Mac.</p>")
 
@@ -475,26 +421,25 @@
 
     def test_keep_old_enclosure(self, mock):
 
         settings.FEEDS_KEEP_OLD_ENCLOSURES = True
 
         # to pick up the settings change
         reload(utils)
-        reload(utils_internal)
 
         self._populate_mock(mock, status=200, test_file="media_content.xml", content_type="application/rss+xml")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
-        read_feed(src, output=NullOutput())
+        read_feed(src)
 
         self._populate_mock(mock, status=200, test_file="media_content_changed.xml", content_type="application/rss+xml")
 
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
         post = src.posts.all()[0]
         self.assertEqual(post.enclosures.count(), 2)
 
         self.assertEqual(post.current_enclosures.count(), 1)
         self.assertEqual(post.old_enclosures.count(), 1)
@@ -505,22 +450,21 @@
 
     def test_save_json(self, mock):
 
         settings.FEEDS_SAVE_JSON = True
 
         # to pick up the settings change
         reload(utils)
-        reload(utils_internal)
 
         self._populate_mock(mock, status=200, test_file="media_content.xml", content_type="application/rss+xml")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
         self.assertEqual(src.json["feed"]["link"], "https://toot.community/@xurble")
 
         post = src.posts.all()[0]
         self.assertEqual(post.json["summary"], post.body)
 
     def test_sanitize_1(self, mock):
@@ -531,15 +475,15 @@
 
         self._populate_mock(mock, status=200, test_file="rss_xhtml_body.xml", content_type="application/rss+xml")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
         # Read the feed once to get the 1 post  and the etag
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)
         p = src.posts.all()[0]
 
         self.assertFalse("<script>" in p.body)
 
@@ -551,29 +495,29 @@
 
         self._populate_mock(mock, status=200, test_file="sanitizer_bad_comment.xml", content_type="application/rss+xml")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
         # read the feed to update the name
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)
         self.assertEqual(src.name, "safe")
 
     def test_sanitize_attrs(self, mock):
 
         self._populate_mock(mock, status=200, test_file="sanitizer_img_attrs.xml", content_type="application/rss+xml")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
         # read the feed to update the name
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)
 
         body = src.posts.all()[0].body
 
         self.assertTrue("<img" in body)
@@ -583,15 +527,15 @@
     def create_source(self, mock, test_name, test_fn):
         self._populate_mock(mock, status=200,
                             test_file=test_fn,
                             content_type="application/rss+xml")
         src = Source(name=test_name, feed_url=BASE_URL, interval=0)
         src.save()
         # read the feed to update the name
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
         self.assertEqual(src.status_code, 200)
         return src
 
     def test_catch_long_guid_short_url(self, mock):
         test_name = "long guid short url"
         src = self.create_source(mock, test_name, "long_guid_tests.xml")
@@ -616,15 +560,15 @@
 
         ls = timezone.now()
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0, last_success=ls, last_change=ls)
         src.save()
 
         # Read the feed once to get the 1 post  and the etag
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)
         self.assertEqual(src.posts.count(), 2)  # got the one post
         self.assertEqual(src.interval, 60)
         self.assertEqual(src.etag, "an-etag")
         self.assertNotEqual(src.last_success, ls)
@@ -632,37 +576,36 @@
 
     def test_save_json(self, mock):
 
         settings.FEEDS_SAVE_JSON = True
 
         # to pick up the settings change
         reload(utils)
-        reload(utils_internal)
 
         self._populate_mock(mock, status=200, test_file="json_simple_two_entry.json", content_type="application/json")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
         self.assertEqual(src.json["title"], src.name)
 
         post = src.posts.all()[0]
         self.assertEqual(post.json["url"], post.link)
 
     def test_sanitize_1(self, mock):
 
         self._populate_mock(mock, status=200, test_file="json_simple_two_entry.json", content_type="application/json")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
         # Read the feed once to get the 1 post  and the etag
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)
         p = src.posts.all()[0]
 
         self.assertFalse("<script>" in p.body)
 
@@ -674,29 +617,29 @@
 
         self._populate_mock(mock, status=200, test_file="sanitizer_bad_comment.json", content_type="application/json")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
         # read the feed to update the name
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)
         self.assertEqual(src.name, "safe")
 
     def test_podcast(self, mock):
 
         self._populate_mock(mock, status=200, test_file="podcast.json", content_type="application/json")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
         # read the feed to update the name
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)
 
         post = src.posts.all()[0]
 
         self.assertEqual(post.enclosures.count(), 1)
@@ -710,39 +653,39 @@
         self._populate_mock(mock, status=200, test_file="rss_xhtml_body.xml", content_type="application/xml+rss")
         self._populate_mock(mock, status=304, test_file="empty_file.txt", content_type="application/xml+rss", etag="an-etag")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
         # Read the feed once to get the 1 post  and the etag
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)
         self.assertEqual(src.posts.count(), 1)  # got the one post
         self.assertEqual(src.interval, 60)
         self.assertEqual(src.etag, "an-etag")
 
         # Read the feed again to get a 304 and a small increment to the interval
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
         self.assertEqual(src.posts.count(), 1)  # should have no more
         self.assertEqual(src.status_code, 304)
         self.assertEqual(src.interval, 70)
         self.assertTrue(src.live)
 
     def test_not_a_feed(self, mock):
 
         self._populate_mock(mock, status=200, test_file="spurious_text_file.txt", content_type="text/plain")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)  # it returned a page, but not a  feed
         self.assertEqual(src.posts.count(), 0)  # can't have got any
         self.assertEqual(src.interval, 120)
         self.assertTrue(src.live)
 
@@ -751,120 +694,43 @@
         self._populate_mock(mock, status=403, test_file="empty_file.txt", content_type="text/plain")
 
         ls = timezone.now()
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0, last_success=ls)
         src.save()
 
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 403)  # it returned a page, but not a  feed
         self.assertEqual(src.posts.count(), 0)  # can't have got any
         self.assertFalse(src.live)
 
-    def test_cloudflared_standard(self, mock):
-
-        settings.FEEDS_DRIPFEED_KEY = "Key"
-
-        # to pick up the settings change
-        reload(utils)
-
-        self._populate_mock(mock, status=403, test_file="empty_file.txt", content_type="text/plain", is_cloudflare=True)
-
-        mock.register_uri('PUT', "https://dripfeed.app/api/v1/feeds/", content=b"""{"feed": {"uuid": "aa48333e-c40d-47ac-8a46-a13352dd8505", "name": "Elephant", "source_url": "http://feed.com/", "status_code": 200, "last_polled": "2024-03-17T18:48:19Z", "next_poll": "2024-03-25T03:06:08.991Z", "content_type": "text/plain", "etag": "06b06eb5", "error_code": "not-feed", "last_result": "Server response was not a feed", "dripfeed_url": "https://dripfeed.app/feed/aa48333e-c40d-47ac-8a46-a13352dd8505/", "live": true}, "detail": "OK"}""")
-
-        ls = timezone.now()
-
-        src = Source(name="test1", feed_url=BASE_URL, interval=0, last_success=ls)
-        src.save()
-
-        read_feed(src, output=NullOutput())
-        src.refresh_from_db()
-
-        self.assertEqual(src.status_code, 403)  # it returned a page, but not a  feed
-        self.assertEqual(src.posts.count(), 0)  # can't have got any
-        self.assertTrue(src.live)
-        self.assertTrue(src.is_cloudflare)
-        self.assertEqual(src.alt_url, "https://dripfeed.app/feed/aa48333e-c40d-47ac-8a46-a13352dd8505/")
-
-    def test_cloudflared_already_dripfed(self, mock):
-
-        settings.FEEDS_DRIPFEED_KEY = "Key"
-
-        # to pick up the settings change
-        reload(utils)
-
-        self._populate_mock(mock, status=403, test_file="empty_file.txt", content_type="text/plain", is_cloudflare=True)
-
-        mock.register_uri('PUT', "https://dripfeed.app/api/v1/feeds/", status_code=400, content=b"""{"detail": "Already subscribed to this feed."}""")
-        mock.register_uri('GET', "https://dripfeed.app/api/v1/feeds/", content=b"""{"feeds": [{"uuid": "aa48333e-c40d-47ac-8a46-a13352dd8505", "name": "Elephant", "source_url": "http://feed.com/", "status_code": 200, "last_polled": "2024-03-17T18:48:19Z", "next_poll": "2024-03-25T03:06:08.991Z", "content_type": "text/plain", "etag": "06b06eb5", "error_code": "not-feed", "last_result": "Server response was not a feed", "dripfeed_url": "https://dripfeed.app/feed/aa48333e-c40d-47ac-8a46-a13352dd8505/", "live": true}], "detail": "OK"}""")
-
-        ls = timezone.now()
-
-        src = Source(name="test1", feed_url=BASE_URL, interval=0, last_success=ls)
-        src.save()
-
-        read_feed(src, output=NullOutput())
-        src.refresh_from_db()
-
-        self.assertEqual(src.status_code, 403)  # it returned a page, but not a  feed
-        self.assertEqual(src.posts.count(), 0)  # can't have got any
-        self.assertTrue(src.live)
-        self.assertTrue(src.is_cloudflare)
-        self.assertEqual(src.alt_url, "https://dripfeed.app/feed/aa48333e-c40d-47ac-8a46-a13352dd8505/")
-
-    def test_cloudflared_cant_dripfeed(self, mock):
-
-        settings.FEEDS_DRIPFEED_KEY = "Key"
-
-        # to pick up the settings change
-        reload(utils)
-
-        self._populate_mock(mock, status=403, test_file="empty_file.txt", content_type="text/plain", is_cloudflare=True)
-
-        mock.register_uri('PUT', "https://dripfeed.app/api/v1/feeds/", status_code=403, content=b"""{"detail": "Maximum number of feeds reached."}""")
-
-        ls = timezone.now()
-
-        src = Source(name="test1", feed_url=BASE_URL, interval=0, last_success=ls)
-        src.save()
-
-        read_feed(src, output=NullOutput())
-        src.refresh_from_db()
-
-        self.assertEqual(src.status_code, 403)  # it returned a page, but not a  feed
-        self.assertEqual(src.posts.count(), 0)  # can't have got any
-        self.assertTrue(src.live)
-        self.assertTrue(src.is_cloudflare)
-        self.assertIsNone(src.alt_url)
-        self.assertEqual(src.last_result, "Failed add to Dripfeed: Maximum number of feeds reached.")
-
     def test_feed_gone(self, mock):
 
         self._populate_mock(mock, status=410, test_file="empty_file.txt", content_type="text/plain")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 410)  # it returned a page, but not a  feed
         self.assertEqual(src.posts.count(), 0)  # can't have got any
         self.assertFalse(src.live)
 
     def test_feed_not_found(self, mock):
 
         self._populate_mock(mock, status=404, test_file="empty_file.txt", content_type="text/plain")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 404)  # it returned a page, but not a  feed
         self.assertEqual(src.posts.count(), 0)  # can't have got any
         self.assertTrue(src.live)
         self.assertEqual(src.interval, 120)
 
@@ -875,39 +741,39 @@
         self._populate_mock(mock, status=200, test_file="rss_xhtml_body.xml", content_type="application/xml+rss",  url=new_url)
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
         self.assertIsNone(src.last_302_start)
 
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)
         self.assertEqual(src.last_302_url, new_url)  # this is where  went
         self.assertIsNotNone(src.last_302_start)
         self.assertEqual(src.posts.count(), 1)  # after following redirect will have 1 post
         self.assertEqual(src.interval, 60)
         self.assertTrue(src.live)
 
         # do it all again -  shouldn't change
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)  # it returned a page, but not a  feed
         self.assertEqual(src.last_302_url, new_url)  # this is where  went
         self.assertIsNotNone(src.last_302_start)
         self.assertEqual(src.posts.count(), 1)  # after following redirect will have 1 post
         self.assertEqual(src.interval, 80)
         self.assertTrue(src.live)
 
         # now we test making it permaent
         src.last_302_start = timezone.now() - timedelta(days=365)
         src.save()
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)
         self.assertEqual(src.last_302_url, ' ')
         self.assertIsNone(src.last_302_start)
         self.assertEqual(src.posts.count(), 1)
         self.assertEqual(src.interval, 100)
@@ -919,51 +785,51 @@
         new_url = "http://new.feed.com/"
         self._populate_mock(mock, status=301, test_file="empty_file.txt", content_type="text/plain", headers={"Location": new_url})
         self._populate_mock(mock, status=200, test_file="rss_xhtml_body.xml", content_type="application/xml+rss",  url=new_url)
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 301)
         self.assertEqual(src.interval, 60)
         self.assertEqual(src.feed_url, new_url)
 
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)
         self.assertEqual(src.posts.count(), 1)
         self.assertEqual(src.interval, 60)
         self.assertTrue(src.live)
 
     def test_server_error_1(self, mock):
 
         self._populate_mock(mock, status=500, test_file="empty_file.txt", content_type="text/plain")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 500)  # error
         self.assertEqual(src.posts.count(), 0)  # can't have got any
         self.assertTrue(src.live)
         self.assertEqual(src.interval, 120)
 
     def test_server_error_2(self, mock):
 
         self._populate_mock(mock, status=503, test_file="empty_file.txt", content_type="text/plain")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
-        read_feed(src, output=NullOutput())
+        read_feed(src)
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 503)  # error!
         self.assertEqual(src.posts.count(), 0)  # can't have got any
         self.assertTrue(src.live)
         self.assertEqual(src.interval, 120)
```

### Comparing `django_feed_reader-2.0.0/setup.py` & `django-feed-reader-2.0.0b1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 import setuptools
 
 
-with open('readme.rst', encoding='utf-8') as f:
+with open('readme.md', encoding='utf-8') as f:
     long_description = f.read()
 
 
 setuptools.setup(
     name='django-feed-reader',
-    version='2.0.0',
+    version='2.0.0-beta.1',
     description='An RSS feed reading library for Django.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Gareth Simpson',
     author_email='g@xurble.org',
     url='https://github.com/xurble/django-feed-reader',
     license='MIT',
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        'dripfeed-client',
         'sgmllib3k',
         'requests',
         'feedparser>=6.0.0',
         'beautifulsoup4',
         'pyrfc3339',
         'Django>=2.2'
     ],
```

