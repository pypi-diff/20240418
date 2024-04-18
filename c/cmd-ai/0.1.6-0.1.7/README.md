# Comparing `tmp/cmd_ai-0.1.6.tar.gz` & `tmp/cmd_ai-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmd_ai-0.1.6.tar", last modified: Mon Jan 15 09:50:28 2024, max compression
+gzip compressed data, was "cmd_ai-0.1.7.tar", last modified: Tue Jan 16 15:06:41 2024, max compression
```

## Comparing `cmd_ai-0.1.6.tar` & `cmd_ai-0.1.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-01-15 09:50:28.433340 cmd_ai-0.1.6/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     2546 2024-01-15 09:50:28.433340 cmd_ai-0.1.6/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     2275 2024-01-15 09:50:23.000000 cmd_ai-0.1.6/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-01-15 09:50:28.433340 cmd_ai-0.1.6/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    15378 2024-01-15 09:50:25.000000 cmd_ai-0.1.6/bin/cmd_ai
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-01-15 09:50:28.433340 cmd_ai-0.1.6/cmd_ai/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      245 2023-11-21 14:40:25.000000 cmd_ai-0.1.6/cmd_ai/__init__.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1129 2023-11-21 16:13:50.000000 cmd_ai-0.1.6/cmd_ai/api_key.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     7596 2024-01-12 15:46:05.000000 cmd_ai-0.1.6/cmd_ai/config.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     9459 2024-01-05 12:51:47.000000 cmd_ai-0.1.6/cmd_ai/function_chmi.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2296 2023-12-28 08:29:31.000000 cmd_ai-0.1.6/cmd_ai/function_goog.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3228 2023-12-28 08:29:31.000000 cmd_ai-0.1.6/cmd_ai/function_webc.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    17337 2024-01-12 15:56:37.000000 cmd_ai-0.1.6/cmd_ai/g_askme.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6149 2023-11-21 16:13:50.000000 cmd_ai-0.1.6/cmd_ai/key_enter.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      555 2023-12-06 16:02:32.000000 cmd_ai-0.1.6/cmd_ai/pipe.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4916 2024-01-08 08:00:50.000000 cmd_ai-0.1.6/cmd_ai/speak.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     7455 2024-01-15 09:50:11.000000 cmd_ai-0.1.6/cmd_ai/syscom.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8161 2024-01-15 09:50:11.000000 cmd_ai-0.1.6/cmd_ai/texts.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2736 2023-11-21 16:13:51.000000 cmd_ai-0.1.6/cmd_ai/topbar.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1077 2023-11-21 16:13:51.000000 cmd_ai-0.1.6/cmd_ai/unitname.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       21 2024-01-15 09:50:28.000000 cmd_ai-0.1.6/cmd_ai/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-01-15 09:50:28.433340 cmd_ai-0.1.6/cmd_ai.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     2546 2024-01-15 09:50:28.000000 cmd_ai-0.1.6/cmd_ai.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      460 2024-01-15 09:50:28.000000 cmd_ai-0.1.6/cmd_ai.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2024-01-15 09:50:28.000000 cmd_ai-0.1.6/cmd_ai.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       68 2024-01-15 09:50:28.000000 cmd_ai-0.1.6/cmd_ai.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        7 2024-01-15 09:50:28.000000 cmd_ai-0.1.6/cmd_ai.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2024-01-15 09:50:28.433340 cmd_ai-0.1.6/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1215 2024-01-02 20:26:23.000000 cmd_ai-0.1.6/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-01-16 15:06:41.565851 cmd_ai-0.1.7/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     2546 2024-01-16 15:06:41.565851 cmd_ai-0.1.7/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     2275 2024-01-16 15:06:38.000000 cmd_ai-0.1.7/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-01-16 15:06:41.561851 cmd_ai-0.1.7/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    15422 2024-01-16 15:06:40.000000 cmd_ai-0.1.7/bin/cmd_ai
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-01-16 15:06:41.565851 cmd_ai-0.1.7/cmd_ai/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      245 2023-11-21 14:40:25.000000 cmd_ai-0.1.7/cmd_ai/__init__.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1129 2023-11-21 16:13:50.000000 cmd_ai-0.1.7/cmd_ai/api_key.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     7596 2024-01-12 15:46:05.000000 cmd_ai-0.1.7/cmd_ai/config.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     9459 2024-01-05 12:51:47.000000 cmd_ai-0.1.7/cmd_ai/function_chmi.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2296 2023-12-28 08:29:31.000000 cmd_ai-0.1.7/cmd_ai/function_goog.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3228 2023-12-28 08:29:31.000000 cmd_ai-0.1.7/cmd_ai/function_webc.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    17337 2024-01-12 15:56:37.000000 cmd_ai-0.1.7/cmd_ai/g_askme.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6149 2023-11-21 16:13:50.000000 cmd_ai-0.1.7/cmd_ai/key_enter.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      555 2023-12-06 16:02:32.000000 cmd_ai-0.1.7/cmd_ai/pipe.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4916 2024-01-08 08:00:50.000000 cmd_ai-0.1.7/cmd_ai/speak.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     7455 2024-01-15 09:50:11.000000 cmd_ai-0.1.7/cmd_ai/syscom.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8161 2024-01-15 09:50:11.000000 cmd_ai-0.1.7/cmd_ai/texts.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2736 2023-11-21 16:13:51.000000 cmd_ai-0.1.7/cmd_ai/topbar.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1077 2023-11-21 16:13:51.000000 cmd_ai-0.1.7/cmd_ai/unitname.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       21 2024-01-16 15:06:41.000000 cmd_ai-0.1.7/cmd_ai/version.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-01-16 15:06:41.565851 cmd_ai-0.1.7/cmd_ai.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     2546 2024-01-16 15:06:41.000000 cmd_ai-0.1.7/cmd_ai.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      460 2024-01-16 15:06:41.000000 cmd_ai-0.1.7/cmd_ai.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2024-01-16 15:06:41.000000 cmd_ai-0.1.7/cmd_ai.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       68 2024-01-16 15:06:41.000000 cmd_ai-0.1.7/cmd_ai.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        7 2024-01-16 15:06:41.000000 cmd_ai-0.1.7/cmd_ai.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2024-01-16 15:06:41.565851 cmd_ai-0.1.7/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1215 2024-01-02 20:26:23.000000 cmd_ai-0.1.7/setup.py
```

### Comparing `cmd_ai-0.1.6/PKG-INFO` & `cmd_ai-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmd_ai
-Version: 0.1.6
+Version: 0.1.7
 Summary: Another ChatGTP project in commandline of linux
 Home-page: http://gitlab.com/me/cmd_ai
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `cmd_ai-0.1.6/README.md` & `cmd_ai-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.1.6/bin/cmd_ai` & `cmd_ai-0.1.7/bin/cmd_ai`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
             resco = re.sub( r'#\+end_src.*$',  "", resco , flags=re.DOTALL) # ignore \n
             with open( config.CONFIG['pyscript'] , "w" ) as f:
                 f.write("#!/usr/bin/env python3\n\n")
                 f.write(resco)
             config.PYSCRIPT_EXISTS = True
 
     # sheller
-    if config.CONFIG['current_role'] == "sheller":
+    if config.CONFIG['current_role'] == "sheller" or config.CONFIG['current_role'] == "piper":
         if resiw.find("#+begin_src")>=0 and  resiw.find("#+end_src")>10:
             resco = re.sub(  r'^.*#\+begin_src(.*?)\n', "",  resiw, flags=re.DOTALL ) # ignore \n
             resco = re.sub( r'#\+end_src.*$',  "", resco , flags=re.DOTALL) # ignore \n
             with open( config.CONFIG['shscript'] , "w" ) as f:
                 f.write("#!/bin/bash\n\n")
                 f.write(resco)
             config.SHSCRIPT_EXISTS = True
```

### Comparing `cmd_ai-0.1.6/cmd_ai/api_key.py` & `cmd_ai-0.1.7/cmd_ai/api_key.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.1.6/cmd_ai/config.py` & `cmd_ai-0.1.7/cmd_ai/config.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.1.6/cmd_ai/function_chmi.py` & `cmd_ai-0.1.7/cmd_ai/function_chmi.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.1.6/cmd_ai/function_goog.py` & `cmd_ai-0.1.7/cmd_ai/function_goog.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.1.6/cmd_ai/function_webc.py` & `cmd_ai-0.1.7/cmd_ai/function_webc.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.1.6/cmd_ai/g_askme.py` & `cmd_ai-0.1.7/cmd_ai/g_askme.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.1.6/cmd_ai/key_enter.py` & `cmd_ai-0.1.7/cmd_ai/key_enter.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.1.6/cmd_ai/pipe.py` & `cmd_ai-0.1.7/cmd_ai/pipe.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.1.6/cmd_ai/speak.py` & `cmd_ai-0.1.7/cmd_ai/speak.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.1.6/cmd_ai/syscom.py` & `cmd_ai-0.1.7/cmd_ai/syscom.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.1.6/cmd_ai/texts.py` & `cmd_ai-0.1.7/cmd_ai/texts.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.1.6/cmd_ai/topbar.py` & `cmd_ai-0.1.7/cmd_ai/topbar.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.1.6/cmd_ai/unitname.py` & `cmd_ai-0.1.7/cmd_ai/unitname.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.1.6/cmd_ai.egg-info/PKG-INFO` & `cmd_ai-0.1.7/cmd_ai.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmd-ai
-Version: 0.1.6
+Version: 0.1.7
 Summary: Another ChatGTP project in commandline of linux
 Home-page: http://gitlab.com/me/cmd_ai
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `cmd_ai-0.1.6/setup.py` & `cmd_ai-0.1.7/setup.py`

 * *Files identical despite different names*

