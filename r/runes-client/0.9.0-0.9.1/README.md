# Comparing `tmp/runes-client-0.9.0.tar.gz` & `tmp/runes-client-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runes-client-0.9.0.tar", last modified: Fri Apr 12 20:00:08 2024, max compression
+gzip compressed data, was "runes-client-0.9.1.tar", last modified: Thu Apr 18 00:03:54 2024, max compression
```

## Comparing `runes-client-0.9.0.tar` & `runes-client-0.9.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-12 20:00:08.687825 runes-client-0.9.0/
--rw-r--r--   0 stevehiehn   (501) staff       (20)    35140 2024-03-13 21:22:47.000000 runes-client-0.9.0/LICENSE.md
--rw-r--r--   0 stevehiehn   (501) staff       (20)     6262 2024-04-12 20:00:08.687609 runes-client-0.9.0/PKG-INFO
--rw-r--r--   0 stevehiehn   (501) staff       (20)     5723 2024-04-09 00:18:41.000000 runes-client-0.9.0/README.md
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-12 20:00:08.683999 runes-client-0.9.0/runes_client/
--rw-r--r--   0 stevehiehn   (501) staff       (20)      663 2024-04-12 18:49:27.000000 runes-client-0.9.0/runes_client/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)    10334 2024-04-12 04:09:34.000000 runes-client-0.9.0/runes_client/api_client.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     1193 2024-04-12 01:39:49.000000 runes-client-0.9.0/runes_client/config.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)    38952 2024-04-12 19:19:52.000000 runes-client-0.9.0/runes_client/core.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)      277 2024-03-13 21:22:47.000000 runes-client-0.9.0/runes_client/decorators.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     4446 2024-03-13 21:22:47.000000 runes-client-0.9.0/runes_client/dn_tracer.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     1404 2024-03-13 21:22:47.000000 runes-client-0.9.0/runes_client/file_uploader.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-12 20:00:08.685365 runes-client-0.9.0/runes_client/output/
--rw-r--r--   0 stevehiehn   (501) staff       (20)       63 2024-03-13 21:22:47.000000 runes-client-0.9.0/runes_client/output/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     6818 2024-04-08 05:37:47.000000 runes-client-0.9.0/runes_client/output/results_handler.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-12 20:00:08.686035 runes-client-0.9.0/runes_client/utils/
--rw-r--r--   0 stevehiehn   (501) staff       (20)       61 2024-03-13 21:22:47.000000 runes-client-0.9.0/runes_client/utils/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     3060 2024-03-13 21:22:47.000000 runes-client-0.9.0/runes_client/utils/audio_utils.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)      572 2024-03-13 21:22:47.000000 runes-client-0.9.0/runes_client/utils/file_type_classifier.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-12 20:00:08.687359 runes-client-0.9.0/runes_client.egg-info/
--rw-r--r--   0 stevehiehn   (501) staff       (20)     6262 2024-04-12 20:00:08.000000 runes-client-0.9.0/runes_client.egg-info/PKG-INFO
--rw-r--r--   0 stevehiehn   (501) staff       (20)      725 2024-04-12 20:00:08.000000 runes-client-0.9.0/runes_client.egg-info/SOURCES.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)        1 2024-04-12 20:00:08.000000 runes-client-0.9.0/runes_client.egg-info/dependency_links.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       56 2024-04-12 20:00:08.000000 runes-client-0.9.0/runes_client.egg-info/entry_points.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       72 2024-04-12 20:00:08.000000 runes-client-0.9.0/runes_client.egg-info/requires.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       19 2024-04-12 20:00:08.000000 runes-client-0.9.0/runes_client.egg-info/top_level.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       38 2024-04-12 20:00:08.687865 runes-client-0.9.0/setup.cfg
--rw-r--r--   0 stevehiehn   (501) staff       (20)     1556 2024-04-12 19:30:24.000000 runes-client-0.9.0/setup.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-12 20:00:08.687143 runes-client-0.9.0/tests/
--rw-r--r--   0 stevehiehn   (501) staff       (20)        0 2024-03-13 21:22:47.000000 runes-client-0.9.0/tests/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     5372 2024-03-13 21:50:56.000000 runes-client-0.9.0/tests/test_audio_utils.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     6956 2024-03-13 21:50:43.000000 runes-client-0.9.0/tests/test_core.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)    13164 2024-04-09 00:18:41.000000 runes-client-0.9.0/tests/test_registration.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)      683 2024-03-13 21:50:56.000000 runes-client-0.9.0/tests/test_results_handler.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-18 00:03:54.008017 runes-client-0.9.1/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    35140 2024-03-13 21:22:47.000000 runes-client-0.9.1/LICENSE.md
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     7947 2024-04-18 00:03:54.007737 runes-client-0.9.1/PKG-INFO
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     7408 2024-04-17 23:56:47.000000 runes-client-0.9.1/README.md
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-18 00:03:54.004276 runes-client-0.9.1/runes_client/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      663 2024-04-12 18:49:27.000000 runes-client-0.9.1/runes_client/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    10334 2024-04-12 04:09:34.000000 runes-client-0.9.1/runes_client/api_client.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1193 2024-04-12 01:39:49.000000 runes-client-0.9.1/runes_client/config.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    38952 2024-04-12 19:19:52.000000 runes-client-0.9.1/runes_client/core.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      277 2024-03-13 21:22:47.000000 runes-client-0.9.1/runes_client/decorators.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     4446 2024-03-13 21:22:47.000000 runes-client-0.9.1/runes_client/dn_tracer.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1404 2024-03-13 21:22:47.000000 runes-client-0.9.1/runes_client/file_uploader.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-18 00:03:54.005526 runes-client-0.9.1/runes_client/output/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       63 2024-03-13 21:22:47.000000 runes-client-0.9.1/runes_client/output/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     6818 2024-04-08 05:37:47.000000 runes-client-0.9.1/runes_client/output/results_handler.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-18 00:03:54.006211 runes-client-0.9.1/runes_client/utils/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       61 2024-03-13 21:22:47.000000 runes-client-0.9.1/runes_client/utils/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     3060 2024-03-13 21:22:47.000000 runes-client-0.9.1/runes_client/utils/audio_utils.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      572 2024-03-13 21:22:47.000000 runes-client-0.9.1/runes_client/utils/file_type_classifier.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-18 00:03:54.007512 runes-client-0.9.1/runes_client.egg-info/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     7947 2024-04-18 00:03:53.000000 runes-client-0.9.1/runes_client.egg-info/PKG-INFO
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      725 2024-04-18 00:03:53.000000 runes-client-0.9.1/runes_client.egg-info/SOURCES.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)        1 2024-04-18 00:03:53.000000 runes-client-0.9.1/runes_client.egg-info/dependency_links.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       56 2024-04-18 00:03:53.000000 runes-client-0.9.1/runes_client.egg-info/entry_points.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       72 2024-04-18 00:03:53.000000 runes-client-0.9.1/runes_client.egg-info/requires.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       19 2024-04-18 00:03:53.000000 runes-client-0.9.1/runes_client.egg-info/top_level.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       38 2024-04-18 00:03:54.008063 runes-client-0.9.1/setup.cfg
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1556 2024-04-18 00:00:22.000000 runes-client-0.9.1/setup.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-18 00:03:54.007286 runes-client-0.9.1/tests/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)        0 2024-03-13 21:22:47.000000 runes-client-0.9.1/tests/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     5372 2024-03-13 21:50:56.000000 runes-client-0.9.1/tests/test_audio_utils.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     6956 2024-03-13 21:50:43.000000 runes-client-0.9.1/tests/test_core.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    13164 2024-04-09 00:18:41.000000 runes-client-0.9.1/tests/test_registration.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      683 2024-03-13 21:50:56.000000 runes-client-0.9.1/tests/test_results_handler.py
```

### Comparing `runes-client-0.9.0/LICENSE.md` & `runes-client-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.0/PKG-INFO` & `runes-client-0.9.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,19 @@
-Metadata-Version: 2.1
-Name: runes-client
-Version: 0.9.0
-Summary: Runes client enables remote execution of python code triggered from a Crucible Plugin on the Signals & Sorcery platform.
-Home-page: https://dawnet.tools
-Author: Steve Hiehn
-Author-email: stevehiehn@gmail.com
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: aiohttp
-Requires-Dist: websockets
-Requires-Dist: nest-asyncio
-Requires-Dist: sentry-sdk
-Requires-Dist: pydub
-Requires-Dist: librosa
-Requires-Dist: pytest-asyncio
-
+![signals_and_sorcery_logo](https://storage.googleapis.com/docs-assets/sas_runes_client_2.png)
 # Signals & Sorcery
 
-Signals & Socery is a platform for that connects Rune AIs to Crucible plugins.
+Signals & Sorcery is a platform for that connects Rune AIs to Crucible plugins.
 
 For more information:
 
 - [Signals & Sorcery DOCS](https://signalsandsorcery.com/)
 
 - [Community Discord](https://discord.gg/UcHCjfpRkV)
 
-# elixir-client
+# RUNES CLIENT
 
 The Runes Client (this repo) is a python3 pip package.  It is used to create Rune AIs.  Rune AIs are [Jupyter Notebooks](https://jupyter.org/) scripted using the elixir client and packaged as containers. The client is responsible for moving data and files backand forth from the plugin (and server).   The client allows a user to register python functions with the Signals & Sorcery discovery server. After a function has been registered it can then be triggered remotely from any of the [Crucible plugins](https://signalsandsorcery.com/crucible-plugins/).   
 
 ## Installation
 
 ```python
 pip install runes-client --upgrade
@@ -41,29 +24,54 @@
 from the root of the source code dir run:
 ```python
 pip uninstall runes-client -y && pip install -e . && pytest -s
 ```
 
 ## Usage
 
-This is a simple example of a DAWNet remote script created using the runes-client.  The script defines an arbitrary function that takes two arguments, an integer and a RunesFilePath.  The function is registered with the DAWNet discovery server.  The script then connects to the DAWNet discovery server and waits for a remote trigger. 
+This is a simple example of a RUNES script created using the runes-client.  The script defines an arbitrary function that takes two arguments, an integer and a RunesFilePath.  The function is registered with the SignalsAndSorceryAPI server.  The script then connects to the SignalsAndSorceryAPI server and waits for a plugin to interact with it. 
 
 For thorough documentation and tutorials visit: [https://dawnet.tools/client/](https://dawnet.tools/client/)
 
 ```python
-import runes_client.core as rune 
+import runes_client.core as runes 
 from runes_client import RunesFilePath, ui_param
 
-# The token is generated by the DAWNet plugin.  
-# It is used by the discovery server to associate the remote with the plugin.
-TOKEN="0715c132-0b31-406e-b562-9206c479a48a" 
+# The token generated by the Crucible plugin.  
+# The token is used by the discovery server.  It associates the RUNE with the plugin.
+TOKEN="0715c132-0b31-406e-b562-9206c479a48a"
+
+# There are two separate function you need to register.  
+# 1. The imports.  This is where you load any libraries you need to use in your RUNE.  This is important so that the RUNE is aware when dependencies are loaded and its ready to be called from the plugin.
+# 2. The method.  This is the primary function of the RUNE.  This is where you write the code that will be executed when the RUNE is triggered.
+
+# Name the function anything you like.  This is the imports function.  This is where you load any libraries you need to use in your RUNE.
+async def register_imports():
+    
+    # perform any ```pip install <package>``` here
+   
+    import uuid, os, random, shutil 
+
+    # all imports need to be made global.  If your imports are straight forward you can use the `make_imports_global` function.
+    # If you need to do something more complex you will need to manually make the imports global. For example, in this case we download a large pre-trained model and need to make it global.
+
+    # global model
+    # model = MusicGen.get_pretrained('facebook/musicgen-melody')
+
+    runes.make_imports_global([uuid, os, random, shutil])
+    
+    #NOTE: `make_imports_global()` does not support imports with aliases.  You will need to manually make these global.
+    
+# Now register the imports function with the discovery server.
+runes.register_imports(register_imports)
 
-# The registered method can be named anything. Note: the method must be `async`.  
+# The registered method can be named anything.  This is the primary function of the RUNE.  
+# This function will be rendered as a web form in the crucible plugin. Note: the method must be `async`.  
 # All parameters must be type hinted.  
-# 4 parameter types are supported: int, float, str, RunesFilePath
+# Five parameter types are supported: int, float, str, bool, RunesFilePath
 # RunesFilePath is a special type. When the file is sent to the remote, it is intercepted by the system and 
 # transported to a temp dir on the remote.  In this case the variable `b` is local path to the file.
 
 # The `ui_param` is an optional decorator. It is used to define how the parameter input UI will be rendered in the plugin.  
 # If the decorator is not used, the parameter will be rendered as a text input field. 
 @ui_param('a', 'RunesNumberSlider', min=0, max=10, step=1, default=5)
 @ui_param('c', 'RunesMultiChoice', options=['cherries', 'oranges', 'grapes'], default='grapes')
@@ -71,60 +79,60 @@
     try: 
         # -----------------------------------------
         # This is where you can write custom code to operate on the input params.
         # ex param `a` could be the number of variations created from param `b` using something like MusicLM
         # -----------------------------------------
         
         # This is how you send results back to the plugin, when processing is complete.
-        await rune.results().add_file(b) 
+        await runes.results().add_file(b) 
         # This message is displayed in the plugin.
-        await rune.results().add_message("This is a message XYZ") 
+        await runes.results().add_message("This is a message XYZ") 
 
         return True
     except Exception as e: 
         #explicitly send an error message back to the plugin
-        await rune.results().add_error(f"Method encountered an error: {e}")
+        await runes.results().add_error(f"Method encountered an error: {e}")
         return False
 
 
 # The token generated by the plugin. 
-rune.set_token(token=TOKEN)
+runes.set_token(token=TOKEN)
 # The name of the remote.  This is displayed in the plugin.
-rune.set_name("My Remote Code")
+runes.set_name("My Remote Code")
 # The description of the remote.  This is displayed in the plugin.
-rune.set_description("This is not a real description.")
+runes.set_description("This is not a real description.")
 # Register the method with the discovery server.
-rune.register_method(arbitrary_method)
+runes.register_method(arbitrary_method)
 
 # When a file is sent to the remote as a RunesFilePath, it will become available at this sample rate. 
-rune.set_input_target_sample_rate(44100) #supported values [22050, 32000, 44100, 48000]
+runes.set_input_target_sample_rate(44100) #supported values [22050, 32000, 44100, 48000]
 # When a file is sent to the remote as a RunesFilePath, it will become available at this bit rate. 
-rune.set_input_target_bit_depth(16) #supported values [16, 24, 32]
+runes.set_input_target_bit_depth(16) #supported values [16, 24, 32]
 # When a file is sent to the remote as a RunesFilePath, it will become available with this number of channels.
-rune.set_input_target_channels(2) #supported values [1, 2] mono/stereo respectively
+runes.set_input_target_channels(2) #supported values [1, 2] mono/stereo respectively
 # When a file is sent to the remote as a RunesFilePath, it will become available in this format.
-rune.set_input_target_format('wav') #supported values ["wav", "mp3", "aif", "flac"]
+runes.set_input_target_format('wav') #supported values ["wav", "mp3", "aif", "flac"]
 
 # When results are sent back to the plugin, they will be sent at this sample rate.
-rune.set_output_target_sample_rate(44100)
+runes.set_output_target_sample_rate(44100)
 # When results are sent back to the plugin, they will be sent at this bit rate.
-rune.set_output_target_bit_depth(16)
+runes.set_output_target_bit_depth(16)
 # When results are sent back to the plugin, they will be sent with this number of channels.
-rune.set_output_target_channels(2)
+runes.set_output_target_channels(2)
 # When results are sent back to the plugin, they will be sent in this format.
-rune.set_output_target_format('wav')
+runes.set_output_target_format('wav')
 
 # This should be the last line of the script.  It connects to the discovery server and waits for a remote trigger.
-rune.connect_to_server()
+runes.connect_to_server()
 ```
 
 
 ## CONFIGURATION:
 
-*Note:* If the following environment variables are not set, the client will use the default values.  The default values will point to the public DAWNet server.  If you wish to host your own instance you will need to configure the following environment variables. 
+*Note:* If the following environment variables are not set, the client will use the default values.  The default values will point to the public Signals & Sorcery server (https://signalsandsorceryapi.com/api/swagger/).  If you wish to host your own instance you will need to configure the following environment variables. 
 
 ```
 export DN_CLIENT_API_BASE_URL='https://signalsandsorceryapi.com/'
 export DN_CLIENT_SOCKET_IP='0.0.0.0'
 export DN_CLIENT_SOCKET_PORT='8765'
 export DN_CLIENT_SENTRY_API_KEY='XXX'
 "DN_CLIENT_STORAGE_BUCKET", "https://storage.googleapis.com/your_gcp_bucket/"
```

### Comparing `runes-client-0.9.0/runes_client/__init__.py` & `runes-client-0.9.1/runes_client/__init__.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.0/runes_client/api_client.py` & `runes-client-0.9.1/runes_client/api_client.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.0/runes_client/config.py` & `runes-client-0.9.1/runes_client/config.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.0/runes_client/core.py` & `runes-client-0.9.1/runes_client/core.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.0/runes_client/dn_tracer.py` & `runes-client-0.9.1/runes_client/dn_tracer.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.0/runes_client/file_uploader.py` & `runes-client-0.9.1/runes_client/file_uploader.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.0/runes_client/output/results_handler.py` & `runes-client-0.9.1/runes_client/output/results_handler.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.0/runes_client/utils/audio_utils.py` & `runes-client-0.9.1/runes_client/utils/audio_utils.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.0/runes_client/utils/file_type_classifier.py` & `runes-client-0.9.1/runes_client/utils/file_type_classifier.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.0/runes_client.egg-info/SOURCES.txt` & `runes-client-0.9.1/runes_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.0/setup.py` & `runes-client-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 """
 
 if not is_ffmpeg_installed():
     print(ffmpeg_warning_msg)
 
 setup(
     name="runes-client",
-    version="0.9.0",
+    version="0.9.1",
     packages=find_packages(),
     install_requires=[
         "aiohttp",
         "websockets",
         "nest-asyncio",
         "sentry-sdk",
         "pydub",
```

### Comparing `runes-client-0.9.0/tests/test_audio_utils.py` & `runes-client-0.9.1/tests/test_audio_utils.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.0/tests/test_core.py` & `runes-client-0.9.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.0/tests/test_registration.py` & `runes-client-0.9.1/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.0/tests/test_results_handler.py` & `runes-client-0.9.1/tests/test_results_handler.py`

 * *Files identical despite different names*

