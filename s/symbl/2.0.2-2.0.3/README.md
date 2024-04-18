# Comparing `tmp/symbl-2.0.2.tar.gz` & `tmp/symbl-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbl-2.0.2.tar", last modified: Wed Apr 17 09:19:44 2024, max compression
+gzip compressed data, was "symbl-2.0.3.tar", last modified: Wed Apr 17 23:56:38 2024, max compression
```

## Comparing `symbl-2.0.2.tar` & `symbl-2.0.3.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 09:19:44.533825 symbl-2.0.2/
--rw-r--r--   0 manojmali   (501) staff       (20)    11357 2024-04-16 22:31:01.000000 symbl-2.0.2/LICENSE
--rw-r--r--   0 manojmali   (501) staff       (20)     1832 2024-04-17 09:19:44.533615 symbl-2.0.2/PKG-INFO
--rw-r--r--   0 manojmali   (501) staff       (20)       38 2024-04-17 09:19:44.533866 symbl-2.0.2/setup.cfg
--rw-r--r--   0 manojmali   (501) staff       (20)     3837 2024-04-17 09:19:04.000000 symbl-2.0.2/setup.py
-drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 09:19:44.528768 symbl-2.0.2/symbl/
--rw-r--r--   0 manojmali   (501) staff       (20)     4310 2024-04-16 22:31:01.000000 symbl-2.0.2/symbl/AuthenticationToken.py
--rw-r--r--   0 manojmali   (501) staff       (20)     2207 2024-04-16 22:31:01.000000 symbl-2.0.2/symbl/Connection.py
--rw-r--r--   0 manojmali   (501) staff       (20)     4546 2024-04-17 09:16:55.000000 symbl-2.0.2/symbl/Conversations.py
--rw-r--r--   0 manojmali   (501) staff       (20)      594 2024-04-16 22:31:01.000000 symbl-2.0.2/symbl/__init__.py
-drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 09:19:44.530030 symbl-2.0.2/symbl/async_api/
--rw-r--r--   0 manojmali   (501) staff       (20)     4036 2024-04-16 22:31:01.000000 symbl-2.0.2/symbl/async_api/Audio.py
--rw-r--r--   0 manojmali   (501) staff       (20)     2041 2024-04-16 22:31:01.000000 symbl-2.0.2/symbl/async_api/Text.py
--rw-r--r--   0 manojmali   (501) staff       (20)     4029 2024-04-16 22:31:01.000000 symbl-2.0.2/symbl/async_api/Video.py
--rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.2/symbl/async_api/__init__.py
-drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 09:19:44.530211 symbl-2.0.2/symbl/configs/
--rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.2/symbl/configs/__init__.py
--rw-r--r--   0 manojmali   (501) staff       (20)      188 2024-04-16 22:31:01.000000 symbl-2.0.2/symbl/configs/configs.py
-drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 09:19:44.530581 symbl-2.0.2/symbl/conversations_api/
--rw-r--r--   0 manojmali   (501) staff       (20)     6019 2024-04-17 09:16:55.000000 symbl-2.0.2/symbl/conversations_api/ConversationsApi.py
--rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.2/symbl/conversations_api/__init__.py
-drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 09:19:44.530918 symbl-2.0.2/symbl/jobs_api/
--rw-r--r--   0 manojmali   (501) staff       (20)     2437 2024-04-16 22:31:01.000000 symbl-2.0.2/symbl/jobs_api/Job.py
--rw-r--r--   0 manojmali   (501) staff       (20)      446 2024-04-16 22:31:01.000000 symbl-2.0.2/symbl/jobs_api/JobStatus.py
--rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.2/symbl/jobs_api/__init__.py
-drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 09:19:44.531251 symbl-2.0.2/symbl/streaming_api/
--rw-r--r--   0 manojmali   (501) staff       (20)     1959 2024-04-16 22:31:01.000000 symbl-2.0.2/symbl/streaming_api/StreamingApi.py
--rw-r--r--   0 manojmali   (501) staff       (20)     3187 2024-04-16 22:31:01.000000 symbl-2.0.2/symbl/streaming_api/StreamingConnection.py
--rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.2/symbl/streaming_api/__init__.py
-drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 09:19:44.531597 symbl-2.0.2/symbl/telephony_api/
--rw-r--r--   0 manojmali   (501) staff       (20)     3587 2024-04-16 22:31:01.000000 symbl-2.0.2/symbl/telephony_api/TelephonyApi.py
--rw-r--r--   0 manojmali   (501) staff       (20)      996 2024-04-16 22:31:01.000000 symbl-2.0.2/symbl/telephony_api/TelephonyValidators.py
--rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.2/symbl/telephony_api/__init__.py
-drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 09:19:44.532270 symbl-2.0.2/symbl/utils/
--rw-r--r--   0 manojmali   (501) staff       (20)      478 2024-04-16 22:31:01.000000 symbl-2.0.2/symbl/utils/Decorators.py
--rw-r--r--   0 manojmali   (501) staff       (20)     3286 2024-04-16 22:31:01.000000 symbl-2.0.2/symbl/utils/Helper.py
--rw-r--r--   0 manojmali   (501) staff       (20)     1501 2024-04-16 22:31:01.000000 symbl-2.0.2/symbl/utils/Logger.py
--rw-r--r--   0 manojmali   (501) staff       (20)      682 2024-04-16 22:31:01.000000 symbl-2.0.2/symbl/utils/Threads.py
--rw-r--r--   0 manojmali   (501) staff       (20)      132 2024-04-16 22:31:01.000000 symbl-2.0.2/symbl/utils/__init__.py
-drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 09:19:44.529333 symbl-2.0.2/symbl.egg-info/
--rw-r--r--   0 manojmali   (501) staff       (20)     1832 2024-04-17 09:19:44.000000 symbl-2.0.2/symbl.egg-info/PKG-INFO
--rw-r--r--   0 manojmali   (501) staff       (20)     1095 2024-04-17 09:19:44.000000 symbl-2.0.2/symbl.egg-info/SOURCES.txt
--rw-r--r--   0 manojmali   (501) staff       (20)        1 2024-04-17 09:19:44.000000 symbl-2.0.2/symbl.egg-info/dependency_links.txt
--rw-r--r--   0 manojmali   (501) staff       (20)       66 2024-04-17 09:19:44.000000 symbl-2.0.2/symbl.egg-info/requires.txt
--rw-r--r--   0 manojmali   (501) staff       (20)       12 2024-04-17 09:19:44.000000 symbl-2.0.2/symbl.egg-info/top_level.txt
-drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 09:19:44.533423 symbl-2.0.2/tests/
--rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.2/tests/__init__.py
--rw-r--r--   0 manojmali   (501) staff       (20)     4567 2024-04-16 22:31:01.000000 symbl-2.0.2/tests/audio_test.py
--rw-r--r--   0 manojmali   (501) staff       (20)     4519 2024-04-16 22:31:01.000000 symbl-2.0.2/tests/authentication_token_test.py
--rw-r--r--   0 manojmali   (501) staff       (20)    12904 2024-04-16 22:31:01.000000 symbl-2.0.2/tests/conversations_api_test.py
--rw-r--r--   0 manojmali   (501) staff       (20)    11742 2024-04-16 22:31:01.000000 symbl-2.0.2/tests/conversations_test.py
--rw-r--r--   0 manojmali   (501) staff       (20)     2569 2024-04-16 22:31:01.000000 symbl-2.0.2/tests/telephony_test.py
--rw-r--r--   0 manojmali   (501) staff       (20)     2797 2024-04-16 22:31:01.000000 symbl-2.0.2/tests/text_test.py
--rw-r--r--   0 manojmali   (501) staff       (20)     4611 2024-04-16 22:31:01.000000 symbl-2.0.2/tests/video_test.py
+drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 23:56:38.624976 symbl-2.0.3/
+-rw-r--r--   0 manojmali   (501) staff       (20)    11357 2024-04-16 22:31:01.000000 symbl-2.0.3/LICENSE
+-rw-r--r--   0 manojmali   (501) staff       (20)     1958 2024-04-17 23:56:38.624764 symbl-2.0.3/PKG-INFO
+-rw-r--r--   0 manojmali   (501) staff       (20)       38 2024-04-17 23:56:38.625025 symbl-2.0.3/setup.cfg
+-rw-r--r--   0 manojmali   (501) staff       (20)     3837 2024-04-17 23:56:31.000000 symbl-2.0.3/setup.py
+drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 23:56:38.618509 symbl-2.0.3/symbl/
+-rw-r--r--   0 manojmali   (501) staff       (20)     4310 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/AuthenticationToken.py
+-rw-r--r--   0 manojmali   (501) staff       (20)     2207 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/Connection.py
+-rw-r--r--   0 manojmali   (501) staff       (20)     4546 2024-04-17 09:16:55.000000 symbl-2.0.3/symbl/Conversations.py
+-rw-r--r--   0 manojmali   (501) staff       (20)      594 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/__init__.py
+drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 23:56:38.620051 symbl-2.0.3/symbl/async_api/
+-rw-r--r--   0 manojmali   (501) staff       (20)     4036 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/async_api/Audio.py
+-rw-r--r--   0 manojmali   (501) staff       (20)     2041 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/async_api/Text.py
+-rw-r--r--   0 manojmali   (501) staff       (20)     4029 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/async_api/Video.py
+-rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/async_api/__init__.py
+-rw-r--r--   0 manojmali   (501) staff       (20)      251 2024-04-17 23:45:22.000000 symbl-2.0.3/symbl/callScore.py
+drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 23:56:38.620238 symbl-2.0.3/symbl/configs/
+-rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/configs/__init__.py
+-rw-r--r--   0 manojmali   (501) staff       (20)      188 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/configs/configs.py
+drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 23:56:38.621106 symbl-2.0.3/symbl/conversations_api/
+-rw-r--r--   0 manojmali   (501) staff       (20)     6056 2024-04-17 22:07:23.000000 symbl-2.0.3/symbl/conversations_api/ConversationsApi.py
+-rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/conversations_api/__init__.py
+drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 23:56:38.621477 symbl-2.0.3/symbl/jobs_api/
+-rw-r--r--   0 manojmali   (501) staff       (20)     2437 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/jobs_api/Job.py
+-rw-r--r--   0 manojmali   (501) staff       (20)      446 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/jobs_api/JobStatus.py
+-rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/jobs_api/__init__.py
+drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 23:56:38.621992 symbl-2.0.3/symbl/streaming_api/
+-rw-r--r--   0 manojmali   (501) staff       (20)     1959 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/streaming_api/StreamingApi.py
+-rw-r--r--   0 manojmali   (501) staff       (20)     3187 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/streaming_api/StreamingConnection.py
+-rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/streaming_api/__init__.py
+drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 23:56:38.622424 symbl-2.0.3/symbl/telephony_api/
+-rw-r--r--   0 manojmali   (501) staff       (20)     3587 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/telephony_api/TelephonyApi.py
+-rw-r--r--   0 manojmali   (501) staff       (20)      996 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/telephony_api/TelephonyValidators.py
+-rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/telephony_api/__init__.py
+drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 23:56:38.623137 symbl-2.0.3/symbl/utils/
+-rw-r--r--   0 manojmali   (501) staff       (20)      478 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/utils/Decorators.py
+-rw-r--r--   0 manojmali   (501) staff       (20)     3286 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/utils/Helper.py
+-rw-r--r--   0 manojmali   (501) staff       (20)     1501 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/utils/Logger.py
+-rw-r--r--   0 manojmali   (501) staff       (20)      682 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/utils/Threads.py
+-rw-r--r--   0 manojmali   (501) staff       (20)      132 2024-04-16 22:31:01.000000 symbl-2.0.3/symbl/utils/__init__.py
+drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 23:56:38.619339 symbl-2.0.3/symbl.egg-info/
+-rw-r--r--   0 manojmali   (501) staff       (20)     1958 2024-04-17 23:56:38.000000 symbl-2.0.3/symbl.egg-info/PKG-INFO
+-rw-r--r--   0 manojmali   (501) staff       (20)     1114 2024-04-17 23:56:38.000000 symbl-2.0.3/symbl.egg-info/SOURCES.txt
+-rw-r--r--   0 manojmali   (501) staff       (20)        1 2024-04-17 23:56:38.000000 symbl-2.0.3/symbl.egg-info/dependency_links.txt
+-rw-r--r--   0 manojmali   (501) staff       (20)       66 2024-04-17 23:56:38.000000 symbl-2.0.3/symbl.egg-info/requires.txt
+-rw-r--r--   0 manojmali   (501) staff       (20)       12 2024-04-17 23:56:38.000000 symbl-2.0.3/symbl.egg-info/top_level.txt
+drwxr-xr-x   0 manojmali   (501) staff       (20)        0 2024-04-17 23:56:38.624466 symbl-2.0.3/tests/
+-rw-r--r--   0 manojmali   (501) staff       (20)        0 2024-04-16 22:31:01.000000 symbl-2.0.3/tests/__init__.py
+-rw-r--r--   0 manojmali   (501) staff       (20)     4567 2024-04-16 22:31:01.000000 symbl-2.0.3/tests/audio_test.py
+-rw-r--r--   0 manojmali   (501) staff       (20)     4519 2024-04-16 22:31:01.000000 symbl-2.0.3/tests/authentication_token_test.py
+-rw-r--r--   0 manojmali   (501) staff       (20)    12904 2024-04-16 22:31:01.000000 symbl-2.0.3/tests/conversations_api_test.py
+-rw-r--r--   0 manojmali   (501) staff       (20)    11742 2024-04-16 22:31:01.000000 symbl-2.0.3/tests/conversations_test.py
+-rw-r--r--   0 manojmali   (501) staff       (20)     2569 2024-04-16 22:31:01.000000 symbl-2.0.3/tests/telephony_test.py
+-rw-r--r--   0 manojmali   (501) staff       (20)     2797 2024-04-16 22:31:01.000000 symbl-2.0.3/tests/text_test.py
+-rw-r--r--   0 manojmali   (501) staff       (20)     4611 2024-04-16 22:31:01.000000 symbl-2.0.3/tests/video_test.py
```

### Comparing `symbl-2.0.2/LICENSE` & `symbl-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `symbl-2.0.2/PKG-INFO` & `symbl-2.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 Metadata-Version: 2.1
 Name: symbl
-Version: 2.0.2
+Version: 2.0.3
 Summary: symbl.ai SDK
 Home-page: 
 Author-email: info@symbl.ai
 Keywords: Symbl.ai SDK
 License-File: LICENSE
+Requires-Dist: symbl_rest>=1.0.11
+Requires-Dist: websocket-client>=0.59.0
+Requires-Dist: pyaudio~=0.2.12
+Requires-Dist: numpy
 
     &lt;h1&gt;Symbl&#x27;s APIs for external consumers.&lt;/h1&gt; &lt;h2&gt;Language Insights API&lt;/h2&gt; Symbl&#x27;s Language Insights API provides an interface for applications to perform the analysis on the raw text and get insights from it. The API automatically detects sentence boundaries and punctuates the sentences, and also returns the updated messages in the response. Conversations are the most unstructured piece of information that we represent information in, and which most of the leads to lot of loss of information by not being able to capture them correctly.&lt;br/&gt; Language Insights API focuses on understanding such texts and generate the useful and important information from them. &lt;br/&gt; Currently the API supports detection of the Action Items in any type of unstructured text. In future the same API will also have support to detect \&quot;Information\&quot; and \&quot;Event\&quot;, where Information is any informational piece and Event is a reference to something that has happened in the past.&lt;br/&gt; &lt;h2&gt;Telephony Integration&lt;/h2&gt; Symbl can currently integrate with two types of telephony endpoints: 1. SIP trunks&lt;br/&gt; 2. PSTN endpoints&lt;br/&gt; Results are sent via HTTP WebHooks as and when they are available.&lt;br/&gt; &lt;h2&gt;Flow&lt;/h2&gt; 1. External Application invokes REST API to join a meeting/session, with the mode (SIP/PSTN) and joining details&lt;br/&gt; 2. Symbl joins the meeting via SIP or PSTN integration&lt;br/&gt; 3. Symbl continuously processes the audio stream received&lt;br/&gt; 4. Symbl calls WebHook whenever transcription results are available&lt;br/&gt;  # noqa: E501
```

### Comparing `symbl-2.0.2/setup.py` & `symbl-2.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
 
 setup(
     name="symbl",
-    version="2.0.2",
+    version="2.0.3",
     description="symbl.ai SDK",
     author_email="info@symbl.ai",
     url="",
     keywords=["Symbl.ai SDK"],
     install_requires=["symbl_rest >= 1.0.11", "websocket-client >= 0.59.0", "pyaudio ~= 0.2.12", "numpy"],
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `symbl-2.0.2/symbl/AuthenticationToken.py` & `symbl-2.0.3/symbl/AuthenticationToken.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.2/symbl/Connection.py` & `symbl-2.0.3/symbl/Connection.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.2/symbl/Conversations.py` & `symbl-2.0.3/symbl/Conversations.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.2/symbl/__init__.py` & `symbl-2.0.3/symbl/__init__.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.2/symbl/async_api/Audio.py` & `symbl-2.0.3/symbl/async_api/Audio.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.2/symbl/async_api/Text.py` & `symbl-2.0.3/symbl/async_api/Text.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.2/symbl/async_api/Video.py` & `symbl-2.0.3/symbl/async_api/Video.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.2/symbl/conversations_api/ConversationsApi.py` & `symbl-2.0.3/symbl/conversations_api/ConversationsApi.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,17 @@
             return self.conversations_api_rest.get_call_score_by_conversation_id(conversation_id)
         except:
             return {'message': 'The conversationId is either invalid or does not exist.'}
 
     @initialize_api_client
     def get_call_score_status(self, conversation_id, credentials=None):
         try:
-            return self.conversations_api_rest.get_call_score_status_by_conversation_id(conversation_id)
-        except:
+            res = self.conversations_api_rest.get_call_score_status_by_conversation_id(conversation_id)
+            return res
+        except Exception as e:
             return {'message': 'The conversationId is either invalid or does not exist.'}
 
     @initialize_api_client
     def get_follow_ups(self, conversation_id, credentials=None ):  
         try:
             return self.conversations_api_rest.get_follow_ups_by_conversation_id(conversation_id)
         except:
```

### Comparing `symbl-2.0.2/symbl/jobs_api/Job.py` & `symbl-2.0.3/symbl/jobs_api/Job.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.2/symbl/streaming_api/StreamingApi.py` & `symbl-2.0.3/symbl/streaming_api/StreamingApi.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.2/symbl/streaming_api/StreamingConnection.py` & `symbl-2.0.3/symbl/streaming_api/StreamingConnection.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.2/symbl/telephony_api/TelephonyApi.py` & `symbl-2.0.3/symbl/telephony_api/TelephonyApi.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.2/symbl/telephony_api/TelephonyValidators.py` & `symbl-2.0.3/symbl/telephony_api/TelephonyValidators.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.2/symbl/utils/Helper.py` & `symbl-2.0.3/symbl/utils/Helper.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.2/symbl/utils/Logger.py` & `symbl-2.0.3/symbl/utils/Logger.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.2/symbl/utils/Threads.py` & `symbl-2.0.3/symbl/utils/Threads.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.2/symbl.egg-info/PKG-INFO` & `symbl-2.0.3/symbl.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 Metadata-Version: 2.1
 Name: symbl
-Version: 2.0.2
+Version: 2.0.3
 Summary: symbl.ai SDK
 Home-page: 
 Author-email: info@symbl.ai
 Keywords: Symbl.ai SDK
 License-File: LICENSE
+Requires-Dist: symbl_rest>=1.0.11
+Requires-Dist: websocket-client>=0.59.0
+Requires-Dist: pyaudio~=0.2.12
+Requires-Dist: numpy
 
     &lt;h1&gt;Symbl&#x27;s APIs for external consumers.&lt;/h1&gt; &lt;h2&gt;Language Insights API&lt;/h2&gt; Symbl&#x27;s Language Insights API provides an interface for applications to perform the analysis on the raw text and get insights from it. The API automatically detects sentence boundaries and punctuates the sentences, and also returns the updated messages in the response. Conversations are the most unstructured piece of information that we represent information in, and which most of the leads to lot of loss of information by not being able to capture them correctly.&lt;br/&gt; Language Insights API focuses on understanding such texts and generate the useful and important information from them. &lt;br/&gt; Currently the API supports detection of the Action Items in any type of unstructured text. In future the same API will also have support to detect \&quot;Information\&quot; and \&quot;Event\&quot;, where Information is any informational piece and Event is a reference to something that has happened in the past.&lt;br/&gt; &lt;h2&gt;Telephony Integration&lt;/h2&gt; Symbl can currently integrate with two types of telephony endpoints: 1. SIP trunks&lt;br/&gt; 2. PSTN endpoints&lt;br/&gt; Results are sent via HTTP WebHooks as and when they are available.&lt;br/&gt; &lt;h2&gt;Flow&lt;/h2&gt; 1. External Application invokes REST API to join a meeting/session, with the mode (SIP/PSTN) and joining details&lt;br/&gt; 2. Symbl joins the meeting via SIP or PSTN integration&lt;br/&gt; 3. Symbl continuously processes the audio stream received&lt;br/&gt; 4. Symbl calls WebHook whenever transcription results are available&lt;br/&gt;  # noqa: E501
```

### Comparing `symbl-2.0.2/symbl.egg-info/SOURCES.txt` & `symbl-2.0.3/symbl.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 setup.py
 symbl/AuthenticationToken.py
 symbl/Connection.py
 symbl/Conversations.py
 symbl/__init__.py
+symbl/callScore.py
 symbl.egg-info/PKG-INFO
 symbl.egg-info/SOURCES.txt
 symbl.egg-info/dependency_links.txt
 symbl.egg-info/requires.txt
 symbl.egg-info/top_level.txt
 symbl/async_api/Audio.py
 symbl/async_api/Text.py
```

### Comparing `symbl-2.0.2/tests/audio_test.py` & `symbl-2.0.3/tests/audio_test.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.2/tests/authentication_token_test.py` & `symbl-2.0.3/tests/authentication_token_test.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.2/tests/conversations_api_test.py` & `symbl-2.0.3/tests/conversations_api_test.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.2/tests/conversations_test.py` & `symbl-2.0.3/tests/conversations_test.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.2/tests/telephony_test.py` & `symbl-2.0.3/tests/telephony_test.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.2/tests/text_test.py` & `symbl-2.0.3/tests/text_test.py`

 * *Files identical despite different names*

### Comparing `symbl-2.0.2/tests/video_test.py` & `symbl-2.0.3/tests/video_test.py`

 * *Files identical despite different names*

