# Comparing `tmp/tap-linkedin-ads-2.3.0.tar.gz` & `tmp/tap-linkedin-ads-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tap-linkedin-ads-2.3.0.tar", last modified: Mon Apr 15 10:01:00 2024, max compression
+gzip compressed data, was "tap-linkedin-ads-2.3.1.tar", last modified: Thu Apr 18 05:49:19 2024, max compression
```

## Comparing `tap-linkedin-ads-2.3.0.tar` & `tap-linkedin-ads-2.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 10:01:00.000000 tap-linkedin-ads-2.3.0/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 10:01:00.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13369 2024-04-15 09:55:17.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/transform.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14809 2024-04-15 09:55:17.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/client.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 10:01:00.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1696 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/account_users.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2192 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/creatives.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13824 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/ad_analytics_by_campaign.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5113 2024-04-15 09:55:17.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/video_ads.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12277 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/campaigns.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13791 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/ad_analytics_by_creative.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2989 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/campaign_groups.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3471 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/accounts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34765 2024-04-15 09:55:17.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/streams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2706 2023-11-06 17:25:42.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/schema.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1620 2024-04-13 15:56:16.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5775 2024-04-15 09:55:17.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      612 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/discover.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 10:01:00.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       73 2024-04-15 10:01:00.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-15 10:01:00.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2024-04-15 10:01:00.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      328 2024-04-15 10:01:00.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      814 2024-04-15 10:01:00.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       17 2024-04-15 10:01:00.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-15 10:01:00.000000 tap-linkedin-ads-2.3.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      328 2024-04-15 10:01:00.000000 tap-linkedin-ads-2.3.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      840 2024-04-15 09:55:17.000000 tap-linkedin-ads-2.3.0/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17019 2024-04-15 09:55:17.000000 tap-linkedin-ads-2.3.0/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 05:49:19.715004 tap-linkedin-ads-2.3.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      328 2024-04-18 05:49:19.715004 tap-linkedin-ads-2.3.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17019 2024-04-18 05:08:56.000000 tap-linkedin-ads-2.3.1/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-18 05:49:19.715004 tap-linkedin-ads-2.3.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      840 2024-04-18 05:45:19.000000 tap-linkedin-ads-2.3.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 05:49:19.711004 tap-linkedin-ads-2.3.1/tap_linkedin_ads/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1620 2024-04-13 14:22:08.000000 tap-linkedin-ads-2.3.1/tap_linkedin_ads/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14809 2024-04-18 05:08:56.000000 tap-linkedin-ads-2.3.1/tap_linkedin_ads/client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      612 2023-10-09 11:03:06.000000 tap-linkedin-ads-2.3.1/tap_linkedin_ads/discover.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2706 2024-04-13 14:22:08.000000 tap-linkedin-ads-2.3.1/tap_linkedin_ads/schema.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 05:49:19.715004 tap-linkedin-ads-2.3.1/tap_linkedin_ads/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1696 2023-10-09 11:03:06.000000 tap-linkedin-ads-2.3.1/tap_linkedin_ads/schemas/account_users.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3471 2023-10-09 11:03:06.000000 tap-linkedin-ads-2.3.1/tap_linkedin_ads/schemas/accounts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13824 2023-10-09 11:03:06.000000 tap-linkedin-ads-2.3.1/tap_linkedin_ads/schemas/ad_analytics_by_campaign.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13791 2023-10-09 11:03:06.000000 tap-linkedin-ads-2.3.1/tap_linkedin_ads/schemas/ad_analytics_by_creative.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2989 2023-10-09 11:03:06.000000 tap-linkedin-ads-2.3.1/tap_linkedin_ads/schemas/campaign_groups.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12277 2023-10-09 11:03:06.000000 tap-linkedin-ads-2.3.1/tap_linkedin_ads/schemas/campaigns.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2192 2023-10-09 11:03:06.000000 tap-linkedin-ads-2.3.1/tap_linkedin_ads/schemas/creatives.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5113 2024-04-18 05:08:56.000000 tap-linkedin-ads-2.3.1/tap_linkedin_ads/schemas/video_ads.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34810 2024-04-18 05:45:19.000000 tap-linkedin-ads-2.3.1/tap_linkedin_ads/streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5775 2024-04-18 05:08:56.000000 tap-linkedin-ads-2.3.1/tap_linkedin_ads/sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13369 2024-04-18 05:08:56.000000 tap-linkedin-ads-2.3.1/tap_linkedin_ads/transform.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 05:49:19.711004 tap-linkedin-ads-2.3.1/tap_linkedin_ads.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      328 2024-04-18 05:49:19.000000 tap-linkedin-ads-2.3.1/tap_linkedin_ads.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      814 2024-04-18 05:49:19.000000 tap-linkedin-ads-2.3.1/tap_linkedin_ads.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-18 05:49:19.000000 tap-linkedin-ads-2.3.1/tap_linkedin_ads.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2024-04-18 05:49:19.000000 tap-linkedin-ads-2.3.1/tap_linkedin_ads.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       73 2024-04-18 05:49:19.000000 tap-linkedin-ads-2.3.1/tap_linkedin_ads.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       17 2024-04-18 05:49:19.000000 tap-linkedin-ads-2.3.1/tap_linkedin_ads.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tap-linkedin-ads-2.3.0/tap_linkedin_ads/transform.py` & `tap-linkedin-ads-2.3.1/tap_linkedin_ads/transform.py`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.3.0/tap_linkedin_ads/client.py` & `tap-linkedin-ads-2.3.1/tap_linkedin_ads/client.py`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/account_users.json` & `tap-linkedin-ads-2.3.1/tap_linkedin_ads/schemas/account_users.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/creatives.json` & `tap-linkedin-ads-2.3.1/tap_linkedin_ads/schemas/creatives.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/ad_analytics_by_campaign.json` & `tap-linkedin-ads-2.3.1/tap_linkedin_ads/schemas/ad_analytics_by_campaign.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/video_ads.json` & `tap-linkedin-ads-2.3.1/tap_linkedin_ads/schemas/video_ads.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/campaigns.json` & `tap-linkedin-ads-2.3.1/tap_linkedin_ads/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/ad_analytics_by_creative.json` & `tap-linkedin-ads-2.3.1/tap_linkedin_ads/schemas/ad_analytics_by_creative.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/campaign_groups.json` & `tap-linkedin-ads-2.3.1/tap_linkedin_ads/schemas/campaign_groups.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/accounts.json` & `tap-linkedin-ads-2.3.1/tap_linkedin_ads/schemas/accounts.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.3.0/tap_linkedin_ads/streams.py` & `tap-linkedin-ads-2.3.1/tap_linkedin_ads/streams.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         for link in links:
             rel = link.get('rel')
             if rel == 'next':
                 href = link.get('href')
                 if href:
                     # url must be kept encoded for the creatives endpoint.
                     # Ref - https://learn.microsoft.com/en-us/linkedin/marketing/integrations/ads/account-structure/create-and-manage-creatives?view=li-lms-2023-01&tabs=http#sample-request-3
-                    if "rest/creatives" in href:
+                    if "rest/creatives" in href or "rest/posts" in href:
                         return 'https://api.linkedin.com{}'.format(href)
                     # Prepare next page URL
                     next_url = 'https://api.linkedin.com{}'.format(urllib.parse.unquote(href))
     return next_url
 
 def shift_sync_window(params, today, date_window_size, forced_window_size=None):
     """
@@ -613,15 +613,16 @@
     key_properties = ["content_reference"]
     foreign_key = "id"
     path = "posts"
     data_key = "elements"
     parent = "accounts"
     params = {
         "q": "dscAdAccount",
-        "dscAdTypes": "List(VIDEO)"
+        "dscAdTypes": "List(VIDEO)",
+        "count":100
     }
     headers = {'X-Restli-Protocol-Version': "2.0.0"}
 
     def sync_endpoint(self, *args, **kwargs):
         try:
             return super().sync_endpoint(*args, **kwargs)
         except Exception as error:
```

### Comparing `tap-linkedin-ads-2.3.0/tap_linkedin_ads/schema.py` & `tap-linkedin-ads-2.3.1/tap_linkedin_ads/schema.py`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.3.0/tap_linkedin_ads/__init__.py` & `tap-linkedin-ads-2.3.1/tap_linkedin_ads/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.3.0/tap_linkedin_ads/sync.py` & `tap-linkedin-ads-2.3.1/tap_linkedin_ads/sync.py`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.3.0/tap_linkedin_ads/discover.py` & `tap-linkedin-ads-2.3.1/tap_linkedin_ads/discover.py`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.3.0/tap_linkedin_ads.egg-info/SOURCES.txt` & `tap-linkedin-ads-2.3.1/tap_linkedin_ads.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.3.0/setup.py` & `tap-linkedin-ads-2.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(name='tap-linkedin-ads',
-      version='2.3.0',
+      version='2.3.1',
       description='Singer.io tap for extracting data from the LinkedIn Marketing Ads API API 2.0',
       author='jeff.huth@bytecode.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_linkedin_ads'],
       install_requires=[
           'backoff==1.8.0',
           'requests==2.22.0',
```

### Comparing `tap-linkedin-ads-2.3.0/README.md` & `tap-linkedin-ads-2.3.1/README.md`

 * *Files identical despite different names*

