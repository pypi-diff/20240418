# Comparing `tmp/krypper_tgstat-0.1.7.1.tar.gz` & `tmp/krypper_tgstat-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krypper_tgstat-0.1.7.1.tar", last modified: Thu Apr 18 13:27:28 2024, max compression
+gzip compressed data, was "krypper_tgstat-0.1.8.tar", last modified: Thu Apr 18 13:47:27 2024, max compression
```

## Comparing `krypper_tgstat-0.1.7.1.tar` & `krypper_tgstat-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-18 13:27:28.328367 krypper_tgstat-0.1.7.1/
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)     1063 2024-04-15 06:40:20.000000 krypper_tgstat-0.1.7.1/LICENSE
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      957 2024-04-18 13:27:28.328367 krypper_tgstat-0.1.7.1/PKG-INFO
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      103 2024-04-15 06:40:20.000000 krypper_tgstat-0.1.7.1/README.md
-drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-18 13:27:28.327367 krypper_tgstat-0.1.7.1/krypper_tgstat/
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      244 2024-04-18 13:26:52.000000 krypper_tgstat-0.1.7.1/krypper_tgstat/__init__.py
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)    10375 2024-04-18 13:25:29.000000 krypper_tgstat-0.1.7.1/krypper_tgstat/classes.py
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)     2906 2024-04-18 13:20:59.000000 krypper_tgstat-0.1.7.1/krypper_tgstat/enums.py
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      666 2024-04-15 06:45:39.000000 krypper_tgstat-0.1.7.1/krypper_tgstat/exceptions.py
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)     8210 2024-04-15 06:47:48.000000 krypper_tgstat-0.1.7.1/krypper_tgstat/tg_stat.py
-drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-18 13:27:28.328367 krypper_tgstat-0.1.7.1/krypper_tgstat.egg-info/
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      957 2024-04-18 13:27:28.000000 krypper_tgstat-0.1.7.1/krypper_tgstat.egg-info/PKG-INFO
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      382 2024-04-18 13:27:28.000000 krypper_tgstat-0.1.7.1/krypper_tgstat.egg-info/SOURCES.txt
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)        1 2024-04-18 13:27:28.000000 krypper_tgstat-0.1.7.1/krypper_tgstat.egg-info/dependency_links.txt
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)       17 2024-04-18 13:27:28.000000 krypper_tgstat-0.1.7.1/krypper_tgstat.egg-info/requires.txt
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)       15 2024-04-18 13:27:28.000000 krypper_tgstat-0.1.7.1/krypper_tgstat.egg-info/top_level.txt
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)       38 2024-04-18 13:27:28.329367 krypper_tgstat-0.1.7.1/setup.cfg
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)     1289 2024-04-18 13:26:59.000000 krypper_tgstat-0.1.7.1/setup.py
-drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-18 13:27:28.328367 krypper_tgstat-0.1.7.1/tests/
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)    37040 2024-04-15 07:20:55.000000 krypper_tgstat-0.1.7.1/tests/test_TGStatSync.py
+drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-18 13:47:27.363109 krypper_tgstat-0.1.8/
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)     1063 2024-04-15 06:40:20.000000 krypper_tgstat-0.1.8/LICENSE
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      955 2024-04-18 13:47:27.363109 krypper_tgstat-0.1.8/PKG-INFO
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      103 2024-04-15 06:40:20.000000 krypper_tgstat-0.1.8/README.md
+drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-18 13:47:27.361109 krypper_tgstat-0.1.8/krypper_tgstat/
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      242 2024-04-18 13:44:27.000000 krypper_tgstat-0.1.8/krypper_tgstat/__init__.py
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)    10375 2024-04-18 13:25:29.000000 krypper_tgstat-0.1.8/krypper_tgstat/classes.py
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)     2906 2024-04-18 13:20:59.000000 krypper_tgstat-0.1.8/krypper_tgstat/enums.py
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      666 2024-04-18 13:43:39.000000 krypper_tgstat-0.1.8/krypper_tgstat/exceptions.py
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)     8067 2024-04-18 13:43:49.000000 krypper_tgstat-0.1.8/krypper_tgstat/tg_stat.py
+drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-18 13:47:27.363109 krypper_tgstat-0.1.8/krypper_tgstat.egg-info/
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      955 2024-04-18 13:47:27.000000 krypper_tgstat-0.1.8/krypper_tgstat.egg-info/PKG-INFO
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      382 2024-04-18 13:47:27.000000 krypper_tgstat-0.1.8/krypper_tgstat.egg-info/SOURCES.txt
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)        1 2024-04-18 13:47:27.000000 krypper_tgstat-0.1.8/krypper_tgstat.egg-info/dependency_links.txt
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)       17 2024-04-18 13:47:27.000000 krypper_tgstat-0.1.8/krypper_tgstat.egg-info/requires.txt
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)       15 2024-04-18 13:47:27.000000 krypper_tgstat-0.1.8/krypper_tgstat.egg-info/top_level.txt
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)       38 2024-04-18 13:47:27.363109 krypper_tgstat-0.1.8/setup.cfg
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)     1287 2024-04-18 13:44:16.000000 krypper_tgstat-0.1.8/setup.py
+drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-18 13:47:27.362110 krypper_tgstat-0.1.8/tests/
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)    37040 2024-04-15 07:20:55.000000 krypper_tgstat-0.1.8/tests/test_TGStatSync.py
```

### Comparing `krypper_tgstat-0.1.7.1/LICENSE` & `krypper_tgstat-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `krypper_tgstat-0.1.7.1/PKG-INFO` & `krypper_tgstat-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krypper_tgstat
-Version: 0.1.7.1
+Version: 0.1.8
 Summary: Wrapper for TG Stat API writing on Python
 Home-page: https://github.com/KrymmyEM/krypper_tgstat
 Download-URL: https://github.com/KrymmyEM/krypper_tgstat/archive/main.zip
 Author: Evgeny Momotov (KrymmyEM)
 Author-email: evgeny.momotov@gmail.com
 License: MIT License. See LICENSE file
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `krypper_tgstat-0.1.7.1/krypper_tgstat/classes.py` & `krypper_tgstat-0.1.8/krypper_tgstat/classes.py`

 * *Files identical despite different names*

### Comparing `krypper_tgstat-0.1.7.1/krypper_tgstat/enums.py` & `krypper_tgstat-0.1.8/krypper_tgstat/enums.py`

 * *Files identical despite different names*

### Comparing `krypper_tgstat-0.1.7.1/krypper_tgstat/exceptions.py` & `krypper_tgstat-0.1.8/krypper_tgstat/exceptions.py`

 * *Files identical despite different names*

### Comparing `krypper_tgstat-0.1.7.1/krypper_tgstat/tg_stat.py` & `krypper_tgstat-0.1.8/krypper_tgstat/tg_stat.py`

 * *Files 27% similar despite different names*

```diff
@@ -23,45 +23,42 @@
         
     def _send_request(self, method: RequestsMethods, url: str, **kwargs):
         kwargs["token"] = self.token
         response = self.session.request(method=method.value, url=url, params=kwargs)
         return response.json()
     
     
-    def _check_catgory(self, category, sub_category):
-        if category and not isinstance(category, RequestsCategory):
-            raise TGStatTypeError(type(category), type(RequestsCategory), category._name_)
-        
-        if not type(sub_category) in [ChannelsRequests, PostsRequests, StoriesRequests, WordsRequests,
+    def _check_catgory(self, category, api_request):
+        if not type(api_request) in [ChannelsRequests, PostsRequests, StoriesRequests, WordsRequests,
                                         CallbackRequests, UsageRequests, DatabaseRequests]:
-            raise TGStatTypeError(type(category), [ChannelsRequests, PostsRequests, StoriesRequests, WordsRequests,
-                                        CallbackRequests, UsageRequests, DatabaseRequests], sub_category._name_)
+            raise TGStatTypeError(type(api_request), [ChannelsRequests, PostsRequests, StoriesRequests, WordsRequests,
+                                        CallbackRequests, UsageRequests, DatabaseRequests], api_request._name_)
         
         return True
 
     
-    def _build_result(self, data, sub_category: Union[
+    def _build_result(self, data, api_request: Union[
                     ChannelsRequests, PostsRequests, StoriesRequests, WordsRequests,
                     CallbackRequests, UsageRequests, DatabaseRequests
                 ]):
-        self._check_catgory(None, sub_category)
+        self._check_catgory(api_request)
 
         if isinstance(data, str):
             try:
                 data = json.loads(data)
             except:
                 raise TGStatException("Incorrect data value")
 
         if data['status'] == "error":
             raise TGStatAPIError(data["error"])
         
         class_parser = None
         kwargs = {}
         return_type = ReturnTypes.OBJECT
-        if sub_category in [ChannelsRequests.SEARCH, ChannelsRequests.POSTS, ChannelsRequests.STORIES,
+        if api_request in [ChannelsRequests.SEARCH, ChannelsRequests.POSTS, ChannelsRequests.STORIES,
                             ChannelsRequests.MENTIONS, ChannelsRequests.FORWARDS, PostsRequests.SEARCH,
                              WordsRequests.MENTIONS_BY_CHANNELS]:
             class_parser = MassiveResult
             
             key = "result_type"
 
             value_dict = {
@@ -71,21 +68,21 @@
                 ChannelsRequests.STORIES: ResultsType.STORIES,
                 ChannelsRequests.FORWARDS: ResultsType.FORWARDS,
                 ChannelsRequests.MENTIONS:ResultsType.MENTIONS, 
                 WordsRequests.MENTIONS_BY_CHANNELS:ResultsType.MENTIONS_CHANNEL
             }
 
             try:
-                kwargs[key] = value_dict[sub_category]
+                kwargs[key] = value_dict[api_request]
             except:
                 raise TGStatException("Unsupported Enum")
             
             kwargs.update(data["response"])
         
-        elif sub_category in [
+        elif api_request in [
                                 ChannelsRequests.SUBSCRIBERS, ChannelsRequests.VIEWS, ChannelsRequests.AVG_POSTS_REACH,
                                 ChannelsRequests.ER, ChannelsRequests.ERR, ChannelsRequests.ERR24,
                                 WordsRequests.MENTIONS_BY_PERIOD
                             ]:
 
             class_parser = DynamicData
             
@@ -98,21 +95,21 @@
                 ChannelsRequests.ER: DynamicType.ER,
                 ChannelsRequests.ERR: DynamicType.ERR,
                 ChannelsRequests.ERR24: DynamicType.ERR24,
                 WordsRequests.MENTIONS_BY_PERIOD: DynamicType.MENTIONS_BY_PERIOD,
             }
 
             try:
-                kwargs[key] = value_dict[sub_category]
+                kwargs[key] = value_dict[api_request]
             except:
                 raise TGStatException("Unsupported Enum")
 
             return_type = ReturnTypes.LIST 
         
-        elif sub_category in [ChannelsRequests.GET, PostsRequests.GET, StoriesRequests.GET,
+        elif api_request in [ChannelsRequests.GET, PostsRequests.GET, StoriesRequests.GET,
             ChannelsRequests.STAT, PostsRequests.STAT, StoriesRequests.STAT, 
             PostsRequests.STAT_MULTI, StoriesRequests.STAT_MULTI]:
             
             objects_dict = {
                 ChannelsRequests.GET: Channel,
                 PostsRequests.GET: Post,
                 StoriesRequests.GET: Story,
@@ -120,34 +117,34 @@
                 PostsRequests.STAT: GroupStatistic,
                 StoriesRequests.STAT: GroupStatistic,
                 PostsRequests.STAT_MULTI: UnionStatistic,
                 StoriesRequests.STAT_MULTI: UnionStatistic
             }
 
             try:
-                class_parser = objects_dict[sub_category]
+                class_parser = objects_dict[api_request]
             except:
                 raise TGStatException("Unsupported Enum")
             
-            if sub_category not in [PostsRequests.STAT_MULTI, StoriesRequests.STAT_MULTI]:
+            if api_request not in [PostsRequests.STAT_MULTI, StoriesRequests.STAT_MULTI]:
                 kwargs.update(data["response"])
             else:
                 return_type = ReturnTypes.LIST
         
-        elif isinstance(sub_category, DatabaseRequests):
+        elif isinstance(api_request, DatabaseRequests):
             class_parser = DatabaseEntity
 
             database_types = {
                 DatabaseRequests.CATEGORIES: DatabaseTypes.CATEGORIES,
                 DatabaseRequests.COUNTRIES: DatabaseTypes.COUNTRIES,
                 DatabaseRequests.LANGUAGES: DatabaseTypes.LANGUAGES,
             }
 
             try:
-                kwargs["database_type"] = database_types[sub_category]
+                kwargs["database_type"] = database_types[api_request]
             except:
                 raise TGStatException("Unsupported Enum")
             
             return_type = ReturnTypes.LIST
 
         
         if return_type == ReturnTypes.OBJECT:
@@ -161,48 +158,50 @@
                 else:
                     for temp_data_two in data["response"][temp_data]:
                         return_datas.append(class_parser(**kwargs, **temp_data_two))
             
             return return_datas
 
 
-    def get_result(self, data, sub_category: Union[
+    def get_result(self, data, api_request: Union[
                     ChannelsRequests, PostsRequests, StoriesRequests, WordsRequests,
                     CallbackRequests, UsageRequests, DatabaseRequests
                 ]):
                 
-        self._check_catgory(None, sub_category)
+        self._check_catgory(api_request)
 
-        return self._build_result(data, sub_category)
+        return self._build_result(data, api_request)
 
 
-    def api(self, category: RequestsCategory, 
-            sub_category: Union[
+    def api(self, api_request: Union[
                     ChannelsRequests, PostsRequests, StoriesRequests, WordsRequests,
                     CallbackRequests, UsageRequests, DatabaseRequests
                 ], 
             **kwargs):
 
-        self._check_catgory(category, sub_category)
+        self._check_catgory(api_request)
 
-        check_sub_category = {
-            RequestsCategory.CHANNELS: ChannelsRequests,
-            RequestsCategory.POSTS: PostsRequests,
-            RequestsCategory.STORIES: StoriesRequests,
-            RequestsCategory.WORDS: WordsRequests,
-            RequestsCategory.CALLBACK: CallbackRequests,
-            RequestsCategory.USAGE: UsageRequests,
-            RequestsCategory.DATABASE: DatabaseRequests,
+        request_types = {
+            ChannelsRequests: RequestsCategory.CHANNELS,
+            PostsRequests: RequestsCategory.POSTS,
+            StoriesRequests: RequestsCategory.STORIES,
+            WordsRequests: RequestsCategory.WORDS,
+            CallbackRequests: RequestsCategory.CALLBACK,
+            UsageRequests: RequestsCategory.USAGE,
+            DatabaseRequests: RequestsCategory.DATABASE
         }
 
-        if not isinstance(sub_category, check_sub_category[category]):
-            raise TGStatTypeError(type(sub_category), type(check_sub_category[category]), "sub_category")
+        category = request_types.get(api_request, False)
+
+        if not category:
+            raise TGStatTypeError(type(api_request), [ChannelsRequests, PostsRequests, StoriesRequests, WordsRequests,
+                    CallbackRequests, UsageRequests, DatabaseRequests], "api_request")
 
         first_postfix = category.value
-        last_postfix, method = sub_category.value
+        last_postfix, method = api_request.value
         sending_url = self.base_url + "/" + first_postfix + "/" + last_postfix
         response = self._send_request(method, sending_url, **kwargs)
-        result = self._build_result(response, sub_category)
+        result = self._build_result(response, api_request)
 
         return result
```

### Comparing `krypper_tgstat-0.1.7.1/krypper_tgstat.egg-info/PKG-INFO` & `krypper_tgstat-0.1.8/krypper_tgstat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krypper_tgstat
-Version: 0.1.7.1
+Version: 0.1.8
 Summary: Wrapper for TG Stat API writing on Python
 Home-page: https://github.com/KrymmyEM/krypper_tgstat
 Download-URL: https://github.com/KrymmyEM/krypper_tgstat/archive/main.zip
 Author: Evgeny Momotov (KrymmyEM)
 Author-email: evgeny.momotov@gmail.com
 License: MIT License. See LICENSE file
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `krypper_tgstat-0.1.7.1/setup.py` & `krypper_tgstat-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """
 :authors: Evgeny Momotov (KrymmyEM)
 :license: MIT License
 Copyright: (c) 2024 Evgeny
 """
 
-version = "0.1.7.1"
+version = "0.1.8"
 
 long_description = ""
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
```

### Comparing `krypper_tgstat-0.1.7.1/tests/test_TGStatSync.py` & `krypper_tgstat-0.1.8/tests/test_TGStatSync.py`

 * *Files identical despite different names*

