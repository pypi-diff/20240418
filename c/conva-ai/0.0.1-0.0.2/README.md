# Comparing `tmp/conva_ai-0.0.1.tar.gz` & `tmp/conva_ai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conva_ai-0.0.1.tar", last modified: Tue Apr 16 16:05:25 2024, max compression
+gzip compressed data, was "conva_ai-0.0.2.tar", last modified: Thu Apr 18 06:19:03 2024, max compression
```

## Comparing `conva_ai-0.0.1.tar` & `conva_ai-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-16 16:05:25.293982 conva_ai-0.0.1/
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     1156 2024-04-16 16:05:25.293733 conva_ai-0.0.1/PKG-INFO
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      566 2024-04-16 16:05:10.000000 conva_ai-0.0.1/README.md
-drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-16 16:05:25.292211 conva_ai-0.0.1/conva_ai/
--rw-r--r--   0 harikrishnanc   (501) staff       (20)       41 2024-04-16 16:05:10.000000 conva_ai-0.0.1/conva_ai/__init__.py
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      509 2024-04-16 16:05:10.000000 conva_ai-0.0.1/conva_ai/base.py
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     1890 2024-04-16 16:05:10.000000 conva_ai-0.0.1/conva_ai/client.py
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      656 2024-04-16 16:05:10.000000 conva_ai-0.0.1/conva_ai/response.py
-drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-16 16:05:25.293459 conva_ai-0.0.1/conva_ai.egg-info/
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     1156 2024-04-16 16:05:25.000000 conva_ai-0.0.1/conva_ai.egg-info/PKG-INFO
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      278 2024-04-16 16:05:25.000000 conva_ai-0.0.1/conva_ai.egg-info/SOURCES.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)        1 2024-04-16 16:05:25.000000 conva_ai-0.0.1/conva_ai.egg-info/dependency_links.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      107 2024-04-16 16:05:25.000000 conva_ai-0.0.1/conva_ai.egg-info/requires.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)        9 2024-04-16 16:05:25.000000 conva_ai-0.0.1/conva_ai.egg-info/top_level.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      607 2024-04-16 16:05:10.000000 conva_ai-0.0.1/pyproject.toml
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      467 2024-04-16 16:05:10.000000 conva_ai-0.0.1/requirements.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)       38 2024-04-16 16:05:25.294036 conva_ai-0.0.1/setup.cfg
+drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-18 06:19:03.138940 conva_ai-0.0.2/
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     2772 2024-04-18 06:19:03.138684 conva_ai-0.0.2/PKG-INFO
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     2182 2024-04-18 06:03:49.000000 conva_ai-0.0.2/README.md
+drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-18 06:19:03.137420 conva_ai-0.0.2/conva_ai/
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)       41 2024-04-16 19:28:53.000000 conva_ai-0.0.2/conva_ai/__init__.py
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      759 2024-04-18 06:03:49.000000 conva_ai-0.0.2/conva_ai/base.py
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     1900 2024-04-18 06:03:49.000000 conva_ai-0.0.2/conva_ai/client.py
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      667 2024-04-18 06:03:49.000000 conva_ai-0.0.2/conva_ai/response.py
+drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-18 06:19:03.138392 conva_ai-0.0.2/conva_ai.egg-info/
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     2772 2024-04-18 06:19:03.000000 conva_ai-0.0.2/conva_ai.egg-info/PKG-INFO
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      278 2024-04-18 06:19:03.000000 conva_ai-0.0.2/conva_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)        1 2024-04-18 06:19:03.000000 conva_ai-0.0.2/conva_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      107 2024-04-18 06:19:03.000000 conva_ai-0.0.2/conva_ai.egg-info/requires.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)        9 2024-04-18 06:19:03.000000 conva_ai-0.0.2/conva_ai.egg-info/top_level.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      607 2024-04-18 06:03:49.000000 conva_ai-0.0.2/pyproject.toml
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      467 2024-04-16 16:45:03.000000 conva_ai-0.0.2/requirements.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)       38 2024-04-18 06:19:03.138988 conva_ai-0.0.2/setup.cfg
```

### Comparing `conva_ai-0.0.1/conva_ai/client.py` & `conva_ai-0.0.2/conva_ai/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,31 +14,31 @@
         query: str,
         stream: bool = False,
         capability_group: str = "",
     ) -> AsyncGenerator[ConvaAIResponse, None]:
         app_context: dict = {}
         request_id = uuid.uuid4().hex
         response = requests.post(
-            f"{self.host}/v1/assistants/{self.assistant_id}/text2action",
+            f"{self.host}/v1/assistants/{self.copilot_id}/text2action",
             json={
                 "type": "text2action",
                 "request_id": request_id,
-                "assistant_id": self.assistant_id,
-                "assistant_version": self.assistant_version,
+                "assistant_id": self.copilot_id,
+                "assistant_version": self.copilot_version,
                 "device_id": str(uuid.getnode()),
                 "input_query": query,
                 "domain_name": self.domain,
                 "app_context": app_context,
                 "conversation_history": "{}" if not self.keep_conversation_history else self.history,
                 "capability_group": capability_group,
             },
             headers={"Authorization": self.api_key, "Content-Type": "application/json"},
             stream=stream,
         )
-        client = sseclient.SSEClient(response)
+        client = sseclient.SSEClient(response)  # type: ignore
         for event in client.events():
             event_data = event.data
             event_response = json.loads(event_data)
             rt = event_response.get("response_type", "assistant")
 
             if rt != "status":
                 is_final = event_response.get("is_final", False)
```

### Comparing `conva_ai-0.0.1/pyproject.toml` & `conva_ai-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "conva_ai"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Slang Labs", email="support@slanglabs.in" },
 ]
 dynamic = ["dependencies"]
 description = "Python SDK for using Conva AI co-pilots"
 readme = "README.md"
 requires-python = ">=3.10"
```

