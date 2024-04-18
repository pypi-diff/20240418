# Comparing `tmp/symbl-2.0.3.tar.gz` & `tmp/symbl-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbl-2.0.3.tar", last modified: Wed Apr 17 23:56:38 2024, max compression
+gzip compressed data, was "symbl-2.0.4.tar", last modified: Thu Apr 18 16:03:30 2024, max compression
```

## Comparing `symbl-2.0.3.tar` & `symbl-2.0.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 23:56:38.624976 symbl-2.0.3/
--rw-r--r--   0 manojmali   (501) staff       (20)    11357 2024-04-16 22:31:01.000000 symbl-2.0.3/LICENSE
--rw-r--r--   0 manojmali   (501) staff       (20)     1958 2024-04-17 23:56:38.624764 symbl-2.0.3/PKG-INFO
--rw-r--r--   0 manojmali   (501) staff       (20)       38 2024-04-17 23:56:38.625025 symbl-2.0.3/setup.cfg
--rw-r--r--   0 manojmali   (501) staff       (20)     3837 2024-04-17 23:56:31.000000 symbl-2.0.3/setup.py
-drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 23:56:38.618509 symbl-2.0.3/symbl/
--rw-r--r--   0 manojmali   (501) staff       (20)     4310 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/AuthenticationToken.py
--rw-r--r--   0 manojmali   (501) staff       (20)     2207 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/Connection.py
--rw-r--r--   0 manojmali   (501) staff       (20)     4546 2024-04-17 09:16:55.000000 symbl-2.0.3/symbl/Conversations.py
--rw-r--r--   0 manojmali   (501) staff       (20)      594 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/__init__.py
-drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 23:56:38.620051 symbl-2.0.3/symbl/async_api/
--rw-r--r--   0 manojmali   (501) staff       (20)     4036 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/async_api/Audio.py
--rw-r--r--   0 manojmali   (501) staff       (20)     2041 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/async_api/Text.py
--rw-r--r--   0 manojmali   (501) staff       (20)     4029 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/async_api/Video.py
--rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/async_api/__init__.py
--rw-r--r--   0 manojmali   (501) staff       (20)      251 2024-04-17 23:45:22.000000 symbl-2.0.3/symbl/callScore.py
-drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 23:56:38.620238 symbl-2.0.3/symbl/configs/
--rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/configs/__init__.py
--rw-r--r--   0 manojmali   (501) staff       (20)      188 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/configs/configs.py
-drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 23:56:38.621106 symbl-2.0.3/symbl/conversations_api/
--rw-r--r--   0 manojmali   (501) staff       (20)     6056 2024-04-17 22:07:23.000000 symbl-2.0.3/symbl/conversations_api/ConversationsApi.py
--rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/conversations_api/__init__.py
-drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 23:56:38.621477 symbl-2.0.3/symbl/jobs_api/
--rw-r--r--   0 manojmali   (501) staff       (20)     2437 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/jobs_api/Job.py
--rw-r--r--   0 manojmali   (501) staff       (20)      446 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/jobs_api/JobStatus.py
--rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/jobs_api/__init__.py
-drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 23:56:38.621992 symbl-2.0.3/symbl/streaming_api/
--rw-r--r--   0 manojmali   (501) staff       (20)     1959 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/streaming_api/StreamingApi.py
--rw-r--r--   0 manojmali   (501) staff       (20)     3187 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/streaming_api/StreamingConnection.py
--rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/streaming_api/__init__.py
-drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 23:56:38.622424 symbl-2.0.3/symbl/telephony_api/
--rw-r--r--   0 manojmali   (501) staff       (20)     3587 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/telephony_api/TelephonyApi.py
--rw-r--r--   0 manojmali   (501) staff       (20)      996 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/telephony_api/TelephonyValidators.py
--rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/telephony_api/__init__.py
-drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 23:56:38.623137 symbl-2.0.3/symbl/utils/
--rw-r--r--   0 manojmali   (501) staff       (20)      478 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/utils/Decorators.py
--rw-r--r--   0 manojmali   (501) staff       (20)     3286 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/utils/Helper.py
--rw-r--r--   0 manojmali   (501) staff       (20)     1501 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/utils/Logger.py
--rw-r--r--   0 manojmali   (501) staff       (20)      682 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/utils/Threads.py
--rw-r--r--   0 manojmali   (501) staff       (20)      132 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/utils/__init__.py
-drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 23:56:38.619339 symbl-2.0.3/symbl.egg-info/
--rw-r--r--   0 manojmali   (501) staff       (20)     1958 2024-04-17 23:56:38.000000 symbl-2.0.3/symbl.egg-info/PKG-INFO
--rw-r--r--   0 manojmali   (501) staff       (20)     1114 2024-04-17 23:56:38.000000 symbl-2.0.3/symbl.egg-info/SOURCES.txt
--rw-r--r--   0 manojmali   (501) staff       (20)        1 2024-04-17 23:56:38.000000 symbl-2.0.3/symbl.egg-info/dependency_links.txt
--rw-r--r--   0 manojmali   (501) staff       (20)       66 2024-04-17 23:56:38.000000 symbl-2.0.3/symbl.egg-info/requires.txt
--rw-r--r--   0 manojmali   (501) staff       (20)       12 2024-04-17 23:56:38.000000 symbl-2.0.3/symbl.egg-info/top_level.txt
-drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 23:56:38.624466 symbl-2.0.3/tests/
--rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.3/tests/__init__.py
--rw-r--r--   0 manojmali   (501) staff       (20)     4567 2024-04-16 22:31:01.000000 symbl-2.0.3/tests/audio_test.py
--rw-r--r--   0 manojmali   (501) staff       (20)     4519 2024-04-16 22:31:01.000000 symbl-2.0.3/tests/authentication_token_test.py
--rw-r--r--   0 manojmali   (501) staff       (20)    12904 2024-04-16 22:31:01.000000 symbl-2.0.3/tests/conversations_api_test.py
--rw-r--r--   0 manojmali   (501) staff       (20)    11742 2024-04-16 22:31:01.000000 symbl-2.0.3/tests/conversations_test.py
--rw-r--r--   0 manojmali   (501) staff       (20)     2569 2024-04-16 22:31:01.000000 symbl-2.0.3/tests/telephony_test.py
--rw-r--r--   0 manojmali   (501) staff       (20)     2797 2024-04-16 22:31:01.000000 symbl-2.0.3/tests/text_test.py
--rw-r--r--   0 manojmali   (501) staff       (20)     4611 2024-04-16 22:31:01.000000 symbl-2.0.3/tests/video_test.py
+drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-18 16:03:30.944374 symbl-2.0.4/
+-rw-r--r--   0 manojmali   (501) staff       (20)    11357 2024-04-16 22:31:01.000000 symbl-2.0.4/LICENSE
+-rw-r--r--   0 manojmali   (501) staff       (20)     1958 2024-04-18 16:03:30.944141 symbl-2.0.4/PKG-INFO
+-rw-r--r--   0 manojmali   (501) staff       (20)       38 2024-04-18 16:03:30.944422 symbl-2.0.4/setup.cfg
+-rw-r--r--   0 manojmali   (501) staff       (20)     3837 2024-04-18 16:01:48.000000 symbl-2.0.4/setup.py
+drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-18 16:03:30.936076 symbl-2.0.4/symbl/
+-rw-r--r--   0 manojmali   (501) staff       (20)     4310 2024-04-16 22:31:01.000000 symbl-2.0.4/symbl/AuthenticationToken.py
+-rw-r--r--   0 manojmali   (501) staff       (20)     2207 2024-04-16 22:31:01.000000 symbl-2.0.4/symbl/Connection.py
+-rw-r--r--   0 manojmali   (501) staff       (20)     4546 2024-04-17 09:16:55.000000 symbl-2.0.4/symbl/Conversations.py
+-rw-r--r--   0 manojmali   (501) staff       (20)      594 2024-04-16 22:31:01.000000 symbl-2.0.4/symbl/__init__.py
+drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-18 16:03:30.937503 symbl-2.0.4/symbl/async_api/
+-rw-r--r--   0 manojmali   (501) staff       (20)     4036 2024-04-16 22:31:01.000000 symbl-2.0.4/symbl/async_api/Audio.py
+-rw-r--r--   0 manojmali   (501) staff       (20)     2041 2024-04-16 22:31:01.000000 symbl-2.0.4/symbl/async_api/Text.py
+-rw-r--r--   0 manojmali   (501) staff       (20)     4029 2024-04-16 22:31:01.000000 symbl-2.0.4/symbl/async_api/Video.py
+-rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.4/symbl/async_api/__init__.py
+-rw-r--r--   0 manojmali   (501) staff       (20)      257 2024-04-18 15:56:59.000000 symbl-2.0.4/symbl/callScore.py
+drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-18 16:03:30.937670 symbl-2.0.4/symbl/configs/
+-rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.4/symbl/configs/__init__.py
+-rw-r--r--   0 manojmali   (501) staff       (20)      188 2024-04-16 22:31:01.000000 symbl-2.0.4/symbl/configs/configs.py
+drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-18 16:03:30.938129 symbl-2.0.4/symbl/conversations_api/
+-rw-r--r--   0 manojmali   (501) staff       (20)     6482 2024-04-18 16:00:11.000000 symbl-2.0.4/symbl/conversations_api/ConversationsApi.py
+-rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.4/symbl/conversations_api/__init__.py
+drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-18 16:03:30.938529 symbl-2.0.4/symbl/jobs_api/
+-rw-r--r--   0 manojmali   (501) staff       (20)     2437 2024-04-16 22:31:01.000000 symbl-2.0.4/symbl/jobs_api/Job.py
+-rw-r--r--   0 manojmali   (501) staff       (20)      446 2024-04-16 22:31:01.000000 symbl-2.0.4/symbl/jobs_api/JobStatus.py
+-rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.4/symbl/jobs_api/__init__.py
+drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-18 16:03:30.938872 symbl-2.0.4/symbl/streaming_api/
+-rw-r--r--   0 manojmali   (501) staff       (20)     1959 2024-04-16 22:31:01.000000 symbl-2.0.4/symbl/streaming_api/StreamingApi.py
+-rw-r--r--   0 manojmali   (501) staff       (20)     3187 2024-04-16 22:31:01.000000 symbl-2.0.4/symbl/streaming_api/StreamingConnection.py
+-rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.4/symbl/streaming_api/__init__.py
+drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-18 16:03:30.941630 symbl-2.0.4/symbl/telephony_api/
+-rw-r--r--   0 manojmali   (501) staff       (20)     3587 2024-04-16 22:31:01.000000 symbl-2.0.4/symbl/telephony_api/TelephonyApi.py
+-rw-r--r--   0 manojmali   (501) staff       (20)      996 2024-04-16 22:31:01.000000 symbl-2.0.4/symbl/telephony_api/TelephonyValidators.py
+-rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.4/symbl/telephony_api/__init__.py
+drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-18 16:03:30.942330 symbl-2.0.4/symbl/utils/
+-rw-r--r--   0 manojmali   (501) staff       (20)      478 2024-04-16 22:31:01.000000 symbl-2.0.4/symbl/utils/Decorators.py
+-rw-r--r--   0 manojmali   (501) staff       (20)     3286 2024-04-16 22:31:01.000000 symbl-2.0.4/symbl/utils/Helper.py
+-rw-r--r--   0 manojmali   (501) staff       (20)     1501 2024-04-16 22:31:01.000000 symbl-2.0.4/symbl/utils/Logger.py
+-rw-r--r--   0 manojmali   (501) staff       (20)      682 2024-04-16 22:31:01.000000 symbl-2.0.4/symbl/utils/Threads.py
+-rw-r--r--   0 manojmali   (501) staff       (20)      132 2024-04-16 22:31:01.000000 symbl-2.0.4/symbl/utils/__init__.py
+drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-18 16:03:30.936829 symbl-2.0.4/symbl.egg-info/
+-rw-r--r--   0 manojmali   (501) staff       (20)     1958 2024-04-18 16:03:30.000000 symbl-2.0.4/symbl.egg-info/PKG-INFO
+-rw-r--r--   0 manojmali   (501) staff       (20)     1114 2024-04-18 16:03:30.000000 symbl-2.0.4/symbl.egg-info/SOURCES.txt
+-rw-r--r--   0 manojmali   (501) staff       (20)        1 2024-04-18 16:03:30.000000 symbl-2.0.4/symbl.egg-info/dependency_links.txt
+-rw-r--r--   0 manojmali   (501) staff       (20)       66 2024-04-18 16:03:30.000000 symbl-2.0.4/symbl.egg-info/requires.txt
+-rw-r--r--   0 manojmali   (501) staff       (20)       12 2024-04-18 16:03:30.000000 symbl-2.0.4/symbl.egg-info/top_level.txt
+drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-18 16:03:30.943868 symbl-2.0.4/tests/
+-rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.4/tests/__init__.py
+-rw-r--r--   0 manojmali   (501) staff       (20)     4567 2024-04-16 22:31:01.000000 symbl-2.0.4/tests/audio_test.py
+-rw-r--r--   0 manojmali   (501) staff       (20)     4519 2024-04-16 22:31:01.000000 symbl-2.0.4/tests/authentication_token_test.py
+-rw-r--r--   0 manojmali   (501) staff       (20)    12904 2024-04-16 22:31:01.000000 symbl-2.0.4/tests/conversations_api_test.py
+-rw-r--r--   0 manojmali   (501) staff       (20)    11742 2024-04-16 22:31:01.000000 symbl-2.0.4/tests/conversations_test.py
+-rw-r--r--   0 manojmali   (501) staff       (20)     2569 2024-04-16 22:31:01.000000 symbl-2.0.4/tests/telephony_test.py
+-rw-r--r--   0 manojmali   (501) staff       (20)     2797 2024-04-16 22:31:01.000000 symbl-2.0.4/tests/text_test.py
+-rw-r--r--   0 manojmali   (501) staff       (20)     4611 2024-04-16 22:31:01.000000 symbl-2.0.4/tests/video_test.py
```

### Comparing `symbl-2.0.3/LICENSE` & `symbl-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `symbl-2.0.3/PKG-INFO` & `symbl-2.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbl
-Version: 2.0.3
+Version: 2.0.4
 Summary: symbl.ai SDK
 Home-page: 
 Author-email: info@symbl.ai
 Keywords: Symbl.ai SDK
 License-File: LICENSE
 Requires-Dist: symbl_rest>=1.0.11
 Requires-Dist: websocket-client>=0.59.0
```

### Comparing `symbl-2.0.3/setup.py` & `symbl-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
 
 setup(
     name="symbl",
-    version="2.0.3",
+    version="2.0.4",
     description="symbl.ai SDK",
     author_email="info@symbl.ai",
     url="",
     keywords=["Symbl.ai SDK"],
     install_requires=["symbl_rest >= 1.0.11", "websocket-client >= 0.59.0", "pyaudio ~= 0.2.12", "numpy"],
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `symbl-2.0.3/symbl/AuthenticationToken.py` & `symbl-2.0.4/symbl/AuthenticationToken.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.3/symbl/Connection.py` & `symbl-2.0.4/symbl/Connection.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.3/symbl/Conversations.py` & `symbl-2.0.4/symbl/Conversations.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.3/symbl/__init__.py` & `symbl-2.0.4/symbl/__init__.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.3/symbl/async_api/Audio.py` & `symbl-2.0.4/symbl/async_api/Audio.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.3/symbl/async_api/Text.py` & `symbl-2.0.4/symbl/async_api/Text.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.3/symbl/async_api/Video.py` & `symbl-2.0.4/symbl/async_api/Video.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.3/symbl/conversations_api/ConversationsApi.py` & `symbl-2.0.4/symbl/conversations_api/ConversationsApi.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,22 @@
     def get_call_score(self, conversation_id, credentials=None):
         try:
             return self.conversations_api_rest.get_call_score_by_conversation_id(conversation_id)
         except:
             return {'message': 'The conversationId is either invalid or does not exist.'}
 
     @initialize_api_client
+    def get_call_score_insights_url(self, conversation_id, credentials=None):
+        try:
+            params = {'include_call_score': True}
+            return self.conversations_api_rest.get_experience_url_by_conversation_id(conversation_id, **correct_boolean_values(params))
+        except Exception as e:
+            return {'message': 'The conversationId is either invalid or does not exist.'}
+
+    @initialize_api_client
     def get_call_score_status(self, conversation_id, credentials=None):
         try:
             res = self.conversations_api_rest.get_call_score_status_by_conversation_id(conversation_id)
             return res
         except Exception as e:
             return {'message': 'The conversationId is either invalid or does not exist.'}
```

### Comparing `symbl-2.0.3/symbl/jobs_api/Job.py` & `symbl-2.0.4/symbl/jobs_api/Job.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.3/symbl/streaming_api/StreamingApi.py` & `symbl-2.0.4/symbl/streaming_api/StreamingApi.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.3/symbl/streaming_api/StreamingConnection.py` & `symbl-2.0.4/symbl/streaming_api/StreamingConnection.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.3/symbl/telephony_api/TelephonyApi.py` & `symbl-2.0.4/symbl/telephony_api/TelephonyApi.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.3/symbl/telephony_api/TelephonyValidators.py` & `symbl-2.0.4/symbl/telephony_api/TelephonyValidators.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.3/symbl/utils/Helper.py` & `symbl-2.0.4/symbl/utils/Helper.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.3/symbl/utils/Logger.py` & `symbl-2.0.4/symbl/utils/Logger.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.3/symbl/utils/Threads.py` & `symbl-2.0.4/symbl/utils/Threads.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.3/symbl.egg-info/PKG-INFO` & `symbl-2.0.4/symbl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbl
-Version: 2.0.3
+Version: 2.0.4
 Summary: symbl.ai SDK
 Home-page: 
 Author-email: info@symbl.ai
 Keywords: Symbl.ai SDK
 License-File: LICENSE
 Requires-Dist: symbl_rest>=1.0.11
 Requires-Dist: websocket-client>=0.59.0
```

### Comparing `symbl-2.0.3/symbl.egg-info/SOURCES.txt` & `symbl-2.0.4/symbl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `symbl-2.0.3/tests/audio_test.py` & `symbl-2.0.4/tests/audio_test.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.3/tests/authentication_token_test.py` & `symbl-2.0.4/tests/authentication_token_test.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.3/tests/conversations_api_test.py` & `symbl-2.0.4/tests/conversations_api_test.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.3/tests/conversations_test.py` & `symbl-2.0.4/tests/conversations_test.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.3/tests/telephony_test.py` & `symbl-2.0.4/tests/telephony_test.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.3/tests/text_test.py` & `symbl-2.0.4/tests/text_test.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.3/tests/video_test.py` & `symbl-2.0.4/tests/video_test.py`

 * *Files identical despite different names*

